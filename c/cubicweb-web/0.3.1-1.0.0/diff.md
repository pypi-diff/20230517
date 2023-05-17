# Comparing `tmp/cubicweb-web-0.3.1.tar.gz` & `tmp/cubicweb-web-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-web-0.3.1.tar", last modified: Tue Jan 24 15:11:18 2023, max compression
+gzip compressed data, was "cubicweb-web-1.0.0.tar", last modified: Wed May 17 07:42:18 2023, max compression
```

## Comparing `cubicweb-web-0.3.1.tar` & `cubicweb-web-1.0.0.tar`

### file list

```diff
@@ -1,410 +1,461 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.532790 cubicweb-web-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      496 2023-01-24 15:11:18.532790 cubicweb-web-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.368790 cubicweb-web-0.3.1/cubicweb_web/
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/action.py
--rw-rw-rw-   0 root         (0) root         (0)    21197 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/application.py
--rw-rw-rw-   0 root         (0) root         (0)     6976 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/box.py
--rw-rw-rw-   0 root         (0) root         (0)    17724 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/bwcompat.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/captcha.py
--rw-rw-rw-   0 root         (0) root         (0)     4834 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/ccplugin.py
--rw-rw-rw-   0 root         (0) root         (0)    29058 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/component.py
--rw-rw-rw-   0 root         (0) root         (0)     8635 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.436790 cubicweb-web-0.3.1/cubicweb_web/data/
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/accessories-text-editor.png
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/add_button.png
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/asc.gif
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/banner.png
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/bg.gif
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/bg_trame_grise.png
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/black-check.png
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/black-uncheck.png
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/bullet.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/bullet_orange.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/button.png
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/calendar.gif
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cancel.png
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/contextFreeBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/contextualBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/critical.png
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.acl.css
--rw-rw-rw-   0 root         (0) root         (0)     3589 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.ajax.box.js
--rw-rw-rw-   0 root         (0) root         (0)    24133 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.ajax.js
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.calendar.css
--rw-rw-rw-   0 root         (0) root         (0)     9665 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.calendar.js
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.calendar_popup.css
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.compat.js
--rw-rw-rw-   0 root         (0) root         (0)    18494 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.css
--rw-rw-rw-   0 root         (0) root         (0)    18483 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.edition.js
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.facets.css
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.facets.js
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.fckcwconfig-full.js
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.fckcwconfig.js
--rw-rw-rw-   0 root         (0) root         (0)     1505 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.flot.js
--rw-rw-rw-   0 root         (0) root         (0)     3811 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.form.css
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.html_tree.css
--rw-rw-rw-   0 root         (0) root         (0)     4595 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.htmlhelpers.js
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.ie.css
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.image.js
--rw-rw-rw-   0 root         (0) root         (0)    12621 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.js
--rw-rw-rw-   0 root         (0) root         (0)     1975 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.log.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.log.js
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.login.css
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.manageview.css
--rw-rw-rw-   0 root         (0) root         (0)    16860 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.pictograms.css
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.preferences.css
--rw-rw-rw-   0 root         (0) root         (0)     4559 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.preferences.js
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.print.css
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.python.js
--rw-rw-rw-   0 root         (0) root         (0)     2754 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.reledit.js
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.schema.css
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.suggest.css
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.tablesorter.css
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.tableview.css
--rw-rw-rw-   0 root         (0) root         (0)     2901 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.timetable.css
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.treeview.css
--rw-rw-rw-   0 root         (0) root         (0)    19668 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.widgets.js
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/desc.gif
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/download.gif
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/dublincore-button.png
--rw-rw-rw-   0 root         (0) root         (0)     2179 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/dublincore-icon.png
--rw-rw-rw-   0 root         (0) root         (0)    67968 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/entypo.eot
--rw-rw-rw-   0 root         (0) root         (0)    97203 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/entypo.svg
--rw-rw-rw-   0 root         (0) root         (0)    67680 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/entypo.ttf
--rw-rw-rw-   0 root         (0) root         (0)    42064 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/entypo.woff
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/error.png
--rw-rw-rw-   0 root         (0) root         (0)    42086 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/excanvas.js
--rw-rw-rw-   0 root         (0) root         (0)    34494 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/feed-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/feed-icon16x16.png
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/feed-icon32x32.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/file.gif
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/folder-closed.gif
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/folder.gif
--rw-rw-rw-   0 root         (0) root         (0)    11147 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   151629 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.locale.js
--rw-rw-rw-   0 root         (0) root         (0)    51213 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.min.js
--rw-rw-rw-   0 root         (0) root         (0)      668 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.print.css
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/go.png
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/go_next.png
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/go_prev.png
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/gradient-grey-up.png
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/gradient-grey.gif
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/help.png
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/help_ie.png
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/icon_blank.png
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/icon_bookmark.gif
--rw-rw-rw-   0 root         (0) root         (0)      401 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/icon_emailaddress.gif
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/icon_euser.gif
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/icon_map.png
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/icon_state.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.448790 cubicweb-web-0.3.1/cubicweb_web/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/animated-overlay.gif
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_flat_75_ffffff_40x100.png
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_glass_65_ffffff_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_glass_75_dadada_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-rw-rw-   0 root         (0) root         (0)     3824 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_222222_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_454545_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_888888_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/incontextBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/information.png
--rw-rw-rw-   0 root         (0) root         (0)    16621 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-migrate.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.452790 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/changelog.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.456790 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/file.gif
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/folder-closed.gif
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/folder.gif
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/minus.gif
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/plus.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-black.gif
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-default.gif
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-red.gif
--rw-rw-rw-   0 root         (0) root         (0)     2946 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.css
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js
--rw-rw-rw-   0 root         (0) root         (0)     8065 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.js
--rw-rw-rw-   0 root         (0) root         (0)    13015 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js
--rw-rw-rw-   0 root         (0) root         (0)     1563 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/readme.md
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)     1536 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.cookie.js
--rw-rw-rw-   0 root         (0) root         (0)    89666 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.flot.js
--rw-rw-rw-   0 root         (0) root         (0)   273199 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    85184 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.qtip.js
--rw-rw-rw-   0 root         (0) root         (0)    38404 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.qtip.min.js
--rw-rw-rw-   0 root         (0) root         (0)    41257 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.tablesorter.js
--rw-rw-rw-   0 root         (0) root         (0)     8760 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.timePicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.timepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    32456 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.css
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.datepicker-de.js
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.datepicker-es.js
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.datepicker-fr.js
--rw-rw-rw-   0 root         (0) root         (0)   435844 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.js
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/liveclipboard-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2606 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/loading.gif
--rw-rw-rw-   0 root         (0) root         (0)     9083 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb-gray.svg
--rw-rw-rw-   0 root         (0) root         (0)     3438 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb-icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     7325 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb-text.svg
--rw-rw-rw-   0 root         (0) root         (0)     9202 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/logo-logilab.png
--rw-rw-rw-   0 root         (0) root         (0)     4835 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/microformats-button.png
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/microformats-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/minus.gif
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/no-check-no-border.png
--rw-rw-rw-   0 root         (0) root         (0)      537 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/ok.png
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/pen_icon.png
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/plus.gif
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/plus.png
--rw-rw-rw-   0 root         (0) root         (0)    79752 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/porkys.ttf
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/puce.png
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/puce_down.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/puce_down_black.png
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/puce_up.png
--rw-rw-rw-   0 root         (0) root         (0)     3151 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/pygments.css
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/required.png
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/rss-button.png
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/rss.png
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/search.png
--rw-rw-rw-   0 root         (0) root         (0)      959 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/sendcancel.png
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/sendok.png
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/trash_can.png
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/trash_can_small.png
--rw-rw-rw-   0 root         (0) root         (0)    27374 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/ui.all.css
--rw-rw-rw-   0 root         (0) root         (0)     5055 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/up.gif
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/data/upload.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.456790 cubicweb-web-0.3.1/cubicweb_web/ext/
--rw-rw-rw-   0 root         (0) root         (0)    17396 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/ext/rest.py
--rw-rw-rw-   0 root         (0) root         (0)    69654 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/facet.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/form.py
--rw-rw-rw-   0 root         (0) root         (0)    49323 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/formfields.py
--rw-rw-rw-   0 root         (0) root         (0)    42471 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)    11249 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/htmlwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)    55646 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/http_headers.py
--rw-rw-rw-   0 root         (0) root         (0)     6189 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/httpcache.py
--rw-rw-rw-   0 root         (0) root         (0)     4971 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/propertysheet.py
--rw-rw-rw-   0 root         (0) root         (0)    40194 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/request.py
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/schemaviewer.py
--rw-rw-rw-   0 root         (0) root         (0)     6699 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/uihelper.py
--rw-rw-rw-   0 root         (0) root         (0)    19948 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.484790 cubicweb-web-0.3.1/cubicweb_web/views/
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/_vid_by_mimetype.py
--rw-rw-rw-   0 root         (0) root         (0)    14788 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    16562 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/ajaxcontroller.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/ajaxedit.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/apacherewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     6730 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)    46301 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/autoform.py
--rw-rw-rw-   0 root         (0) root         (0)     8920 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/basecomponents.py
--rw-rw-rw-   0 root         (0) root         (0)    11545 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/basecontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)    22595 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     6017 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     9230 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     9783 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     4352 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/csvexport.py
--rw-rw-rw-   0 root         (0) root         (0)    17032 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/cwproperties.py
--rw-rw-rw-   0 root         (0) root         (0)    16247 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/cwsources.py
--rw-rw-rw-   0 root         (0) root         (0)    10516 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/cwuser.py
--rw-rw-rw-   0 root         (0) root         (0)     7028 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     2465 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/dotgraphview.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/edit_attributes.pt
--rw-rw-rw-   0 root         (0) root         (0)    20973 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/editcontroller.py
--rw-rw-rw-   0 root         (0) root         (0)    12471 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/editforms.py
--rw-rw-rw-   0 root         (0) root         (0)     4687 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/editviews.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/emailaddress.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/error.py
--rw-rw-rw-   0 root         (0) root         (0)    16347 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/facets.py
--rw-rw-rw-   0 root         (0) root         (0)    20026 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/formrenderers.py
--rw-rw-rw-   0 root         (0) root         (0)    18194 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     7798 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/ibreadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     8266 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/idownloadable.py
--rw-rw-rw-   0 root         (0) root         (0)     5584 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/json.py
--rw-rw-rw-   0 root         (0) root         (0)    16883 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/magicsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     9042 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/management.py
--rw-rw-rw-   0 root         (0) root         (0)    15324 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     9023 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/owl.py
--rw-rw-rw-   0 root         (0) root         (0)     4632 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/plots.py
--rw-rw-rw-   0 root         (0) root         (0)    18367 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/primary.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/pyviews.py
--rw-rw-rw-   0 root         (0) root         (0)     5345 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)    22006 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/reledit.py
--rw-rw-rw-   0 root         (0) root         (0)    29416 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/searchrestriction.py
--rw-rw-rw-   0 root         (0) root         (0)     7050 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)     7293 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/startup.py
--rw-rw-rw-   0 root         (0) root         (0)    10082 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/staticcontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)    48960 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/tableview.py
--rw-rw-rw-   0 root         (0) root         (0)     9630 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     8971 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/timetable.py
--rw-rw-rw-   0 root         (0) root         (0)    12731 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/treeview.py
--rw-rw-rw-   0 root         (0) root         (0)    29932 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/uicfg.py
--rw-rw-rw-   0 root         (0) root         (0)     8479 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/undohistory.py
--rw-rw-rw-   0 root         (0) root         (0)    11752 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/urlpublishing.py
--rw-rw-rw-   0 root         (0) root         (0)     9037 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/urlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/vcard.py
--rw-rw-rw-   0 root         (0) root         (0)     7288 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/wdoc.py
--rw-rw-rw-   0 root         (0) root         (0)    17749 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     2320 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/xbel.py
--rw-rw-rw-   0 root         (0) root         (0)    10676 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/views/xmlrss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.496790 cubicweb-web-0.3.1/cubicweb_web/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/about_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/about_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/add_content_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/add_content_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/advanced_usage_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/advanced_usage_schema_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/advanced_usage_schema_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/bookmarks_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/bookmarks_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_last_update_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_last_update_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_rss_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_rss_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/glossary_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      728 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/glossary_fr.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.496790 cubicweb-web-0.3.1/cubicweb_web/wdoc/images/
--rw-rw-rw-   0 root         (0) root         (0)     5590 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/images/userprefs_en.png
--rw-rw-rw-   0 root         (0) root         (0)     6423 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/images/userprefs_fr.png
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/main_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/search_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/search_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/search_sample_queries_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/search_sample_queries_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/standard_usage_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/standard_usage_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/toc.xml
--rw-rw-rw-   0 root         (0) root         (0)     6393 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/tut_rql_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     7275 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/tut_rql_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/userprefs_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/wdoc/userprefs_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)    21681 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/cubicweb_web/webconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.376789 cubicweb-web-0.3.1/cubicweb_web.egg-info/
--rw-r--r--   0 root         (0) root         (0)      496 2023-01-24 15:11:16.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13403 2023-01-24 15:11:18.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 15:11:16.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-01-24 15:11:17.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 15:11:16.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-01-24 15:11:17.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-24 15:11:17.000000 cubicweb-web-0.3.1/cubicweb_web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-24 15:11:18.532790 cubicweb-web-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2592 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.512790 cubicweb-web-0.3.1/test/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.516790 cubicweb-web-0.3.1/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.524790 cubicweb-web-0.3.1/test/data/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_blog/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_blog/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.524790 cubicweb-web-0.3.1/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.524790 cubicweb-web-0.3.1/test/data/cubicweb_file/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/data/file.png
--rw-rw-rw-   0 root         (0) root         (0)     2000 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/schema.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.524790 cubicweb-web-0.3.1/test/data/cubicweb_file/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_file/wdoc/toc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.528790 cubicweb-web-0.3.1/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/cubicweb_tag/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/pouet.css
--rw-rw-rw-   0 root         (0) root         (0)     5554 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/sheet1.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/sheet2.py
--rw-rw-rw-   0 root         (0) root         (0)     2353 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/data/views.py
--rw-rw-rw-   0 root         (0) root         (0)    35877 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_application.py
--rw-rw-rw-   0 root         (0) root         (0)     2259 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_breadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_bw_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    24397 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_facet.py
--rw-rw-rw-   0 root         (0) root         (0)    17839 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_form.py
--rw-rw-rw-   0 root         (0) root         (0)     9464 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_formfields.py
--rw-rw-rw-   0 root         (0) root         (0)     3323 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     9711 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_http.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_http_headers.py
--rw-rw-rw-   0 root         (0) root         (0)     6631 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_idownloadable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.528790 cubicweb-web-0.3.1/test/test_js_scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.528790 cubicweb-web-0.3.1/test/test_js_scripts/data/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/data/ajax_url0.html
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/data/ajax_url1.html
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/data/ajaxresult.json
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/data/test_htmlhelpers.html
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/data/test_utils.html
--rw-rw-rw-   0 root         (0) root         (0)     6549 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/jest.config.js
--rw-rw-rw-   0 root         (0) root         (0)   122226 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/package.json
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/setup.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.528790 cubicweb-web-0.3.1/test/test_js_scripts/test/
--rw-rw-rw-   0 root         (0) root         (0)     7373 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/test/ajax.test.js
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/test/htmlhelpers.test.js
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/test/utils.js
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_js_scripts/test/utils.test.js
--rw-rw-rw-   0 root         (0) root         (0)    13292 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_magicsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_propertysheet.py
--rw-rw-rw-   0 root         (0) root         (0)    22955 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_reledit.py
--rw-rw-rw-   0 root         (0) root         (0)     5652 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     9053 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_uicfg.py
--rw-rw-rw-   0 root         (0) root         (0)     8517 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_urlpublisher.py
--rw-rw-rw-   0 root         (0) root         (0)     9732 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_urlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     3104 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     2791 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_apacherewrite.py
--rw-rw-rw-   0 root         (0) root         (0)    54822 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_basecontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)    13848 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     2076 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_cwsources.py
--rw-rw-rw-   0 root         (0) root         (0)     1791 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_debug_html.py
--rw-rw-rw-   0 root         (0) root         (0)    19065 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_editforms.py
--rw-rw-rw-   0 root         (0) root         (0)     3423 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_errorform.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_forms.py
--rw-rw-rw-   0 root         (0) root         (0)     4530 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_json.py
--rw-rw-rw-   0 root         (0) root         (0)     6177 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_pyviews.py
--rw-rw-rw-   0 root         (0) root         (0)     4912 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_searchrestriction.py
--rw-rw-rw-   0 root         (0) root         (0)     7246 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_staticcontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_treeview.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_wdoc.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_views_xmlrss.py
--rw-rw-rw-   0 root         (0) root         (0)    29061 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_viewselector.py
--rw-rw-rw-   0 root         (0) root         (0)     5929 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_web.py
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/test_webconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test/testutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.532790 cubicweb-web-0.3.1/test_auto/
--rw-rw-rw-   0 root         (0) root         (0)     9991 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test_auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 15:11:18.532790 cubicweb-web-0.3.1/test_auto/data/
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test_auto/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/test_auto/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-01-24 15:10:08.000000 cubicweb-web-0.3.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.050228 cubicweb-web-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-05-17 07:42:18.050228 cubicweb-web-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.934229 cubicweb-web-1.0.0/cubicweb_web/
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/action.py
+-rw-rw-rw-   0 root         (0) root         (0)    21197 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     6976 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/box.py
+-rw-rw-rw-   0 root         (0) root         (0)    20703 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/bwcompat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     4834 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/ccplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    29090 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     8635 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.978229 cubicweb-web-1.0.0/cubicweb_web/data/
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/accessories-text-editor.png
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/add_button.png
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/asc.gif
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/banner.png
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/bg.gif
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/bg_trame_grise.png
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/black-check.png
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/black-uncheck.png
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/bullet.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/bullet_orange.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/button.png
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/calendar.gif
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cancel.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/contextFreeBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/contextualBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/critical.png
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.acl.css
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.ajax.box.js
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.ajax.js
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.calendar.css
+-rw-rw-rw-   0 root         (0) root         (0)     9665 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.calendar.js
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.calendar_popup.css
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.compat.js
+-rw-rw-rw-   0 root         (0) root         (0)    18494 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.css
+-rw-rw-rw-   0 root         (0) root         (0)    18779 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.edition.js
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.facets.css
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.facets.js
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.fckcwconfig-full.js
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.fckcwconfig.js
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.flot.js
+-rw-rw-rw-   0 root         (0) root         (0)     3811 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.form.css
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.html_tree.css
+-rw-rw-rw-   0 root         (0) root         (0)     4595 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.htmlhelpers.js
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.ie.css
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.image.js
+-rw-rw-rw-   0 root         (0) root         (0)    12621 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.js
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.log.css
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.log.js
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.login.css
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.manageview.css
+-rw-rw-rw-   0 root         (0) root         (0)    16860 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.pictograms.css
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.preferences.css
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.preferences.js
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.print.css
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.python.js
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.reledit.js
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.schema.css
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.suggest.css
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.tablesorter.css
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.tableview.css
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.timetable.css
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.treeview.css
+-rw-rw-rw-   0 root         (0) root         (0)    19668 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.widgets.js
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/desc.gif
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/download.gif
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/dublincore-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/dublincore-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)    67968 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/entypo.eot
+-rw-rw-rw-   0 root         (0) root         (0)    97203 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/entypo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    67680 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/entypo.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    42064 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/entypo.woff
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/error.png
+-rw-rw-rw-   0 root         (0) root         (0)    42086 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/excanvas.js
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/feed-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/feed-icon16x16.png
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/feed-icon32x32.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/folder-closed.gif
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)    11147 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   151629 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.locale.js
+-rw-rw-rw-   0 root         (0) root         (0)    51213 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.print.css
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/go.png
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/go_next.png
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/go_prev.png
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/gradient-grey-up.png
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/gradient-grey.gif
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/help.png
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/help_ie.png
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/icon_blank.png
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/icon_bookmark.gif
+-rw-rw-rw-   0 root         (0) root         (0)      401 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/icon_emailaddress.gif
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/icon_euser.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/icon_map.png
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/icon_state.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.982229 cubicweb-web-1.0.0/cubicweb_web/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/animated-overlay.gif
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_glass_75_dadada_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_222222_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_454545_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_888888_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/incontextBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/information.png
+-rw-rw-rw-   0 root         (0) root         (0)    16621 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-migrate.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.982229 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/
+-rw-rw-rw-   0 root         (0) root         (0)     1772 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/changelog.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.986229 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/folder-closed.gif
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/minus.gif
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/plus.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-black.gif
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-default.gif
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-red.gif
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js
+-rw-rw-rw-   0 root         (0) root         (0)     8065 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.js
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.cookie.js
+-rw-rw-rw-   0 root         (0) root         (0)    89666 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.flot.js
+-rw-rw-rw-   0 root         (0) root         (0)   273199 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    85184 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.qtip.js
+-rw-rw-rw-   0 root         (0) root         (0)    38404 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.qtip.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    41257 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.tablesorter.js
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.timePicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.timepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    32456 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.css
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.datepicker-de.js
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.datepicker-es.js
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.datepicker-fr.js
+-rw-rw-rw-   0 root         (0) root         (0)   435844 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.js
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/liveclipboard-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/loading.gif
+-rw-rw-rw-   0 root         (0) root         (0)     9083 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb-gray.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb-icon.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/logo-logilab.png
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/microformats-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/microformats-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/minus.gif
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/no-check-no-border.png
+-rw-rw-rw-   0 root         (0) root         (0)      537 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/ok.png
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/pen_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/plus.gif
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)    79752 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/porkys.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/puce.png
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/puce_down.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/puce_down_black.png
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/puce_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/pygments.css
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/required.png
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/rss-button.png
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/rss.png
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/search.png
+-rw-rw-rw-   0 root         (0) root         (0)      959 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/sendcancel.png
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/sendok.png
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/trash_can.png
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/trash_can_small.png
+-rw-rw-rw-   0 root         (0) root         (0)    27374 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/ui.all.css
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/up.gif
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/data/upload.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.986229 cubicweb-web-1.0.0/cubicweb_web/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39146 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.986229 cubicweb-web-1.0.0/cubicweb_web/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17396 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/ext/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    69654 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/facet.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/form.py
+-rw-rw-rw-   0 root         (0) root         (0)    49324 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)    42471 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    11249 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/htmlwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    55646 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/http_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6189 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/httpcache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/propertysheet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.990229 cubicweb-web-1.0.0/cubicweb_web/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/pyramid/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/pyramid/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/pyramid/url_redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)    40224 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/schemaviewer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6699 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/uihelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    10833 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19979 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.006229 cubicweb-web-1.0.0/cubicweb_web/views/
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/_vid_by_mimetype.py
+-rw-rw-rw-   0 root         (0) root         (0)    14788 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16562 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/ajaxcontroller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/ajaxedit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/apacherewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)    46301 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/autoform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/basecomponents.py
+-rw-rw-rw-   0 root         (0) root         (0)    11545 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/basecontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)    20464 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)    22595 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     6017 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     9230 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9783 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/csvexport.py
+-rw-rw-rw-   0 root         (0) root         (0)    17032 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/cwproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)    16247 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/cwsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    10516 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/cwuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     7028 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     2465 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/dotgraphview.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/edit_attributes.pt
+-rw-rw-rw-   0 root         (0) root         (0)    20973 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/editcontroller.py
+-rw-rw-rw-   0 root         (0) root         (0)    12498 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/editviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/emailaddress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    16347 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)    20026 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)    18194 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     7798 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/ibreadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8266 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/idownloadable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    16883 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/magicsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     9042 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/management.py
+-rw-rw-rw-   0 root         (0) root         (0)    17293 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9023 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/owl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4632 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    18367 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/primary.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/pyviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     5345 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    22006 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)    29416 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/searchrestriction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7050 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7293 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)    10082 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/staticcontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)    48960 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/tableview.py
+-rw-rw-rw-   0 root         (0) root         (0)     9630 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/timetable.py
+-rw-rw-rw-   0 root         (0) root         (0)    12731 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/treeview.py
+-rw-rw-rw-   0 root         (0) root         (0)    29932 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/uicfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     8479 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/undohistory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14784 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/urlpublishing.py
+-rw-rw-rw-   0 root         (0) root         (0)     9037 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/urlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/vcard.py
+-rw-rw-rw-   0 root         (0) root         (0)     7288 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/wdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    17749 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/xbel.py
+-rw-rw-rw-   0 root         (0) root         (0)    10739 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/views/xmlrss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.014228 cubicweb-web-1.0.0/cubicweb_web/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/about_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/about_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/add_content_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/add_content_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/advanced_usage_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/advanced_usage_schema_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/advanced_usage_schema_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/bookmarks_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/bookmarks_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_last_update_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_last_update_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_rss_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_rss_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/glossary_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/glossary_fr.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.014228 cubicweb-web-1.0.0/cubicweb_web/wdoc/images/
+-rw-rw-rw-   0 root         (0) root         (0)     5590 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/images/userprefs_en.png
+-rw-rw-rw-   0 root         (0) root         (0)     6423 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/images/userprefs_fr.png
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/main_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      312 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/search_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/search_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/search_sample_queries_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/search_sample_queries_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/standard_usage_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/standard_usage_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/toc.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6393 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/tut_rql_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7275 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/tut_rql_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/userprefs_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/wdoc/userprefs_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17550 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/cubicweb_web/webconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.938228 cubicweb-web-1.0.0/cubicweb_web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14985 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-17 07:42:17.000000 cubicweb-web-1.0.0/cubicweb_web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 07:42:18.050228 cubicweb-web-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.030228 cubicweb-web-1.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.034228 cubicweb-web-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.034228 cubicweb-web-1.0.0/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_blog/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.034228 cubicweb-web-1.0.0/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.038229 cubicweb-web-1.0.0/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.038229 cubicweb-web-1.0.0/test/data/cubicweb_file/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/data/file.png
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.038229 cubicweb-web-1.0.0/test/data/cubicweb_file/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_file/wdoc/toc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.038229 cubicweb-web-1.0.0/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/cubicweb_tag/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:17.930229 cubicweb-web-1.0.0/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.042229 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.042229 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.042229 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.042229 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/INSTALLER
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/METADATA
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/RECORD
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/WHEEL
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/pouet.css
+-rw-rw-rw-   0 root         (0) root         (0)     8663 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/sheet1.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/sheet2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/data/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    35882 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_breadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_bw_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)    12888 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    24397 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_facet.py
+-rw-rw-rw-   0 root         (0) root         (0)    17839 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     9449 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3291 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9718 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_http.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_http_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     6668 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_idownloadable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.046229 cubicweb-web-1.0.0/test/test_js_scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.046229 cubicweb-web-1.0.0/test/test_js_scripts/data/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/data/ajax_url0.html
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/data/ajax_url1.html
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/data/ajaxresult.json
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/data/test_htmlhelpers.html
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/data/test_utils.html
+-rw-rw-rw-   0 root         (0) root         (0)     6549 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/jest.config.js
+-rw-rw-rw-   0 root         (0) root         (0)   122226 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/package.json
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/setup.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.046229 cubicweb-web-1.0.0/test/test_js_scripts/test/
+-rw-rw-rw-   0 root         (0) root         (0)     7373 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/test/ajax.test.js
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/test/htmlhelpers.test.js
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/test/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_js_scripts/test/utils.test.js
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_login.py
+-rw-rw-rw-   0 root         (0) root         (0)    13290 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_magicsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6986 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_propertysheet.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_pyramid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_pyramid_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_pyramid_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)    23077 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6069 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     9086 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_uicfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_url_redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8483 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_urlpublisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     9697 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_urlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_apacherewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    54751 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_basecontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)    13844 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_cwsources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_debug_html.py
+-rw-rw-rw-   0 root         (0) root         (0)    19638 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_errorform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4531 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     6177 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_pyviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_searchrestriction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7239 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_staticcontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_treeview.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_wdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_views_xmlrss.py
+-rw-rw-rw-   0 root         (0) root         (0)    29065 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_viewselector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     5948 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_web.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_webconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/test_webtest.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/testutils.js
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.050228 cubicweb-web-1.0.0/test_auto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test_auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 07:42:18.050228 cubicweb-web-1.0.0/test_auto/data/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test_auto/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/test_auto/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2023-05-17 07:42:08.000000 cubicweb-web-1.0.0/tox.ini
```

### Comparing `cubicweb-web-0.3.1/MANIFEST.in` & `cubicweb-web-1.0.0/MANIFEST.in`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,24 @@
 recursive-include test/data bootstrap_cubes *.py *.xml
 recursive-include test/data *.css *.py *.png *.gif *.ico *.ttf *.svg *.woff *.eot *.md
 recursive-include test/test_js_scripts *.html *.json
 recursive-include test_auto/data bootstrap_cubes *.py
 recursive-include cubicweb_web/test *.xml *.png *.css *.js
 recursive-include cubicweb_web/test/data bootstrap_cubes *.py
 recursive-include cubicweb_web/test_js_scripts *.js *.html *.json
+recursive-include test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info *
+
+include test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
 
 include *.ini
 
+prune test/test_js_scripts/node_modules
+
+exclude cubicweb_web/i18n/*.po
+exclude test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
+exclude test/data/uicache/cubicweb.css
+
 exclude .gitlab-ci.yml
 exclude .yamllint
 exclude Dockerfile
 exclude CHANGELOG.md
 exclude node_modules
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/__init__.py` & `cubicweb-web-1.0.0/cubicweb_web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,7 +102,8 @@
     "INTERNAL_FIELD_VALUE",
     "stdmsgs",
 ]
 
 
 def includeme(config: Configurator):
     config.include(".bwcompat")
+    config.include(".pyramid")
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/__pkginfo__.py` & `cubicweb-web-1.0.0/cubicweb_web/__pkginfo__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb_web application packaging information"""
 
 
 modname = "web"
 distname = "cubicweb-web"
 
-numversion = (0, 3, 1)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Legacy component for web application"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/web"
 
-__depends__ = {"cubicweb": ">= 3.38.0", "yams": ">= 0.48"}
+__depends__ = {"cubicweb": ">= 4.0.0,<5.0.0", "yams": ">= 0.48"}
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python :: 3",
     "Programming Language :: JavaScript",
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/_exceptions.py` & `cubicweb-web-1.0.0/cubicweb_web/_exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,22 +17,15 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """exceptions used in the core of the CubicWeb web application"""
 
 import http.client as http_client
 
 from cubicweb import CubicWebException, Unauthorized  # noqa # backward compatibility
-from cubicweb.to_refactor._exceptions import (  # noqa # backward compatibility
-    PublishException,
-    Redirect,
-    LogOut,
-    RemoteCallFailed,
-    RequestError,
-    NotFound,
-)
+from cubicweb.utils import json_dumps
 
 
 class DirectResponse(Exception):
     """Used to supply a twitted HTTP Response directly"""
 
     def __init__(self, response):
         self.response = response
@@ -42,14 +35,66 @@
     """raised when a session id is found but associated session is not found or
     invalid"""
 
 
 # Publish related exception
 
 
+class PublishException(CubicWebException):
+    """base class for publishing related exception"""
+
+    def __init__(self, *args, **kwargs):
+        self.status = kwargs.pop("status", http_client.OK)
+        super().__init__(*args, **kwargs)
+
+
+class Redirect(PublishException):
+    """raised to redirect the http request"""
+
+    def __init__(self, location, status=http_client.SEE_OTHER):
+        super().__init__(status=status)
+        self.location = location
+
+
+class LogOut(PublishException):
+    """raised to ask for deauthentication of a logged in user"""
+
+    def __init__(self, url=None):
+        super().__init__()
+        self.url = url
+
+
+class RequestError(PublishException):
+    """raised when a request can't be served because of a bad input"""
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("status", http_client.BAD_REQUEST)
+        super().__init__(*args, **kwargs)
+
+
+class RemoteCallFailed(RequestError):
+    """raised when a json remote call fails"""
+
+    def __init__(self, reason="", status=http_client.INTERNAL_SERVER_ERROR):
+        super().__init__(reason, status=status)
+        self.reason = reason
+
+    def dumps(self):
+        return json_dumps({"reason": self.reason})
+
+
+class NotFound(RequestError):
+    """raised when something was not found. In most case,
+    a 404 error should be returned"""
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("status", http_client.NOT_FOUND)
+        super().__init__(*args, **kwargs)
+
+
 class StatusResponse(PublishException):
     def __init__(self, status, content=""):
         super().__init__(status=status)
         self.content = content
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.status!r}, {self.content!r})"
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/action.py` & `cubicweb-web-1.0.0/cubicweb_web/action.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/application.py` & `cubicweb-web-1.0.0/cubicweb_web/application.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/box.py` & `cubicweb-web-1.0.0/cubicweb_web/box.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/bwcompat.py` & `cubicweb-web-1.0.0/cubicweb_web/bwcompat.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,43 +17,60 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 """Backward compatibility layer for CubicWeb to run as a Pyramid application."""
 
 import inspect
+import itertools
 import logging
 import sys
 import traceback
 import warnings
 from cgi import FieldStorage
+from contextlib import contextmanager
 from datetime import datetime
 from urllib.parse import quote
 
 import pyramid
 from pyramid import httpexceptions
 from pyramid import security
 from pyramid import tweens
 from pyramid.csrf import check_csrf_token, check_csrf_origin, get_csrf_token
 from pyramid.httpexceptions import HTTPSeeOther, HTTPException
 from pyramid.settings import asbool
 
 import yams
 import cubicweb
 from cubicweb.debug import emit_to_debug_channel
-from cubicweb.pyramid.core import cw_to_pyramid
-from cubicweb.to_refactor._exceptions import PublishException, LogOut
+from rql import BadRQLQuery
 
 from cubicweb_web.application import CubicWebPublisher
 from cubicweb_web.request import CubicWebRequestBase
 from cubicweb_web.view import inject_html_generating_call_on_w
+from cubicweb_web._exceptions import (
+    PublishException,
+    LogOut,
+    Redirect,
+    RequestError,
+    RemoteCallFailed,
+    NotFound,
+)
 
 log = logging.getLogger(__name__)
 
 
+NO_SESSION_ERROR_MSG = (
+    "No session factory registered, you can use pyramid_session_redis or "
+    "include in pyramid.ini cubicweb.pyramid.session (which is not recommended "
+    "for production instance. You can also see the Sessions chapter of the Pyramid documentation, "
+    "if you want to define your own session factory."
+)
+
+
 class PyramidSessionHandler(object):
     """A CW Session handler that rely on the pyramid API to fetch the needed
     informations.
 
     It implements the :class:`cubicweb.web.application.CookieSessionHandler`
     API.
     """
@@ -64,14 +81,58 @@
     def get_session(self, req):
         return req._request.cw_session
 
     def logout(self, req, goto_url):
         raise LogOut(url=goto_url)
 
 
+def _cw_headers(request):
+    return itertools.chain(
+        *[
+            [(k, item) for item in v]
+            for k, v in request.cw_request.headers_out.getAllRawHeaders()
+        ]
+    )
+
+
+@contextmanager
+def cw_to_pyramid(request):
+    """Context manager to wrap a call to the cubicweb API.
+
+    All CW exceptions will be transformed into their pyramid equivalent.
+    When needed, some CW reponse bits may be converted too (mainly headers)"""
+    try:
+        yield
+    except Redirect as ex:
+        assert 300 <= ex.status < 400
+        raise httpexceptions.status_map[ex.status](
+            ex.location, headers=_cw_headers(request)
+        )
+    except cubicweb.Unauthorized:
+        raise httpexceptions.HTTPForbidden(
+            request.cw_request._(
+                "You're not authorized to access this page. "
+                "If you think you should, please contact the site "
+                "administrator."
+            ),
+            headers=_cw_headers(request),
+        )
+    except cubicweb.Forbidden:
+        raise httpexceptions.HTTPForbidden(
+            request.cw_request._(
+                "This action is forbidden. "
+                "If you think it should be allowed, please contact the site "
+                "administrator."
+            ),
+            headers=_cw_headers(request),
+        )
+    except (BadRQLQuery, RequestError):
+        raise
+
+
 class CubicWebPyramidHandler(object):
     """A Pyramid request handler that rely on a cubicweb instance to do the
     whole job
 
     :param appli: A CubicWeb 'Application' object.
     """
 
@@ -191,15 +252,15 @@
                 # XXX The validation_error_handler implementation is light, we
                 # should redo it better in cw_to_pyramid, so it can be properly
                 # handled when raised from a cubicweb view.
                 # BUT the real handling of validation errors should be done
                 # earlier in the controllers, not here. In the end, the
                 # ValidationError should never by handled here.
                 content = self.appli.validation_error_handler(cubicweb_request, ex)
-            except cubicweb.to_refactor._exceptions.RemoteCallFailed as exception:
+            except RemoteCallFailed as exception:
                 raise pyramid.httpexceptions.exception_response(
                     exception.status,
                     body=exception.dumps(),
                     content_type="application/json",
                     charset="utf-8",
                 )
 
@@ -218,15 +279,15 @@
                 params = ""
 
                 new_path = request.path_qs
                 if new_path != "/":
                     params = f"?postlogin_path={quote(new_path)}"
 
                 raise HTTPSeeOther(f"/login{params}")
-        except cubicweb.to_refactor._exceptions.NotFound as ex:
+        except NotFound as ex:
             if not cubicweb_request.cnx:
                 new_path = request.path_qs
                 params = f"?postlogin_path={quote(new_path)}" if new_path != "/" else ""
                 raise HTTPSeeOther(f"/login{params}")
             view = cubicweb_registry["views"].select("404", cubicweb_request)
             content = cubicweb_registry["views"].main_template(
                 cubicweb_request, view=view
@@ -355,29 +416,42 @@
     status_out = property(_get_status_out, _set_status_out)
 
     @property
     def message(self):
         """Returns a '<br>' joined list of the cubicweb current message and the
         default pyramid flash queue messages.
         """
-        return "\n<br>\n".join(
-            self._request.session.pop_flash()
-            + self._request.session.pop_flash("cubicweb")
-        )
+        try:
+            return "\n<br>\n".join(
+                self._request.session.pop_flash()
+                + self._request.session.pop_flash("cubicweb")
+            )
+        except AttributeError:
+            log.exception(NO_SESSION_ERROR_MSG)
+            return ""
 
     def set_message(self, msg):
-        self.reset_message()
-        self._request.session.flash(msg, "cubicweb")
+        try:
+            self.reset_message()
+            self._request.session.flash(msg, "cubicweb")
+        except AttributeError:
+            log.exception(NO_SESSION_ERROR_MSG)
 
     def set_message_id(self, msgid):
-        self.reset_message()
-        self.set_message(self._request.session.pop(msgid, ""))
+        try:
+            self.reset_message()
+            self.set_message(self._request.session.pop(msgid, ""))
+        except AttributeError:
+            log.exception(NO_SESSION_ERROR_MSG)
 
     def reset_message(self):
-        self._request.session.pop_flash("cubicweb")
+        try:
+            self._request.session.pop_flash("cubicweb")
+        except AttributeError:
+            log.exception(NO_SESSION_ERROR_MSG)
 
 
 def _cw_request(request):
     """Obtains a CubicWeb request wrapper for the pyramid request.
 
     :param request: A pyramid request
     :return: A CubicWeb request
@@ -434,14 +508,35 @@
             if not (300 <= e.code < 400):
                 traceback.print_exc()
             raise
 
         return response
 
 
+def render_view(request, vid, **kwargs):
+    """Helper function to render a CubicWeb view.
+
+    :param request: A pyramid request
+    :param vid: A CubicWeb view id
+    :param kwargs: Keyword arguments to select and instanciate the view
+    :returns: The rendered view content
+    """
+    vreg = request.registry["cubicweb.registry"]
+    # XXX The select() function could, know how to handle a pyramid
+    # request, and feed it directly to the views that supports it.
+    # On the other hand, we could refine the View concept and decide it works
+    # with a cnx, and never with a WebRequest
+
+    with cw_to_pyramid(request):
+        view = vreg["views"].select(vid, request.cw_request, **kwargs)
+        view.set_stream()
+        view.render()
+        return view._stream.getvalue()
+
+
 def includeme(config):
     """Set up a tween app that will handle the request if the main application
     raises a HTTPNotFound exception.
 
     This is to keep legacy compatibility for cubes that makes use of the
     cubicweb urlresolvers.
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/captcha.py` & `cubicweb-web-1.0.0/cubicweb_web/captcha.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/ccplugin.py` & `cubicweb-web-1.0.0/cubicweb_web/ccplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/component.py` & `cubicweb-web-1.0.0/cubicweb_web/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 from logilab.mtconverter import xml_escape
 
 from cubicweb import Unauthorized, role, target, tags
 from cubicweb import _
 from cubicweb.appobject import AppObject
 from cubicweb.predicates import (
     no_cnx,
-    paginated_rset,
     one_line_rset,
     non_final_entity,
     partial_relation_possible,
     partial_has_related_entities,
 )
 from cubicweb.schema import display_name
 from cubicweb.uilib import js, domid
 from cubicweb.utils import json_dumps, js_href
-from cubicweb_web.view import ReloadableMixIn, Component
+
 from cubicweb_web import INTERNAL_FIELD_VALUE, stdmsgs
+from cubicweb_web.view import ReloadableMixIn, Component
+from cubicweb_web.predicates import paginated_rset
 
 
 # abstract base class for navigation components ################################
 
 
 class NavigationComponent(Component):
     """abstract base class for navigation components"""
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/controller.py` & `cubicweb-web-1.0.0/cubicweb_web/controller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/banner.png` & `cubicweb-web-1.0.0/cubicweb_web/data/banner.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/black-check.png` & `cubicweb-web-1.0.0/cubicweb_web/data/black-check.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/black-uncheck.png` & `cubicweb-web-1.0.0/cubicweb_web/data/black-uncheck.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cancel.png` & `cubicweb-web-1.0.0/cubicweb_web/data/cancel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.acl.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.acl.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.ajax.box.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.ajax.box.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.ajax.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.ajax.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.calendar.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.calendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.calendar.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.calendar.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.calendar_popup.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.calendar_popup.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.compat.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.compat.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.edition.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.edition.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -533,14 +533,25 @@
     result,
     cbargs
 ) {
     // Success
     if (result[0]) {
         if (onsuccess) {
             onsuccess(result, formid, cbargs);
+            if (typeof onsuccess === "function") {
+                try {
+                    onsuccess(result, formid, cbargs);
+                } catch (error) {
+                    console.error(error);
+                    return false;
+                }
+            } else {
+                console.error("onsuccess is not a function!");
+                return false;
+            }
         } else {
             document.location.href = result[1];
         }
         return true;
     }
     if (onfailure && !onfailure(result, formid, cbargs)) {
         return false;
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.facets.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.facets.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.facets.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.facets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.fckcwconfig-full.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.fckcwconfig-full.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.fckcwconfig.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.fckcwconfig.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.flot.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.flot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.form.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.form.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.html_tree.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.html_tree.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.htmlhelpers.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.htmlhelpers.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.ie.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.ie.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.image.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.image.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.log.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.log.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.login.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.login.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.pictograms.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.pictograms.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.preferences.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.preferences.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.preferences.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.preferences.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.python.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.python.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.reledit.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.reledit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.schema.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.schema.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.suggest.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.suggest.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.tableview.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.tableview.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.timetable.css` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.timetable.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/cubicweb.widgets.js` & `cubicweb-web-1.0.0/cubicweb_web/data/cubicweb.widgets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/download.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/download.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/dublincore-button.png` & `cubicweb-web-1.0.0/cubicweb_web/data/dublincore-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/dublincore-icon.png` & `cubicweb-web-1.0.0/cubicweb_web/data/dublincore-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/entypo.eot` & `cubicweb-web-1.0.0/cubicweb_web/data/entypo.eot`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/entypo.svg` & `cubicweb-web-1.0.0/cubicweb_web/data/entypo.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/entypo.ttf` & `cubicweb-web-1.0.0/cubicweb_web/data/entypo.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/entypo.woff` & `cubicweb-web-1.0.0/cubicweb_web/data/entypo.woff`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/error.png` & `cubicweb-web-1.0.0/cubicweb_web/data/error.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/excanvas.js` & `cubicweb-web-1.0.0/cubicweb_web/data/excanvas.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/favicon.ico` & `cubicweb-web-1.0.0/cubicweb_web/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/feed-icon.png` & `cubicweb-web-1.0.0/cubicweb_web/data/feed-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/feed-icon16x16.png` & `cubicweb-web-1.0.0/cubicweb_web/data/feed-icon16x16.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/feed-icon32x32.png` & `cubicweb-web-1.0.0/cubicweb_web/data/feed-icon32x32.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.css` & `cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.js` & `cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.locale.js` & `cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.locale.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.min.js` & `cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/fullcalendar.print.css` & `cubicweb-web-1.0.0/cubicweb_web/data/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/go_next.png` & `cubicweb-web-1.0.0/cubicweb_web/data/go_next.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/go_prev.png` & `cubicweb-web-1.0.0/cubicweb_web/data/go_prev.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/gradient-grey.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/gradient-grey.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/help.png` & `cubicweb-web-1.0.0/cubicweb_web/data/help.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/help_ie.png` & `cubicweb-web-1.0.0/cubicweb_web/data/help_ie.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/icon_map.png` & `cubicweb-web-1.0.0/cubicweb_web/data/icon_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/images/animated-overlay.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_222222_256x240.png` & `cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png` & `cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_454545_256x240.png` & `cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_888888_256x240.png` & `cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png` & `cubicweb-web-1.0.0/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-migrate.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-migrate.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/changelog.md` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/changelog.md`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.css` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/readme.md` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/readme.md`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery-treeview/screenshot.png` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery-treeview/screenshot.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.cookie.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.flot.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.qtip.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.qtip.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.qtip.min.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.qtip.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.tablesorter.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.timePicker.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.timePicker.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.timepicker.css` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.timepicker.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.css` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.datepicker-de.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.datepicker-de.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.datepicker-es.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.datepicker-es.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.datepicker-fr.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.datepicker-fr.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/jquery.ui.js` & `cubicweb-web-1.0.0/cubicweb_web/data/jquery.ui.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/liveclipboard-icon.png` & `cubicweb-web-1.0.0/cubicweb_web/data/liveclipboard-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/loading.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/loading.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb-gray.svg` & `cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb-gray.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb-icon.svg` & `cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb-icon.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb-text.svg` & `cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb-text.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/logo-cubicweb.svg` & `cubicweb-web-1.0.0/cubicweb_web/data/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/logo-logilab.png` & `cubicweb-web-1.0.0/cubicweb_web/data/logo-logilab.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/logo.png` & `cubicweb-web-1.0.0/cubicweb_web/data/logo.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/microformats-button.png` & `cubicweb-web-1.0.0/cubicweb_web/data/microformats-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/microformats-icon.png` & `cubicweb-web-1.0.0/cubicweb_web/data/microformats-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/minus.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/minus.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/ok.png` & `cubicweb-web-1.0.0/cubicweb_web/data/ok.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/plus.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/plus.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/porkys.ttf` & `cubicweb-web-1.0.0/cubicweb_web/data/porkys.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/pygments.css` & `cubicweb-web-1.0.0/cubicweb_web/data/pygments.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/rss-button.png` & `cubicweb-web-1.0.0/cubicweb_web/data/rss-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/sendcancel.png` & `cubicweb-web-1.0.0/cubicweb_web/data/sendcancel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/sendok.png` & `cubicweb-web-1.0.0/cubicweb_web/data/sendok.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/trash_can.png` & `cubicweb-web-1.0.0/cubicweb_web/data/trash_can.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/trash_can_small.png` & `cubicweb-web-1.0.0/cubicweb_web/data/trash_can_small.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/ui.all.css` & `cubicweb-web-1.0.0/cubicweb_web/data/ui.all.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/uiprops.py` & `cubicweb-web-1.0.0/cubicweb_web/data/uiprops.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/data/upload.gif` & `cubicweb-web-1.0.0/cubicweb_web/data/upload.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/ext/rest.py` & `cubicweb-web-1.0.0/cubicweb_web/ext/rest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/facet.py` & `cubicweb-web-1.0.0/cubicweb_web/facet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/form.py` & `cubicweb-web-1.0.0/cubicweb_web/form.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/formfields.py` & `cubicweb-web-1.0.0/cubicweb_web/formfields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1238,15 +1238,15 @@
     (`role`).
 
     The field is initialized according to information found in the schema,
     though any value can be explicitly specified using `kwargs`.
     """
     fieldclass = None
     # We do not know how to use more than the first rdef of the given rschema:
-    rdef = eschema.relation_definition(rschema, role, takefirst=True)
+    rdef = eschema.relation_definition(rschema, role, take_first=True)
     if role == "subject":
         targetschema = rdef.object
         if rschema.final:
             if rdef.get("internationalizable"):
                 kwargs.setdefault("internationalizable", True)
     else:
         targetschema = rdef.subject
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/formwidgets.py` & `cubicweb-web-1.0.0/cubicweb_web/formwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/htmlwidgets.py` & `cubicweb-web-1.0.0/cubicweb_web/htmlwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/http_headers.py` & `cubicweb-web-1.0.0/cubicweb_web/http_headers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/httpcache.py` & `cubicweb-web-1.0.0/cubicweb_web/httpcache.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/propertysheet.py` & `cubicweb-web-1.0.0/cubicweb_web/propertysheet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/request.py` & `cubicweb-web-1.0.0/cubicweb_web/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,24 @@
 from logilab.common.deprecation import class_renamed
 from rql.utils import rqlvar_maker
 
 from cubicweb import AuthenticationError
 from cubicweb import set_log_methods
 from cubicweb.req import RequestSessionAndConnectionBase
 from cubicweb.uilib import remove_html_tags, js
-from cubicweb.utils import HTMLHead, make_uid
+from cubicweb.utils import make_uid
 from cubicweb_web import (
     INTERNAL_FIELD_VALUE,
     LOGGER,
     NothingToEdit,
     RequestError,
 )
 from cubicweb_web.http_headers import Headers, Cookie
 from cubicweb_web.httpcache import get_validators
+from cubicweb_web.utils import HTMLHead
 
 _MARKER = object()
 
 
 def build_cb_uid(seed):
     sha = sha1((f"{time.time()}{seed}{random.random()}").encode("ascii"))
     return "cb_%s" % (sha.hexdigest())
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/schemaviewer.py` & `cubicweb-web-1.0.0/cubicweb_web/schemaviewer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/uihelper.py` & `cubicweb-web-1.0.0/cubicweb_web/uihelper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/view.py` & `cubicweb-web-1.0.0/cubicweb_web/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,18 +31,20 @@
 from cubicweb import NotAnEntity, AuthenticationError
 from cubicweb import _
 from cubicweb import entity
 from cubicweb.appobject import AppObject
 from cubicweb.predicates import non_final_entity, nonempty_rset, none_rset
 from cubicweb.schema import display_name
 from cubicweb.uilib import domid
-from cubicweb.utils import UStringIO, HTMLStream, format_and_escape_string
+from cubicweb.utils import UStringIO, format_and_escape_string
 from cubicweb.devtools.htmlparser import STRICT_DOCTYPE, TRANSITIONAL_DOCTYPE
 
 # robots control
+from cubicweb_web.utils import HTMLStream
+
 NOINDEX = '<meta name="ROBOTS" content="NOINDEX" />'
 NOFOLLOW = '<meta name="ROBOTS" content="NOFOLLOW" />'
 
 TRANSITIONAL_DOCTYPE_NOEXT = TRANSITIONAL_DOCTYPE  # bw compat
 STRICT_DOCTYPE_NOEXT = STRICT_DOCTYPE  # bw compat
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/__init__.py` & `cubicweb-web-1.0.0/cubicweb_web/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/_vid_by_mimetype.py` & `cubicweb-web-1.0.0/cubicweb_web/views/_vid_by_mimetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/actions.py` & `cubicweb-web-1.0.0/cubicweb_web/views/actions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/ajaxcontroller.py` & `cubicweb-web-1.0.0/cubicweb_web/views/ajaxcontroller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/ajaxedit.py` & `cubicweb-web-1.0.0/cubicweb_web/views/ajaxedit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/apacherewrite.py` & `cubicweb-web-1.0.0/cubicweb_web/views/apacherewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/authentication.py` & `cubicweb-web-1.0.0/cubicweb_web/views/authentication.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/autoform.py` & `cubicweb-web-1.0.0/cubicweb_web/views/autoform.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/basecomponents.py` & `cubicweb-web-1.0.0/cubicweb_web/views/basecomponents.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,17 @@
         if msg is None:
             msg = self._cw.message  # XXX don't call self._cw.message twice
         self.w(
             '<div id="appMsg" onclick="%s" class="%s">\n',
             toggle_action("appMsg"),
             (msg and " " or "hidden"),
         )
-        self.w('<div class="message" id="%s">%s</div>', self.domid, msg)
+        self.w('<div class="message" id="%s">', self.domid)
+        self.w(str(msg), escape=False)
+        self.w("</div>")
         self.w("</div>")
 
 
 # contextual components ########################################################
 
 
 class MetaDataComponent(component.EntityCtxComponent):
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/basecontrollers.py` & `cubicweb-web-1.0.0/cubicweb_web/views/basecontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/basetemplates.py` & `cubicweb-web-1.0.0/cubicweb_web/views/basetemplates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/baseviews.py` & `cubicweb-web-1.0.0/cubicweb_web/views/baseviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/bookmark.py` & `cubicweb-web-1.0.0/cubicweb_web/views/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/boxes.py` & `cubicweb-web-1.0.0/cubicweb_web/views/boxes.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/calendar.py` & `cubicweb-web-1.0.0/cubicweb_web/views/calendar.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/csvexport.py` & `cubicweb-web-1.0.0/cubicweb_web/views/csvexport.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/cwproperties.py` & `cubicweb-web-1.0.0/cubicweb_web/views/cwproperties.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/cwsources.py` & `cubicweb-web-1.0.0/cubicweb_web/views/cwsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/cwuser.py` & `cubicweb-web-1.0.0/cubicweb_web/views/cwuser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/debug.py` & `cubicweb-web-1.0.0/cubicweb_web/views/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/dotgraphview.py` & `cubicweb-web-1.0.0/cubicweb_web/views/dotgraphview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/edit_attributes.pt` & `cubicweb-web-1.0.0/cubicweb_web/views/edit_attributes.pt`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/editcontroller.py` & `cubicweb-web-1.0.0/cubicweb_web/views/editcontroller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/editforms.py` & `cubicweb-web-1.0.0/cubicweb_web/views/editforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 from cubicweb import _
 from cubicweb.predicates import (
     one_line_rset,
     non_final_entity,
     specified_etype_implements,
     is_instance,
 )
+from cubicweb.uilib import eid_param
+
 from cubicweb_web.view import EntityView
-from cubicweb_web import stdmsgs, eid_param, formwidgets as fw
+from cubicweb_web import stdmsgs, formwidgets as fw
 from cubicweb_web.form import FormViewMixIn
 from cubicweb_web.views import uicfg, forms
 
 _pvdc = uicfg.primaryview_display_ctrl
 
 
 class DeleteConfForm(forms.CompositeForm):
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/editviews.py` & `cubicweb-web-1.0.0/cubicweb_web/views/editviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/emailaddress.py` & `cubicweb-web-1.0.0/cubicweb_web/views/emailaddress.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/error.py` & `cubicweb-web-1.0.0/cubicweb_web/views/error.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/facets.py` & `cubicweb-web-1.0.0/cubicweb_web/views/facets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/formrenderers.py` & `cubicweb-web-1.0.0/cubicweb_web/views/formrenderers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/forms.py` & `cubicweb-web-1.0.0/cubicweb_web/views/forms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/ibreadcrumbs.py` & `cubicweb-web-1.0.0/cubicweb_web/views/ibreadcrumbs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/idownloadable.py` & `cubicweb-web-1.0.0/cubicweb_web/views/idownloadable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/json.py` & `cubicweb-web-1.0.0/cubicweb_web/views/json.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/magicsearch.py` & `cubicweb-web-1.0.0/cubicweb_web/views/magicsearch.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/management.py` & `cubicweb-web-1.0.0/cubicweb_web/views/management.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/navigation.py` & `cubicweb-web-1.0.0/cubicweb_web/views/navigation.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,21 +45,24 @@
   .. autoclass:: NextPrevNavigationComponent
 """
 
 
 from datetime import datetime
 
 from logilab.mtconverter import xml_escape
