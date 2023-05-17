# Comparing `tmp/tryton-6.8.0.tar.gz` & `tmp/tryton-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryton-6.8.0.tar", last modified: Mon May  1 12:07:21 2023, max compression
+gzip compressed data, was "tryton-6.8.1.tar", last modified: Wed May 17 20:35:32 2023, max compression
```

## Comparing `tryton-6.8.0.tar` & `tryton-6.8.1.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.101585 tryton-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)    18236 2023-05-01 11:19:08.000000 tryton-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-05-01 11:19:08.000000 tryton-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 tryton-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 tryton-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-05-01 12:07:21.101585 tryton-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-6.8.0/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.011584 tryton-6.8.0/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2067 2023-04-15 07:12:15.000000 tryton-6.8.0/bin/tryton
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-01-16 14:00:21.000000 tryton-6.8.0/catalan.nsh
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/darwin/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.011584 tryton-6.8.0/darwin/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-01-16 14:00:21.000000 tryton-6.8.0/darwin/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-01-16 14:00:21.000000 tryton-6.8.0/darwin/gtk-3.0/gtk.immodules
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.014917 tryton-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/glossary.rst
--rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/installation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 tryton-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    18793 2023-04-21 10:10:00.000000 tryton-6.8.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-01-16 14:00:21.000000 tryton-6.8.0/english.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-01-16 14:00:21.000000 tryton-6.8.0/farsi.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-01-16 14:00:21.000000 tryton-6.8.0/french.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-01-16 14:00:21.000000 tryton-6.8.0/german.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 tryton-6.8.0/make-darwin-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 tryton-6.8.0/make-win32-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-01-16 14:00:21.000000 tryton-6.8.0/portuguese.nsh
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4684 2023-04-15 07:12:15.000000 tryton-6.8.0/setup-freeze.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-05-01 12:07:21.101585 tryton-6.8.0/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-04-15 07:12:15.000000 tryton-6.8.0/setup.nsi
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4338 2023-04-15 07:12:15.000000 tryton-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-01-16 14:00:21.000000 tryton-6.8.0/slovenian.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-01-16 14:00:21.000000 tryton-6.8.0/spanish.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-04-15 07:12:15.000000 tryton-6.8.0/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.018251 tryton-6.8.0/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)     1926 2023-05-01 11:19:00.000000 tryton-6.8.0/tryton/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.021584 tryton-6.8.0/tryton/action/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/action/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6763 2023-04-28 07:46:16.000000 tryton-6.8.0/tryton/action/main.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3157 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/client.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.031584 tryton-6.8.0/tryton/common/
--rw-r--r--   0 ced       (1000) ced       (1000)     2380 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/common/button.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6607 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererbinary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererbutton.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/common/cellrendererclickablepixbuf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrenderercombo.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererfloat.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrendererinteger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrenderertext.py
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/cellrenderertoggle.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46398 2023-05-01 07:33:35.000000 tryton-6.8.0/tryton/common/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/completion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20371 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/common/datetime_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17206 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28998 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/common/entry_position.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/common/environment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/focus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/htmltextbuffer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/number_entry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5776 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/common/popup_menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/richtext.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8276 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/common/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/common/underline.py
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/common/widget_style.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7606 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/config.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.031584 tryton-6.8.0/tryton/data/locale/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/tryton/data/locale/bg/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.031584 tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     8847 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21360 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/tryton/data/locale/ca/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18982 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20106 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:20.998251 tryton-6.8.0/tryton/data/locale/cs/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     4634 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    17715 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/de/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19498 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20639 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/es/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19256 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20589 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/es_419/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7108 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    15820 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/et/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    13577 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18343 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/fa/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16794 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22236 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/fi/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    13490 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/fr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19662 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20744 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/hu/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17282 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20326 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/id/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.034918 tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     6983 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    15314 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/it/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15104 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19228 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/ja_JP/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/lo/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18515 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    26787 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/lt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16294 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20304 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/nl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18765 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19815 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/pl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17623 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19642 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/pt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15182 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19825 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/ro/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.038251 tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19191 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20017 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.001584 tryton-6.8.0/tryton/data/locale/ru/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    10072 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21758 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/sl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    12234 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18742 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/tr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    14027 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13211 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/tryton.pot
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/uk/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    23076 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    24539 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/locale/zh_CN/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.041585 tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16690 2023-05-01 11:19:01.000000 tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18708 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/tryton/data/pixmaps/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.064918 tryton-6.8.0/tryton/data/pixmaps/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-add.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-archive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-attach.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-back.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-bookmark.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-cancel.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-clear.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-copy.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-create.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-date.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-delete.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-drag.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-email.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-error.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-exit.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-export.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-filter.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-bold.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-italic.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-format-underline.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-forward.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-history.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.png
--rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-import.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-info.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-launch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-link.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-log.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-menu.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-note.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-ok.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-print.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-public.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-question.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-refresh.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-remove.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-save.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-search.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-send.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-star-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-star.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-switch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-translate.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-undo.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-warning.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.icns
--rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.ico
--rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/device_cookie.py
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/fingerprints.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.064918 tryton-6.8.0/tryton/gui/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42035 2023-04-28 07:46:16.000000 tryton-6.8.0/tryton/gui/main.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.074918 tryton-6.8.0/tryton/gui/window/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-01 11:19:08.000000 tryton-6.8.0/tryton/gui/window/about.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/board.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29228 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/dblogin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13478 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    34216 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/infobar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/limit.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3646 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/nomodal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/preference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/revision.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/tabcontent.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.078252 tryton-6.8.0/tryton/gui/window/view_board/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_board/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_board/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_board/view_board.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.078252 tryton-6.8.0/tryton/gui/window/view_form/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.078252 tryton-6.8.0/tryton/gui/window/view_form/model/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    43599 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/view_form/model/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/model/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25729 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/view_form/model/record.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.081585 tryton-6.8.0/tryton/gui/window/view_form/screen/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/screen/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    52272 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/view_form/screen/screen.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.084918 tryton-6.8.0/tryton/gui/window/view_form/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6078 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.084918 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9781 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21657 2023-05-01 07:33:35.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.094919 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8330 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22073 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/image.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12565 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14370 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22440 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5687 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/textbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5254 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/url.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10682 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/bar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15923 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/graph.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/pie.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51013 2023-04-28 07:46:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6926 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13785 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    49457 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/view_form/view/screen_container.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/win_csv.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20797 2023-04-30 10:46:36.000000 tryton-6.8.0/tryton/gui/window/win_export.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19552 2023-04-21 08:36:08.000000 tryton-6.8.0/tryton/gui/window/win_form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9390 2023-04-20 14:47:34.000000 tryton-6.8.0/tryton/gui/window/win_import.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/gui/window/win_search.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/window.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14869 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/gui/window/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13612 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/jsonrpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/plugins/
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/plugins/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.098252 tryton-6.8.0/tryton/plugins/translation/
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/plugins/translation/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21766 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4903 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/rpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.101585 tryton-6.8.0/tryton/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/tests/test_common.py
--rw-r--r--   0 ced       (1000) ced       (1000)    43500 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/tests/test_common_domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:16.000000 tryton-6.8.0/tryton/tests/test_common_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/tests/test_common_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6440 2023-04-15 07:12:15.000000 tryton-6.8.0/tryton/translate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-01-16 14:00:21.000000 tryton-6.8.0/tryton.desktop
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.021584 tryton-6.8.0/tryton.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    10575 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 tryton-6.8.0/tryton.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       69 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        7 2023-05-01 12:07:20.000000 tryton-6.8.0/tryton.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.004917 tryton-6.8.0/win32/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:21.101585 tryton-6.8.0/win32/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-01-16 14:00:21.000000 tryton-6.8.0/win32/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-01-16 14:00:21.000000 tryton-6.8.0/win32/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.521705 tryton-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18337 2023-05-17 20:35:29.000000 tryton-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-05-17 20:35:28.000000 tryton-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:32.000000 tryton-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:32.000000 tryton-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-05-17 20:35:32.521705 tryton-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-05-01 12:17:32.000000 tryton-6.8.1/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.308369 tryton-6.8.1/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2067 2023-05-01 12:17:32.000000 tryton-6.8.1/bin/tryton
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-05-01 12:17:32.000000 tryton-6.8.1/catalan.nsh
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/darwin/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.308369 tryton-6.8.1/darwin/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-05-01 12:17:32.000000 tryton-6.8.1/darwin/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-05-01 12:17:32.000000 tryton-6.8.1/darwin/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.311703 tryton-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-05-01 12:17:32.000000 tryton-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-05-01 12:17:32.000000 tryton-6.8.1/doc/glossary.rst
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-05-01 12:17:32.000000 tryton-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-05-01 12:17:32.000000 tryton-6.8.1/doc/installation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:32.000000 tryton-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    18793 2023-05-01 12:17:32.000000 tryton-6.8.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-05-01 12:17:32.000000 tryton-6.8.1/english.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-05-01 12:17:32.000000 tryton-6.8.1/farsi.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-05-01 12:17:32.000000 tryton-6.8.1/french.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-05-01 12:17:32.000000 tryton-6.8.1/german.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-01 12:17:32.000000 tryton-6.8.1/make-darwin-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-05-01 12:17:32.000000 tryton-6.8.1/make-win32-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-05-01 12:17:32.000000 tryton-6.8.1/portuguese.nsh
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4684 2023-05-01 12:17:32.000000 tryton-6.8.1/setup-freeze.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-05-17 20:35:32.521705 tryton-6.8.1/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-05-01 12:17:32.000000 tryton-6.8.1/setup.nsi
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4338 2023-05-01 12:17:32.000000 tryton-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-05-01 12:17:32.000000 tryton-6.8.1/slovenian.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-05-01 12:17:32.000000 tryton-6.8.1/spanish.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-05-01 12:17:32.000000 tryton-6.8.1/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.315036 tryton-6.8.1/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1926 2023-05-01 12:18:02.000000 tryton-6.8.1/tryton/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.318369 tryton-6.8.1/tryton/action/
+-rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/action/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6763 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/action/main.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3157 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/client.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.338370 tryton-6.8.1/tryton/common/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2380 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/button.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6607 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrendererbinary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrendererbutton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrendererclickablepixbuf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrenderercombo.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrendererfloat.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrendererinteger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrenderertext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/cellrenderertoggle.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46442 2023-05-13 22:17:11.000000 tryton-6.8.1/tryton/common/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/completion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20371 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/datetime_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17206 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    28998 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/entry_position.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/environment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/focus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/htmltextbuffer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/number_entry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5776 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/popup_menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/richtext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8276 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/underline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/common/widget_style.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7606 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/config.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.338370 tryton-6.8.1/tryton/data/locale/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/bg/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.338370 tryton-6.8.1/tryton/data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8847 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21360 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/bg/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/ca/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.341703 tryton-6.8.1/tryton/data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18982 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20106 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/ca/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/cs/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.341703 tryton-6.8.1/tryton/data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4634 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    17715 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/cs/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/de/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.341703 tryton-6.8.1/tryton/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19498 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/de/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20639 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/de/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/es/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.341703 tryton-6.8.1/tryton/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19256 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/es/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20589 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/es/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/es_419/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.341703 tryton-6.8.1/tryton/data/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7108 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    15820 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/et/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.345036 tryton-6.8.1/tryton/data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13577 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/et/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18343 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/et/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/fa/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.345036 tryton-6.8.1/tryton/data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16794 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22236 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/fa/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/fi/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.345036 tryton-6.8.1/tryton/data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    13490 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/fi/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/fr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.348370 tryton-6.8.1/tryton/data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19662 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20744 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/fr/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/hu/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.348370 tryton-6.8.1/tryton/data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17282 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20326 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/hu/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/id/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.348370 tryton-6.8.1/tryton/data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6983 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/id/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    15314 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/id/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/it/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.348370 tryton-6.8.1/tryton/data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15104 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/it/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19228 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/it/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/ja_JP/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.351703 tryton-6.8.1/tryton/data/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.295036 tryton-6.8.1/tryton/data/locale/lo/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.351703 tryton-6.8.1/tryton/data/locale/lo/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18515 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    26787 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/lo/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/lt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.351703 tryton-6.8.1/tryton/data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16294 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20304 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/lt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/nl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.351703 tryton-6.8.1/tryton/data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18765 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19815 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/nl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/pl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.355037 tryton-6.8.1/tryton/data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17623 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19642 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/pl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/pt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.355037 tryton-6.8.1/tryton/data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15182 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19825 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/pt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/ro/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.355037 tryton-6.8.1/tryton/data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19191 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20017 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/ro/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/ru/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.355037 tryton-6.8.1/tryton/data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10072 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21758 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/ru/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/sl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.358370 tryton-6.8.1/tryton/data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    12234 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18742 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/sl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/tr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.358370 tryton-6.8.1/tryton/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14027 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/tr/LC_MESSAGES/tryton.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13211 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/tryton.pot
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/uk/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.358370 tryton-6.8.1/tryton/data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    23076 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    24539 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/uk/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/locale/zh_CN/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.358370 tryton-6.8.1/tryton/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16690 2023-05-17 20:35:24.000000 tryton-6.8.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18708 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/tryton/data/pixmaps/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.425037 tryton-6.8.1/tryton/data/pixmaps/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-add.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-archive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-attach.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-back.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-bookmark.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-cancel.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-clear.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-copy.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-create.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-date.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-delete.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-drag.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-email.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-error.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-exit.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-export.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-filter.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-bold.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-italic.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-format-underline.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-forward.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-history.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-icon.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-icon.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-import.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-info.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-launch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-link.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-log.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-menu.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-note.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-ok.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-print.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-public.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-question.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-refresh.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-remove.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-save.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-search.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-send.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-star-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-star.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-switch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-translate.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-unarchive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-undo.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-warning.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton.icns
+-rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton.ico
+-rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/data/pixmaps/tryton/tryton.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/device_cookie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/fingerprints.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.428371 tryton-6.8.1/tryton/gui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42035 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/main.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.451704 tryton-6.8.1/tryton/gui/window/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-17 20:35:28.000000 tryton-6.8.1/tryton/gui/window/about.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/board.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29228 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/dblogin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13478 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    34216 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/infobar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/limit.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3646 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/nomodal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/preference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/revision.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/tabcontent.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.455038 tryton-6.8.1/tryton/gui/window/view_board/
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_board/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_board/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_board/view_board.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.455038 tryton-6.8.1/tryton/gui/window/view_form/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.458371 tryton-6.8.1/tryton/gui/window/view_form/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43599 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/model/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/model/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25729 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/model/record.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.461704 tryton-6.8.1/tryton/gui/window/view_form/screen/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/screen/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    52272 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/screen/screen.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.471705 tryton-6.8.1/tryton/gui/window/view_form/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6078 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/calendar_.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.475038 tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9781 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21657 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.501705 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8330 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/checkbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22073 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/dictionary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/image.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12565 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14370 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22440 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/progressbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7436 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/state_widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5687 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/textbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5254 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/url.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10682 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/graph.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.508372 tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/bar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15923 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/graph.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/pie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51013 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6926 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/list_form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.511705 tryton-6.8.1/tryton/gui/window/view_form/view/list_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/list_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13785 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/list_gtk/editabletree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    49457 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/list_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/view_form/view/screen_container.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/win_csv.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20797 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/win_export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19552 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/win_form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9390 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/win_import.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/win_search.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14869 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/gui/window/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13612 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/jsonrpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.511705 tryton-6.8.1/tryton/plugins/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/plugins/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.515038 tryton-6.8.1/tryton/plugins/translation/
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/plugins/translation/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21766 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4903 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/rpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.518372 tryton-6.8.1/tryton/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/tests/test_common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43500 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/tests/test_common_domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/tests/test_common_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/tests/test_common_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6440 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton/translate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-05-01 12:17:32.000000 tryton-6.8.1/tryton.desktop
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.318369 tryton-6.8.1/tryton.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2269 2023-05-17 20:35:31.000000 tryton-6.8.1/tryton.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    10575 2023-05-17 20:35:32.000000 tryton-6.8.1/tryton.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:35:31.000000 tryton-6.8.1/tryton.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:35:31.000000 tryton-6.8.1/tryton.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       69 2023-05-17 20:35:31.000000 tryton-6.8.1/tryton.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        7 2023-05-17 20:35:31.000000 tryton-6.8.1/tryton.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.298369 tryton-6.8.1/win32/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-17 20:35:32.521705 tryton-6.8.1/win32/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-05-01 12:17:32.000000 tryton-6.8.1/win32/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-05-01 12:17:32.000000 tryton-6.8.1/win32/gtk-3.0/gtk.immodules
```

### Comparing `tryton-6.8.0/CHANGELOG` & `tryton-6.8.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.1 - 2023-05-17
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Include events to logs
 * Add option to disable thread
 * Remove support for Python 3.7
 * Add support for Python 3.11
