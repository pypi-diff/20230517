# Comparing `tmp/ubiquity-student-0.8.2.tar.gz` & `tmp/ubiquity-student-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubiquity-student-0.8.2.tar", last modified: Fri Jan 20 09:18:55 2023, max compression
+gzip compressed data, was "ubiquity-student-1.0.1.tar", last modified: Wed May 17 06:34:00 2023, max compression
```

## Comparing `ubiquity-student-0.8.2.tar` & `ubiquity-student-1.0.1.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.177985 ubiquity-student-0.8.2/
--rw-r--r--   0 root         (0) root         (0)     2851 2023-01-20 09:18:55.177985 ubiquity-student-0.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-20 09:18:55.177985 ubiquity-student-0.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2993 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.073984 ubiquity-student-0.8.2/src/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.077984 ubiquity-student-0.8.2/src/ubiquity/
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8936 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/argument_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.077984 ubiquity-student-0.8.2/src/ubiquity/controllers/
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7941 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/controllers/config_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8980 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/controllers/main_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     5921 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/controllers/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.077984 ubiquity-student-0.8.2/src/ubiquity/images/
--rw-rw-rw-   0 root         (0) root         (0)     2139 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/images/ubiquity_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.069984 ubiquity-student-0.8.2/src/ubiquity/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.069984 ubiquity-student-0.8.2/src/ubiquity/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.077984 ubiquity-student-0.8.2/src/ubiquity/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6194 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/locale/fr/LC_MESSAGES/ubiquity-student.mo
--rw-rw-rw-   0 root         (0) root         (0)     5223 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/ubiquity_student.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.081984 ubiquity-student-0.8.2/src/ubiquity/views/
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.081984 ubiquity-student-0.8.2/src/ubiquity/views/cui/
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/cui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8398 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/cui/main_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.081984 ubiquity-student-0.8.2/src/ubiquity/views/gui/
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.085984 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/about.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/choice.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6555 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/open.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/preference.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/main_view.py
--rw-rw-rw-   0 root         (0) root         (0)     5278 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/menu_bar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.089984 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/
--rw-rw-rw-   0 root         (0) root         (0)     2368 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sun_valley_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sun_valley_light.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.089984 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1349 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2961 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.089984 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.129984 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-up.png
--rwxrwxrwx   0 root         (0) root         (0)      262 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      373 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      363 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      377 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      301 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      276 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      288 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-pressed.png
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      386 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/card.png
--rwxrwxrwx   0 root         (0) root         (0)      383 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      474 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      294 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      362 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      358 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      363 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      312 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      353 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      302 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      353 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      129 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/empty.png
--rwxrwxrwx   0 root         (0) root         (0)      273 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      335 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-focus.png
--rwxrwxrwx   0 root         (0) root         (0)      269 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      324 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-invalid.png
--rwxrwxrwx   0 root         (0) root         (0)      297 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook-border.png
--rwxrwxrwx   0 root         (0) root         (0)      186 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook.png
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-hor.png
--rwxrwxrwx   0 root         (0) root         (0)      214 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-vert.png
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-hor.png
--rwxrwxrwx   0 root         (0) root         (0)      160 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-vert.png
--rwxrwxrwx   0 root         (0) root         (0)      553 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      853 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      786 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      552 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      602 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      616 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      621 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-hor.png
--rwxrwxrwx   0 root         (0) root         (0)      215 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-vert.png
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-down.png
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-thumb.png
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-trough.png
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-left.png
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-right.png
--rwxrwxrwx   0 root         (0) root         (0)      236 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-up.png
--rwxrwxrwx   0 root         (0) root         (0)      264 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-thumb.png
--rwxrwxrwx   0 root         (0) root         (0)      343 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-trough.png
--rwxrwxrwx   0 root         (0) root         (0)      128 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/separator.png
--rwxrwxrwx   0 root         (0) root         (0)      276 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/sizegrip.png
--rwxrwxrwx   0 root         (0) root         (0)      733 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      963 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      623 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      936 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      859 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      265 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-selected.png
--rwxrwxrwx   0 root         (0) root         (0)      295 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      317 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-pressed.png
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-rest.png
--rwxrwxrwx   0 root         (0) root         (0)    19668 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.173985 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-up.png
--rwxrwxrwx   0 root         (0) root         (0)      271 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      374 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      367 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      384 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      307 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      306 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      394 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/card.png
--rwxrwxrwx   0 root         (0) root         (0)      381 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      476 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      473 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      299 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      365 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      362 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      367 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      324 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      334 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      302 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      129 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/empty.png
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      331 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-focus.png
--rwxrwxrwx   0 root         (0) root         (0)      302 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      324 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-invalid.png
--rwxrwxrwx   0 root         (0) root         (0)      308 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook-border.png
--rwxrwxrwx   0 root         (0) root         (0)      185 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook.png
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-hor.png
--rwxrwxrwx   0 root         (0) root         (0)      216 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-vert.png
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-hor.png
--rwxrwxrwx   0 root         (0) root         (0)      161 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-vert.png
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      837 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      764 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      773 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      521 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      573 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      636 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      658 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-hor.png
--rwxrwxrwx   0 root         (0) root         (0)      214 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-vert.png
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-down.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-thumb.png
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-trough.png
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-left.png
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-right.png
--rwxrwxrwx   0 root         (0) root         (0)      237 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-up.png
--rwxrwxrwx   0 root         (0) root         (0)      262 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-thumb.png
--rwxrwxrwx   0 root         (0) root         (0)      324 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-trough.png
--rwxrwxrwx   0 root         (0) root         (0)      128 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/separator.png
--rwxrwxrwx   0 root         (0) root         (0)      272 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/sizegrip.png
--rwxrwxrwx   0 root         (0) root         (0)      726 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      867 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      880 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      590 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png
--rwxrwxrwx   0 root         (0) root         (0)      906 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      916 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png
--rwxrwxrwx   0 root         (0) root         (0)      857 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png
--rwxrwxrwx   0 root         (0) root         (0)      295 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-hover.png
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-rest.png
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-selected.png
--rwxrwxrwx   0 root         (0) root         (0)      338 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-hover.png
--rwxrwxrwx   0 root         (0) root         (0)      318 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-pressed.png
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-rest.png
--rwxrwxrwx   0 root         (0) root         (0)    19846 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl
--rw-rw-rw-   0 root         (0) root         (0)     6367 2023-01-20 09:10:37.000000 ubiquity-student-0.8.2/src/ubiquity/views/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-20 09:18:55.177985 ubiquity-student-0.8.2/ubiquity_student.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2851 2023-01-20 09:18:54.000000 ubiquity-student-0.8.2/ubiquity_student.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12271 2023-01-20 09:18:55.000000 ubiquity-student-0.8.2/ubiquity_student.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-20 09:18:54.000000 ubiquity-student-0.8.2/ubiquity_student.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-20 09:18:54.000000 ubiquity-student-0.8.2/ubiquity_student.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-20 09:18:54.000000 ubiquity-student-0.8.2/ubiquity_student.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-20 09:18:54.000000 ubiquity-student-0.8.2/ubiquity_student.egg-info/top_level.txt
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.541967 ubiquity-student-1.0.1/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2516 2023-05-17 06:34:00.541967 ubiquity-student-1.0.1/PKG-INFO
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1554 2022-06-20 11:36:26.000000 ubiquity-student-1.0.1/README.md
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)       38 2023-05-17 06:34:00.541967 ubiquity-student-1.0.1/setup.cfg
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2993 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/setup.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)        5 2023-05-17 06:31:15.000000 ubiquity-student-1.0.1/src/VERSION
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      854 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     8936 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/argument_parser.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/controllers/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/controllers/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     7941 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/controllers/config_file.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     9157 2023-05-10 11:20:34.000000 ubiquity-student-1.0.1/src/ubiquity/controllers/main_controller.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6247 2023-05-10 11:20:34.000000 ubiquity-student-1.0.1/src/ubiquity/controllers/worker.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/images/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2139 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/images/ubiquity_icon.png
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.513967 ubiquity-student-1.0.1/src/ubiquity/locale/
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.513967 ubiquity-student-1.0.1/src/ubiquity/locale/fr/
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     4589 2023-05-10 11:20:34.000000 ubiquity-student-1.0.1/src/ubiquity/locale/fr/LC_MESSAGES/ubiquity-student.mo
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     5223 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/model.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     3348 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/ubiquity_student.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2080 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/version.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/views/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/__init__.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/views/cui/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/cui/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     8398 2023-01-12 13:40:26.000000 ubiquity-student-1.0.1/src/ubiquity/views/cui/main_view.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/views/gui/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/__init__.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.517967 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      960 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2001 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/about.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2000 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/base.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1901 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/choice.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     3606 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/form.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6555 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/open.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     3320 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/preference.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     4798 2023-05-10 11:20:34.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/main_view.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     5278 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/menu_bar.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.521967 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2368 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1068 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/base.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1164 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sun_valley_dark.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1168 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sun_valley_light.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.521967 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1063 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/LICENSE
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)     1349 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/__init__.py
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)     2961 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.521967 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.529967 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      270 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      261 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-right.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      262 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      373 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      363 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      377 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      301 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      276 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      288 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      301 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      245 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      238 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      386 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/card.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      383 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      474 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      460 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      475 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      294 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      362 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      358 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      363 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      312 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      353 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      353 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      129 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/empty.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      273 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      335 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-focus.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      269 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-invalid.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      297 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      337 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook-border.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      186 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      193 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      214 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      157 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      160 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-vert.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      553 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      853 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      786 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      830 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      552 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      602 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      616 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      621 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      724 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      808 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      735 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      771 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      216 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      215 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      226 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      254 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-thumb.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      338 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-trough.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      233 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-left.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      227 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-right.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      236 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      264 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-thumb.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      343 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-trough.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      128 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/separator.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      276 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/sizegrip.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      733 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      945 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      963 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      895 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      623 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      927 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      936 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      859 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      265 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      164 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      319 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-selected.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      295 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      317 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      321 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)    19668 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.541967 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      278 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      273 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-right.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      285 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      271 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      374 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      367 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      384 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      326 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      316 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      307 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      306 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      289 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      303 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      238 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      225 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      394 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/card.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      381 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      476 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      467 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      473 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      299 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      365 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      362 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      367 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      334 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      333 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      129 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/empty.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      289 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      331 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-focus.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-invalid.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      308 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      298 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook-border.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      185 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      192 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      216 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      158 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      161 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-vert.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      523 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      837 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      764 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      773 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      521 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      573 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      636 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      576 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      658 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      749 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      675 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      701 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      208 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      214 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      229 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      234 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-thumb.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      321 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-trough.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      232 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-left.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      223 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-right.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      237 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      262 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-thumb.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-trough.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      128 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/separator.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      272 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/sizegrip.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      726 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      867 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      880 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      814 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      590 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      906 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      916 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      857 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      295 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      164 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      318 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-selected.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      338 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      318 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      330 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)    19846 2022-09-19 07:02:28.000000 ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6442 2023-05-10 11:20:34.000000 ubiquity-student-1.0.1/src/ubiquity/views/utils.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-05-17 06:34:00.541967 ubiquity-student-1.0.1/ubiquity_student.egg-info/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2516 2023-05-17 06:34:00.000000 ubiquity-student-1.0.1/ubiquity_student.egg-info/PKG-INFO
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)    12271 2023-05-17 06:34:00.000000 ubiquity-student-1.0.1/ubiquity_student.egg-info/SOURCES.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)        1 2023-05-17 06:34:00.000000 ubiquity-student-1.0.1/ubiquity_student.egg-info/dependency_links.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)       72 2023-05-17 06:34:00.000000 ubiquity-student-1.0.1/ubiquity_student.egg-info/entry_points.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)       17 2023-05-17 06:34:00.000000 ubiquity-student-1.0.1/ubiquity_student.egg-info/requires.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)        4 2023-05-17 06:34:00.000000 ubiquity-student-1.0.1/ubiquity_student.egg-info/top_level.txt
```

### Comparing `ubiquity-student-0.8.2/PKG-INFO` & `ubiquity-student-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 Metadata-Version: 2.1
 Name: ubiquity-student