-from rql.nodes import VariableRef, Constant
+from rql import stmts
+from rql.nodes import VariableRef, Constant, SubQuery
 
 from cubicweb import _
 from cubicweb.entity import EntityAdapter
-from cubicweb.predicates import paginated_rset, sorted_rset, adaptable
+from cubicweb.predicates import sorted_rset, adaptable
 from cubicweb.uilib import cut
+
 from cubicweb_web.view import View
+from cubicweb_web.predicates import paginated_rset
 from cubicweb_web.component import (
     EmptyComponent,
     EntityCtxComponent,
     NavigationComponent,
 )
 
 
@@ -421,7 +424,64 @@
             '<a href="%s" title="%s">%s</a>'
             % (xml_escape(url), xml_escape(title), content)
         )
         w("</div>")
         self._cw.html_headers.add_raw(
             '<link rel="{}" href="{}" />'.format(type, xml_escape(url))
         )
+
+
+def limited_rql(rset):
+    """returns a printable rql for the result set associated to the object,
+    with limit/offset correctly set according to maximum page size and
+    currently displayed page when necessary
+    """
+    # try to get page boundaries from the navigation component
+    # XXX we should probably not have a ref to this component here (eg in
+    #     cubicweb)
+    nav = rset.req.vreg["components"].select_or_none("navigation", rset.req, rset=rset)
+
+    if nav:
+        start, stop = nav.page_boundaries()
+        rql = _limit_offset_rql(rset, stop - start, start)
+    # result set may have be limited manually in which case navigation won't
+    # apply
+    elif rset.limited:
+        rql = _limit_offset_rql(rset, *rset.limited)
+    # navigation component doesn't apply and rset has not been limited, no
+    # need to limit query
+    else:
+        rql = rset.printable_rql()
+
+    return rql
+
+
+def _limit_offset_rql(rset, limit, offset):
+    rqlst = rset.syntax_tree()
+
+    if len(rqlst.children) == 1:
+        select = rqlst.children[0]
+        olimit, ooffset = select.limit, select.offset
+        select.limit, select.offset = limit, offset
+        rql = rqlst.as_string(kwargs=rset.args)
+        # restore original limit/offset
+        select.limit, select.offset = olimit, ooffset
+
+    else:
+        newselect = stmts.Select()
+        newselect.limit = limit
+        newselect.offset = offset
+        aliases = [
+            VariableRef(newselect.get_variable(chr(65 + i), i))
+            for i in range(len(rqlst.children[0].selection))
+        ]
+
+        for vref in aliases:
+            newselect.append_selected(VariableRef(vref.variable))
+
+        newselect.set_with([SubQuery(aliases, rqlst)], check=False)
+        newunion = stmts.Union()
+        newunion.append(newselect)
+        rql = newunion.as_string(kwargs=rset.args)
+        rqlst.parent = None
+
+    return rql
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/owl.py` & `cubicweb-web-1.0.0/cubicweb_web/views/owl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/plots.py` & `cubicweb-web-1.0.0/cubicweb_web/views/plots.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/primary.py` & `cubicweb-web-1.0.0/cubicweb_web/views/primary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/pyviews.py` & `cubicweb-web-1.0.0/cubicweb_web/views/pyviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/rdf.py` & `cubicweb-web-1.0.0/cubicweb_web/views/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/reledit.py` & `cubicweb-web-1.0.0/cubicweb_web/views/reledit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/schema.py` & `cubicweb-web-1.0.0/cubicweb_web/views/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/searchrestriction.py` & `cubicweb-web-1.0.0/cubicweb_web/views/searchrestriction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/sessions.py` & `cubicweb-web-1.0.0/cubicweb_web/views/sessions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/startup.py` & `cubicweb-web-1.0.0/cubicweb_web/views/startup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/staticcontrollers.py` & `cubicweb-web-1.0.0/cubicweb_web/views/staticcontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/tableview.py` & `cubicweb-web-1.0.0/cubicweb_web/views/tableview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/tabs.py` & `cubicweb-web-1.0.0/cubicweb_web/views/tabs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/timetable.py` & `cubicweb-web-1.0.0/cubicweb_web/views/timetable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/treeview.py` & `cubicweb-web-1.0.0/cubicweb_web/views/treeview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/uicfg.py` & `cubicweb-web-1.0.0/cubicweb_web/views/uicfg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/undohistory.py` & `cubicweb-web-1.0.0/cubicweb_web/views/undohistory.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/urlrewrite.py` & `cubicweb-web-1.0.0/cubicweb_web/views/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/vcard.py` & `cubicweb-web-1.0.0/cubicweb_web/views/vcard.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/wdoc.py` & `cubicweb-web-1.0.0/cubicweb_web/views/wdoc.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/workflow.py` & `cubicweb-web-1.0.0/cubicweb_web/views/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/xbel.py` & `cubicweb-web-1.0.0/cubicweb_web/views/xbel.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/views/xmlrss.py` & `cubicweb-web-1.0.0/cubicweb_web/views/xmlrss.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     non_final_entity,
     one_line_rset,
     appobject_selectable,
     adaptable,
 )
 from cubicweb.uilib import simple_sgml_tag
 from cubicweb_web.view import EntityView, AnyRsetView, Component
