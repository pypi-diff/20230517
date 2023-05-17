# Comparing `tmp/xllabelme-5.1.6.tar.gz` & `tmp/xllabelme-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xllabelme-5.1.6.tar", last modified: Wed May 10 14:46:58 2023, max compression
+gzip compressed data, was "xllabelme-5.1.7.tar", last modified: Wed May 17 06:52:23 2023, max compression
```

## Comparing `xllabelme-5.1.6.tar` & `xllabelme-5.1.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.873485 xllabelme-5.1.6/
--rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.6/LICENSE
--rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    11738 2023-05-10 14:46:58.872485 xllabelme-5.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.754389 xllabelme-5.1.6/docs/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.763365 xllabelme-5.1.6/docs/man/
--rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.6/docs/man/labelme.1
--rw-rw-rw-   0        0        0       42 2023-05-10 14:46:58.874481 xllabelme-5.1.6/setup.cfg
--rw-rw-rw-   0        0        0     5290 2023-04-20 12:13:49.000000 xllabelme-5.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.776331 xllabelme-5.1.6/xllabelme/
--rw-rw-rw-   0        0        0     1074 2023-05-10 14:46:56.000000 xllabelme-5.1.6/xllabelme/__init__.py
--rw-rw-rw-   0        0        0     7602 2023-04-18 02:03:52.000000 xllabelme-5.1.6/xllabelme/__main__.py
--rw-rw-rw-   0        0        0    77978 2023-05-10 09:29:11.000000 xllabelme-5.1.6/xllabelme/app.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.791292 xllabelme-5.1.6/xllabelme/cli/
--rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/cli/__init__.py
--rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.6/xllabelme/cli/draw_json.py
--rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.6/xllabelme/cli/draw_label_png.py
--rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.6/xllabelme/cli/json_to_dataset.py
--rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.6/xllabelme/cli/on_docker.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.794282 xllabelme-5.1.6/xllabelme/config/
--rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.6/xllabelme/config/__init__.py
--rw-rw-rw-   0        0        0     2340 2023-04-16 08:40:27.000000 xllabelme-5.1.6/xllabelme/config/default_config.yaml
--rw-rw-rw-   0        0        0    62043 2023-05-10 14:45:43.000000 xllabelme-5.1.6/xllabelme/config/xllabellib.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.849123 xllabelme-5.1.6/xllabelme/icons/
--rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/cancel.png
--rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/close.png
--rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/color-line.png
--rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/color.png
--rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/copy.png
--rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/delete.png
--rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/done.png
--rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/done.svg
--rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/edit.png
--rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/expert.png
--rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/eye.png
--rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.6/xllabelme/icons/feBlend-icon.png
--rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/file.png
--rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/fit-width.png
--rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/fit-window.png
--rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/fit.png
--rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/help.png
--rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/icon.ico
--rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/icon.png
--rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.6/xllabelme/icons/icon2.ico
--rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.6/xllabelme/icons/icon2.png
--rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/labels.png
--rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/labels.svg
--rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/new.png
--rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/next.png
--rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/objects.png
--rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/open.png
--rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/open.svg
--rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/prev.png
--rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/quit.png
--rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save-as.png
--rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save-as.svg
--rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save.png
--rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save.svg
--rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/undo-cross.png
--rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/undo.png
--rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/zoom-in.png
--rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/zoom-out.png
--rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/zoom.png
--rw-rw-rw-   0        0        0     7120 2023-04-20 09:45:20.000000 xllabelme-5.1.6/xllabelme/label_file.py
--rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.6/xllabelme/logger.py
--rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.6/xllabelme/shape.py
--rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.6/xllabelme/testing.py
--rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.6/xllabelme/ts.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.855529 xllabelme-5.1.6/xllabelme/utils/
--rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/utils/__init__.py
--rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/utils/_io.py
--rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/utils/image.py
--rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.6/xllabelme/utils/qt.py
--rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.6/xllabelme/utils/shape.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.871488 xllabelme-5.1.6/xllabelme/widgets/
--rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.6/xllabelme/widgets/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.6/xllabelme/widgets/brightness_contrast_dialog.py
--rw-rw-rw-   0        0        0    35438 2023-04-20 08:18:28.000000 xllabelme-5.1.6/xllabelme/widgets/canvas.py
--rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/widgets/color_dialog.py
--rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/widgets/escapable_qlist_widget.py
--rw-rw-rw-   0        0        0     2451 2023-04-15 14:50:00.000000 xllabelme-5.1.6/xllabelme/widgets/file_dialog_preview.py
--rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.6/xllabelme/widgets/label_dialog.py
--rw-rw-rw-   0        0        0     6388 2023-05-10 09:32:37.000000 xllabelme-5.1.6/xllabelme/widgets/label_list_widget.py
--rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/widgets/tool_bar.py
--rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.6/xllabelme/widgets/unique_label_qlist_widget.py
--rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.6/xllabelme/widgets/zoom_widget.py
--rw-rw-rw-   0        0        0    11161 2023-05-10 13:24:58.000000 xllabelme-5.1.6/xllabelme/xlapp.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.784309 xllabelme-5.1.6/xllabelme.egg-info/
--rw-rw-rw-   0        0        0    11738 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      281 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.870742 xllabelme-5.1.7/
+-rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.7/LICENSE
+-rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    11738 2023-05-17 06:52:23.870742 xllabelme-5.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.792949 xllabelme-5.1.7/docs/
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.798933 xllabelme-5.1.7/docs/man/
+-rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.7/docs/man/labelme.1
+-rw-rw-rw-   0        0        0       42 2023-05-17 06:52:23.870742 xllabelme-5.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     5290 2023-04-20 12:13:49.000000 xllabelme-5.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.806911 xllabelme-5.1.7/xllabelme/
+-rw-rw-rw-   0        0        0     1074 2023-05-17 06:52:22.000000 xllabelme-5.1.7/xllabelme/__init__.py
+-rw-rw-rw-   0        0        0     7602 2023-04-18 02:03:52.000000 xllabelme-5.1.7/xllabelme/__main__.py
+-rw-rw-rw-   0        0        0    78415 2023-05-17 06:43:29.000000 xllabelme-5.1.7/xllabelme/app.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.815888 xllabelme-5.1.7/xllabelme/cli/
+-rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/cli/__init__.py
+-rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.7/xllabelme/cli/draw_json.py
+-rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.7/xllabelme/cli/draw_label_png.py
+-rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.7/xllabelme/cli/json_to_dataset.py
+-rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.7/xllabelme/cli/on_docker.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.818881 xllabelme-5.1.7/xllabelme/config/
+-rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.7/xllabelme/config/__init__.py
+-rw-rw-rw-   0        0        0     2340 2023-04-16 08:40:27.000000 xllabelme-5.1.7/xllabelme/config/default_config.yaml
+-rw-rw-rw-   0        0        0    63772 2023-05-17 06:47:57.000000 xllabelme-5.1.7/xllabelme/config/xllabellib.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.854784 xllabelme-5.1.7/xllabelme/icons/
+-rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/cancel.png
+-rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/close.png
+-rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/color-line.png
+-rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/color.png
+-rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/copy.png
+-rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/delete.png
+-rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/done.png
+-rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/done.svg
+-rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/edit.png
+-rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/expert.png
+-rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/eye.png
+-rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.7/xllabelme/icons/feBlend-icon.png
+-rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/file.png
+-rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/fit-width.png
+-rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/fit-window.png
+-rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/fit.png
+-rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/help.png
+-rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/icon.ico
+-rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/icon.png
+-rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.7/xllabelme/icons/icon2.ico
+-rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.7/xllabelme/icons/icon2.png
+-rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/labels.png
+-rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/labels.svg
+-rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/new.png
+-rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/next.png
+-rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/objects.png
+-rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/open.png
+-rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/open.svg
+-rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/prev.png
+-rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/quit.png
+-rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/save-as.png
+-rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/save-as.svg
+-rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/save.png
+-rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/save.svg
+-rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/undo-cross.png
+-rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/undo.png
+-rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/zoom-in.png
+-rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/zoom-out.png
+-rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/icons/zoom.png
+-rw-rw-rw-   0        0        0     7120 2023-04-20 09:45:20.000000 xllabelme-5.1.7/xllabelme/label_file.py
+-rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.7/xllabelme/logger.py
+-rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.7/xllabelme/shape.py
+-rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.7/xllabelme/testing.py
+-rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.7/xllabelme/ts.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.859771 xllabelme-5.1.7/xllabelme/utils/
+-rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/utils/__init__.py
+-rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/utils/_io.py
+-rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/utils/image.py
+-rw-rw-rw-   0        0        0     6443 2023-05-16 01:39:58.000000 xllabelme-5.1.7/xllabelme/utils/qt.py
+-rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.7/xllabelme/utils/shape.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.869744 xllabelme-5.1.7/xllabelme/widgets/
+-rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.7/xllabelme/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.7/xllabelme/widgets/brightness_contrast_dialog.py
+-rw-rw-rw-   0        0        0    35464 2023-05-13 08:19:03.000000 xllabelme-5.1.7/xllabelme/widgets/canvas.py
+-rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/widgets/color_dialog.py
+-rw-rw-rw-   0        0        0      358 2023-05-16 09:32:37.000000 xllabelme-5.1.7/xllabelme/widgets/escapable_qlist_widget.py
+-rw-rw-rw-   0        0        0     2451 2023-04-15 14:50:00.000000 xllabelme-5.1.7/xllabelme/widgets/file_dialog_preview.py
+-rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.7/xllabelme/widgets/label_dialog.py
+-rw-rw-rw-   0        0        0     6388 2023-05-10 09:32:37.000000 xllabelme-5.1.7/xllabelme/widgets/label_list_widget.py
+-rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.7/xllabelme/widgets/tool_bar.py
+-rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.7/xllabelme/widgets/unique_label_qlist_widget.py
+-rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.7/xllabelme/widgets/zoom_widget.py
+-rw-rw-rw-   0        0        0    11051 2023-05-17 02:23:48.000000 xllabelme-5.1.7/xllabelme/xlapp.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:52:23.811899 xllabelme-5.1.7/xllabelme.egg-info/
+-rw-rw-rw-   0        0        0    11738 2023-05-17 06:52:23.000000 xllabelme-5.1.7/xllabelme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2023-05-17 06:52:23.000000 xllabelme-5.1.7/xllabelme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:52:23.000000 xllabelme-5.1.7/xllabelme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      281 2023-05-17 06:52:23.000000 xllabelme-5.1.7/xllabelme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      116 2023-05-17 06:52:23.000000 xllabelme-5.1.7/xllabelme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 06:52:23.000000 xllabelme-5.1.7/xllabelme.egg-info/top_level.txt
```

### Comparing `xllabelme-5.1.6/LICENSE` & `xllabelme-5.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/PKG-INFO` & `xllabelme-5.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.6
+Version: 5.1.7
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.6 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.7 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.6/README.md` & `xllabelme-5.1.7/README.md`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/docs/man/labelme.1` & `xllabelme-5.1.7/docs/man/labelme.1`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/setup.py` & `xllabelme-5.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/__init__.py` & `xllabelme-5.1.7/xllabelme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 
 # 每当官方有第2位版本号更新，比如5.2、5.3时，我会尽力做个源码的同步
 # 然后我个人功能，会在第3位上自增，比如5.1.2、5.1.3
