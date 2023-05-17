# Comparing `tmp/Flet StoryBoard-1.3.tar.gz` & `tmp/Flet StoryBoard-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flet StoryBoard-1.3.tar", last modified: Sat May  6 16:21:39 2023, max compression
+gzip compressed data, was "Flet StoryBoard-1.4.tar", last modified: Wed May 17 17:29:29 2023, max compression
```

## Comparing `Flet StoryBoard-1.3.tar` & `Flet StoryBoard-1.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.682544 Flet StoryBoard-1.3/Flet_StoryBoard/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/edit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.686544 Flet StoryBoard-1.3/Flet_StoryBoard/engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_subwidgets_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_widget_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/suggesting_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/viewer_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/load_storyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.686544 Flet StoryBoard-1.3/Flet_StoryBoard/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.686544 Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/create_new_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/main_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pyodide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/sections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/edit_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/left_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/preview_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/create_storyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/get_url_icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/list_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/page_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/storyboard_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/All.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/open_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/paragraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/textfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.682544 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.061514 Flet StoryBoard-1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.049514 Flet StoryBoard-1.4/Flet_StoryBoard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-17 17:29:29.000000 Flet StoryBoard-1.4/Flet_StoryBoard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-17 17:29:29.000000 Flet StoryBoard-1.4/Flet_StoryBoard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:29:29.000000 Flet StoryBoard-1.4/Flet_StoryBoard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 17:29:29.000000 Flet StoryBoard-1.4/Flet_StoryBoard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 17:29:29.000000 Flet StoryBoard-1.4/Flet_StoryBoard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-17 17:29:29.061514 Flet StoryBoard-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.053514 Flet StoryBoard-1.4/fletsb/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/edit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.053514 Flet StoryBoard-1.4/fletsb/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/engines/edit_subwidgets_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/engines/edit_widget_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/engines/suggesting_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/engines/viewer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/load_storyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.053514 Flet StoryBoard-1.4/fletsb/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.053514 Flet StoryBoard-1.4/fletsb/pages/Settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/pages/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/pages/Settings/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/pages/create_new_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/pages/main_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/pages/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.053514 Flet StoryBoard-1.4/fletsb/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/sections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/sections/edit_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/sections/left_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/sections/preview_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.057514 Flet StoryBoard-1.4/fletsb/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/create_storyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/get_url_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/list_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/page_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/tools/storyboard_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.057514 Flet StoryBoard-1.4/fletsb/ui_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/ui_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/ui_toolkit/widget_browser_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.057514 Flet StoryBoard-1.4/fletsb/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/All.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:29.061514 Flet StoryBoard-1.4/fletsb/widgets/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/fletsb/widgets/widgets/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:29:29.061514 Flet StoryBoard-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-17 17:29:13.000000 Flet StoryBoard-1.4/setup.py
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/edit.py` & `Flet StoryBoard-1.4/fletsb/edit.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,19 @@
         self.cmd_args = sys.argv
         self.file_name = None
         flet.app(target=self.CNF)
 
         if self.file_name is None and debug_mode:
             print("Debug alert: Unexpected exit, no errors.")
             sys.exit("Exit.")