+from cubicweb_web.views.navigation import limited_rql
 from cubicweb_web import httpcache, component
 
 
 def encode_bytes(value):
     return "<![CDATA[%s]]>" % b64encode(value.getvalue())
 
 
@@ -162,15 +163,15 @@
     title = _("xml export")
     templatable = False
     content_type = "text/xml"
     xml_root = "rset"
 
     def call(self):
         rset, descr = self.cw_rset, self.cw_rset.description
-        entity_schema_for = self._cw.vreg.schema.eschema
+        entity_schema_for = self._cw.vreg.schema.entity_schema_for
         labels = self.columns_labels(tr=False)
         self.w('<?xml version="1.0" encoding="%s"?>\n', self._cw.encoding)
         self.w('<%s query="%s">\n', self.xml_root, rset.printable_rql())
         for rowindex, row in enumerate(self.cw_rset):
             self.w(" <row>\n")
             for colindex, val in enumerate(row):
                 etype = descr[rowindex][colindex]
@@ -208,15 +209,15 @@
 
 
 class RSSFeedURL(Component):
     __regid__ = "rss_feed_url"
     __select__ = non_final_entity()
 
     def feed_url(self):
-        return self._cw.build_url(rql=self.cw_rset.limited_rql(), vid="rss")
+        return self._cw.build_url(rql=limited_rql(self.cw_rset), vid="rss")
 
 
 class RSSEntityFeedURL(Component):
     __regid__ = "rss_feed_url"
     __select__ = one_line_rset() & adaptable("IFeed")
 
     def feed_url(self):
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/about_en.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/about_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/about_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/about_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/advanced_usage_schema_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/advanced_usage_schema_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/bookmarks_en.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/bookmarks_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/bookmarks_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/bookmarks_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_en.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/custom_view_rss_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/custom_view_rss_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/glossary_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/glossary_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/images/userprefs_en.png` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/images/userprefs_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/images/userprefs_fr.png` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/images/userprefs_fr.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/standard_usage_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/standard_usage_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/toc.xml` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/toc.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/tut_rql_en.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/tut_rql_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/tut_rql_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/tut_rql_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/wdoc/userprefs_fr.rst` & `cubicweb-web-1.0.0/cubicweb_web/wdoc/userprefs_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/cubicweb_web/webconfig.py` & `cubicweb-web-1.0.0/cubicweb_web/webconfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 import os
 from os.path import dirname, join, exists, split, isdir
 from uuid import uuid4
 
 from logilab.common.configuration import Method, merge_options
 from logilab.common.decorators import cached, cachedproperty
 
-from cubicweb import ConfigurationError
 from cubicweb import _
 from cubicweb.cwconfig import CubicWebConfiguration, register_persistent_options
+from cubicweb.pyramid.config import AllInOneConfiguration
 
 _DATA_DIR = join(dirname(__file__), "data")
 
 
 register_persistent_options(
     (
         # site-wide only web ui configuration
@@ -120,59 +120,23 @@
                     "default": True,
                     "help": _("should css be compiled and store in uicache"),
                     "group": "ui",
                     "level": 2,
                 },
             ),
             (
-                "anonymous-user",
-                {
-                    "type": "string",
-                    "default": None,
-                    "help": (
-                        "login of the CubicWeb user account to use for anonymous "
-                        "user (if you want to allow anonymous)"
-                    ),
-                    "group": "web",
-                    "level": 1,
-                },
-            ),
-            (
-                "anonymous-password",
-                {
-                    "type": "string",
-                    "default": None,
-                    "help": "password of the CubicWeb user account to use for anonymous user, "
-                    "if anonymous-user is set",
-                    "group": "web",
-                    "level": 1,
-                },
-            ),
-            (
                 "query-log-file",
                 {
                     "type": "string",
                     "default": None,
                     "help": "web instance query log file",
                     "group": "web",
                     "level": 3,
                 },
             ),
-            (
-                "cleanup-anonymous-session-time",
-                {
-                    "type": "time",
-                    "default": "5min",
-                    "help": "Same as cleanup-session-time but specific to anonymous "
-                    "sessions. You can have a much smaller timeout here since it will be "
-                    "transparent to the user. Default to 5min.",
-                    "group": "web",
-                    "level": 3,
-                },
-            ),
             # web configuration
             (
                 "datadir-url",
                 {
                     "type": "string",
                     "default": None,
                     "help": (
@@ -313,96 +277,16 @@
                     "type": "string",
                     "default": None,
                     "help": "The static data resource directory path.",
                     "group": "web",
                     "level": 2,
                 },
             ),
-            (
-                "access-control-allow-origin",
-                {
-                    "type": "csv",
-                    "default": (),
-                    "help": (
-                        'comma-separated list of allowed origin domains or "*" for any domain'
-                    ),
-                    "group": "web",
-                    "level": 2,
-                },
-            ),
-            (
-                "access-control-allow-methods",
-                {
-                    "type": "csv",
-                    "default": (),
-                    "help": ("comma-separated list of allowed HTTP methods"),
-                    "group": "web",
-                    "level": 2,
-                },
-            ),
-            (
-                "access-control-max-age",
-                {
-                    "type": "int",
-                    "default": None,
-                    "help": (
-                        "maximum age of cross-origin resource sharing (in seconds)"
-                    ),
-                    "group": "web",
-                    "level": 2,
-                },
-            ),
-            (
-                "access-control-expose-headers",
-                {
-                    "type": "csv",
-                    "default": (),
-                    "help": (
-                        "comma-separated list of HTTP headers the application "
-                        "declare in response to a preflight request"
-                    ),
-                    "group": "web",
-                    "level": 2,
-                },
-            ),
-            (
-                "access-control-allow-headers",
-                {
-                    "type": "csv",
-                    "default": (),
-                    "help": (
-                        "comma-separated list of HTTP headers the application may set in the "
-                        "response"
-                    ),
-                    "group": "web",
-                    "level": 2,
-                },
-            ),
             # ctl configuration
             (
-                "port",
-                {
-                    "type": "int",
-                    "default": None,
-                    "help": "http server port number (default to 8080)",
-                    "group": "web",
-                    "level": 0,
-                },
-            ),
-            (
-                "interface",
-                {
-                    "type": "string",
-                    "default": "127.0.0.1",
-                    "help": "http server address on which to listen (default to local requests)",
-                    "group": "web",
-                    "level": 1,
-                },
-            ),
-            (
                 "max-post-length",  # XXX specific to "wsgi" server
                 {
                     "type": "bytes",
                     "default": "100MB",
                     "help": "maximum length of HTTP request. Default to 100 MB.",
                     "group": "web",
                     "level": 1,
@@ -422,29 +306,23 @@
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.uiprops = None
         self.datadir_url = None
         self._debug = None
-
-    def anonymous_user(self):
-        """return a login and password to use for anonymous users.
-
-        None may be returned for both if anonymous connection is not
-        allowed or if an empty login is used in configuration
-        """
+        # don't register ReStructured Text directives by simple import, avoid pb
+        # with eg sphinx.
+        # XXX should be done properly with a function from cw.uicfg
         try:
-            user = self["anonymous-user"] or None
-            passwd = self["anonymous-password"]
-        except KeyError:
-            user, passwd = None, None
-        except UnicodeDecodeError:
-            raise ConfigurationError("anonymous information should only contains ascii")
-        return user, passwd
+            from cubicweb_web.ext.rest import cw_rest_init
+        except ImportError:
+            pass
+        else:
+            cw_rest_init()
 
     @property
     def in_debug_mode(self):
         """
         we need all of this because self["debug"] is regularely overwritten in
         the workflow because the configuration is not initialy loaded and
         loaded after most includeme.
@@ -535,33 +413,29 @@
             if exists(fpath):
                 yield join(fpath)
 
     def load_configuration(self, **kw):
         """load instance's configuration files"""
         super().load_configuration(**kw)
         # load external resources definition
-        self._init_base_url()
         self._build_ui_properties()
 
     def _init_base_url(self):
-        # normalize base url(s)
-        baseurl = self["base-url"] or self.default_base_url()
-        if baseurl and baseurl[-1] != "/":
-            baseurl += "/"
-        if not (self.repairing or self.creating):
-            self.global_set_option("base-url", baseurl)
+        super()._init_base_url()
+
         self.datadir_url = self["datadir-url"]
         if self.datadir_url:
             if self.datadir_url[-1] != "/":
                 self.datadir_url += "/"
             if self.mode != "test":
                 self.datadir_url += "%s/" % self.instance_md5_version()
             return
+
         data_relpath = self.data_relpath()
-        self.datadir_url = baseurl + data_relpath
+        self.datadir_url = self._generate_base_url() + data_relpath
 
     def data_relpath(self):
         if self.mode == "test":
             return "data/"
         return "data/%s/" % self.instance_md5_version()
 
     def _build_ui_properties(self):
@@ -618,14 +492,21 @@
         stream.close()
         self.ensure_uid(rpath)
 
     def static_file_del(self, rpath):
         if self.static_file_exists(rpath):
             os.remove(join(self.static_directory, rpath))
 
-    def default_base_url(self):
-        from socket import getfqdn
 
-        return "http://{}:{}/".format(
-            self["host"] or getfqdn().lower(),
-            self["port"] or 8080,
-        )
+class WebAllInOneConfiguration(AllInOneConfiguration, WebConfiguration):
+    """web instance (in a web server) client of a RQL server"""
+
+    name = "all-in-one"
+    options = merge_options(WebConfiguration.options + AllInOneConfiguration.options)
+
+    cubicweb_appobject_path = (
+        WebConfiguration.cubicweb_appobject_path
+        | AllInOneConfiguration.cubicweb_appobject_path
+    )
+    cube_appobject_path = (
+        WebConfiguration.cube_appobject_path | AllInOneConfiguration.cube_appobject_path
+    )
```