```

### Comparing `tryton-6.8.0/COPYRIGHT` & `tryton-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/LICENSE` & `tryton-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/PKG-INFO` & `tryton-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `tryton-6.8.0/bin/tryton` & `tryton-6.8.1/bin/tryton`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/catalan.nsh` & `tryton-6.8.1/catalan.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/darwin/gtk-3.0/gdk-pixbuf.loaders` & `tryton-6.8.1/darwin/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/darwin/gtk-3.0/gtk.immodules` & `tryton-6.8.1/darwin/gtk-3.0/gtk.immodules`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/doc/conf.py` & `tryton-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/doc/glossary.rst` & `tryton-6.8.1/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/doc/installation.rst` & `tryton-6.8.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/doc/usage.rst` & `tryton-6.8.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/english.nsh` & `tryton-6.8.1/english.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/farsi.nsh` & `tryton-6.8.1/farsi.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/french.nsh` & `tryton-6.8.1/french.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/german.nsh` & `tryton-6.8.1/german.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/portuguese.nsh` & `tryton-6.8.1/portuguese.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/setup-freeze.py` & `tryton-6.8.1/setup-freeze.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/setup.nsi` & `tryton-6.8.1/setup.nsi`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/setup.py` & `tryton-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/slovenian.nsh` & `tryton-6.8.1/slovenian.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/spanish.nsh` & `tryton-6.8.1/spanish.nsh`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/__init__.py` & `tryton-6.8.1/tryton/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-__version__ = "6.8.0"
+__version__ = "6.8.1"
 import locale
 
 import gi
 
 gi.require_version('Gtk', '3.0')
 gi.require_version('Gdk', '3.0')
 gi.require_foreign('cairo')
```