-__version__ = "5.1.6"
+__version__ = "5.1.7"
 
 # 2 扩展的更灵活的labelme，兼容官方的功能，但有更强的可视化效果，能查看shape的多个属性值
 __appname__ = f"xllabelme v{__version__}"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
```

### Comparing `xllabelme-5.1.6/xllabelme/__main__.py` & `xllabelme-5.1.7/xllabelme/__main__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/app.py` & `xllabelme-5.1.7/xllabelme/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,14 +590,19 @@
         labelMenu = QtWidgets.QMenu()
         utils.addActions(labelMenu, (edit, delete, clear_label))
         self.labelList.setContextMenuPolicy(Qt.CustomContextMenu)
         self.labelList.customContextMenuRequested.connect(
             self.popLabelListMenu
         )
 
+        self.fileListMenu = QtWidgets.QMenu()
+        self.fileListWidget.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.fileListWidget.customContextMenuRequested.\
+            connect(lambda pos: self.fileListMenu.exec_(self.fileListWidget.mapToGlobal(pos)))
+
         # Store actions for further handling.
         self.actions = utils.struct(
             saveAuto=saveAuto,
             saveWithImageData=saveWithImageData,
             changeOutputDir=changeOutputDir,
             save=save,
             saveAs=saveAs,
@@ -628,30 +633,41 @@
             fitWindow=fitWindow,
             fitWidth=fitWidth,
             brightnessContrast=brightnessContrast,
             zoomActions=zoomActions,
             openNextImg=openNextImg,
             openPrevImg=openPrevImg,
             fileMenuActions=(open_, opendir, save, saveAs, close, quit),
-            tool=(),
+            tool=[],
             # XXX: need to add some actions here to activate the shortcut
-            editMenu=(
+            editMenu=[
+                createMode,
+                createRectangleMode,
+                createCircleMode,
+                createLineMode,
+                createPointMode,
+                createLineStripMode,
+                editMode,
                 edit,
                 duplicate,
                 delete,
                 None,
                 undo,
                 undoLastPoint,
                 None,
                 removePoint,
                 None,
                 toggle_keep_prev_mode,
-            ),
+            ],
+            helpMenu=[
+                help,
+            ],
+            fileListMenu=[],
             # menu shown at right click，canvas里的右键菜单
-            menu=(
+            menu=[
                 createMode,
                 createRectangleMode,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
                 createLineStripMode,
                 editMode,
@@ -659,15 +675,15 @@
                 duplicate,
                 # copy,
                 # paste,
                 delete,
                 undo,
                 undoLastPoint,
                 removePoint,
-            ),
+            ],
             onLoadActive=(
                 close,
                 createMode,
                 createRectangleMode,
                 createCircleMode,
                 createLineMode,
                 createPointMode,
@@ -706,18 +722,18 @@
                 saveWithImageData,
                 close,
                 deleteFile,
                 None,
                 quit,
             ),
         )
-        utils.addActions(self.menus.help, (help,))
+        utils.addActions(self.menus.help, self.actions.helpMenu)
         utils.addActions(
             self.menus.view,
-            (
+            [
                 self.flag_dock.toggleViewAction(),
                 self.label_dock.toggleViewAction(),
                 self.shape_dock.toggleViewAction(),
                 self.file_dock.toggleViewAction(),
                 None,
                 fill_drawing,
                 None,
@@ -729,32 +745,32 @@
                 zoomOrg,
                 keepPrevScale,
                 None,
                 fitWindow,
                 fitWidth,
                 None,
                 brightnessContrast,
-            ),
+            ],
         )
 
         self.menus.file.aboutToShow.connect(self.updateFileMenu)
 
         # Custom context menu for the canvas widget:
         utils.addActions(self.canvas.menus[0], self.actions.menu)
         utils.addActions(
             self.canvas.menus[1],
-            (
+            [
                 action("复制到这里", self.copyShape),
                 action("移动到这里", self.moveShape),
-            ),
+            ],
         )
 
         self.tools = self.toolbar("Tools")
         # Menu buttons on Left