### Comparing `cubicweb-web-0.3.1/cubicweb_web.egg-info/SOURCES.txt` & `cubicweb-web-1.0.0/cubicweb_web.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README
+README.rst
 setup.py
 tox.ini
 cubicweb_web/__init__.py
 cubicweb_web/__pkginfo__.py
 cubicweb_web/_exceptions.py
 cubicweb_web/action.py
 cubicweb_web/application.py
@@ -16,18 +16,21 @@
 cubicweb_web/facet.py
 cubicweb_web/form.py
 cubicweb_web/formfields.py
 cubicweb_web/formwidgets.py
 cubicweb_web/htmlwidgets.py
 cubicweb_web/http_headers.py
 cubicweb_web/httpcache.py
+cubicweb_web/i18n.py
+cubicweb_web/predicates.py
 cubicweb_web/propertysheet.py
 cubicweb_web/request.py
 cubicweb_web/schemaviewer.py
 cubicweb_web/uihelper.py
+cubicweb_web/utils.py
 cubicweb_web/view.py
 cubicweb_web/webconfig.py
 cubicweb_web.egg-info/PKG-INFO
 cubicweb_web.egg-info/SOURCES.txt
 cubicweb_web.egg-info/dependency_links.txt
 cubicweb_web.egg-info/entry_points.txt
 cubicweb_web.egg-info/not-zip-safe