### Comparing `tryton-6.8.0/tryton/action/main.py` & `tryton-6.8.1/tryton/action/main.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/bus.py` & `tryton-6.8.1/tryton/bus.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/client.py` & `tryton-6.8.1/tryton/client.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/__init__.py` & `tryton-6.8.1/tryton/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/button.py` & `tryton-6.8.1/tryton/common/button.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/cellrendererbinary.py` & `tryton-6.8.1/tryton/common/cellrendererbinary.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/cellrendererbutton.py` & `tryton-6.8.1/tryton/common/cellrendererbutton.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/cellrendererclickablepixbuf.py` & `tryton-6.8.1/tryton/common/cellrendererclickablepixbuf.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/cellrendererfloat.py` & `tryton-6.8.1/tryton/common/cellrendererfloat.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/cellrendererinteger.py` & `tryton-6.8.1/tryton/common/cellrendererinteger.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/cellrenderertext.py` & `tryton-6.8.1/tryton/common/cellrenderertext.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/common.py` & `tryton-6.8.1/tryton/common/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1207,29 +1207,29 @@
         except Exception as exception:
             self.error = True
             self.res = False
             self.exception = exception
         else:
             if not self.res:
                 self.error = True
-        if self.callback:
+        if self.callback and CONFIG['thread']:
             # Post to GTK queue to be run by the main thread
             GLib.idle_add(self.process)
         return True
 
     def run(self, process_exception_p=True, callback=None):
         self.process_exception_p = process_exception_p
         self.callback = callback
 