-        self.actions.tool = (
+        self.actions.tool = [
             # open_,
             opendir,
             openNextImg,
             openPrevImg,
             save,
             deleteFile,
             None,
@@ -765,15 +781,15 @@
             # paste,
             delete,
             undo,
             brightnessContrast,
             None,
             zoom,
             fitWidth,
-        )
+        ]
 
         self.statusBar().showMessage(self.tr("%s started.") % __appname__)
         self.statusBar().show()
 
         if output_file is not None and self._config["auto_save"]:
             logger.warn(
                 "If `auto_save` argument is True, `output_file` argument "
@@ -855,30 +871,24 @@
 
     # Support Functions
 
     def noShapes(self):
         return not len(self.labelList)
 
     def populateModeActions(self):
-        tool, menu = self.actions.tool, self.actions.menu
-        self.tools.clear()
-        utils.addActions(self.tools, tool)
-        self.canvas.menus[0].clear()
-        utils.addActions(self.canvas.menus[0], menu)
-        self.menus.edit.clear()
-        actions = (
-            self.actions.createMode,
-            self.actions.createRectangleMode,
-            self.actions.createCircleMode,
-            self.actions.createLineMode,
-            self.actions.createPointMode,
-            self.actions.createLineStripMode,
-            self.actions.editMode,
-        )
-        utils.addActions(self.menus.edit, list(actions) + list(self.actions.editMenu))
+        """ 刷新菜单和工具栏中的动作，我做了重构调整 """
+        def reset_menu(menu, actions):
+            menu.clear()
+            utils.addActions(menu, actions)
+
+        reset_menu(self.menus.edit, self.actions.editMenu)
+        reset_menu(self.menus.help, self.actions.helpMenu)
+        reset_menu(self.tools, self.actions.tool)
+        reset_menu(self.canvas.menus[0], self.actions.menu)
+        reset_menu(self.fileListMenu, self.actions.fileListMenu)
 
     def setDirty(self, dirty=True):
         """
         :param dirty: 需要设置不同级别，默认True处理。这里建议使用位运算区别不同内容的备份。
             1、True，labelme默认处理
             2，需要保存图片数据
         :return:
@@ -1236,15 +1246,15 @@
 
     def loadLabels(self, shapes):
         s = []
         for shape in shapes:
             label = shape["label"]
             points = shape["points"]
             shape_type = shape["shape_type"]
-            flags = shape["flags"]
+            flags = shape["flags"] or {}
             group_id = shape["group_id"]
             other_data = shape["other_data"]
 
             if not points:
                 # skip point-empty shape
                 continue
 
@@ -1368,15 +1378,15 @@
     def labelOrderChanged(self):
         self.setDirty()
         self.canvas.loadShapes([item.shape() for item in self.labelList])
 
     # Callback functions:
 
     def newShape(self):
-        self.project.new_shape()
+        self.project.newShape()
 
     def scrollRequest(self, delta, orientation):
         units = -delta * 0.1  # natural scroll
         bar = self.scrollBars[orientation]
         value = bar.value() + bar.singleStep() * units
         self.setScroll(orientation, value)
```

### Comparing `xllabelme-5.1.6/xllabelme/cli/draw_json.py` & `xllabelme-5.1.7/xllabelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/cli/draw_label_png.py` & `xllabelme-5.1.7/xllabelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/cli/json_to_dataset.py` & `xllabelme-5.1.7/xllabelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/cli/on_docker.py` & `xllabelme-5.1.7/xllabelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/config/__init__.py` & `xllabelme-5.1.7/xllabelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/config/default_config.yaml` & `xllabelme-5.1.7/xllabelme/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/config/xllabellib.py` & `xllabelme-5.1.7/xllabelme/config/xllabellib.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import requests
 import webbrowser
 
 import numpy as np
 
 from PyQt5.QtCore import QPointF, QTranslator, QLocale, QLibraryInfo
-from PyQt5.QtWidgets import QMenu, QAction, QFileDialog, QMessageBox, QActionGroup, QApplication
+from PyQt5.QtWidgets import QMenu, QAction, QFileDialog, QMessageBox, QActionGroup, QApplication, QWidget
 from qtpy import QtGui
 from qtpy.QtCore import Qt
 from PyQt5.QtGui import QImage, QPixmap, QColor
 
 from pyxllib.file.specialist import XlPath
 from pyxllib.algo.geo import rect_bounds
 from pyxllib.algo.pupil import make_index_function
@@ -49,15 +49,19 @@
                                       'text': ''}, ensure_ascii=False),
          },
     'm2303表格标注': {},
     'm2303表格标注二阶段': {
         '_attrs': [['text', 1, 'str', ('可见横线', '可见竖线', '不可见横线', '不可见竖线')]],
         'label_shape_color': ['text'],
     },
-    'm2305公式符号标注': {},
+    'm2305公式符号标注': {
+        'label_shape_color': ['loc'],
+        'label_shape_color2': ['symbo'],
+        'label_shape_color3': ['symbo', 'loc'],
+    },
     # '渊亭OCR':  # 这是比较旧的一套配置字段名
     #     {'_attrs':
     #          [['content_type', 1, 'str', ('印刷体', '手写体', '印章', '其它')],
     #           ['content_kv', 1, 'str', ('key', 'value')],
     #           ["content_class", 1, "str", ("姓名", "身份证号", "联系方式", "采样时间", "检测时间", "核酸结果", "其它类")],
     #           ['text', 1, 'str'],
     #           ],
@@ -166,18 +170,87 @@
     这里设计默认是labelme原版功能
     """
 
     def __init__(self, mainwin):
         self.mainwin = mainwin
         self.xllabel = mainwin.xllabel
         mainwin.showMaximized()  # 窗口最大化
+        self.菜单新增动作 = []
         self.create()
 
+    def __0_基础功能(self):
+        pass
+
+    def 查找控件(self, 名称, 类型=QWidget):
+        return self.mainwin.findChild(类型, 名称)
+
+    def set_label_color(self, label, color=None):
+        """ 对普通文本值，做固定颜色映射 """
+        from xllabelme.xlapp import _COLORS
+        if isinstance(color, str):
+            color = RgbFormatter.from_name(color).to_tuple()
+        self.mainwin.labelDialog.addLabelHistory(label)  # 文本加入检索
+        # 主要为了兼容xllabelme的一个tolist操作，所以要转np
+        _COLORS[label] = np.array(color, 'uint8')  # 颜色做固定映射
+        _COLORS[str({'text': label})] = np.array(color, 'uint8')  # 被转成字典的时候，也要带颜色映射规则
+
+    def __1_菜单类通用工程功能(self):
+        pass
+
+    def 菜单添加动作(self, menu,
+               text=None,  # 显示文本
+               slot=None,  # 触发函数
+               shortcut=None,  # 快捷键
+               icon=None,  # 预设的图标
+               tip=None,  # 详细提示内容
+               checkable=False,  # 可勾选？
+               enabled=True,  # 组件可使用？
+               checked=False,  # 选中状态？
+               name=None,  # 设一个全局名称，可以在其他地方需要的时候检索
+               ):
+        """ 通过这个函数添加的组会，切换project的时候，会自动进行检索销毁
+
+        注意这里的menu不是QMenu对象，而是菜单功能清单，原理流程是
+            1、提前用list存储到mainwin.actions里的动作列表，要展示的actions清单
+            2、调用main.populateModeActions，可以把mainwin.acitons里的功能菜单都更新出来
+            3、新建行为的时候，这个类里会做备份记录
+            4、destroy自动销毁的时候，会用list.index进行检索把对应的action都移除
+        """
+        if text is None:
+            self.菜单新增动作.append([menu, None])
+            menu.append(None)
+        else:
+            action = utils.newAction(self.mainwin, self.mainwin.tr(text), slot,
+                                     shortcut, icon, self.mainwin.tr(tip), checkable, enabled, checked)
+            if name:
+                action.setObjectName(name)
+            self.菜单新增动作.append([menu, action])
+            menu.append(action)
+            return action
+
+    def 菜单栏_编辑_添加动作(self, *args, **kwargs):
+        return self.菜单添加动作(self.mainwin.actions.editMenu, *args, **kwargs)
+
+    def 菜单栏_帮助_添加文档(self, 文档名称, 文档链接):
+        return self.菜单添加动作(self.mainwin.actions.helpMenu, 文档名称, lambda: webbrowser.open(文档链接))
+
+    def 左侧栏菜单添加动作(self, *args, **kwargs):
+        return self.菜单添加动作(self.mainwin.actions.tool, *args, **kwargs)
+
+    def 画布右键菜单添加动作(self, *args, **kwargs):
+        return self.菜单添加动作(self.mainwin.actions.menu, *args, **kwargs)
+
+    def 文件列表右键菜单添加动作(self, *args, **kwargs):
+        return self.菜单添加动作(self.mainwin.actions.fileListMenu, *args, **kwargs)
+
+    def __2_定制菜单(self):
+        pass
+
     def config_settings_menu(self):
-        """ Label菜单栏 """
+        """ 菜单栏_设置 """
         mainwin, xllabel = self.mainwin, self.xllabel
 
         def create_project_menu():
             # 1 关联选择任务后的回调函数
             def func(action):
                 # 1 内置数据格式
                 action.setCheckable(True)
@@ -289,173 +362,73 @@
         settings_menu.addAction(create_auto_rec_text_action())
         settings_menu.addAction(create_savefile_without_dialog_action())
         # 关闭该功能，发现原本就有类似的功能，是我重复造轮子了
         # settings_menu.addAction(create_set_image_root_action())
         settings_menu.addSeparator()
         settings_menu.addAction(create_reset_config_action())
 
-    def convert_to_rectangle_action(self):
-        """ 将shape形状改为四边形 """
-
-        def func():
-            item, shape = self.xllabel.get_current_select_shape()
-            if shape:
-                shape.shape_type = 'rectangle'
-                pts = [(p.x(), p.y()) for p in shape.points]
-                l, t, r, b = rect_bounds(pts)
-                shape.points = [QPointF(l, t), QPointF(r, b)]
-                mainwin.updateShape(shape, item)
-                mainwin.setDirty()
-
-        mainwin = self.mainwin
-        a = utils.newAction(mainwin,
-                            mainwin.tr("Convert to Rectangle"),
-                            func,
-                            None,  # 快捷键
-                            None,  # 图标
-                            mainwin.tr("将当前shape形状转为Rectangle矩形"),  # 左下角的提示
-                            enabled=False,
-                            )
-        return a
-
-    def rotate_image_action(self):
-        """ 旋转图片 """
-
-        def flip_points(sp, h):
-            from pyxllib.algo.geo import resort_quad_points
-            pts = sp.points
-            if sp.shape_type == 'rectangle':
-                # 矩形要特殊处理，仍然确保第1个点在左上角
-                x1, y1 = pts[0].x(), pts[0].y()
-                x2, y2 = pts[1].x(), pts[1].y()
-
-                pts[0].setX(h - y2)
-                pts[0].setY(x1)
-                pts[1].setX(h - y1)
-                pts[1].setY(x2)
-            elif sp.shape_type == 'polygon' and len(pts) == 4:
-                pts = [[h - p.y(), p.x()] for p in pts]
-                pts = resort_quad_points(pts)
-                for p1, p2 in zip(sp.points, pts):
-                    p1.setX(p2[0])
-                    p1.setY(p2[1])
-            else:  # 其他形状暂不特殊处理
-                for point in sp.points:
-                    x = point.x()  # 要中转存储下，不然等下x会被新值覆盖
-                    point.setX(h - point.y())
-                    point.setY(x)
-
-        def func():
-            """ 每次执行顺时针旋转90度 """
-            from PyQt5.QtGui import QTransform
-
-            # 1 旋转shapes坐标
-            canvas = mainwin.canvas
-            h = canvas.pixmap.height()
-            shapes = canvas.shapes
-            for sp in shapes:
-                flip_points(sp, h)
-
-            # 2 旋转图片
-            mainwin.updateShapes(shapes)
-            transform = QTransform()
-            transform.rotate(90)
-            canvas.pixmap = canvas.pixmap.transformed(transform)
-            mainwin.image = canvas.pixmap.toImage()
-
-            # 3 end
-            canvas.repaint()
-            mainwin.setDirty(3)
-
-        mainwin = self.mainwin
-        a = utils.newAction(mainwin,
-                            mainwin.tr("旋转图片"),
-                            func,
-                            None,  # 快捷键
-                            None,  # 图标
-                            mainwin.tr("将图片和当前标注的形状，顺时针旋转90度，可以多次操作调整到合适方向。"
-                                       "注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。"
-                                       "注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。")  # 左下角的提示
-                            )
-        return a
-
-    # def deskew_image_action(self):
-    #     def func():
-    #         canvas = mainwin.canvas
-    #         image = q_pixmap_to_np_array(canvas.pixmap)
-    #         image = xlcv.deskew_image(image)
-    #         canvas.pixmap = np_array_to_q_pixmap(image)
-    #         canvas.repaint()
-    #         mainwin.setDirty(2)
-    #
-    #     mainwin = self.mainwin
-    #     a = utils.newAction(mainwin,
-    #                         mainwin.tr("歪斜图片矫正"),
-    #                         func,
-    #                         None,  # 快捷键
-    #                         None,  # 图标
-    #                         mainwin.tr("歪斜比较严重的图片，可以尝试使用该功能矫正。"
-    #                                    "注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。"
-    #                                    "注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。")  # 左下角的提示
-    #                         )
-    #     return a
-
-    def create(self):
+    def create(self, update=True):
+        """ 子类也可能调用这个方法，此时populateModeActions不需要提前执行 """
         mainwin = self.mainwin
 
         # 1 设置菜单
         self.config_settings_menu()
 
-        # 2 帮助菜单
-        # mainwin.actions.helpMenu = list(mainwin.actions.editMenu) + [
-        #     ]
-
-        # 3 编辑菜单
-        mainwin.add_point_to_edge_action = utils.qt.newCheckableAction(
-            mainwin,
-            mainwin.tr("Add Point to Edge Enable"),  # 这个功能默认是开启的，导致兼职很容易经常误触增加多边形顶点，默认应该关闭
-            tip=mainwin.tr("选中shape的edge时，增加分割点"),
-        )
-        mainwin.delete_selected_shape_with_warning_action = utils.qt.newCheckableAction(
-            mainwin,
-            mainwin.tr("Delete Selected Shape With Warning"),
-            checked=True,
-        )
-        mainwin.actions.editMenu = list(mainwin.actions.editMenu) + [
-            None,
-            mainwin.add_point_to_edge_action,
-            mainwin.delete_selected_shape_with_warning_action,
-        ]
-
-        # 4 右键菜单增加功能
-        mainwin.actions.menu = list(mainwin.actions.menu) + [
-            None,
-            self.convert_to_rectangle_action(),
-            self.xllabel.split_shape_action(),
-            None,
-            self.rotate_image_action(),
-            # self.deskew_image_action(),  # 歪斜矫正
-        ]
-
-        # 5 一些操作习惯
-        mainwin.populateModeActions()
+        # 2 编辑菜单
+        # 这个功能原labelme默认是开启的，导致兼职很容易经常误触增加多边形顶点，默认应该关闭
+        self.菜单栏_编辑_添加动作()
+        mainwin.add_point_to_edge_action = \
+            self.菜单栏_编辑_添加动作('允许在多边形边上点击添加新顶点', checkable=True, tip='选中shape的edge时，增加分割点')
+        mainwin.delete_selected_shape_with_warning_action = \
+            self.菜单栏_编辑_添加动作('删除形状时会弹出提示框', checkable=True, checked=True, tip='选中shape的edge时，增加分割点')
+
+        # 3 画布菜单
+        self.画布右键菜单添加动作()
+        mainwin.convert_to_rectangle_action = \
+            self.画布右键菜单添加动作('将该多边形转为矩形', self.convert_to_rectangle, enabled=False)
+        mainwin.split_shape_action = \
+            self.画布右键菜单添加动作('切分该形状', self.xllabel.split_shape, enabled=False,
+                            tip='在当前鼠标点击位置，将一个shape拆成两个shape（注意，该功能会强制拆出两个矩形框）')
+        self.画布右键菜单添加动作()
+        self.画布右键菜单添加动作('旋转图片', self.rotate_image,
+                        tip='将图片和当前标注的形状，顺时针旋转90度，可以多次操作调整到合适方向。'
+                            '注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。'
+                            '注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。')
+        # self.画布右键菜单添加动作('歪斜图片矫正', self.deskew_image,
+        #                 tip='歪斜比较严重的图片，可以尝试使用该功能矫正。'
+        #                     '注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。'
+        #                     '注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。')
 
-    def shapeSelectionChanged(self, n_selected):
-        """ 选中shape时会激活的功能 """
-        menu = self.mainwin.actions.menu
-        menu[-4].setEnabled(n_selected)
-        menu[-3].setEnabled(n_selected)
+        # + 更新菜单的显示
+        if update:
+            mainwin.populateModeActions()
 
     def destroy(self):
         """ 销毁项目相关配置 """
         self.mainwin.menus.settings.clear()
-        self.mainwin.actions.editMenu = self.mainwin.actions.editMenu[:-3]
-        self.mainwin.actions.menu = self.mainwin.actions.menu[:-5]
 
-    def update_shape(self, shape, label_list_item=None):
+        for menu, action in list(reversed(self.菜单新增动作)):
+            if action is not None:  # 如果 action 不是 None，那么从 menu 中移除它
+                action.deleteLater()  # 这个好像不用显式执行，其他官方原本的action都没有执行，但执行下应该问题也不大
+            for i in range(len(menu) - 1, -1, -1):
+                if menu[i] is action:
+                    menu.pop(i)
+                    break
+        self.菜单新增动作 = []  # 清空 菜单新增动作 列表
+
+    def __3_修改原版有的接口(self):
+        """ 原版labelme有实现，但这里作了定制修改 """
+
+    def shapeSelectionChanged(self, n_selected):
+        """ 遍历所有跟选中shape时会激活有关的Action动作 """
+        mainwin = self.mainwin
+        mainwin.convert_to_rectangle_action.setEnabled(n_selected)
+        mainwin.split_shape_action.setEnabled(n_selected)
+
+    def updateShape(self, shape, label_list_item=None):
         """
         :param shape:
         :param label_list_item: item是shape的父级，挂在labelList下的项目
         """
         mainwin = self.mainwin
         label_list_item = LabelListWidgetItem(shape.label, shape)
         hashtext = shape.label
@@ -475,94 +448,192 @@
         parse_htext(hashtext)
         mainwin.labelDialog.addLabelHistory(hashtext)
 
         mainwin._update_shape_color(shape)
 
         return label_list_item
 
-    def new_shape(self):
-        """Pop-up and give focus to the label editor.
+    def get_default_label(self, shape=None):
+        """ 这个是自己自己扩展的一个获得默认文本值的功能 """
+        return ''
 
-        position MUST be in global coordinates.
+    def newShape(self, text=None):
+        """ 新建标注框时的规则
         """
         mainwin = self.mainwin
         items = mainwin.uniqLabelList.selectedItems()
-        text = None
         if items:
             text = items[0].data(Qt.UserRole)
         flags = {}
         group_id = None
-        if mainwin._config["display_label_popup"] or not text:
+        if mainwin._config["display_label_popup"]:
             previous_text = mainwin.labelDialog.edit.text()
-
-            text = self.get_default_label(shape=mainwin.canvas.shapes[-1])
             text, flags, group_id = mainwin.labelDialog.popUp(text)
-
             if not text:
                 mainwin.labelDialog.edit.setText(previous_text)
 
+        if text is None:
+            text = self.get_default_label(shape=mainwin.canvas.shapes[-1])
+
         if text and not mainwin.validateLabel(text):
             mainwin.errorMessage(
                 mainwin.tr("Invalid label"),
                 mainwin.tr("Invalid label '{}' with validation type '{}'").format(
                     text, mainwin._config["validate_label"]
                 ),
             )
             text = ""
         if text:
             mainwin.labelList.clearSelection()
             shape = mainwin.canvas.setLastLabel(text, flags)
             shape.group_id = group_id
+            # shape.description = description
             mainwin.addLabel(shape)
             mainwin.actions.editMode.setEnabled(True)
             mainwin.actions.undoLastPoint.setEnabled(False)
             mainwin.actions.undo.setEnabled(True)
             mainwin.setDirty()
         else:
             mainwin.canvas.undoLastLine()
             mainwin.canvas.shapesBackups.pop()
 
-    def get_default_label(self, shape=None):
-        """ 新建框的时候，使用的默认label值
-
-        在这里可以定制不同项目生成新标注框的规则
-        这里有办法获取原图，也有办法获取标注的shape，从而可以智能推断，给出识别值的
-        """
-        return self.mainwin.labelDialog.edit.text()
+    def __4_自己扩展的功能(self):
+        pass
 
     def open_last_workspace(self):
         """ 打开上一次退出软件的工作空间状态 """
         # 如果保存了目录和文件，打开上次工作状态
         if 'lastOpenDir' in self.xllabel.meta_cfg:
             d = XlPath(self.xllabel.meta_cfg['lastOpenDir'])
             if d.is_dir():
                 if 'filename' in self.xllabel.meta_cfg:
                     p = d / self.xllabel.meta_cfg['filename']
                     if p.is_file():
                         self.mainwin.importDirImages(d, filename=str(p), offset=0)
                         return
                 self.mainwin.importDirImages(d)
 
-    def set_label_color(self, label, color=None):
-        """ 对普通文本值，做固定颜色映射 """
-        from xllabelme.xlapp import _COLORS
+    def convert_to_rectangle(self):
+        """ 将shape形状改为四边形 """
+        item, shape = self.xllabel.get_current_select_shape()
+        if shape:
+            shape.shape_type = 'rectangle'
+            pts = [(p.x(), p.y()) for p in shape.points]
+            l, t, r, b = rect_bounds(pts)
+            shape.points = [QPointF(l, t), QPointF(r, b)]
+            self.mainwin.updateShape(shape, item)
+            self.mainwin.setDirty()
 
-        if isinstance(color, str):
-            color = RgbFormatter.from_name(color).to_tuple()
+    def rotate_image(self):
+        """ 旋转图片，每次执行顺时针旋转90度 """
 
-        self.mainwin.labelDialog.addLabelHistory(label)  # 文本加入检索
-        # 主要为了兼容xllabelme的一个tolist操作，所以要转np
-        _COLORS[label] = np.array(color, 'uint8')  # 颜色做固定映射
-        _COLORS[str({'text': label})] = np.array(color, 'uint8')  # 被转成字典的时候，也要带颜色映射规则
+        def flip_points(sp, h):
+            from pyxllib.algo.geo import resort_quad_points
+            pts = sp.points
+            if sp.shape_type == 'rectangle':
+                # 矩形要特殊处理，仍然确保第1个点在左上角
+                x1, y1 = pts[0].x(), pts[0].y()
+                x2, y2 = pts[1].x(), pts[1].y()
+
+                pts[0].setX(h - y2)
+                pts[0].setY(x1)
+                pts[1].setX(h - y1)
+                pts[1].setY(x2)
+            elif sp.shape_type == 'polygon' and len(pts) == 4:
+                pts = [[h - p.y(), p.x()] for p in pts]
+                pts = resort_quad_points(pts)
+                for p1, p2 in zip(sp.points, pts):
+                    p1.setX(p2[0])
+                    p1.setY(p2[1])
+            else:  # 其他形状暂不特殊处理
+                for point in sp.points:
+                    x = point.x()  # 要中转存储下，不然等下x会被新值覆盖
+                    point.setX(h - point.y())
+                    point.setY(x)
+
+        from PyQt5.QtGui import QTransform
+
+        # 1 旋转shapes坐标
+        mainwin = self.mainwin
+        canvas = mainwin.canvas
+        h = canvas.pixmap.height()
+        shapes = canvas.shapes
+        for sp in shapes:
+            flip_points(sp, h)
+
+        # 2 旋转图片
+        mainwin.updateShapes(shapes)
+        transform = QTransform()
+        transform.rotate(90)
+        canvas.pixmap = canvas.pixmap.transformed(transform)
+        mainwin.image = canvas.pixmap.toImage()
+
+        # 3 end
+        canvas.repaint()
+        mainwin.setDirty(3)
+
+    def deskew_image(self):
+        """ 歪斜图片矫正 """
+        from pyxllib.xlcv import xlcv
+        mainwin = self.mainwin
+        canvas = mainwin.canvas
+        image = q_pixmap_to_np_array(canvas.pixmap)
+        image = xlcv.deskew_image(image)
+        canvas.pixmap = np_array_to_q_pixmap(image)
+        canvas.repaint()
+        mainwin.setDirty(2)
+
+    def move_file(self, dst):
+        """ 把指定的文件移到其他目录、子目录里，可以参考 'm2303表格标注' 里的运用 """
+        # 0 准备
+        m = self.mainwin
+        fw = self.fileListWidget
+        item = fw.currentItem()
+        t = item.text()
+
+        if t.startswith(dst + '/'):
+            # 已经是分好类的，不处理
+            return
+
+        dst_path = XlPath.init(dst, m.lastOpenDir)
+        dst_path.mkdir(exist_ok=True)
+
+        # 1 移动文件
+        p = m.get_image_path()
+        p.move(dst_path / p.name)
+        p2 = m.get_label_path()
+        p2.move(dst_path / p2.name)
+
+        # 2 更新标签
+        item.setText(dst + '/' + p.name)
 
 
 class 增强版xllabelme(原版labelme):
     """ xllabelme扩展功能 """
 
-    def update_shape(self, shape, label_list_item=None):
+    def __2_定制菜单(self):
+        pass
+
+    def create(self, update=True):
+        super().create(False)
+        mainwin = self.mainwin
+
+        self.左侧栏菜单添加动作()
+        self.切换检查动作 = \
+            self.左侧栏菜单添加动作('切换检查', self.switch_check_mode, 'F1',
+                           tip='（快捷键：F1）切换不同的数据检查模式，有不同的高亮方案。')
+        self.switch_check_mode(update=False)  # 把更精细的tip提示更新出来
+
+        if update:
+            mainwin.populateModeActions()
+
+    def __3_修改原版有的接口(self):
+        pass
+
+    def updateShape(self, shape, label_list_item=None):
         """
         :param shape:
         :param label_list_item: item是shape的父级，挂在labelList下的项目
         """
         mainwin = self.mainwin
         # 1 确定显示的文本 text
         self.xllabel.update_other_data(shape)
@@ -646,36 +717,38 @@
         if xllabel.auto_rec_text and xllabel.xlapi and shape:
             k = 'label' if 'label' in xllabel.keys else 'text'
             text, score = xllabel.rec_text(shape.points)
             label = xllabel.set_label_attr(label, k, text)
             label = xllabel.set_label_attr(label, 'score', score)
         return label
 
-    def new_shape(self):
+    def newShape(self, text=None):
         """ 新建标注框时的规则
         """
         mainwin = self.mainwin
         items = mainwin.uniqLabelList.selectedItems()
-        text = None
         if items:
             text = items[0].data(Qt.UserRole)
         flags = {}
         group_id = None
-        if mainwin._config["display_label_popup"] or not text:
+        if mainwin._config["display_label_popup"]:
             previous_text = mainwin.labelDialog.edit.text()
 
             shape = Shape()
             shape.label = self.get_default_label(shape=mainwin.canvas.shapes[-1])
             shape = mainwin.labelDialog.popUp2(shape, mainwin)
             if shape is not None:
                 text, flags, group_id = shape.label, shape.flags, shape.group_id
 
             if not text:
                 mainwin.labelDialog.edit.setText(previous_text)
 
+        if text is None:
+            text = self.get_default_label(shape=mainwin.canvas.shapes[-1])
+
         if text and not mainwin.validateLabel(text):
             mainwin.errorMessage(
                 mainwin.tr("Invalid label"),
                 mainwin.tr("Invalid label '{}' with validation type '{}'").format(
                     text, mainwin._config["validate_label"]
                 ),
             )
@@ -689,22 +762,63 @@
             mainwin.actions.undoLastPoint.setEnabled(False)
             mainwin.actions.undo.setEnabled(True)
             mainwin.setDirty()
         else:
             mainwin.canvas.undoLastLine()
             mainwin.canvas.shapesBackups.pop()
 
+    def __4_自己扩展的功能(self):
+        pass
+
+    def switch_check_mode(self, *, update=True):
+        """ 设置不同的高亮格式 """
+        if update:
+            self.xllabel.default_shape_color_mode += 1
+            self.xllabel.reset()
+            self.mainwin.updateLabelListItems()
+
+        # 提示给出更具体的使用的范式配置
+        act = self.切换检查动作
+        tip = act.toolTip()
+        tip = re.sub(r'当前配置.*$', '', tip)
+        tip += '当前配置：' + ', '.join(self.xllabel.cfg['label_shape_color'])
+        act.setStatusTip(tip)
+        act.setToolTip(tip)
+
 
 class 文字通用(增强版xllabelme):
+
+    def __3_修改原版有的接口(self):
+        """ 原版labelme有实现，但这里作了定制修改 """
+
     def get_default_label(self, shape=None):
         d = {'text': '', 'category': '', 'text_kv': 'value', 'text_type': '印刷体'}
         return json.dumps(d, ensure_ascii=False)
 
 
 class m2302中科院题库(增强版xllabelme):
+
+    def __2_定制菜单(self):
+        pass
+
+    def create(self, update=True):
+        super().create(False)
+        mainwin = self.mainwin
+
+        self.左侧栏菜单添加动作('标注排序', self.resort_shapes, tip='重新对目前标注的框进行排序')
+        self.左侧栏菜单添加动作('检查全文章', self.browser_paper, tip='将内容按照shapes的顺序拼接成完整的文章，并检查公式渲染效果')
+        # todo 检查文本行
+        # todo 检查小分块
+
+        if update:
+            mainwin.populateModeActions()
+
+    def __3_修改原版有的接口(self):
+        """ 原版labelme有实现，但这里作了定制修改 """
+
     def get_default_label(self, shape=None):
         from pyxllib.cv.xlcvlib import xlcv
         from pyxlpr.data.imtextline import TextlineShape
 
         # 1 获得基本内容。如果开了识别接口，要调api。
         mainwin = self.mainwin
         xllabel = mainwin.xllabel
@@ -731,72 +845,18 @@
                 line_id = line_id0
             else:
                 line_id = line_id0 + 1
         d['line_id'] = line_id
 
         return json.dumps(d, ensure_ascii=False)
 
-    def create(self):
-        super().create()
-        mainwin = self.mainwin
-
-        action = functools.partial(utils.newAction, mainwin)
-        self.changeCheckAction = action(
-            "切换检查",
-            self.change_check,
-            'F1',  # 快捷键
-            None,
-            "（快捷键：F1）切换不同的数据检查模式，有不同的高亮方案。",
-            enabled=True,
-        )
-        resortShapesAction = action(
-            "标注排序",
-            self.resortShapes,
-            None,
-            None,
-            "重新对目前标注的框进行排序。",
-            enabled=True,
-        )
-        self.change_check(update=False)  # 把更精细的tip提示更新出来
-
-        checkFormulaAction = action(
-            "检查全文章",
-            self.browser_paper,
-            None,
-            None,
-            "将内容按照shapes的顺序拼接成完整的文章，并检查公式渲染效率",
-            enabled=True,
-        )
-        # 检查文本行
-        # 检查小分块
-        mainwin.actions.tool = list(mainwin.actions.tool) + [
-            None,
-            self.changeCheckAction,
-            resortShapesAction,
-            checkFormulaAction,
-        ]
-
-        mainwin.populateModeActions()
-
-    def change_check(self, *, update=True):
-        """ 设置不同的高亮格式 """
-        if update:
-            self.xllabel.default_shape_color_mode += 1
-            self.xllabel.reset()
-            self.mainwin.updateLabelListItems()
-
-        # 提示给出更具体的使用的范式配置
-        act = self.changeCheckAction
-        tip = act.toolTip()
-        tip = re.sub(r'当前配置.*$', '', tip)
-        tip += '当前配置：' + ', '.join(self.xllabel.cfg['label_shape_color'])
-        act.setStatusTip(tip)
-        act.setToolTip(tip)
+    def __4_自己扩展的功能(self):
+        pass
 
-    def resortShapes(self):
+    def resort_shapes(self):
         """ m2302中科院题库用，更新行号问题 """
         from pyxlpr.data.imtextline import TextlineShape
 
         mainwin = self.mainwin
         # 目前只用于一个项目
         if self.xllabel.meta_cfg['current_mode'] != 'm2302中科院题库':
             return
@@ -851,92 +911,97 @@
         # 2 获取渲染网页
         title = self.mainwin.get_label_path().stem
         r = requests.post('https://xmutpriu.com/latex/paper', json={'title': title, 'content': content})
         p = XlPath.init(title + '.html', XlPath.tempdir())
         p.write_text(r.text)
         webbrowser.open(p)
 
-    def destroy(self):
-        self.mainwin.actions.tool = self.mainwin.actions.tool[:-4]
-        self.mainwin.populateModeActions()
-        super().destroy()
-
 
 class m2303表格标注(原版labelme):
-    def get_default_label(self, shape=None):
-        return '表格'
 
-    def move_file(self, dst):
-        # 0 准备
-        m = self.mainwin
-        fw = self.fileListWidget
-        item = fw.currentItem()
-        t = item.text()
+    def __2_定制菜单(self):
+        pass
 
-        if t.startswith(dst + '/'):
-            # 已经是分好类的，不处理
-            return
+    def create(self, update=True):
+        super().create(False)
+        mainwin = self.mainwin
+        mainwin._config["display_label_popup"] = False  # 关闭这个参数可以在添加标注的时候不弹窗
 
-        dst_path = XlPath.init(dst, m.lastOpenDir)
-        dst_path.mkdir(exist_ok=True)
+        self.菜单栏_帮助_添加文档('表格标注文档', 'https://www.yuque.com/xlpr/data/zw58v08ay3rsy0hk?singleDoc#')
 
-        # 1 移动文件
-        p = m.get_image_path()
-        p.move(dst_path / p.name)
-        p2 = m.get_label_path()
-        p2.move(dst_path / p2.name)
+        self.文件列表右键菜单添加动作('移到"无表格"', lambda: self.move_file('无表格'))
+        # self.文件列表右键菜单添加动作('移到"重复图"', lambda: self.move_file('重复图'))
 
-        # 2 更新标签
-        item.setText(dst + '/' + p.name)
+        # 3 canvas右键可以添加一个全图方框的标注
+        self.画布右键菜单添加动作()
+        self.画布右键菜单添加动作('全图标记一个表格矩形框', self.add_full_image_table_label,
+                        tip='整张图都是一个完整的表格，全部画一个框')
 
-    def create(self):
-        super().create()
-
-        # 1 帮助文档
-        mainwin = self.mainwin
-        self.help_action = utils.newAction(mainwin,
-                                           mainwin.tr("表格标注文档"),
-                                           lambda: webbrowser.open("https://docs.qq.com/doc/DUnZJQnN1YkZMZkpx"))
-        mainwin.menus.help.addAction(self.help_action)
-
-        # 2 文件列表的右键菜单
-        fileListWidget = self.fileListWidget = mainwin.fileListWidget
-        self.menu = QMenu(self.fileListWidget)
-        self.menu.addAction('移到"无表格"', lambda: self.move_file('无表格'))
-        self.menu.addAction('移到"重复图"', lambda: self.move_file('重复图'))
-        fileListWidget.setContextMenuPolicy(Qt.CustomContextMenu)
-        fileListWidget.customContextMenuRequested.connect(lambda pos: self.menu.exec_(fileListWidget.mapToGlobal(pos)))
+        if update:
+            mainwin.populateModeActions()  # 要运行下这个才会更新菜单
 
     def destroy(self):
-        self.mainwin.menus.help.removeAction(self.help_action)
-        self.fileListWidget.customContextMenuRequested.disconnect()
+        self.mainwin._config["display_label_popup"] = True
         super().destroy()
 
+    def __3_修改原版有的接口(self):
+        """ 原版labelme有实现，但这里作了定制修改 """
+
+    def get_default_label(self, shape=None):
+        return 'table'
+
+    def __4_自己扩展的功能(self):
+        pass
+
+    def add_full_image_table_label(self):
+        """ 这里有些底层操作想封装的，但一封装又失去了灵活性。有时候批量添加的时候，也不用每次都刷新
+        想着就还是暂时先不封装
+        """
+        mainwin = self.mainwin
+        shape = Shape('table', shape_type='polygon', flags={})
+        # labelme的形状，下标是0开始，并且是左闭右闭的区间值
+        h, w = mainwin.image.height() - 1, mainwin.image.width() - 1
+        shape.points = [QPointF(0, 0), QPointF(w, 0), QPointF(w, h), QPointF(0, h)]
+        mainwin.canvas.shapes.append(shape)
+        mainwin.canvas.storeShapes()
+        mainwin.canvas.update()
+        mainwin.addLabel(shape)
+        mainwin.actions.editMode.setEnabled(True)
+        mainwin.actions.undoLastPoint.setEnabled(False)
+        mainwin.setDirty()
+
 
 class m2303表格标注二阶段(增强版xllabelme):
 
-    def create(self):
-        super().create()
+    def __2_定制菜单(self):
+        pass
+
+    def create(self, update=True):
+        super().create(False)
 
         mainwin = self.mainwin
-        url = "https://www.yuque.com/xlpr/data/kvq2g82zvk5x1lkb?singleDoc#"
-        self.help_action = utils.newAction(mainwin, mainwin.tr("表格二阶段标注说明"),
-                                           lambda: webbrowser.open(url))
-        mainwin.menus.help.addAction(self.help_action)
+        mainwin._config["display_label_popup"] = False  # 关闭这个参数可以在添加标注的时候不弹窗
+
+        self.菜单栏_帮助_添加文档('表格二阶段标注说明', 'https://www.yuque.com/xlpr/data/kvq2g82zvk5x1lkb?singleDoc#')
 
         self.set_label_color('可见横线', (0, 123, 255))  # 蓝色
         self.set_label_color('可见竖线', (40, 167, 69))  # 绿色
         self.set_label_color('不可见横线', (174, 223, 247))  # 不可见是可见对应的浅色
         self.set_label_color('不可见竖线', (180, 244, 190))
 
-    def destroy(self):
-        self.mainwin.menus.help.removeAction(self.help_action)
+        if update:
+            mainwin.populateModeActions()
 
+    def destroy(self):
+        self.mainwin._config["display_label_popup"] = True
         super().destroy()
 
+    def __3_修改原版有的接口(self):
+        """ 原版labelme有实现，但这里作了定制修改 """
+
     def get_default_label(self, shape=None):
         """ 还有些细节要调，如果弹窗，应该给出默认的几种类别文本 """
         from pyxllib.cv.xlcvlib import xlcv
 
         # 0 注意：标注过程中，是可以修改框的位置的
         # shape.points = [QPointF(100, 100), QPointF(200, 200)]
 
@@ -956,74 +1021,34 @@
         color = im.mean()  # 计算平均颜色，越接近255，表示越是空白图。
 
         # 3 自动识别线类型
         visible_tag = '可见' if color < 250 else '不可见'
         line_tag = '竖线' if height > width else '横线'
         return json.dumps({'text': visible_tag + line_tag}, ensure_ascii=False)
 
-    def new_shape(self):
-        """ 不用弹窗，直接给类别
-        """
-        mainwin = self.mainwin
-        items = mainwin.uniqLabelList.selectedItems()
-        text = None
-        if items:
-            text = items[0].data(Qt.UserRole)
-        flags = {}
-        group_id = None
-        if mainwin._config["display_label_popup"] or not text:
-            previous_text = mainwin.labelDialog.edit.text()
 
-            shape = Shape()
-            shape.label = self.get_default_label(shape=mainwin.canvas.shapes[-1])
-            # shape = mainwin.labelDialog.popUp2(shape, mainwin)
-            if shape is not None:
-                text, flags, group_id = shape.label, shape.flags, shape.group_id
+class m2305公式符号标注(增强版xllabelme):
 
-            if not text:
-                mainwin.labelDialog.edit.setText(previous_text)
-
-        if text and not mainwin.validateLabel(text):
-            mainwin.errorMessage(
-                mainwin.tr("Invalid label"),
-                mainwin.tr("Invalid label '{}' with validation type '{}'").format(
-                    text, mainwin._config["validate_label"]
-                ),
-            )
-            text = ""
-        if text:
-            mainwin.labelList.clearSelection()
-            shape = mainwin.canvas.setLastLabel(text, flags)
-            shape.group_id = group_id
-            mainwin.addLabel(shape)
-            mainwin.actions.editMode.setEnabled(True)
-            mainwin.actions.undoLastPoint.setEnabled(False)
-            mainwin.actions.undo.setEnabled(True)
-            mainwin.setDirty()
-        else:
-            mainwin.canvas.undoLastLine()
-            mainwin.canvas.shapesBackups.pop()
+    def __2_定制菜单(self):
+        pass
 
-class m2305公式符号标注(原版labelme):
-    def create(self):
-        super().create()
+    def create(self, update=True):
+        super().create(False)
 
         mainwin = self.mainwin
-        url = "https://www.yuque.com/xlpr/data/sn3uglc7g6l49akv?singleDoc#"
-        self.help_action = utils.newAction(mainwin, mainwin.tr("公式符号标注说明"),
-                                           lambda: webbrowser.open(url))
-        mainwin.menus.help.addAction(self.help_action)
+        self.菜单栏_帮助_添加文档('公式符号标注说明', 'https://www.yuque.com/xlpr/data/sn3uglc7g6l49akv?singleDoc#')
 
-    def destroy(self):
-        self.mainwin.menus.help.removeAction(self.help_action)
+        if update:
+            mainwin.populateModeActions()
 
-        super().destroy()
+    def __3_修改原版有的接口(self):
+        """ 原版labelme有实现，但这里作了定制修改 """
 
-    def new_shape(self):
-        """ 这个项目的new_shape比较特别，并不实际添加shape，而是把无效的矩形框重新替换标注
+    def newShape(self):
+        """ 这个项目的newShape比较特别，并不实际添加shape，而是把无效的矩形框重新替换标注
 
         这个功能是有一定通用性的，以后可以考虑怎么加到一般功能性框架。
         """
         # 1 找到第一个未显示的shape
         mainwin = self.mainwin
         model = mainwin.labelList.model()
         for index in range(model.rowCount()):
@@ -1035,14 +1060,15 @@
 
         # 2 更新shapes位置
         shapes = mainwin.canvas.shapes
 
         mainwin.labelList.clearSelection()
 
         item.shape().points = shapes[-1].points
+        item.shape().shape_type = shapes[-1].shape_type
         item.setCheckState(Qt.Checked)
         mainwin.canvas.shapes = shapes[:-1]
 
         mainwin.actions.editMode.setEnabled(True)
         mainwin.actions.undoLastPoint.setEnabled(False)
         mainwin.actions.undo.setEnabled(True)
         mainwin.setDirty()
@@ -1128,15 +1154,15 @@
                 else:
                     x['items'] = tuple(x['items'])
         self.keys = [x['key'] for x in cfg['attrs']]
         self.hide_attrs = [x['key'] for x in cfg['attrs'] if x['show'] == 0]
         self.cfg = cfg
 
         # 5 确定当前配色方案
-        ms = re.findall(r'(label_shape_color(?:\d+)?),', ','.join(self.cfg.keys()))
+        ms = re.findall(r'(label_shape_color(?:\d+)?)(?:,|$)', ','.join(self.cfg.keys()))
         if ms:
             idx = self.default_shape_color_mode % len(ms)
             self.cfg['label_shape_color'] = self.cfg[ms[idx]]
 
         # 6 设置项目
         if project:
             self.mainwin.project = self.open_project()
@@ -1231,33 +1257,34 @@
 
     def parse_shape(self, shape):
         """ xllabelme相关扩展功能，常用的shape解析
 
         :return:
             showtext，需要重定制展示内容
             hashtext，用于哈希颜色计算的label
-            labeldata，解析成字典的数据，如果其本身标注并不是字典，则该参数为空值
+            labelattr，解析成字典的数据，如果其本身标注并不是字典，则该参数为空值
         """
         # 1 默认值，后面根据参数情况会自动调整
         showtext = shape.label
         labelattr = self.get_labelattr(shape.label)
 
         # 2 hashtext
         # self.hashtext成员函数只简单分析labelattr，作为shape_color需要扩展考虑更多特殊情况
         hashtext = self.get_hashtext(labelattr)
+        # dprint(labelattr, hashtext)
         if not hashtext:
             if 'label' in labelattr:
                 hashtext = labelattr['label']
             elif 'id' in labelattr:
                 hashtext = labelattr['id']
             elif labelattr:
                 hashtext = next(iter(labelattr.values()))
             else:
                 hashtext = showtext
-        hashtext = str(hashtext)
+        hashtext = str(hashtext) or ' '  # 如果是空字符串，就映射到一个空格
 
         # 3 showtext
         if labelattr:
             # 3.1 隐藏部分属性
             hide_attrs = self.hide_attrs
             showdict = {k: v for k, v in labelattr.items() if k not in hide_attrs}
             # 3.2 排序
@@ -1320,23 +1347,25 @@
         :param labelattr:
         :param mode:
             label_shape_color
             label_line_color
             label_vertex_fill_colorS
         :return:
             如果 labelattr 有对应key，action也有开，则返回拼凑的哈希字符串值
-            否则返回 None
+            否则返回 ''
         """
         ls = []
         attrs = self.cfg.get(mode, [])
         for k in attrs:
             if k in labelattr:
-                ls.append(str(labelattr[k]))
+                ls.append(str(labelattr[k]) or ' ')
         if ls:
             return ', '.join(ls)
+        else:
+            return ''
 
     @classmethod
     def update_other_data(cls, shape):
         labelattr = cls.get_labelattr(shape.label, shape.other_data)
         if labelattr:
             shape.label = cls.json_dumps(labelattr)
             shape.other_data = {}
@@ -1456,70 +1485,58 @@
             return None, None
         item = mainwin.currentItem()
         if item is None:
             return None, None
         shape = item.shape()
         return item, shape
 
-    def split_shape_action(self):
+    def split_shape(self):
         """ 将一个框拆成两个框
 
         TODO 支持对任意四边形的拆分
         策略1：现有交互机制上，选择参考点后，拆分出多边形
         策略2：出来一把剪刀，通过画线指定切分的详细形式
         """
-
-        def func():
-            item, shape = self.get_current_select_shape()
-            if shape:
-                # 1 获取两个shape
-                # 第1个形状
-                pts = [(p.x(), p.y()) for p in shape.points]
-                l, t, r, b = rect_bounds(pts)
-                p = mainwin.canvas.prevPoint.x()  # 光标点击的位置
-                shape.shape_type = 'rectangle'
-                shape.points = [QPointF(l, t), QPointF(p, b)]
-
-                # 第2个形状
-                shape2 = shape.copy()
-                shape2.points = [QPointF(p, t), QPointF(r, b)]
-
-                # 2 调整label
-                # 如果开了识别模型，更新识别结果
-                if self.auto_rec_text and self.xlapi:
-                    self.update_shape_text(shape)
-                    self.update_shape_text(shape2)
-                else:  # 否则按几何比例重分配文本
-                    from pyxlpr.data.imtextline import merge_labels_by_widths
-                    text = self.get_labelattr(shape.label).get('text', '')
-                    text1, text2 = merge_labels_by_widths(list(text), [p - l, r - p], '')
-                    self.update_shape_text(shape, text1)
-                    self.update_shape_text(shape2, text2)
-
-                # 3 更新到shapes里
-                mainwin.canvas.selectedShapes.append(shape2)
-                mainwin.addLabel(shape2)
-                shapes = mainwin.canvas.shapes
-                idx = shapes.index(shape)
-                shapes = shapes[:idx + 1] + [shape2] + shapes[idx + 1:]  # 在相邻位置插入新的shape
-                mainwin.updateShapes(shapes)
-                mainwin.setDirty()
-
         mainwin = self.mainwin
-        a = utils.newAction(mainwin,
-                            mainwin.tr("Split Shape"),
-                            func,
-                            None,  # shortcut
-                            None,  # icon
-                            mainwin.tr("在当前鼠标点击位置，将一个shape拆成两个shape（注意，该功能会强制拆出两个矩形框）"),
-                            enabled=False,
-                            )
-        return a
+        item, shape = self.get_current_select_shape()
+        if shape:
+            # 1 获取两个shape
+            # 第1个形状
+            pts = [(p.x(), p.y()) for p in shape.points]
+            l, t, r, b = rect_bounds(pts)
+            p = mainwin.canvas.prevPoint.x()  # 光标点击的位置
+            shape.shape_type = 'rectangle'
+            shape.points = [QPointF(l, t), QPointF(p, b)]
+
+            # 第2个形状
+            shape2 = shape.copy()
+            shape2.points = [QPointF(p, t), QPointF(r, b)]
+
+            # 2 调整label
+            # 如果开了识别模型，更新识别结果
+            if self.auto_rec_text and self.xlapi:
+                self.update_shape_text(shape)
+                self.update_shape_text(shape2)
+            else:  # 否则按几何比例重分配文本
+                from pyxlpr.data.imtextline import merge_labels_by_widths
+                text = self.get_labelattr(shape.label).get('text', '')
+                text1, text2 = merge_labels_by_widths(list(text), [p - l, r - p], '')
+                self.update_shape_text(shape, text1)
+                self.update_shape_text(shape2, text2)
+
+            # 3 更新到shapes里
+            mainwin.canvas.selectedShapes.append(shape2)
+            mainwin.addLabel(shape2)
+            shapes = mainwin.canvas.shapes
+            idx = shapes.index(shape)
+            shapes = shapes[:idx + 1] + [shape2] + shapes[idx + 1:]  # 在相邻位置插入新的shape
+            mainwin.updateShapes(shapes)
+            mainwin.setDirty()
 
-    def change_check(self, update=True):
+    def switch_check_mode(self, update=True):
         """ 设置不同的高亮格式 """
         if update:
             self.default_shape_color_mode += 1
             self.reset()
             self.mainwin.updateLabelListItems()
 
         # 提示给出更具体的使用的范式配置
```

### Comparing `xllabelme-5.1.6/xllabelme/icons/cancel.png` & `xllabelme-5.1.7/xllabelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/close.png` & `xllabelme-5.1.7/xllabelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/color-line.png` & `xllabelme-5.1.7/xllabelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/color.png` & `xllabelme-5.1.7/xllabelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/copy.png` & `xllabelme-5.1.7/xllabelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/delete.png` & `xllabelme-5.1.7/xllabelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/done.png` & `xllabelme-5.1.7/xllabelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/done.svg` & `xllabelme-5.1.7/xllabelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/edit.png` & `xllabelme-5.1.7/xllabelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/expert.png` & `xllabelme-5.1.7/xllabelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/eye.png` & `xllabelme-5.1.7/xllabelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/feBlend-icon.png` & `xllabelme-5.1.7/xllabelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/file.png` & `xllabelme-5.1.7/xllabelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/fit-width.png` & `xllabelme-5.1.7/xllabelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/fit-window.png` & `xllabelme-5.1.7/xllabelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/fit.png` & `xllabelme-5.1.7/xllabelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/help.png` & `xllabelme-5.1.7/xllabelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/icon.ico` & `xllabelme-5.1.7/xllabelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/icon.png` & `xllabelme-5.1.7/xllabelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/icon2.ico` & `xllabelme-5.1.7/xllabelme/icons/icon2.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/icon2.png` & `xllabelme-5.1.7/xllabelme/icons/icon2.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/labels.png` & `xllabelme-5.1.7/xllabelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/labels.svg` & `xllabelme-5.1.7/xllabelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/new.png` & `xllabelme-5.1.7/xllabelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/next.png` & `xllabelme-5.1.7/xllabelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/objects.png` & `xllabelme-5.1.7/xllabelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/open.png` & `xllabelme-5.1.7/xllabelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/open.svg` & `xllabelme-5.1.7/xllabelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/prev.png` & `xllabelme-5.1.7/xllabelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/quit.png` & `xllabelme-5.1.7/xllabelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/save-as.png` & `xllabelme-5.1.7/xllabelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/save-as.svg` & `xllabelme-5.1.7/xllabelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/save.png` & `xllabelme-5.1.7/xllabelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/save.svg` & `xllabelme-5.1.7/xllabelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/undo-cross.png` & `xllabelme-5.1.7/xllabelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/undo.png` & `xllabelme-5.1.7/xllabelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/zoom-in.png` & `xllabelme-5.1.7/xllabelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/zoom-out.png` & `xllabelme-5.1.7/xllabelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/icons/zoom.png` & `xllabelme-5.1.7/xllabelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/label_file.py` & `xllabelme-5.1.7/xllabelme/label_file.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/logger.py` & `xllabelme-5.1.7/xllabelme/logger.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/shape.py` & `xllabelme-5.1.7/xllabelme/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/testing.py` & `xllabelme-5.1.7/xllabelme/testing.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/ts.py` & `xllabelme-5.1.7/xllabelme/ts.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/utils/__init__.py` & `xllabelme-5.1.7/xllabelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/utils/_io.py` & `xllabelme-5.1.7/xllabelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/utils/image.py` & `xllabelme-5.1.7/xllabelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/utils/qt.py` & `xllabelme-5.1.7/xllabelme/utils/qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
         b.setIcon(newIcon(icon))
     if slot is not None:
         b.clicked.connect(slot)
     return b
 
 
 def newAction(
-        parent,
-        text,
-        slot=None,
-        shortcut=None,
-        icon=None,
-        tip=None,
-        checkable=False,
-        enabled=True,
-        checked=False,
+        parent,  # 父类
+        text,  # 显示文本
+        slot=None,  # 触发函数
+        shortcut=None,  # 快捷键
+        icon=None,  # 预设的图标
+        tip=None,  # 详细提示内容
+        checkable=False,  # 可勾选？
+        enabled=True,  # 组件可使用？
+        checked=False,  # 选中状态？
 ):
     """Create a new action and assign callbacks, shortcuts, etc."""
     a = QtWidgets.QAction(text, parent)
     if icon is not None:
         a.setIconText(text.replace(" ", "\n"))
         a.setIcon(newIcon(icon))
     if shortcut is not None:
```

### Comparing `xllabelme-5.1.6/xllabelme/utils/shape.py` & `xllabelme-5.1.7/xllabelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/__init__.py` & `xllabelme-5.1.7/xllabelme/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/brightness_contrast_dialog.py` & `xllabelme-5.1.7/xllabelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/canvas.py` & `xllabelme-5.1.7/xllabelme/widgets/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
                 self.hEdge = None
                 shape.highlightVertex(index, shape.MOVE_VERTEX)
                 self.overrideCursor(CURSOR_POINT)
                 self.setToolTip(self.mainwin.tr("Click & drag to move point"))
                 self.setStatusTip(self.toolTip())
                 self.update()
                 break
-            elif index_edge is not None and shape.canAddPoint() and self.mainwin.check_add_point_to_edge:
+            elif index_edge is not None and shape.canAddPoint() and self.mainwin.add_point_to_edge_action.isChecked():
                 # 悬停在edge多边形边上
                 if self.selectedVertex():
                     self.hShape.highlightClear()
                 self.prevhVertex = self.hVertex
                 self.hVertex = None
                 self.prevhShape = self.hShape = shape
                 self.prevhEdge = self.hEdge = index_edge
@@ -404,15 +404,15 @@
                         if self.createMode == "circle":
                             self.current.shape_type = "circle"
                         self.line.points = [pos, pos]
                         self.setHiding()
                         self.drawingPolygon.emit(True)
                         self.update()
             elif self.editing():
-                if self.selectedEdge() and self.mainwin.check_add_point_to_edge:
+                if self.selectedEdge() and self.mainwin.add_point_to_edge_action.isChecked():
                     self.addPointToEdge()
                 elif (
                     self.selectedVertex()
                     and int(ev.modifiers()) == QtCore.Qt.ShiftModifier
                 ):
                     # Delete point if: left-click + SHIFT on a point
                     self.removeSelectedPoint()
```

### Comparing `xllabelme-5.1.6/xllabelme/widgets/color_dialog.py` & `xllabelme-5.1.7/xllabelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/file_dialog_preview.py` & `xllabelme-5.1.7/xllabelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/label_dialog.py` & `xllabelme-5.1.7/xllabelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/label_list_widget.py` & `xllabelme-5.1.7/xllabelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/tool_bar.py` & `xllabelme-5.1.7/xllabelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/unique_label_qlist_widget.py` & `xllabelme-5.1.7/xllabelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/widgets/zoom_widget.py` & `xllabelme-5.1.7/xllabelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.6/xllabelme/xlapp.py` & `xllabelme-5.1.7/xllabelme/xlapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                 '检测时间': '蓝色',
                 '核酸结果': '红色',
                 '14天经过或途经': '绿色',
                 '健康码颜色': '鲜绿色',
                 '其他类': '亮灰色'})
 
 _COLORS = {k: np.array(RgbFormatter.from_name(v).to_tuple(), 'uint8') for k, v in _COLORS.items()}
+_COLORS[' '] = np.array((128, 128, 128), 'uint8')  # 空值强制映射为灰色
 
 
 class XlMainWindow(MainWindow):
     def __init__(
             self,
             config=None,
             filename=None,
@@ -138,15 +139,15 @@
 
     def updateLabelListItems(self):
         for i in range(len(self.labelList)):
             item = self.labelList[i]
             self.updateShape(item.shape(), item)
 
     def updateShape(self, shape, label_list_item=None):
-        return self.project.update_shape(shape, label_list_item)
+        return self.project.updateShape(shape, label_list_item)
 
     def _get_rgb_by_label(self, label):
         """ 该函数可以强制限定某些映射颜色 """
         if label in _COLORS:
             return _COLORS[label]
 
         # 原来的颜色配置代码
@@ -224,19 +225,14 @@
             return True
         except LabelFileError as e:
             self.errorMessage(
                 self.tr("Error saving label data"), self.tr("<b>%s</b>") % e
             )
             return False
 
-    @property
-    def check_add_point_to_edge(self):
-        """ 判断添加点到多边形edge上的功能是否有打开 """
-        return self.add_point_to_edge_action.isChecked()
-
     def __get_describe(self):
         """ 各种悬停的智能提示 """
 
     def get_pos_desc(self, pos, brief=False):
         """ 当前光标所在位置的提示
 
         :param pos: 相对原图尺寸、位置的坐标点
```

### Comparing `xllabelme-5.1.6/xllabelme.egg-info/PKG-INFO` & `xllabelme-5.1.7/xllabelme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.6
+Version: 5.1.7
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.6 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.7 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.6/xllabelme.egg-info/SOURCES.txt` & `xllabelme-5.1.7/xllabelme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