@@ -205,15 +208,23 @@
 cubicweb_web/data/jquery-treeview/images/treeview-default.gif
 cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
 cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
 cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
 cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
 cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
 cubicweb_web/data/jquery-treeview/images/treeview-red.gif
+cubicweb_web/devtools/__init__.py
+cubicweb_web/devtools/testlib.py
+cubicweb_web/ext/__init__.py
 cubicweb_web/ext/rest.py
+cubicweb_web/pyramid/__init__.py
+cubicweb_web/pyramid/login.py
+cubicweb_web/pyramid/predicates.py
+cubicweb_web/pyramid/test.py
+cubicweb_web/pyramid/url_redirection.py
 cubicweb_web/views/__init__.py
 cubicweb_web/views/_vid_by_mimetype.py
 cubicweb_web/views/actions.py
 cubicweb_web/views/ajaxcontroller.py
 cubicweb_web/views/ajaxedit.py
 cubicweb_web/views/apacherewrite.py
 cubicweb_web/views/authentication.py
@@ -302,26 +313,39 @@
 cubicweb_web/wdoc/images/userprefs_en.png
 cubicweb_web/wdoc/images/userprefs_fr.png
 test/__init__.py
 test/test_application.py
 test/test_breadcrumbs.py
 test/test_bw_request.py
 test/test_controller.py
+test/test_csrf.py
+test/test_entity.py
 test/test_facet.py
 test/test_form.py
 test/test_formfields.py
 test/test_formwidgets.py
 test/test_http.py
 test/test_http_headers.py
+test/test_httptest.py
+test/test_i18n.py
 test/test_idownloadable.py
+test/test_login.py
 test/test_magicsearch.py
+test/test_predicates.py
 test/test_propertysheet.py
+test/test_pyramid.py
+test/test_pyramid_hooks.py
+test/test_pyramid_predicates.py
 test/test_reledit.py
 test/test_request.py
+test/test_rest.py
+test/test_rset.py
+test/test_testlib.py
 test/test_uicfg.py
+test/test_url_redirection.py
 test/test_urlpublisher.py
 test/test_urlrewrite.py
 test/test_views_actions.py
 test/test_views_apacherewrite.py
 test/test_views_basecontrollers.py
 test/test_views_basetemplates.py
 test/test_views_baseviews.py
@@ -336,41 +360,60 @@
 test/test_views_pyviews.py
 test/test_views_searchrestriction.py
 test/test_views_staticcontrollers.py
 test/test_views_treeview.py
 test/test_views_wdoc.py
 test/test_views_xmlrss.py
 test/test_viewselector.py
+test/test_vregistry.py
 test/test_web.py
 test/test_webconfig.py
+test/test_webtest.py
 test/testutils.js
+test/unittest_utils.py
 test/data/bootstrap_cubes
 test/data/entities.py
 test/data/pouet.css
 test/data/schema.py
 test/data/sheet1.py
 test/data/sheet2.py
 test/data/views.py
 test/data/cubicweb_blog/__init__.py
 test/data/cubicweb_blog/__pkginfo__.py
 test/data/cubicweb_blog/entities.py
 test/data/cubicweb_blog/schema.py
+test/data/cubicweb_card/__init__.py
+test/data/cubicweb_card/__pkginfo__.py
+test/data/cubicweb_card/entities.py
+test/data/cubicweb_card/schema.py
 test/data/cubicweb_file/__init__.py
 test/data/cubicweb_file/__pkginfo__.py
 test/data/cubicweb_file/entities.py
 test/data/cubicweb_file/hooks.py
 test/data/cubicweb_file/schema.py
 test/data/cubicweb_file/uiprops.py
 test/data/cubicweb_file/views.py
 test/data/cubicweb_file/data/file.png
 test/data/cubicweb_file/wdoc/toc.xml
 test/data/cubicweb_tag/__init__.py
 test/data/cubicweb_tag/__pkginfo__.py
 test/data/cubicweb_tag/schema.py
 test/data/cubicweb_tag/views.py
+test/data/libpython/cubicweb_i18ntestcube/__init__.py
+test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+test/data/libpython/cubicweb_i18ntestcube/schema.py
+test/data/libpython/cubicweb_i18ntestcube/views.py
+test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/INSTALLER
+test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/METADATA
+test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/RECORD
+test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/WHEEL
+test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/entry_points.txt
+test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/top_level.txt
+test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
 test/test_js_scripts/jest.config.js
 test/test_js_scripts/package-lock.json
 test/test_js_scripts/package.json
 test/test_js_scripts/setup.js
 test/test_js_scripts/data/ajax_url0.html
 test/test_js_scripts/data/ajax_url1.html
 test/test_js_scripts/data/ajaxresult.json
```

### Comparing `cubicweb-web-0.3.1/setup.py` & `cubicweb-web-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 license = __pkginfo__["license"]
 description = __pkginfo__["description"]
 web = __pkginfo__["web"]
 author = __pkginfo__["author"]
 author_email = __pkginfo__["author_email"]
 classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, "README")) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
@@ -74,10 +74,13 @@
     packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
         "cubicweb.cubes": [
             "web=cubicweb_web",
         ],