+            return
+        
+        if self.file_name is None:
+            sys.exit("Exit.")
+            return
 
         if not str(self.file_name).endswith(".fletsb"):
             self.file_name = str(self.file_name) + ".fletsb"
 
         if debug_mode:
             print("Debug alert: About to run the editor.")
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_subwidgets_engine.py` & `Flet StoryBoard-1.4/fletsb/engines/edit_subwidgets_engine.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_widget_engine.py` & `Flet StoryBoard-1.4/fletsb/engines/edit_widget_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 tf = flet.TextField(width=160, bgcolor=flet.colors.WHITE, color=flet.colors.BLACK, label=prop_name)
                 tf.value = prop_value
                 self.section_view.controls.append(flet.Row([tf], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = tf
                 if "multi_line" in default_args[prop_name]:
                     tf.multiline = True
 
-            elif isinstance(prop_type(), int):
+            elif type(prop_type()) == type(int()):
                 slid = flet.Slider(min=0, max=500, divisions=500, label="{value}", width=160)
                 slid.value = int(prop_value)
                 self.section_view.controls.append(
                     flet.Row(
                         [
                             flet.Text(
                                 f"{prop_name}:",
@@ -78,15 +78,15 @@
                     flet.Row(
                         [slid],
                         alignment=flet.MainAxisAlignment.CENTER
                     )
                 )
                 self.all_fields[prop_name] = slid
 
-            elif isinstance(prop_type(), bool):
+            elif type(prop_type()) == type(bool()):
                 tog = flet.Switch()
                 tog.value = prop_value
                 self.section_view.controls.append(
                     flet.Row([flet.Text(f"{prop_name}", color=flet.colors.WHITE, size=13), tog],
                              alignment=flet.MainAxisAlignment.CENTER, spacing=25))
                 self.all_fields[prop_name] = tog
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/engines/suggesting_engine.py` & `Flet StoryBoard-1.4/fletsb/engines/suggesting_engine.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/engines/viewer_engine.py` & `Flet StoryBoard-1.4/fletsb/engines/viewer_engine.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/load_storyboard.py` & `Flet StoryBoard-1.4/fletsb/load_storyboard.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 from .tools.storyboard_class import StoryBoard
 from .widgets.All import all_widgets
 import json
 import flet
 
 
 class LoadStoryBoard:
-    def __init__(self, target_function, storyboard_file_path: str):
+    def __init__(self, target_function, storyboard_file_path: str, view=flet.FLET_APP):
         # set up the important props
         self.current_page_name = "main"
         self.file_path = storyboard_file_path
         self.development_mode = False
         self.all_widgets = all_widgets
         self.dict_content = json.loads(open(self.file_path, encoding="utf-8").read())
         self.target_function = target_function
 
         # copy of things
         self.viewerEngine = viewerEngine
         # Run the app.
-        flet.app(target=self.run)
+        flet.app(target=self.run, view=view)
 
     def run(self, page: flet.Page):
         self.storyboard_class = StoryBoard(page=page, main_class=self)
         page.vertical_alignment = page.vertical_alignment = flet.MainAxisAlignment.CENTER
         self.page = page
         ve = viewerEngine(self, self.dict_content, self.current_page_name, page, page, self.development_mode)
         self.target_function(self.storyboard_class)
-        page.update()
-
-    def setup_storyboard_class(self):
-        pass
+        page.update()
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/pages.py` & `Flet StoryBoard-1.4/fletsb/pages/Settings/pages.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/pages/create_new_file.py` & `Flet StoryBoard-1.4/fletsb/pages/create_new_file.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/pages/main_page.py` & `Flet StoryBoard-1.4/fletsb/pages/main_page.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/pages/settings.py` & `Flet StoryBoard-1.4/fletsb/pages/settings.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/sections/edit_section.py` & `Flet StoryBoard-1.4/fletsb/sections/edit_section.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/sections/left_section.py` & `Flet StoryBoard-1.4/fletsb/sections/left_section.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/sections/preview_section.py` & `Flet StoryBoard-1.4/fletsb/sections/preview_section.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/tools/color_picker.py` & `Flet StoryBoard-1.4/fletsb/tools/color_picker.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/tools/create_storyboard.py` & `Flet StoryBoard-1.4/fletsb/tools/create_storyboard.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/tools/get_url_icon.py` & `Flet StoryBoard-1.4/fletsb/tools/get_url_icon.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/tools/list_picker.py` & `Flet StoryBoard-1.4/fletsb/tools/list_picker.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/tools/storyboard_class.py` & `Flet StoryBoard-1.4/fletsb/tools/storyboard_class.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
             self.__page,
             self.__main_class.development_mode
         )
         self.__page.update()
 
     def close_window(self):
         """Close the window"""
-        self.__page.window_close()
+        self.__page.window_close()
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py` & `Flet StoryBoard-1.4/fletsb/ui_toolkit/widget_browser_frame.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/All.py` & `Flet StoryBoard-1.4/fletsb/widgets/All.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from .widgets.title import Title
 from .widgets.open_url import Open_Url
 from .widgets.button import Button
 from .widgets.label import Label
 from .widgets.markdown import Markdown
 from .widgets.paragraph import Paragraph
 from .widgets.row import Row
+from .widgets.column import Column
 from .widgets.image import Image
 from .widgets.padding import Padding
 from .widgets.textfield import TextField
 from .widgets.navigator import Navigator
 
 all_widgets = {
     "Title": {"icon": "TEXT_FIELDS_ROUNDED", "class": Title},
+    "TextField": {"icon": "INPUT_ROUNDED", "class": TextField},
     "Open Url": {"icon": "INSERT_LINK_SHARP", "class": Open_Url},
     "Button": {"icon": "SMART_BUTTON_ROUNDED", "class": Button},
     "Label": {"icon": "MEDICAL_INFORMATION_OUTLINED", "class": Label},
     "Markdown": {"icon": "TEXT_SNIPPET_ROUNDED", "class": Markdown},
     "Paragraph": {"icon": "SHORT_TEXT_ROUNDED", "class": Paragraph},
     "Row": {"icon": "VIEW_COLUMN_OUTLINED", "class": Row},
+    "Column" : {"icon":"TABLE_ROWS_SHARP", "class":Column},
     "Image": {"icon": "IMAGE_OUTLINED", "class": Image},
     "Padding": {"icon": "SPACE_BAR_ROUNDED", "class": Padding},
-    "TextField": {"icon": "INPUT_ROUNDED", "class": TextField},
     "Navigator": {"icon": "NAVIGATE_NEXT", "class": Navigator}
 }
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/button.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/button.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/image.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/image.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/label.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/label.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/markdown.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/markdown.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/navigator.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/navigator.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/open_url.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/open_url.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/padding.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/padding.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/paragraph.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/paragraph.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/row.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/row.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/textfield.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/textfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
         self.parent = parent
         self.main_class = main_class
         self.self_object = flet.TextField(
             on_focus=self.on_start_type,
             on_change=self.on_change_text,
             on_submit=self.on_end_type,
             selection_color=flet.colors.BLACK,
-            cursor_color=flet.colors.BLACK,
-            # issue: focused_color can't have value "color"
-            focused_color="color"
+            cursor_color=flet.colors.BLACK
         )
 
         # all args
         self.args = {
             "text": {"type": str, "default_value": ""},
             "label": {"type": str, "default_value": "text.."},
             "hint_text": {"type": str, "default_value": "text.."},
```

### Comparing `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/title.py` & `Flet StoryBoard-1.4/fletsb/widgets/widgets/title.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/LICENSE` & `Flet StoryBoard-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.3/README.md` & `Flet StoryBoard-1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Flet StoryBoard
 Flet StoryBoard is a python library that have an easy to use tools for building graphical interfaces based on python `flet` library. Powerful interfaces with simple usability.
+
+So build UI apps using without coding the front-end, then connect it with python back-end!!!
+
 You can use these tools with only two main and simple functions!
 
 ## Goal 🏁
 My goal is to allow programmers to focus on the back-end, and build the front-end using just a simple easy-to-use window without any front-end coding require.
 
 ## installation ⬇️
 - Python > 3.7
@@ -36,23 +39,23 @@
 
 ## usage & examples 🤝
 There is a very simple docs here about library usage.
 [docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki)
 
 ### create/edit your own StoryBoard
 ```cmd
-python3 -m Flet_StoryBoard.edit myUI.fletsb
+python3 -m fletsb.edit myUI.fletsb
 ```
 It will edit the existing one or create a new one if not.
 
 ### load a StoryBoard
 To load your StoryBoard on your app, you can do this example code:
 
 ```python
-from Flet_StoryBoard import LoadStoryBoard, StoryBoard
+from fletsb import LoadStoryBoard, StoryBoard
 
 def main (storyBoard:StoryBoard):
     pass
 
 LoadStoryBoard(target_function=main, storyboard_file_path="myUI.fletsb")
 ```
```