-        if callback:
+        if callback and CONFIG['thread']:
             # Parent is only useful if it is asynchronous
             # otherwise the cursor is not updated.
             self.parent = get_toplevel_window()
             self._cursor_timeout = GLib.timeout_add(3000, self._set_cursor)
-            Thread(target=self.start).run()
+            Thread(target=self.start).start()
             return
         else:
             self.start()
             return self.process()
 
     def _set_cursor(self):
         self._cursor_timeout = None
```

### Comparing `tryton-6.8.0/tryton/common/completion.py` & `tryton-6.8.1/tryton/common/completion.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/datetime_.py` & `tryton-6.8.1/tryton/common/datetime_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/domain_inversion.py` & `tryton-6.8.1/tryton/common/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/domain_parser.py` & `tryton-6.8.1/tryton/common/domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/environment.py` & `tryton-6.8.1/tryton/common/environment.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/focus.py` & `tryton-6.8.1/tryton/common/focus.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/htmltextbuffer.py` & `tryton-6.8.1/tryton/common/htmltextbuffer.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/number_entry.py` & `tryton-6.8.1/tryton/common/number_entry.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/popup_menu.py` & `tryton-6.8.1/tryton/common/popup_menu.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/richtext.py` & `tryton-6.8.1/tryton/common/richtext.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/selection.py` & `tryton-6.8.1/tryton/common/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/timedelta.py` & `tryton-6.8.1/tryton/common/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/common/underline.py` & `tryton-6.8.1/tryton/common/underline.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/config.py` & `tryton-6.8.1/tryton/config.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/bg/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: bg\n"
 "Language-Team: bg <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/bg/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/ca/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ca\n"
 "Language-Team: ca <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/ca/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/cs/LC_MESSAGES/tryton.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/cs/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/de/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/de/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/de/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/es/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/es/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/es/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es_419\n"
 "Language-Team: es_419 <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/et/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: et\n"
 "Language-Team: et <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/et/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/et/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/fa/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/fa/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/fi/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/fr/LC_MESSAGES/tryton.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/fr/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/hu/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu\n"
 "Language-Team: hu <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/hu/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/id/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: id\n"
 "Language-Team: id <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/id/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/id/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/it/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/it/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/it/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja_JP\n"
 "Language-Team: ja_JP <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/lo/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lo\n"
 "Language-Team: lo <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/lo/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/lt/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lt\n"
 "Language-Team: lt <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/lt/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/nl/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/nl/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/pl/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/pl/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/pt/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pt\n"
 "Language-Team: pt <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/pt/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/ro/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ro\n"
 "Language-Team: ro <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/ro/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/ru/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/ru/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/sl/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: sl\n"
 "Language-Team: sl <LL@li.org>\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/sl/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/tr/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/tr/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/tryton.pot` & `tryton-6.8.1/tryton/data/locale/tryton.pot`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/uk/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/uk/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo` & `tryton-6.8.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-05-01 13:19+0200\n"