+        "cubicweb.i18ncube": [
+            "web=cubicweb_web.i18n:WebI18nCubeMessageExtractor",
+        ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-web-0.3.1/test/data/cubicweb_blog/schema.py` & `cubicweb-web-1.0.0/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/data/cubicweb_file/entities.py` & `cubicweb-web-1.0.0/test/data/cubicweb_file/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/data/cubicweb_file/hooks.py` & `cubicweb-web-1.0.0/test/data/cubicweb_file/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/data/cubicweb_file/schema.py` & `cubicweb-web-1.0.0/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/data/cubicweb_tag/schema.py` & `cubicweb-web-1.0.0/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/data/cubicweb_tag/views.py` & `cubicweb-web-1.0.0/test/data/cubicweb_tag/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/data/entities.py` & `cubicweb-web-1.0.0/test/data/entities.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,18 +13,50 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from cubicweb.predicates import is_instance
-from cubicweb.entities.adapters import ITreeAdapter
+from cubicweb.entities.adapters import ITreeAdapter, IDownloadableAdapter
 from cubicweb.entities import AnyEntity, fetch_config
 
 
+class Societe(AnyEntity):
+    __regid__ = "Societe"
+    fetch_attrs = ("nom",)
+
+
+class Personne(Societe):
+    """customized class forne Person entities"""
+
+    __regid__ = "Personne"
+    fetch_attrs, cw_fetch_order = fetch_config(["nom", "prenom"])
+    rest_attr = "nom"
+
+
+class Ami(Societe):
+    __regid__ = "Ami"
+    fetch_attrs, cw_fetch_order = fetch_config(["nom", "prenom"])
+    rest_attr = "nom"
+
+
+class Ville(AnyEntity):
+    __regid__ = "Ville"
+    rest_attr = "insee"
+
+
+class Note(AnyEntity):
+    __regid__ = "Note"
+
+
+class FakeFileIDownloadableAdapter(IDownloadableAdapter):
+    __select__ = is_instance("FakeFile")
+
+
 class TreeNode(AnyEntity):
     __regid__ = "TreeNode"
     fetch_attrs, cw_fetch_order = fetch_config(["name"])
 
 
 class ITreeNode(ITreeAdapter):
     __select__ = is_instance("TreeNode")
```

### Comparing `cubicweb-web-0.3.1/test/data/schema.py` & `cubicweb-web-1.0.0/test/data/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,26 +15,34 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from yams.buildobjs import (
     EntityType,
     RelationDefinition,
+    ComputedRelation,
     SubjectRelation,
     String,
     Int,
     Datetime,
     Boolean,
     Float,
     TZDatetime,
+    Bytes,
+    RichString,
 )
 from yams.constraints import IntervalBoundConstraint
 
 from cubicweb import _
-from cubicweb.schema import RRQLExpression
+from cubicweb.schema import (
+    RRQLExpression,
+    RQLConstraint,
+    RQLVocabularyConstraint,
+    WorkflowableEntityType,
+)
 
 
 def rperms(var, read=("managers", "users")):
     return {
         "read": read,
         "add": ("managers", RRQLExpression(f"U has_update_permission {var}")),
         "delete": (
@@ -50,15 +58,15 @@
     )
     amount = Int(constraints=[IntervalBoundConstraint(0, 100)])
     reason = String(maxsize=20, vocabulary=["canceled", "sold"])
 
 
 class tags(RelationDefinition):
     subject = "Tag"
-    object = ("BlogEntry", "CWUser")
+    object = ("BlogEntry", "CWUser", "Ami", "Personne", "Note")
 
 
 class checked_by(RelationDefinition):
     subject = "BlogEntry"
     object = "CWUser"
     cardinality = "?*"
     __permissions__ = {
@@ -83,16 +91,17 @@
         ),
         "delete": (
             "managers",
             "validators",
             "owners",
         ),
     }
-    nom = String(fulltextindexed=True, required=True, maxsize=64)
-    prenom = String(fulltextindexed=True, maxsize=64)
+    nom = String(fulltextindexed=True, required=True)
+    prenom = String(fulltextindexed=True)
+    type = String()
     sexe = String(
         maxsize=1,
         default="M",
         __permissions__={
             "read": (
                 "managers",
                 "users",
@@ -111,33 +120,61 @@
     datenaiss = Datetime()
     tzdatenaiss = TZDatetime()
     test = Boolean()
     description = String()
     salary = Float()
     travaille = SubjectRelation("Societe")
     tags = SubjectRelation("BlogEntry")
+    evaluee = SubjectRelation(("Note", "Personne"))
+    connait = SubjectRelation(
+        "Personne",
+        symmetric=True,
+        constraints=[
+            RQLConstraint("NOT S identity O"),
+            # conflicting constraints, see cw_unrelated_rql tests in
+            # unittest_entity.py
+            RQLVocabularyConstraint('NOT (S connait P, P nom "toto")'),
+            RQLVocabularyConstraint('S travaille P, P nom "tutu"'),
+        ],
+    )
+    actionnaire = SubjectRelation(
+        "Societe",
+        cardinality="??",
+        constraints=[RQLConstraint("NOT EXISTS(O contrat_exclusif S)")],
+    )
+    dirige = SubjectRelation(
+        "Societe", cardinality="??", constraints=[RQLConstraint("S actionnaire O")]
+    )
+    associe = SubjectRelation(
+        "Personne",
+        cardinality="?*",
+        constraints=[RQLConstraint("S actionnaire SOC, O actionnaire SOC")],
+    )
 
 
 class connait(RelationDefinition):
     subject = "CWUser"
     object = "Personne"
 
 
 class Societe(EntityType):
-    nom = String(maxsize=64, fulltextindexed=True)
+    nom = String(fulltextindexed=True)
     web = String(maxsize=128)
     type = String(maxsize=128)  # attribute in common with Note
     tel = Int()
     fax = Int()
     rncs = String(maxsize=128)
     ad1 = String(maxsize=128)
     ad2 = String(maxsize=128)
     ad3 = String(maxsize=128)
     cp = String(maxsize=12)
     ville = String(maxsize=32)
+    evaluee = SubjectRelation("Note")
+    fournit = SubjectRelation(("Service", "Produit"), cardinality="1*")
+    contrat_exclusif = SubjectRelation("Personne", cardinality="??")
 
 
 # enough relations to cover most reledit use cases
 class Project(EntityType):
     __permissions__ = {
         "read": ("managers", "users", "guests"),
         "add": ("managers", "validators", "contributors"),
@@ -200,7 +237,91 @@
     name = String(required=True)
     filed_under = SubjectRelation("Folder", description=_("parent folder"))
 
 
 class TreeNode(EntityType):
     name = String(required=True)
     parent = SubjectRelation("TreeNode", cardinality="?*")
+
+
+class Note(EntityType):
+    type = String()
+    ecrit_par = SubjectRelation("Personne")
+
+
+class SubNote(Note):
+    __specializes_schema__ = True
+    description = String()
+
+
+class buddies(ComputedRelation):
+    rule = "S in_group G, O in_group G"
+
+
+class Ami(EntityType):
+    """A Person, for which surname is not required"""
+
+    prenom = String()
+    nom = String()
+
+
+class Ville(EntityType):
+    insee = Int(required=True)
+
+
+class Service(EntityType):
+    fabrique_par = SubjectRelation("Personne", cardinality="1*")
+
+
+class Produit(EntityType):
+    fabrique_par = SubjectRelation("Usine", cardinality="1*", inlined=True)
+
+
+class Usine(EntityType):
+    lieu = String(required=True)
+
+
+class evaluee(RelationDefinition):
+    subject = "CWUser"
+    object = "Note"
+
+
+class StateFull(WorkflowableEntityType):
+    name = String()
+
+
+class Reference(EntityType):
+    nom = String(unique=True)
+    ean = String(unique=True, required=True)
+
+
+class FakeFile(EntityType):
+    title = String(fulltextindexed=True, maxsize=256)
+    data = Bytes(required=True, fulltextindexed=True, description=_("file to upload"))
+    data_format = String(
+        required=True,
+        maxsize=128,
+        description=_(
+            "MIME type of the file. Should be dynamically set at upload time."
+        ),
+    )
+    data_encoding = String(
+        maxsize=32,
+        description=_(
+            "encoding of the file when it applies (e.g. text). "
+            "Should be dynamically set at upload time."
+        ),
+    )
+    data_name = String(
+        required=True,
+        fulltextindexed=True,
+        description=_("name of the file. Should be dynamically set at upload time."),
+    )
+    description = RichString(
+        fulltextindexed=True, internationalizable=True, default_format="text/rest"
+    )
+
+
+class Company(EntityType):
+    order = Int()
+    name = String()
+    description = RichString()
```

### Comparing `cubicweb-web-0.3.1/test/data/views.py` & `cubicweb-web-1.0.0/test/data/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,34 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 import hashlib
 
-from cubicweb.predicates import has_related_entities
+from cubicweb_web.views import tableview
+from cubicweb.server import Service
+from cubicweb.predicates import has_related_entities, match_user_groups
+
 from cubicweb_web.views.ajaxcontroller import ajaxfunc
 from cubicweb_web.views.ibreadcrumbs import IBreadCrumbsAdapter
+from cubicweb_web.views import xmlrss
+
+
+xmlrss.RSSIconBox.visible = True
+
+
+class TestService(Service):
+    __regid__ = "test_service"
+    __select__ = Service.__select__ & match_user_groups("managers")
+    passed_here = []
+
+    def call(self, msg):
+        self.passed_here.append(msg)
+        return "babar"
 
 
 def _recursive_replace_stream_by_md5(tree):
     """Search for streams (i.e. object that have a 'read' method) in a tree
     (whose branches are lists or tuples), and substitute them by their md5 hash,
     leaving other leafs identical. A copy of the tree with only lists as
     branches is returned.
@@ -56,7 +73,11 @@
 
 
 class FolderIBreadCrumbsAdapter(IBreadCrumbsAdapter):
     __select__ = IBreadCrumbsAdapter.__select__ & has_related_entities("filed_under")
 
     def parent_entity(self):
         return self.entity.filed_under[0]
+
+
+class CustomRsetTableView(tableview.RsetTableView):
+    __regid__ = "mytable"
```

### Comparing `cubicweb-web-0.3.1/test/test_application.py` & `cubicweb-web-1.0.0/test/test_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,24 @@
 """unit tests for cubicweb.web.application"""
 
 import base64
 import http.client
 from http.cookies import SimpleCookie
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.fake import FakeRequest
 from cubicweb.devtools.testlib import real_error_handling
 from logilab.common.decorators import clear_cache
 from logilab.common.testlib import TestCase, unittest_main
 
 from cubicweb_web import LogOut, Redirect, INTERNAL_FIELD_VALUE
 from cubicweb_web import view
 from cubicweb_web.application import anonymized_request
+from cubicweb_web.devtools.testlib import FakeRequest, PyramidWebCWTC
 from cubicweb_web.views.basecontrollers import ViewController
 from cubicweb_web.views.urlrewrite import SimpleReqRewriter, rgx
-from test import WebCWTC
 
 
 class FakeMapping:
     """emulates a mapping module"""
 
     def __init__(self):
         self.ENTITIES_MAP = {}
@@ -146,15 +145,15 @@
         self.ctrl.execute_linkto(eid=8)
         self.assertEqual(
             self.ctrl._cursor.executed,
             ["SET X works_for Y WHERE X eid 8, Y eid %s" % i for i in (12, 13, 14)],
         )
 
 
-class ApplicationTC(WebCWTC):
+class ApplicationTC(PyramidWebCWTC):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.config.global_set_option("allow-email-login", True)
 
     def test_cnx_user_groups_sync(self):
         with self.admin_access.client_cnx() as cnx:
```

### Comparing `cubicweb-web-0.3.1/test/test_breadcrumbs.py` & `cubicweb-web-1.0.0/test/test_breadcrumbs.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
 
+from cubicweb_web.devtools.testlib import WebCWTC
 
-class BreadCrumbsTC(CubicWebTC):
+
+class BreadCrumbsCWTC(WebCWTC):
     def test_base(self):
         with self.admin_access.web_request() as req:
             f1 = req.create_entity("Folder", name="par&ent")
             f2 = req.create_entity("Folder", name="chi&ld")
             req.cnx.execute(
                 "SET F2 filed_under F1 WHERE F1 eid %(f1)s, F2 eid %(f2)s",
                 {"f1": f1.eid, "f2": f2.eid},
```

### Comparing `cubicweb-web-0.3.1/test/test_bw_request.py` & `cubicweb-web-1.0.0/test/test_bw_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from io import BytesIO
 
 import pyramid.request
 import webtest
 
-from cubicweb.pyramid.test import PyramidCWTest
-
 from cubicweb_web.bwcompat import CubicWebPyramidRequest
+from cubicweb_web.devtools.testlib import PyramidWebCWTC
 
 
-class WSGIAppTest(PyramidCWTest):
+class WSGIAppTest(PyramidWebCWTC):
     def make_request(self, path, environ=None, **kw):
         r = webtest.app.TestRequest.blank(path, environ, **kw)
 
         request = pyramid.request.Request(r.environ)
         request.registry = self.pyr_registry
 
         return request
```

### Comparing `cubicweb-web-0.3.1/test/test_controller.py` & `cubicweb-web-1.0.0/test/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 """
 
 from datetime import datetime, date, time
 
 from logilab.common.testlib import unittest_main
 
-from cubicweb.devtools import testlib
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class BaseControllerTC(testlib.CubicWebTC):
+class BaseControllerCWTC(WebCWTC):
     def test_parse_datetime_ok(self):
         with self.admin_access.web_request() as req:
             ctrl = self.vreg["controllers"].select("view", req)
             pd = ctrl._cw.parse_datetime
             self.assertIsInstance(pd("2006/06/24 12:18"), datetime)
             self.assertIsInstance(pd("2006/06/24"), date)
             self.assertIsInstance(pd("2006/06/24 12:18", "Datetime"), datetime)
```

### Comparing `cubicweb-web-0.3.1/test/test_facet.py` & `cubicweb-web-1.0.0/test/test_facet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from logilab.common.date import datetime2ticks
 
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb_web import facet
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class BaseFacetTC(CubicWebTC):
+class BaseFacetCWTC(WebCWTC):
     def prepare_rqlst(
         self,
         req,
         rql="CWUser X",
         mainvar="X",
         expected_baserql="Any X WHERE X is CWUser",
         expected_preparedrql="DISTINCT Any  WHERE X is CWUser",
```

### Comparing `cubicweb-web-0.3.1/test/test_form.py` & `cubicweb-web-1.0.0/test/test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from datetime import datetime
 
 import pytz
 from lxml import html
 
 from cubicweb import Binary, ValidationError
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.formfields import (
     IntField,
     StringField,
     RichTextField,
     PasswordField,
     DateTimeField,
     FileField,
@@ -37,15 +38,15 @@
 )
 from cubicweb_web.formwidgets import DateTimePicker, JQueryDateTimePicker
 from cubicweb_web.views.formrenderers import FormRenderer
 from cubicweb_web.views.forms import EntityFieldsForm, FieldsForm
 from cubicweb_web.views.workflow import ChangeStateForm
 
 
-class FieldsFormTC(CubicWebTC):
+class FieldsFormCWTC(WebCWTC):
     def test_form_field_format(self):
         with self.admin_access.web_request() as req:
             form = FieldsForm(req, None)
             self.assertEqual(StringField().format(form), "text/plain")
             req.cnx.execute(
                 'INSERT CWProperty X: X pkey "ui.default-text-format", X value "text/rest", X for_user U WHERE U login "admin"'
             )
@@ -78,15 +79,15 @@
         ) as req:
             self._cw = req
             self.formvalues = {}
             date = widget.process_field_data(self, field)
             self.assertIsNone(date)
 
 
-class EntityFieldsFormTC(CubicWebTC):
+class EntityFieldsFormCWTC(WebCWTC):
     def test_form_field_choices(self):
         with self.admin_access.web_request() as req:
             b = req.create_entity(
                 "BlogEntry", title="di mascii code", content="a best-seller"
             )
             t = req.create_entity("Tag", name="x")
             form1 = self.vreg["forms"].select("edition", req, entity=t)
```

### Comparing `cubicweb-web-0.3.1/test/test_formfields.py` & `cubicweb-web-1.0.0/test/test_formfields.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """unittests for cw.web.formfields"""
 
 from logilab.common.testlib import TestCase, unittest_main, mock_object as mock
 
 import cubicweb
-from cubicweb import devtools
-from cubicweb.devtools.testlib import CubicWebTC
+
+from cubicweb_web.devtools.testlib import WebCWTC, WebApptestConfiguration
 from cubicweb_web.formfields import (
     guess_field,
     StringField,
     RichTextField,
     DateTimeField,
     RelationField,
     FileField,
@@ -38,20 +38,20 @@
 )
 from cubicweb_web.formwidgets import PasswordInput, Select, Radio
 from cubicweb_web.views.forms import EntityFieldsForm, FieldsForm
 
 
 def setUpModule(*args):
     global schema
-    config = devtools.TestServerConfiguration("data", __file__)
+    config = WebApptestConfiguration("data", __file__)
     config.bootstrap_cubes()
     schema = config.load_schema()
 
 
-class GuessFieldTC(CubicWebTC):
+class GuessFieldCWTC(WebCWTC):
     def test_state_fields(self):
         with self.admin_access.web_request() as req:
             title_field = guess_field(schema["State"], schema["name"], req=req)
             self.assertIsInstance(title_field, StringField)
             self.assertEqual(title_field.required, True)
 
         with self.admin_access.web_request() as req:
@@ -151,15 +151,15 @@
             self.assertIsInstance(field.widget, Radio)
             self.assertEqual(
                 field.vocabulary(mock(req=mock(_=cubicweb._))),
                 [("maybe", "1"), ("no", "")],
             )
 
 
-class MoreFieldsTC(CubicWebTC):
+class MoreFieldsCWTC(WebCWTC):
     def test_rtf_format_field(self):
         with self.admin_access.web_request() as req:
             req.use_fckeditor = lambda: False
             e = self.vreg["etypes"].etype_class("State")(req)
             form = EntityFieldsForm(req, entity=e)
             description_field = guess_field(schema["State"], schema["description"])
             description_format_field = description_field.get_format_field(form)
@@ -186,15 +186,15 @@
             e = self.vreg["etypes"].etype_class("CWProperty")(req)
             renderer = self.vreg["formrenderers"].select("base", req)
             form = EntityFieldsForm(req, entity=e)
             form.formvalues = {}
             field.render(form, renderer)
 
 
-class CompoundFieldTC(CubicWebTC):
+class CompoundFieldCWTC(WebCWTC):
     def test_multipart(self):
         """Ensures that compound forms have needs_multipart set if their children require it"""
 
         class AForm(FieldsForm):
             comp = CompoundField([IntField(), StringField()])
 
         with self.admin_access.web_request() as req:
```

### Comparing `cubicweb-web-0.3.1/test/test_formwidgets.py` & `cubicweb-web-1.0.0/test/test_formwidgets.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """unittests for cw.web.formwidgets"""
 
 from logilab.common.testlib import unittest_main, mock_object as mock
 
-from cubicweb.devtools import fake
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb_web import formwidgets, formfields
+from cubicweb_web.devtools.testlib import WebCWTC, FakeRequest
 from cubicweb_web.views.forms import FieldsForm
 
 
-class WidgetsTC(CubicWebTC):
+class WidgetsCWTC(WebCWTC):
     def test_editableurl_widget(self):
         field = formfields.guess_field(self.schema["Bookmark"], self.schema["path"])
         widget = formwidgets.EditableURLWidget()
-        req = fake.FakeRequest(form={"path-subjectfqs:A": "param=value&vid=view"})
+        req = FakeRequest(form={"path-subjectfqs:A": "param=value&vid=view"})
         form = mock(_cw=req, formvalues={}, edited_entity=mock(eid="A"))
         self.assertEqual(
             widget.process_field_data(form, field), "?param=value%26vid%3Dview"
         )
 
     def test_bitselect_widget(self):
         field = formfields.guess_field(
@@ -46,15 +45,15 @@
             ),
             (
                 "deux",
                 "2",
             ),
         ]
         widget = formwidgets.BitSelect()
-        req = fake.FakeRequest(form={"ordernum-subject:A": ["1", "2"]})
+        req = FakeRequest(form={"ordernum-subject:A": ["1", "2"]})
         form = mock(
             _cw=req, formvalues={}, edited_entity=mock(eid="A"), form_previous_values=()
         )
         self.assertMultiLineEqual(
             widget._render(form, field, None),
             """\
 <select id="ordernum-subject:A" multiple="multiple" name="ordernum-subject:A" size="2">
```

### Comparing `cubicweb-web-0.3.1/test/test_http.py` & `cubicweb-web-1.0.0/test/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common.testlib import TestCase, unittest_main, tag, Tags
 
-from cubicweb.devtools.fake import FakeRequest
+from cubicweb_web.devtools.testlib import FakeRequest
 
 
 def _test_cache(hin, hout, method="GET"):
     """forge and process an HTTP request using given headers in/out and method,
     then return it once its .is_client_cache_valid() method has been called.
 
     req.status_out is None if the page should have been calculated.
```

### Comparing `cubicweb-web-0.3.1/test/test_http_headers.py` & `cubicweb-web-1.0.0/test/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_idownloadable.py` & `cubicweb-web-1.0.0/test/test_idownloadable.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from datetime import datetime
 from functools import partial
 
 from pytz import utc
 
-from cubicweb.devtools.testlib import CubicWebTC, real_error_handling
+from cubicweb.devtools.testlib import real_error_handling
 from cubicweb.entity import EntityAdapter
 from cubicweb.predicates import is_instance
 from cubicweb_web import http_headers
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
 class IDownloadableUser(EntityAdapter):
     __regid__ = "IDownloadable"
     __select__ = is_instance("CWUser")
 
     def download_content_type(self):
@@ -54,15 +55,15 @@
     def download_file_name(self):
         return self.entity.name + ".txt"
 
     def download_data(self):
         raise OSError()
 
 
-class IDownloadableTC(CubicWebTC):
+class IDownloadableCWTC(WebCWTC):
     def setUp(self):
         super().setUp()
         self.vreg.register(IDownloadableUser)
         self.addCleanup(partial(self.vreg.unregister, IDownloadableUser))
 
     def test_header_simple_case(self):
         with self.admin_access.web_request() as req:
```

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/data/test_htmlhelpers.html` & `cubicweb-web-1.0.0/test/test_js_scripts/data/test_htmlhelpers.html`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/data/test_utils.html` & `cubicweb-web-1.0.0/test/test_js_scripts/data/test_utils.html`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/jest.config.js` & `cubicweb-web-1.0.0/test/test_js_scripts/jest.config.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/package-lock.json` & `cubicweb-web-1.0.0/test/test_js_scripts/package-lock.json`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/test/ajax.test.js` & `cubicweb-web-1.0.0/test/test_js_scripts/test/ajax.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/test/htmlhelpers.test.js` & `cubicweb-web-1.0.0/test/test_js_scripts/test/htmlhelpers.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/test/utils.js` & `cubicweb-web-1.0.0/test/test_js_scripts/test/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_js_scripts/test/utils.test.js` & `cubicweb-web-1.0.0/test/test_js_scripts/test/utils.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_magicsearch.py` & `cubicweb-web-1.0.0/test/test_magicsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """Unit tests for cw.web.views.magicsearch"""
 
 from contextlib import contextmanager
 
 from logilab.common.testlib import unittest_main
 from rql import BadRQLQuery, RQLSyntaxError
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views.magicsearch import (
     QSPreProcessor,
     QueryTranslator,
 )
 
 translations = {
     "CWUser": "Utilisateur",
@@ -45,15 +45,15 @@
     return translations.get(msgid, msgid)
 
 
 def _ctxtranslate(ctx, msgid):
     return _translate(msgid)
 
 
-class QueryTranslatorTC(CubicWebTC):
+class QueryTranslatorCWTC(WebCWTC):
     """test suite for QueryTranslatorTC"""
 
     @contextmanager
     def proc(self):
         with self.admin_access.web_request() as req:
             self.vreg.config.translations = {"en": (_translate, _ctxtranslate)}
             proc = self.vreg["components"].select("magicsearch", req)
@@ -80,15 +80,15 @@
             rql = "Any P WHERE P is Utilisateur, P adel C, P nom 'Smith'"
             (rql,) = proc.preprocess_query(rql)
             self.assertEqual(
                 rql, 'Any P WHERE P is CWUser, P use_email C, P surname "Smith"'
             )
 
 
-class QSPreProcessorTC(CubicWebTC):
+class QSPreProcessorCWTC(WebCWTC):
     """test suite for QSPreProcessor"""
 
     @contextmanager
     def proc(self):
         self.vreg.config.translations = {"en": (_translate, _ctxtranslate)}
         with self.admin_access.web_request() as req:
             proc = self.vreg["components"].select("magicsearch", req)
@@ -266,15 +266,15 @@
                 BadRQLQuery, proc.preprocess_query, "Any X WHERE X is Something"
             )
 
 
 # Processor Chains tests ############################################
 
 
-class ProcessorChainTC(CubicWebTC):
+class ProcessorChainCWTC(WebCWTC):
     """test suite for magic_search's processor chains"""
 
     @contextmanager
     def proc(self):
         self.vreg.config.translations = {"en": (_translate, _ctxtranslate)}
         with self.admin_access.web_request() as req:
             proc = self.vreg["components"].select("magicsearch", req)
```

### Comparing `cubicweb-web-0.3.1/test/test_propertysheet.py` & `cubicweb-web-1.0.0/test/test_propertysheet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_reledit.py` & `cubicweb-web-1.0.0/test/test_reledit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,31 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """
 mainly regression-preventing tests for reledit views
 """
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views.uicfg import reledit_ctrl
 
 
 class ReleditMixinTC:
     def setup_database(self):
         with self.admin_access.client_cnx() as cnx:
             self.proj = cnx.create_entity(
                 "Project", title="cubicweb-world-domination"
             ).eid
             self.tick = cnx.create_entity("Ticket", title="write the code").eid
             self.toto = cnx.create_entity("Personne", nom="Toto").eid
             cnx.commit()
 
 
-class ClickAndEditFormTC(ReleditMixinTC, CubicWebTC):
+class ClickAndEditFormCWTC(ReleditMixinTC, WebCWTC):
     def setup_database(self):
         super().setup_database()
         with self.admin_access.client_cnx() as cnx:
             cnx.create_entity("CWGroup", name="validators")
             cnx.create_entity("CWGroup", name="contributors")
 
             self.create_user(
@@ -241,15 +242,15 @@
                     role=role,
                     formid="edition" if rtype == "long_desc" else "base",
                 ),
                 rtype,
             )
 
 
-class ClickAndEditFormUICFGTC(ReleditMixinTC, CubicWebTC):
+class ClickAndEditFormUICFGTC(ReleditMixinTC, WebCWTC):
     def setup_database(self):
         super().setup_database()
         with self.admin_access.client_cnx() as cnx:
             cnx.execute(
                 "SET T concerns P WHERE T eid %(t)s, P eid %(p)s",
                 {"t": self.tick, "p": self.proj},
             )
@@ -295,15 +296,19 @@
                 include_final=True
             ):
                 if rschema not in reledit:
                     continue
                 rtype = rschema.type
                 self.assertMultiLineEqual(
                     reledit[rtype]
-                    % {"eid": self.proj, "toto": self.toto, "tick": self.tick},
+                    % {
+                        "eid": self.proj,
+                        "toto": req.cnx.entity_from_eid(self.toto).nom,
+                        "tick": self.tick,
+                    },
                     proj.view("reledit", rtype=rtype, role=role),
                     rtype,
                 )
         reledit_ctrl.clear()
         reledit_ctrl._tagdefs.update(old_rctl)
```

### Comparing `cubicweb-web-0.3.1/test/test_request.py` & `cubicweb-web-1.0.0/test/test_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """misc. unittests for utility functions
 """
 
 import unittest
 from functools import partial
 
+from cubicweb import ObjectNotFound
 from cubicweb.devtools import BASE_URL
 from cubicweb.devtools.fake import FakeConfig, FakeCWRegistryStore
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.request import (
     CubicWebRequestBase,
     _parse_accept_header,
     _mimetype_sort_key,
     _mimetype_parser,
     _charset_sort_key,
 )
@@ -142,9 +145,17 @@
         self.assertEqual(req.build_url(), f"{BASE_URL}view")
         self.assertEqual(req.build_url("foo"), f"{BASE_URL}foo")
         req.set_language("fr")
         self.assertEqual(req.build_url(), f"{BASE_URL}view")
         self.assertEqual(req.build_url("foo"), f"{BASE_URL}foo")
 
 
+class RequestCWTC(WebCWTC):
+    def test_view_catch_ex(self):
+        with self.admin_access.web_request() as req:
+            rset = req.execute('CWUser X WHERE X login "hop"')
+            self.assertEqual(req.view("oneline", rset, "null"), "")
+            self.assertRaises(ObjectNotFound, req.view, "onelinee", rset, "null")
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cubicweb-web-0.3.1/test/test_uicfg.py` & `cubicweb-web-1.0.0/test/test_uicfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 import copy
 import warnings
 
 from yams.buildobjs import RelationDefinition, EntityType
 
-from cubicweb.devtools.testlib import CubicWebTC, BaseTestCase
+from cubicweb.devtools.testlib import BaseTestCase
 from cubicweb.schema import build_schema_from_namespace
 from cubicweb_web import uihelper, formwidgets as fwdgs
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views import uicfg
 
 abaa = uicfg.actionbox_appearsin_addmenu
 
 
-class UICFGTC(CubicWebTC):
+class UICFGTC(WebCWTC):
     def test_default_actionbox_appearsin_addmenu_config(self):
         self.assertFalse(abaa.etype_get("TrInfo", "wf_info_for", "object", "CWUser"))
 
 
-class DefinitionOrderTC(CubicWebTC):
+class DefinitionOrderCWTC(WebCWTC):
     """This test check that when multiple definition could match a key, only
     the more accurate apply"""
 
     def setUp(self):
         super().setUp()
         for rtag in (uicfg.autoform_section, uicfg.autoform_field_kwargs):
             rtag._old_tagdefs = copy.deepcopy(rtag._tagdefs)
@@ -137,15 +138,15 @@
         section_conf = uicfg.autoform_section.get("CWUser", "in_group", "*", "subject")
         self.assertCountEqual(section_conf, ["main_hidden", "muledit_attributes"])
         self.assertEqual(
             afk_get("CWUser", "firstname", "String", "subject"), {"order": 1}
         )
 
 
-class UicfgRegistryTC(CubicWebTC):
+class UicfgRegistryCWTC(WebCWTC):
     def test_default_uicfg_object(self):
         "CW default ui config objects must be registered in uicfg registry"
         onames = ("autoform_field", "autoform_section", "autoform_field_kwargs")
         for oname in onames:
             obj = self.vreg["uicfg"].select_or_none(oname)
             self.assertTrue(obj is not None, "%s not found in uicfg registry" % oname)
```

### Comparing `cubicweb-web-0.3.1/test/test_urlpublisher.py` & `cubicweb-web-1.0.0/test/test_urlpublisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """Unit tests for url publishing service"""
 
 import re
 
 from logilab.common.testlib import unittest_main
 
-from cubicweb.devtools.fake import FakeRequest
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.rset import ResultSet
 from cubicweb_web import NotFound, Redirect, views
+from cubicweb_web.devtools.testlib import WebCWTC, FakeRequest
 from cubicweb_web.views.urlrewrite import SimpleReqRewriter
 
 
-class URLPublisherTC(CubicWebTC):
+class URLPublisherCWTC(WebCWTC):
     """test suite for QSPreProcessor"""
 
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             self.create_user(cnx, "ÿsaÿe")
             b = cnx.create_entity("BlogEntry", title="hell'o", content="blabla")
             # take care: Tag's name normalized to lower case
```

### Comparing `cubicweb-web-0.3.1/test/test_urlrewrite.py` & `cubicweb-web-1.0.0/test/test_urlrewrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common import tempattr
 
-from cubicweb.devtools.fake import FakeRequest
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC, FakeRequest
 from cubicweb_web.views.urlrewrite import (
     SimpleReqRewriter,
     SchemaBasedRewriter,
     rgx,
     rgx_action,
 )
 
 
-class UrlRewriteTC(CubicWebTC):
+class UrlRewriteCWTC(WebCWTC):
     def test_auto_extend_rules(self):
         class Rewriter(SimpleReqRewriter):
             rules = [
                 ("foo", dict(rql="Foo F")),
                 ("/index", dict(vid="index2")),
             ]
 
@@ -138,15 +137,15 @@
                     )
                     self.assertEqual(ctrlid, "view")
                     self.assertEqual(x.eid, rset[0][0])
             finally:
                 del BaseTransition._cw_rest_attr_info_cache_
 
 
-class RgxActionRewriteTC(CubicWebTC):
+class RgxActionRewriteCWTC(WebCWTC):
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             p1 = self.create_user(cnx, "user1")
             p1.cw_set(firstname="joe", surname="Dalton")
             p2 = self.create_user(cnx, "user2")
             p2.cw_set(firstname="jack", surname="Dalton")
             self.p1eid = p1.eid
```

### Comparing `cubicweb-web-0.3.1/test/test_views_actions.py` & `cubicweb-web-1.0.0/test/test_views_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common.testlib import unittest_main
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views import actions
 
 
-class ActionsTC(CubicWebTC):
+class ActionsCWTC(WebCWTC):
     def test_view_action(self):
         with self.admin_access.web_request(vid="rss", rql="CWUser X") as req:
             rset = req.execute("CWUser X")
             actions = self.vreg["actions"].poss_visible_objects(req, rset=rset)
             vaction = [action for action in actions if action.__regid__ == "view"][0]
             self.assertEqual(vaction.url(), f"{BASE_URL}view?rql=CWUser%20X")
```

### Comparing `cubicweb-web-0.3.1/test/test_views_apacherewrite.py` & `cubicweb-web-1.0.0/test/test_views_apacherewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test/test_views_basecontrollers.py` & `cubicweb-web-1.0.0/test/test_views_basecontrollers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 
 import time
 from urllib.parse import urlsplit, urlunsplit, urljoin, parse_qs
 
 import lxml
 from cubicweb import Binary, NoSelectableObject, ValidationError, transaction as tx
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.predicates import is_instance
 from cubicweb.schema import RRQLExpression
 from cubicweb.server.hook import Hook, Operation
 from cubicweb.server.session import Connection
 from cubicweb.uilib import rql_for_eid
 from cubicweb.utils import json_dumps
 from logilab.common.testlib import unittest_main
 
 from cubicweb_web import Redirect, RemoteCallFailed, http_headers, formfields as ff
+from cubicweb_web.devtools.testlib import WebCWTC, PyramidWebCWTC
 from cubicweb_web.views.ajaxcontroller import ajaxfunc, AjaxFunction
 from cubicweb_web.views.autoform import get_pending_inserts, get_pending_deletes
-from test import WebCWTC
 
 
-class ViewControllerTC(WebCWTC):
+class ViewControllerTC(PyramidWebCWTC):
     def test_view_ctrl_with_valid_cache_headers(self):
         now = time.time()
         resp = self.webapp.get("/manage")
         self.assertEqual(resp.etag, "manage/guests")
         self.assertEqual(resp.status_code, 200)
         self.assertGreaterEqual(
             http_headers.parseDateTime(resp.headers["Last-Modified"]), int(now)
@@ -60,23 +59,23 @@
     return {
         "eid": [str(user.eid)],
         "_cw_entity_fields:%s" % user.eid: "_cw_generic_field",
         "__type:%s" % user.eid: user.__regid__,
     }
 
 
-class EditControllerTC(WebCWTC):
+class EditControllerTC(PyramidWebCWTC):
     def setUp(self):
-        CubicWebTC.setUp(self)
+        WebCWTC.setUp(self)
         self.assertIn(
             "users", self.schema.entity_schema_for("CWGroup").get_groups("read")
         )
 
     def tearDown(self):
-        CubicWebTC.tearDown(self)
+        WebCWTC.tearDown(self)
         self.assertIn(
             "users", self.schema.entity_schema_for("CWGroup").get_groups("read")
         )
 
     def test_noparam_edit(self):
         """check behaviour of this controller without any form parameter"""
         with self.admin_access.web_request() as req:
@@ -925,29 +924,28 @@
                     values_by_eid["X"]
                 )  # #3064653 raise ValidationError
                 editctrl.edit_entity(values_by_eid["Y"])
             finally:
                 self.schema["described_by_test"].inlined = False
 
 
-class ReportBugControllerTC(CubicWebTC):
+class ReportBugControllerTC(WebCWTC):
     def test_usable_by_guest(self):
         with self.new_access("anon").web_request() as req:
             self.assertRaises(
                 NoSelectableObject, self.vreg["controllers"].select, "reportbug", req
             )
         with self.new_access("anon").web_request(description="hop") as req:
             self.vreg["controllers"].select("reportbug", req)
 
 
-class AjaxControllerTC(CubicWebTC):
+class AjaxControllerTC(WebCWTC):
     tested_controller = "ajax"
 
-    def ctrl(self, req=None):
-        req = req or self.request(url="http://whatever.fr/")
+    def ctrl(self, req):
         return self.vreg["controllers"].select(self.tested_controller, req)
 
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             self.pytag = cnx.create_entity("Tag", name="python")
             self.cubicwebtag = cnx.create_entity("Tag", name="cubicweb")
             self.john = self.create_user(cnx, "John")
@@ -1158,15 +1156,15 @@
         with self.assertRaises(RemoteCallFailed) as cm:
             with self.remote_calling("foo"):
                 pass
         self.assertEqual(cm.exception.status, 400)
         self.assertEqual(cm.exception.reason, "no foo method")
 
 
-class UndoControllerTC(CubicWebTC):
+class UndoControllerTC(WebCWTC):
     def setUp(self):
         # Force undo feature to be turned on
         Connection.undo_actions = property(lambda self: True, lambda self, v: None)
         super().setUp()
 
     def tearDown(self):
         super().tearDown()
@@ -1214,30 +1212,30 @@
             req.form["__redirectpath"] = rpath
             controller = self.vreg["controllers"].select("undo", req)
             with self.assertRaises(Redirect) as cm:
                 controller.publish(rset=None)
             self.assertURLPath(cm.exception.location, rpath)
 
 
-class LoginControllerTC(CubicWebTC):
+class LoginControllerTC(WebCWTC):
     def test_login_with_dest(self):
         with self.admin_access.web_request() as req:
             req.form = {"postlogin_path": "elephants/babar"}
             with self.assertRaises(Redirect) as cm:
                 self.ctrl_publish(req, ctrl="login")
             self.assertEqual(req.build_url("elephants/babar"), cm.exception.location)
 
     def test_login_no_dest(self):
         with self.admin_access.web_request() as req:
             with self.assertRaises(Redirect) as cm:
                 self.ctrl_publish(req, ctrl="login")
             self.assertEqual(req.base_url(), cm.exception.location)
 
 
-class LoginControllerHTTPTC(WebCWTC):
+class LoginControllerHTTPTC(PyramidWebCWTC):
     anonymous_allowed = True
     # this TC depends on the auth mode being 'cookie' and not 'http'
     # (the former being the default, so everything works)
 
     def test_http_error_codes_auth_fail(self):
         response = self.webapp.login(user="toto", password="pouetA", status=403)
         self.assertEqual(response.status_code, 403)
```

### Comparing `cubicweb-web-0.3.1/test/test_views_basetemplates.py` & `cubicweb-web-1.0.0/test/test_views_basetemplates.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from cubicweb.devtools.htmlparser import XMLValidator
-from cubicweb.devtools.testlib import CubicWebTC
 
+from cubicweb_web.devtools.testlib import WebCWTC
 
-class LogFormTemplateTC(CubicWebTC):
+
+class LogFormTemplateCWTC(WebCWTC):
     def _login_labels(self):
         valid = self.content_type_validators.get("text/html", XMLValidator)()
         req = self.requestcls(self.vreg, url="login")
         page = valid.parse_string(self.vreg["views"].main_template(req, "login"))
         return page.find_tag("label")
 
     def test_label(self):
@@ -36,15 +37,15 @@
     def test_display_message(self):
         with self.admin_access.web_request() as req:
             req.set_message("houla hop")
             page = self.view("logform", req=req, id="loginBox", klass="", template=None)
             self.assertIn("houla hop", page.raw_text)
 
 
-class MainNoTopTemplateTC(CubicWebTC):
+class MainNoTopTemplateCWTC(WebCWTC):
     def test_valid_xhtml(self):
         with self.admin_access.web_request() as req:
             self.view("index", template="main-no-top", req=req)
 
 
 if __name__ == "__main__":
     from logilab.common.testlib import unittest_main
```

### Comparing `cubicweb-web-0.3.1/test/test_views_baseviews.py` & `cubicweb-web-1.0.0/test/test_views_baseviews.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common.testlib import unittest_main
 from logilab.mtconverter import html_unescape
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.utils import json
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.view import StartupView, TRANSITIONAL_DOCTYPE
 from cubicweb_web.views import vid_from_rset
 
 
 def loadjson(value):
     return json.loads(html_unescape(value))
 
 
-class VidFromRsetTC(CubicWebTC):
+class VidFromRsetCWTC(WebCWTC):
     def test_no_rset(self):
         with self.admin_access.web_request() as req:
             self.assertEqual(vid_from_rset(req, None, self.schema), "index")
 
     def test_no_entity(self):
         with self.admin_access.web_request() as req:
             rset = req.execute('Any X WHERE X login "blabla"')
@@ -94,15 +95,15 @@
                 "     (DISTINCT Any P,N WHERE P is CWUser, P login N)"
                 "       UNION"
                 "     (DISTINCT Any W,N WHERE W is CWGroup, W name N))"
             )
             self.assertEqual(vid_from_rset(req, rset, self.schema), "table")
 
 
-class TableViewTC(CubicWebTC):
+class TableViewCWTC(WebCWTC):
     def _prepare_entity(self, req):
         e = req.create_entity("State", name="<toto>", description='loo"ong blabla')
         rset = req.execute(
             "Any X, D, CD, NOW - CD WHERE X is State, "
             "X description D, X creation_date CD, X eid %(x)s",
             {"x": e.eid},
         )
@@ -115,15 +116,15 @@
             colrenderers = view.build_column_renderers()[:3]
             self.assertListEqual(
                 [renderer.sortvalue(0) for renderer in colrenderers],
                 ["<toto>", 'loo"ong blabla', e.creation_date],
             )
 
 
-class HTMLStreamTests(CubicWebTC):
+class HTMLStreamTests(WebCWTC):
     def test_set_doctype_reset_xmldecl(self):
         """
         tests `cubicweb.web.request.CubicWebRequestBase.set_doctype`
         with xmldecl reset
         """
 
         class MyView(StartupView):
@@ -176,15 +177,15 @@
                         b'<html xmlns:cubicweb="http://www.cubicweb.org" lang="cz">',
                         b"<head>",
                     ],
                     source_lines[:3],
                 )
 
 