-Version: 0.8.2
+Version: 1.0.1
 Summary: Ubiquity permet le suivi de TP de développement informatique
 Home-page: https://gitlab.insa-rouen.fr/cip/ubiquity
-License: UNKNOWN
 Download-URL: https://gitlab.insa-rouen.fr/cip/ubiquity/-/tags
 Project-URL: Documentation, https://gitlab.insa-rouen.fr/cip/ubiquity/-/wikis/home
 Project-URL: Bug Tracker, https://gitlab.insa-rouen.fr/cip/ubiquity/-/issues
-Description: # Ubiquity
-        
-        Ubiquity est un logiciel de suivi de TP de développement
-        informatique. Il permet aux tuteurs d’encadrer facilement et de
-        manière optimisée un groupe d’étudiants.
-        
-        Grâce à Ubiquity, l’enseignant crée de façon simple, un TP, en
-        déposant un sujet et sa correction annotée. Les étudiants
-        récupèrent ensuite le sujet ainsi que les fichiers sources à compléter.
-        
-        Ubiquity permet aussi à l’enseignant de suivre en temps réel
-        l’avancement de chaque étudiant dans la réalisation du TP, grâce
-        à différents indicateurs. Ainsi, l’enseignant identifie
-        rapidement les étudiants en difficultés. Ubiquity permet aussi aux
-        étudiants de se situer, par rapport à l’avancement de leurs
-        collègues.
-        
-        Ubiquity est un logiciel **opensource** et **gratuit**, disponible sur
-        Windows, MacOs et Linux. Il peut s’utiliser aussi bien en
-        présentiel qu’en distanciel, de manière synchrone ou asynchrone.
-        
-        
-        Pour plus d'information, nous vous invitons à regarder 
-        la vidéo de [présentation d'ubiquity](https://webtv.insa-rouen.fr/videos/presentation-de-ubiquity/) 
-        et à lire le [wiki](https://gitlab.insa-rouen.fr/delestre/ubiquity/-/wikis/home) proposant une documentation fonctionnelle et technique.
-        
-        ## Installation
-        
-        Pour installer l'application : `pip install ubiquity-student`
-        
-        ## Exécution
-        
-        Pour exécuter l'application : `ubiquity-student`
-        
-        ## Licence
-        
-        Distribué sous la License GNU GENERAL PUBLIC LICENSE v3.0. Voir [LICENSE](https://gitlab.insa-rouen.fr/cip/ubiquity/-/blob/master/LICENSE) pour plus d'information.
-Platform: UNKNOWN
 Classifier: Topic :: Education
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: French
 Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
+
+# Ubiquity
+
+Ubiquity est un logiciel de suivi de TP de développement
+informatique. Il permet aux tuteurs d’encadrer facilement et de
+manière optimisée un groupe d’étudiants.
+
+Grâce à Ubiquity, l’enseignant crée de façon simple, un TP, en
+déposant un sujet et sa correction annotée. Les étudiants
+récupèrent ensuite le sujet ainsi que les fichiers sources à compléter.
+
+Ubiquity permet aussi à l’enseignant de suivre en temps réel
+l’avancement de chaque étudiant dans la réalisation du TP, grâce
+à différents indicateurs. Ainsi, l’enseignant identifie
+rapidement les étudiants en difficultés. Ubiquity permet aussi aux
+étudiants de se situer, par rapport à l’avancement de leurs
+collègues.
+
+Ubiquity est un logiciel **opensource** et **gratuit**, disponible sur
+Windows, MacOs et Linux. Il peut s’utiliser aussi bien en
+présentiel qu’en distanciel, de manière synchrone ou asynchrone.
+
+
+Pour plus d'information, nous vous invitons à regarder 
+la vidéo de [présentation d'ubiquity](https://webtv.insa-rouen.fr/videos/presentation-de-ubiquity/) 
+et à lire le [wiki](https://gitlab.insa-rouen.fr/delestre/ubiquity/-/wikis/home) proposant une documentation fonctionnelle et technique.
+
+## Installation
+
+Pour installer l'application : `pip install ubiquity-student`
+
+## Exécution
+
+Pour exécuter l'application : `ubiquity-student`
+
+## Licence
+
+Distribué sous la License GNU GENERAL PUBLIC LICENSE v3.0. Voir [LICENSE](https://gitlab.insa-rouen.fr/cip/ubiquity/-/blob/master/LICENSE) pour plus d'information.
```

### Comparing `ubiquity-student-0.8.2/README.md` & `ubiquity-student-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/setup.py` & `ubiquity-student-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/argument_parser.py` & `ubiquity-student-1.0.1/src/ubiquity/argument_parser.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/controllers/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/controllers/config_file.py` & `ubiquity-student-1.0.1/src/ubiquity/controllers/config_file.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/controllers/main_controller.py` & `ubiquity-student-1.0.1/src/ubiquity/controllers/main_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
         :return: None if the status code is OK, Error if not
         """
         try:
             response = self._check_version()
             if response:
                 return response
             response = requests.get(self._model.url_api_connection_check())
+            if response.status_code == StatusCode.SUSPENDED:
+                return ErrorMessage.PRACTICAL_WORK_SUSPENDED
             if response.status_code != StatusCode.OK:
                 if self.config.check_is_config(self._model):
                     return ErrorMessage.CONFIG_DELETED
                 return ErrorMessage.INVALID_KEYS
             content = loads(response.content)
             self._model.name.set(content['name'])
             self.is_new_project = content['is_new']
@@ -206,11 +208,11 @@
         error = self._check_values()
         if not isinstance(error, ErrorMessage):
             if self.is_new_project:
                 self.extract_zip(has_color)
             elif not self.config.check_directory(self._model):
                 return Returns.CHOICE
             return Returns.OK
-        if error is not ErrorMessage.VERSION and error is not ErrorMessage.CONNECTION_FAILED and \
-                self.config.check_is_config(self._model):
+        if error is not ErrorMessage.VERSION and error is not ErrorMessage.CONNECTION_FAILED \
+                and error is not ErrorMessage.PRACTICAL_WORK_SUSPENDED and self.config.check_is_config(self._model):
             self.config.remove_config(self._model)
         return Returns.ERROR
```

### Comparing `ubiquity-student-0.8.2/src/ubiquity/controllers/worker.py` & `ubiquity-student-1.0.1/src/ubiquity/controllers/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+import signal
 import time
 from enum import unique, IntEnum
 from json import loads
 from os import stat
 from os.path import isfile, join
 from threading import Thread
 from typing import List
@@ -26,14 +27,15 @@
 
 
 @unique
 class StatusCode(IntEnum):
     """Enum class for status codes"""
     OK = 200
     CREATED = 201
+    SUSPENDED = 423
 
 
 def get_current_time() -> str:
     """Function returning the current time
 
     :return: The current time
     """
@@ -136,28 +138,34 @@
             response = requests.post(self._model.url_api_action_file(file_name), data=data)
             if response.status_code in [StatusCode.OK, StatusCode.CREATED]:
                 self._files_watching[file_path] = time_updated_file(file_path)
                 print(f'File {file_path} {"created" if response.status_code == StatusCode.CREATED else "updated" } '
                       f'successfully at {get_current_time()}')
                 if not self._has_gui and self.running:
                     self._get_progress()
+            elif response.status_code == StatusCode.SUSPENDED:
+                self.running = False
+                signal.raise_signal(signal.SIGUSR1)
         except UnicodeDecodeError:
             pass
 
     def _delete(self, file_path) -> None:
         file_name = file_path[len(self._model.directory.get()):]
         response = requests.delete(self._model.url_api_action_file(file_name))
         if response.status_code == StatusCode.OK:
             try:
                 self._files_watching.pop(file_path)
             except KeyError:
                 pass
             print(f'File {file_path} deleted successfully at {get_current_time()}')
             if not self._has_gui and self.running:
                 self._get_progress()
+        elif response.status_code == StatusCode.SUSPENDED:
+            self.running = False
+            signal.raise_signal(signal.SIGUSR1)
 
     def _get_files_to_follow(self) -> List[str]:
         """Method getting the server file paths
 
         :return: The list of file paths
         """
         response = requests.get(self._model.url_api_file_paths())
```

### Comparing `ubiquity-student-0.8.2/src/ubiquity/images/ubiquity_icon.png` & `ubiquity-student-1.0.1/src/ubiquity/images/ubiquity_icon.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/model.py` & `ubiquity-student-1.0.1/src/ubiquity/model.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/ubiquity_student.py` & `ubiquity-student-1.0.1/src/ubiquity/ubiquity_student.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/version.py` & `ubiquity-student-1.0.1/src/ubiquity/version.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/cui/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/views/cui/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/cui/main_view.py` & `ubiquity-student-1.0.1/src/ubiquity/views/cui/main_view.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/about.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/base.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/base.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/choice.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/choice.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/form.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/form.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/open.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/open.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/dialogs/preference.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/dialogs/preference.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/main_view.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/main_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,36 +10,37 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from tkinter import ttk
-from tkinter.constants import W, EW
+import signal
 import webbrowser
+from tkinter import ttk, messagebox
+from tkinter.constants import W, EW
 
 from .dialogs import ChoiceDialog
-from ..utils import is_success_run, LabelEnum
-from ...model import Model
+from ..utils import is_success_run, LabelEnum, ErrorMessage
 from ...controllers.main_controller import MainController, Returns
+from ...model import Model
 
 
 class MainView(ttk.Frame):
     """Class managing the main view of graphic user interface"""
     def __init__(self, parent, has_form, has_color):
         super().__init__()
         self.menu_bar = parent.menu_bar
         self.model: Model = parent.model
         self.main_controller: MainController = parent.controller
         self._has_form: bool = has_form
         self._has_color: bool = has_color
         self.mainframe = ttk.Frame()
         self.mainframe.pack()
+        signal.signal(signal.SIGUSR1, self.stop_suspend)
         if has_form:
             self.main_controller.init_values()
             self._ui_setup()
         else:
             self.submit()
 
     def _ui_setup(self):
@@ -89,14 +90,22 @@
         self.main_controller.stop()
         self._ui_setup()
         self.model.server.set("")
         self.model.student_key.set("")
         self.model.group_key.set("")
         self.model.directory.set("")
 
+    def stop_suspend(self, _signum, _frame):
+        self.model.error.set(ErrorMessage.PRACTICAL_WORK_SUSPENDED.value)
+        if self._has_form:
+            self.menu_bar.close_file()
+            messagebox.showerror(message=self.model.error.get())
+        else:
+            self.stop()
+
     def _open_web_browser(self):
         """Method opening a web browser"""
         webbrowser.open(self.model.url_web_view())
 
     def _clear(self):
         """Method to clear the view"""
         for widget in self.mainframe.winfo_children():
```

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/menu_bar.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/base.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/base.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sun_valley_dark.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sun_valley_dark.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sun_valley_light.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sun_valley_light.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/LICENSE` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/__init__.py` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl` & `ubiquity-student-1.0.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `ubiquity-student-0.8.2/src/ubiquity/views/utils.py` & `ubiquity-student-1.0.1/src/ubiquity/views/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     """Enum class for errors"""
     INVALID_KEYS = _('ERROR: The keys are invalid')
     CONNECTION_FAILED = _('ERROR: Failed to establish the connection')
     DIRECTORY_DOES_NOT_EXIST = _('ERROR: The directory does not exist')
     EMPTY_FIELD = _('ERROR: There are empty input fields')
     CONFIG_DELETED = _('ERROR: The group no longer exists')
     VERSION = _('ERROR: The client version is not valid')
+    PRACTICAL_WORK_SUSPENDED = _('ERROR: The practical work is suspended')
 
 
 class ConsoleColor(Enum):
     """Class console color"""
     SUCCESS = '\033[92m'  # GREEN
     WARNING = '\033[93m'  # YELLOW
     ERROR = '\033[91m'  # RED
```

### Comparing `ubiquity-student-0.8.2/ubiquity_student.egg-info/PKG-INFO` & `ubiquity-student-1.0.1/ubiquity_student.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 Metadata-Version: 2.1
 Name: ubiquity-student
-Version: 0.8.2
+Version: 1.0.1
 Summary: Ubiquity permet le suivi de TP de développement informatique
 Home-page: https://gitlab.insa-rouen.fr/cip/ubiquity
-License: UNKNOWN
 Download-URL: https://gitlab.insa-rouen.fr/cip/ubiquity/-/tags
 Project-URL: Documentation, https://gitlab.insa-rouen.fr/cip/ubiquity/-/wikis/home
 Project-URL: Bug Tracker, https://gitlab.insa-rouen.fr/cip/ubiquity/-/issues
-Description: # Ubiquity
-        
-        Ubiquity est un logiciel de suivi de TP de développement
-        informatique. Il permet aux tuteurs d’encadrer facilement et de
-        manière optimisée un groupe d’étudiants.
-        
-        Grâce à Ubiquity, l’enseignant crée de façon simple, un TP, en
-        déposant un sujet et sa correction annotée. Les étudiants
-        récupèrent ensuite le sujet ainsi que les fichiers sources à compléter.
-        
-        Ubiquity permet aussi à l’enseignant de suivre en temps réel
-        l’avancement de chaque étudiant dans la réalisation du TP, grâce
-        à différents indicateurs. Ainsi, l’enseignant identifie
-        rapidement les étudiants en difficultés. Ubiquity permet aussi aux
-        étudiants de se situer, par rapport à l’avancement de leurs
-        collègues.
-        
-        Ubiquity est un logiciel **opensource** et **gratuit**, disponible sur
-        Windows, MacOs et Linux. Il peut s’utiliser aussi bien en
-        présentiel qu’en distanciel, de manière synchrone ou asynchrone.
-        
-        
-        Pour plus d'information, nous vous invitons à regarder 
-        la vidéo de [présentation d'ubiquity](https://webtv.insa-rouen.fr/videos/presentation-de-ubiquity/) 
-        et à lire le [wiki](https://gitlab.insa-rouen.fr/delestre/ubiquity/-/wikis/home) proposant une documentation fonctionnelle et technique.
-        
-        ## Installation
-        
-        Pour installer l'application : `pip install ubiquity-student`
-        
-        ## Exécution
-        
-        Pour exécuter l'application : `ubiquity-student`
-        
-        ## Licence
-        
-        Distribué sous la License GNU GENERAL PUBLIC LICENSE v3.0. Voir [LICENSE](https://gitlab.insa-rouen.fr/cip/ubiquity/-/blob/master/LICENSE) pour plus d'information.
-Platform: UNKNOWN
 Classifier: Topic :: Education
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: French
 Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
+
+# Ubiquity
+
+Ubiquity est un logiciel de suivi de TP de développement
+informatique. Il permet aux tuteurs d’encadrer facilement et de
+manière optimisée un groupe d’étudiants.
+
+Grâce à Ubiquity, l’enseignant crée de façon simple, un TP, en
+déposant un sujet et sa correction annotée. Les étudiants
+récupèrent ensuite le sujet ainsi que les fichiers sources à compléter.
+
+Ubiquity permet aussi à l’enseignant de suivre en temps réel
+l’avancement de chaque étudiant dans la réalisation du TP, grâce
+à différents indicateurs. Ainsi, l’enseignant identifie
+rapidement les étudiants en difficultés. Ubiquity permet aussi aux
+étudiants de se situer, par rapport à l’avancement de leurs
+collègues.
+
+Ubiquity est un logiciel **opensource** et **gratuit**, disponible sur
+Windows, MacOs et Linux. Il peut s’utiliser aussi bien en
+présentiel qu’en distanciel, de manière synchrone ou asynchrone.
+
+
+Pour plus d'information, nous vous invitons à regarder 
+la vidéo de [présentation d'ubiquity](https://webtv.insa-rouen.fr/videos/presentation-de-ubiquity/) 
+et à lire le [wiki](https://gitlab.insa-rouen.fr/delestre/ubiquity/-/wikis/home) proposant une documentation fonctionnelle et technique.
+
+## Installation
+
+Pour installer l'application : `pip install ubiquity-student`
+
+## Exécution
+
+Pour exécuter l'application : `ubiquity-student`
+
+## Licence
+
+Distribué sous la License GNU GENERAL PUBLIC LICENSE v3.0. Voir [LICENSE](https://gitlab.insa-rouen.fr/cip/ubiquity/-/blob/master/LICENSE) pour plus d'information.
```

### Comparing `ubiquity-student-0.8.2/ubiquity_student.egg-info/SOURCES.txt` & `ubiquity-student-1.0.1/ubiquity_student.egg-info/SOURCES.txt`

 * *Files identical despite different names*