+"POT-Creation-Date: 2023-05-17 22:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-6.8.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po` & `tryton-6.8.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/LICENSE` & `tryton-6.8.1/tryton/data/pixmaps/tryton/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.png` & `tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-icon.png`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-icon.svg` & `tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-icon.svg`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg` & `tryton-6.8.1/tryton/data/pixmaps/tryton/tryton-unarchive.svg`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.icns` & `tryton-6.8.1/tryton/data/pixmaps/tryton/tryton.icns`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.ico` & `tryton-6.8.1/tryton/data/pixmaps/tryton/tryton.ico`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/data/pixmaps/tryton/tryton.svg` & `tryton-6.8.1/tryton/data/pixmaps/tryton/tryton.svg`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/device_cookie.py` & `tryton-6.8.1/tryton/device_cookie.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/fingerprints.py` & `tryton-6.8.1/tryton/fingerprints.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/main.py` & `tryton-6.8.1/tryton/gui/main.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/about.py` & `tryton-6.8.1/tryton/gui/window/about.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/attachment.py` & `tryton-6.8.1/tryton/gui/window/attachment.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/board.py` & `tryton-6.8.1/tryton/gui/window/board.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/dblogin.py` & `tryton-6.8.1/tryton/gui/window/dblogin.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/email_.py` & `tryton-6.8.1/tryton/gui/window/email_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/form.py` & `tryton-6.8.1/tryton/gui/window/form.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/infobar.py` & `tryton-6.8.1/tryton/gui/window/infobar.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/limit.py` & `tryton-6.8.1/tryton/gui/window/limit.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/log.py` & `tryton-6.8.1/tryton/gui/window/log.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/nomodal.py` & `tryton-6.8.1/tryton/gui/window/nomodal.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/note.py` & `tryton-6.8.1/tryton/gui/window/note.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/preference.py` & `tryton-6.8.1/tryton/gui/window/preference.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/revision.py` & `tryton-6.8.1/tryton/gui/window/revision.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/tabcontent.py` & `tryton-6.8.1/tryton/gui/window/tabcontent.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_board/action.py` & `tryton-6.8.1/tryton/gui/window/view_board/action.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_board/view_board.py` & `tryton-6.8.1/tryton/gui/window/view_board/view_board.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/model/field.py` & `tryton-6.8.1/tryton/gui/window/view_form/model/field.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/model/group.py` & `tryton-6.8.1/tryton/gui/window/view_form/model/group.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/model/record.py` & `tryton-6.8.1/tryton/gui/window/view_form/model/record.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/screen/screen.py` & `tryton-6.8.1/tryton/gui/window/view_form/screen/screen.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/__init__.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/binary.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/binary.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/char.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/char.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/checkbox.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/dictionary.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/document.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/document.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/float.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/float.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/image.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/image.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/integer.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/integer.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2many.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/many2many.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/many2one.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/many2one.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/multiselection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/one2many.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/one2many.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/progressbar.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/pyson.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/reference.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/reference.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/richtextbox.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/selection.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/state_widget.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/textbox.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/textbox.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/url.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/url.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/form_gtk/widget.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/form_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/graph.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/bar.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/bar.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/graph.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/line.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/line.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/graph_gtk/pie.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/graph_gtk/pie.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/list.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/list.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/list_form.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/list_form.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/list_gtk/editabletree.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/list_gtk/widget.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/list_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/view_form/view/screen_container.py` & `tryton-6.8.1/tryton/gui/window/view_form/view/screen_container.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/win_csv.py` & `tryton-6.8.1/tryton/gui/window/win_csv.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/win_export.py` & `tryton-6.8.1/tryton/gui/window/win_export.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/win_form.py` & `tryton-6.8.1/tryton/gui/window/win_form.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/win_import.py` & `tryton-6.8.1/tryton/gui/window/win_import.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/win_search.py` & `tryton-6.8.1/tryton/gui/window/win_search.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/window.py` & `tryton-6.8.1/tryton/gui/window/window.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/gui/window/wizard.py` & `tryton-6.8.1/tryton/gui/window/wizard.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/jsonrpc.py` & `tryton-6.8.1/tryton/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/plugins/__init__.py` & `tryton-6.8.1/tryton/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/plugins/translation/__init__.py` & `tryton-6.8.1/tryton/plugins/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/pyson.py` & `tryton-6.8.1/tryton/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/rpc.py` & `tryton-6.8.1/tryton/rpc.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/tests/test_common.py` & `tryton-6.8.1/tryton/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/tests/test_common_domain_parser.py` & `tryton-6.8.1/tryton/tests/test_common_domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/tests/test_common_selection.py` & `tryton-6.8.1/tryton/tests/test_common_selection.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/tests/test_common_timedelta.py` & `tryton-6.8.1/tryton/tests/test_common_timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton/translate.py` & `tryton-6.8.1/tryton/translate.py`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton.desktop` & `tryton-6.8.1/tryton.desktop`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/tryton.egg-info/PKG-INFO` & `tryton-6.8.1/tryton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `tryton-6.8.0/tryton.egg-info/SOURCES.txt` & `tryton-6.8.1/tryton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tryton-6.8.0/win32/gtk-3.0/gdk-pixbuf.loaders` & `tryton-6.8.1/win32/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