-class BaseViewsTC(CubicWebTC):
+class BaseViewsCWTC(WebCWTC):
     def test_null(self):
         with self.admin_access.web_request() as req:
             rset = req.execute('Any X WHERE X login "admin"')
             result = req.view("null", rset)
             self.assertEqual(result, "")
 
     def test_final(self):
```

### Comparing `cubicweb-web-0.3.1/test/test_views_csv.py` & `cubicweb-web-1.0.0/test/test_views_csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 # CubicWeb is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
+from cubicweb_web.devtools.testlib import WebCWTC
 
-from cubicweb.devtools.testlib import CubicWebTC
 
-
-class CSVExportViewsTC(CubicWebTC):
+class CSVExportViewsCWTC(WebCWTC):
     def test_csvexport(self):
         with self.admin_access.web_request() as req:
             rset = req.execute(
                 "Any GN,COUNT(X) GROUPBY GN ORDERBY GN " "WHERE X in_group G, G name GN"
             )
             data = self.view("csvexport", rset, req=req)
             self.assertEqual(
```

### Comparing `cubicweb-web-0.3.1/test/test_views_cwsources.py` & `cubicweb-web-1.0.0/test/test_views_cwsources.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from cubicweb.server.sources import datafeed
 from logilab.common import tempattr
 
-from test import WebCWTC
+from cubicweb_web.devtools.testlib import PyramidWebCWTC
 
 
-class SynchronizeSourceTC(WebCWTC):
+class SynchronizeSourceTC(PyramidWebCWTC):
     def test_synchronize_view(self):
         with self.admin_access.web_request(vid="cw.source-sync") as req:
 
             class AParser(datafeed.DataFeedParser):
                 __regid__ = "testparser"
 
                 def process(self, url, raise_on_error=False):
```

### Comparing `cubicweb-web-0.3.1/test/test_views_debug_html.py` & `cubicweb-web-1.0.0/test/test_views_debug_html.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 import inspect
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.view import View
 
 
-class DebugHtmlRenderingTC(CubicWebTC):
+class DebugHtmlRenderingCWTC(WebCWTC):
     def setUp(self):
         super().setUp()
         View.debug_html_rendering = True
 
     def tearDown(self):
         super().tearDown()
         View.debug_html_rendering = False
```

### Comparing `cubicweb-web-0.3.1/test/test_views_editforms.py` & `cubicweb-web-1.0.0/test/test_views_editforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common import tempattr
 from logilab.common.testlib import unittest_main, mock_object
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.predicates import is_instance
 from cubicweb.schema import RRQLExpression
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.formwidgets import AutoCompletionWidget
 from cubicweb_web.views import uicfg
 from cubicweb_web.views.editforms import DeleteConfFormView
 
 AFFK = uicfg.autoform_field_kwargs
 AFS = uicfg.autoform_section
 
@@ -40,15 +41,15 @@
         (rschema.type, x)
         for rschema, tschemas, x in AFS.relations_by_section(
             entity, formtype, section, permission
         )
     ]
 
 
-class AutomaticEntityFormTC(CubicWebTC):
+class AutomaticEntityFormCWTC(WebCWTC):
     def test_custom_widget(self):
         with self.admin_access.web_request() as req:
             AFFK.tag_subject_of(
                 ("CWUser", "login", "*"),
                 {"widget": AutoCompletionWidget(autocomplete_initfunc="get_logins")},
             )
             form = self.vreg["forms"].select("edition", req, entity=req.user)
@@ -95,14 +96,15 @@
             # (appears here while expected in hidden
             self.assertCountEqual(
                 [x for x in rbc(e, "main", "relations") if x != ("tags", "object")],
                 [
                     ("connait", "subject"),
                     ("custom_workflow", "subject"),
                     ("primary_email", "subject"),
+                    ("evaluee", "subject"),
                     ("checked_by", "object"),
                 ],
             )
             self.assertListEqual(
                 rbc(e, "main", "inlined"),
                 [
                     ("use_email", "subject"),
@@ -139,14 +141,15 @@
         with self.admin_access.web_request() as req:
             e = self.vreg["etypes"].etype_class("Personne")(req)
             self.assertListEqual(
                 rbc(e, "main", "attributes"),
                 [
                     ("nom", "subject"),
                     ("prenom", "subject"),
+                    ("type", "subject"),
                     ("sexe", "subject"),
                     ("promo", "subject"),
                     ("titre", "subject"),
                     ("ass", "subject"),
                     ("web", "subject"),
                     ("tel", "subject"),
                     ("fax", "subject"),
@@ -174,16 +177,26 @@
                 ],
             )
             self.assertCountEqual(
                 rbc(e, "main", "relations"),
                 [
                     ("travaille", "subject"),
                     ("manager", "object"),
-                    ("connait", "object"),
                     ("tags", "subject"),
+                    ("evaluee", "subject"),
+                    ("actionnaire", "subject"),
+                    ("dirige", "subject"),
+                    ("associe", "subject"),
+                    ("connait", "subject"),
+                    ("tags", "object"),
+                    ("contrat_exclusif", "object"),
+                    ("ecrit_par", "object"),
+                    ("evaluee", "object"),
+                    ("associe", "object"),
+                    ("fabrique_par", "object"),
                 ],
             )
             self.assertListEqual(rbc(e, "main", "hidden"), [])
 
     def test_edition_form(self):
         with self.admin_access.web_request() as req:
             rset = req.execute("CWUser X LIMIT 1")
@@ -223,14 +236,15 @@
     def test_editable_attributes(self):
         with self.admin_access.web_request() as req:
             entity = self.vreg["etypes"].etype_class("Personne")(req)
             form = self.vreg["forms"].select("edition", req, entity=entity)
             expected = [
                 ("nom", "subject"),
                 ("prenom", "subject"),
+                ("type", "subject"),
                 ("sexe", "subject"),
                 ("promo", "subject"),
                 ("titre", "subject"),
                 ("ass", "subject"),
                 ("web", "subject"),
                 ("tel", "subject"),
                 ("fax", "subject"),
@@ -316,15 +330,15 @@
                 self.assertTrue(
                     autoform.check_inlined_rdef_permissions(
                         rschema, role, tschema, ttype
                     )
                 )
 
 
-class FormViewsTC(CubicWebTC):
+class FormViewsCWTC(WebCWTC):
     def test_delete_conf_formview(self):
         with self.admin_access.web_request() as req:
             rset = req.execute("CWGroup X")
             self.view("deleteconf", rset, template=None, req=req).source
 
     def test_delete_conf_formview_composite(self):
         with self.admin_access.cnx() as cnx:
```

### Comparing `cubicweb-web-0.3.1/test/test_views_errorform.py` & `cubicweb-web-1.0.0/test/test_views_errorform.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 import re
 import sys
 
 from logilab.common.testlib import unittest_main
 
 from cubicweb import Forbidden
-from cubicweb.devtools.testlib import CubicWebTC
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.view import StartupView
 from cubicweb_web import Redirect
 
 
-class ErrorViewTC(CubicWebTC):
+class ErrorViewCWTC(WebCWTC):
     def setUp(self):
         super().setUp()
         self.vreg.config["submit-mail"] = "test@logilab.fr"
         self.vreg.config["print-traceback"] = "yes"
 
     def test_error_generation(self):
         """
```

### Comparing `cubicweb-web-0.3.1/test/test_views_forms.py` & `cubicweb-web-1.0.0/test/test_views_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common import tempattr, attrdict
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views.autoform import InlinedFormField
 from cubicweb_web.views.forms import EntityFieldsForm
 
 
-class InlinedFormTC(CubicWebTC):
+class InlinedFormCWTC(WebCWTC):
     def test_linked_to(self):
         with self.admin_access.web_request() as req:
             formview = req.vreg["views"].select(
                 "inline-creation",
                 req,
                 etype="File",
                 rtype="described_by_test",
```

### Comparing `cubicweb-web-0.3.1/test/test_views_json.py` & `cubicweb-web-1.0.0/test/test_views_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 # CubicWeb is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
+from cubicweb_web.devtools.testlib import WebCWTC
 
-from cubicweb.devtools.testlib import CubicWebTC
 
-
-class JsonViewsTC(CubicWebTC):
+class JsonViewsCWTC(WebCWTC):
     anonymize = True
     res_jsonp_data = b'[["guests", 1]]'
 
     def setUp(self):
         super().setUp()
         self.config.global_set_option("anonymize-jsonp-queries", self.anonymize)
 
@@ -98,15 +97,15 @@
             data = self.view("ejsonexport", rset, req=req)
             self.assertEqual(
                 req.headers_out.getRawHeaders("content-type"), ["application/json"]
             )
             self.assertEqual(data, [])
 
 
-class NotAnonymousJsonViewsTC(JsonViewsTC):
+class NotAnonymousJsonViewsTC(JsonViewsCWTC):
     anonymize = False
     res_jsonp_data = b'[["guests", 1], ["managers", 1]]'
 
 
 if __name__ == "__main__":
     from logilab.common.testlib import unittest_main
```

### Comparing `cubicweb-web-0.3.1/test/test_views_navigation.py` & `cubicweb-web-1.0.0/test/test_views_navigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb.web.views.navigation unit tests"""
 
 from logilab.common.testlib import unittest_main
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views.ibreadcrumbs import BreadCrumbEntityVComponent
 from cubicweb_web.views.navigation import (
     PageNavigation,
     SortedNavigation,
     PageNavigationSelect,
 )
 
 BreadCrumbEntityVComponent.visible = True
 
 
-class NavigationTC(CubicWebTC):
+class NavigationCWTC(WebCWTC):
     def test_navigation_selection_whatever(self):
         with self.admin_access.web_request() as req:
             rset = req.execute("Any X,N WHERE X name N")
             navcomp = self.vreg["components"].select("navigation", req, rset=rset)
             self.assertIsInstance(navcomp, PageNavigation)
             req.set_search_state("W:X:Y:Z")
             navcomp = self.vreg["components"].select("navigation", req, rset=rset)
```

### Comparing `cubicweb-web-0.3.1/test/test_views_pyviews.py` & `cubicweb-web-1.0.0/test/test_views_pyviews.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 from logilab.common.testlib import unittest_main
 
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class PyViewsTC(CubicWebTC):
+class PyViewsCWTC(WebCWTC):
     def test_pyvaltable(self):
         with self.admin_access.web_request() as req:
             view = self.vreg["views"].select(
                 "pyvaltable", req, pyvalue=[[1, "a"], [2, "b"]]
             )
             content = view.render(pyvalue=[[1, "a"], [2, "b"]], headers=["num", "char"])
             self.assertEqual(
```

### Comparing `cubicweb-web-0.3.1/test/test_views_searchrestriction.py` & `cubicweb-web-1.0.0/test/test_views_searchrestriction.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb_web import facet
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class InsertAttrRelationTC(CubicWebTC):
+class InsertAttrRelationCWTC(WebCWTC):
     def parse(self, query):
         with self.admin_access.cnx() as cnx:
             rqlst = self.vreg.parse(cnx, query)
             rqlst.children[0]
         return rqlst
 
     def _generate(self, rqlst, rel, role, attr):
```

### Comparing `cubicweb-web-0.3.1/test/test_views_staticcontrollers.py` & `cubicweb-web-1.0.0/test/test_views_staticcontrollers.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,56 +19,57 @@
 import os
 import os.path as osp
 from contextlib import contextmanager
 
 from logilab.common import tempattr
 from logilab.common.testlib import Tags
 
-from cubicweb.devtools.testlib import CubicWebTC
-from cubicweb.utils import HTMLHead
+from cubicweb_web.utils import HTMLHead
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views.staticcontrollers import ConcatFilesHandler
 
 
 class staticfilespublishermixin:
     @contextmanager
     def _publish_static_files(self, url, header={}):
         with self.admin_access.web_request(headers=header) as req:
             req._url = url
             self.app_handle_request(req)
             yield req
 
 
-class StaticControllerCacheTC(staticfilespublishermixin, CubicWebTC):
-    tags = CubicWebTC.tags | Tags("static_controller", "cache", "http")
+class StaticControllerCacheCWTC(staticfilespublishermixin, WebCWTC):
+    tags = WebCWTC.tags | Tags("static_controller", "cache", "http")
 
     def test_static_file_are_cached(self):
         with self._publish_static_files("data/cubicweb.css") as req:
             self.assertEqual(200, req.status_out)
             self.assertIn("last-modified", req.headers_out)
         next_headers = {
             "if-modified-since": req.get_response_header("last-modified", raw=True),
         }
         with self._publish_static_files("data/cubicweb.css", next_headers) as req:
             self.assertEqual(304, req.status_out)
 
 
-class StaticDirectoryControllerTC(staticfilespublishermixin, CubicWebTC):
+class StaticDirectoryControllerCWTC(staticfilespublishermixin, WebCWTC):
     def test_check_static_dir_access(self):
         """write a file in the static directory and test the access"""
         staticdir = osp.join(self.vreg.config.static_directory)
         if not os.path.exists(staticdir):
             os.makedirs(staticdir)
         filename = osp.join(staticdir, "test")
         with open(filename, "a"):
             with self._publish_static_files("static/test") as req:
                 self.assertEqual(200, req.status_out)
 
 
-class DataControllerTC(staticfilespublishermixin, CubicWebTC):
-    tags = CubicWebTC.tags | Tags("static_controller", "data", "http")
+class DataControllerCWTC(staticfilespublishermixin, WebCWTC):
+    tags = WebCWTC.tags | Tags("static_controller", "data", "http")
 
     def _check_datafile_ok(self, fname):
         with self._publish_static_files(fname) as req:
             self.assertEqual(200, req.status_out)
             self.assertIn("last-modified", req.headers_out)
             self.assertIn("expires", req.headers_out)
             self.assertEqual(
@@ -109,16 +110,16 @@
             self._check_no_datafile("data/%s/does/not/exist" % hash)
             self._check_datafile_redirect(
                 "data/%s/does/not/exist" % ("0" * len(hash)),
                 "data/{}/{}/does/not/exist".format(hash, "0" * len(hash)),
             )
 
 
-class ConcatFilesTC(CubicWebTC):
-    tags = CubicWebTC.tags | Tags("static_controller", "concat")
+class ConcatFilesCWTC(WebCWTC):
+    tags = WebCWTC.tags | Tags("static_controller", "concat")
 
     def tearDown(self):
         super().tearDown()
         self._cleanup_concat_cache()
 
     def _cleanup_concat_cache(self):
         uicachedir = osp.join(self.config.apphome, "uicache")
```

### Comparing `cubicweb-web-0.3.1/test/test_views_treeview.py` & `cubicweb-web-1.0.0/test/test_views_treeview.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 
 from logilab.common.testlib import unittest_main
 
 from cubicweb.devtools.htmlparser import XMLValidator
-from cubicweb.devtools.testlib import CubicWebTC
 
+from cubicweb_web.devtools.testlib import WebCWTC
 
-class TreeViewTC(CubicWebTC):
+
+class TreeViewCWTC(WebCWTC):
     def test_treeview(self):
         with self.admin_access.repo_cnx() as cnx:
             ce = cnx.create_entity
             root = ce("TreeNode", name="root")
             node = ce("TreeNode", name="node1", parent=root)
             ce("TreeNode", name="leaf1a", parent=node)
             ce("TreeNode", name="leaf1b", parent=node)
```

### Comparing `cubicweb-web-0.3.1/test/test_views_wdoc.py` & `cubicweb-web-1.0.0/test/test_views_wdoc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from unittest import skipUnless
 
-from cubicweb.devtools import testlib
+from cubicweb_web.devtools.testlib import WebCWTC
 
 try:
     import docutils  # noqa
 
     DOCUTILS_AVAILABLE = True
 except ImportError:
     DOCUTILS_AVAILABLE = False
 
 
-class WdocViewsTC(testlib.CubicWebTC):
+class WdocViewsCWTC(WebCWTC):
     @skipUnless(
         DOCUTILS_AVAILABLE, "rest_publish does not support ..winclude without docutils"
     )
     def test(self):
         with self.admin_access.web_request(fid="main") as req:
             page = req.view("wdoc")
         self.assertIn("Site documentation", page)
```

### Comparing `cubicweb-web-0.3.1/test/test_views_xmlrss.py` & `cubicweb-web-1.0.0/test/test_views_xmlrss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
+
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views.xmlrss import SERIALIZERS
 
 
-class EntityXMLViewTC(CubicWebTC):
+class EntityXMLViewCWTC(WebCWTC):
     """see also cw.sobjects.test.unittest_parsers"""
 
     def test(self):
         rels = [
             "tags-object",
             "in_group-subject",
             "in_state-subject",
```

### Comparing `cubicweb-web-0.3.1/test/test_viewselector.py` & `cubicweb-web-1.0.0/test/test_viewselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """XXX rename, split, reorganize this"""
 
 from logilab.common.registry import NoSelectableObject
 from logilab.common.testlib import unittest_main
 
 from cubicweb import Binary, UnknownProperty
-from cubicweb.devtools.testlib import CubicWebTC
 from cubicweb.predicates import is_instance, specified_etype_implements, rql_condition
 from cubicweb_web.action import Action
+from cubicweb_web.devtools.testlib import WebCWTC
 from cubicweb_web.views import (
     primary,
     baseviews,
     tableview,
     editforms,
     management,
     actions,
@@ -73,27 +73,27 @@
         ("rdf.nt", rdf.RDFntriplesView),
         ("rdf.trig", rdf.RDFtrigView),
     ]
 else:
     RDFVIEWS = []
 
 
-class ViewSelectorTC(CubicWebTC):
+class ViewSelectorCWTC(WebCWTC):
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             cnx.create_entity(
                 "BlogEntry", title="une news !", content="cubicweb c'est beau"
             )
             cnx.create_entity("Bookmark", title="un signet !", path="view?vid=index")
             cnx.create_entity("EmailAddress", address="devel@logilab.fr", alias="devel")
             cnx.create_entity("Tag", name="x")
             cnx.commit()
 
 
-class VRegistryTC(ViewSelectorTC):
+class VRegistryTC(ViewSelectorCWTC):
     """test the view selector"""
 
     def _test_registered(self, registry, content):
         try:
             expected = getattr(self, "all_%s" % registry)
         except AttributeError:
             return
@@ -695,15 +695,15 @@
 
 class CWETypeRQLAction(Action):
     __regid__ = "testaction"
     __select__ = is_instance("CWEType") & rql_condition('X name "CWEType"')
     title = "bla"
 
 
-class RQLActionTC(ViewSelectorTC):
+class RQLActionTC(ViewSelectorCWTC):
     def setUp(self):
         super().setUp()
         self.vreg._loadedmods[__name__] = {}
         self.vreg.register(CWETypeRQLAction)
         actionsreg = self.vreg["actions"]
         actionsreg["testaction"][0].__registered__(actionsreg)
```

### Comparing `cubicweb-web-0.3.1/test/test_web.py` & `cubicweb-web-1.0.0/test/test_web.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,18 @@
 import collections
 import hashlib
 import tempfile
 from json import loads
 from os.path import join
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.fake import FakeRequest
 from logilab.common.testlib import TestCase, unittest_main
 from webtest.forms import Upload
 
-from test import WebCWTC
+from cubicweb_web.devtools.testlib import FakeRequest, PyramidWebCWTC
 
 
 class AjaxReplaceUrlTC(TestCase):
     def test_ajax_replace_url_1(self):
         self._test_arurl(
             "fname=view&rql=Person%20P&vid=list", rql="Person P", vid="list"
         )
@@ -56,15 +55,15 @@
         self.assertMultiLineEqual(
             f'function {cbname}() {{ $("#foo").loadxhtml("{BASE_URL}ajax?{qs}",'
             f'{{"pageid": "{req.pageid}"}},"get","replace"); }}',
             req.html_headers.post_inlined_scripts[0],
         )
 
 
-class FileUploadTC(WebCWTC):
+class FileUploadTC(PyramidWebCWTC):
     def _fobject(self, fname):
         return open(join(self.datadir, fname), "rb")
 
     def _fcontent(self, fname):
         with self._fobject(fname) as f:
             return f.read()
 
@@ -112,15 +111,15 @@
                 ["views.py", self._fhash("views.py")],
             ],
         }
         self.assertEqual(webreq.status_code, 200)
         self.assertDictEqual(expect, loads(webreq.text))
 
 
-class LanguageTC(WebCWTC):
+class LanguageTC(PyramidWebCWTC):
     def test_language_neg(self):
         headers = {"Accept-Language": "fr"}
         webreq = self.webapp.get("/", headers=headers)
         webreq.mustcontain(b'lang="fr"')
         vary = [h.lower().strip() for h in webreq.headers.get("Vary").split(",")]
         self.assertIn("accept-language", vary)
         headers = {"Accept-Language": "en"}
@@ -142,15 +141,15 @@
         self.assertEqual(request.status_code, 200)
 
     def test_session_cookie_httponly(self):
         webreq = self.webapp.get("/")
         self.assertIn("HttpOnly", "".join(webreq.headers.getall("Set-Cookie")))
 
 
-class MiscOptionsTC(WebCWTC):
+class MiscOptionsTC(PyramidWebCWTC):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.logfile = tempfile.NamedTemporaryFile()
 
     @classmethod
     def init_config(cls, config):
```

### Comparing `cubicweb-web-0.3.1/test/test_webconfig.py` & `cubicweb-web-1.0.0/test/test_webconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb.web.webconfig unit tests"""
 
 import os
 from os import path
 from unittest import TestCase
 
-from cubicweb.devtools import ApptestConfiguration
+from cubicweb_web.devtools.testlib import WebApptestConfiguration
 
 
 class WebconfigTC(TestCase):
     def setUp(self):
         # need explicit None if dirname(__file__) is empty, see
         # ApptestConfiguration.__init__
-        self.config = ApptestConfiguration("data", __file__)
+        self.config = WebApptestConfiguration("data", __file__)
         self.config._cubes = ["file"]
         self.config.load_configuration()
 
     def test_nonregr_print_css_as_list(self):
         """make sure PRINT_CSS *must* is a list"""
         config = self.config
         print_css = config.uiprops["STYLESHEETS_PRINT"]
```

### Comparing `cubicweb-web-0.3.1/test/testutils.js` & `cubicweb-web-1.0.0/test/testutils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-0.3.1/test_auto/test_views.py` & `cubicweb-web-1.0.0/test_auto/test_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """automatic tests"""
 from cubicweb_web.view import AnyRsetView
-from test_auto import AutomaticWebTest, AutoPopulateTest
+from cubicweb_web.devtools.testlib import AutoPopulateTest, AutomaticWebTest
 
 
 class AutomaticWebTest(AutomaticWebTest):
     application_rql = [
         "Any L,F WHERE E is CWUser, E login L, E firstname F",
         "Any L,F,E WHERE E is CWUser, E login L, E firstname F",
         "Any COUNT(X) WHERE X is CWUser",
```

### Comparing `cubicweb-web-0.3.1/tox.ini` & `cubicweb-web-1.0.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tox]
 envlist = py3-base,py3-auto-test-views,flake8,check-manifest,black
 
 [testenv]
 deps =
   pytest
   webtest
+  docutils
+  pygments
   https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/archive/branch/default/cubicweb-branch-default.zip
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   py3-base: {envpython} -m pytest {posargs:test}
   py3-auto-test-views: {envpython} -m pytest {posargs:test_auto}
 
 [testenv:js]
 skip_install = true
-whitelist_externals =
+allowlist_externals =
   npm
 changedir={toxinidir}/test/test_js_scripts
 commands =
   npm install
   npm run test -- {posargs}
 
 [testenv:flake8]
@@ -52,15 +54,15 @@
 deps =
   black >= 22.12
 commands = black .
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
```

