# Comparing `tmp/deep_copilot-0.0.5.tar.gz` & `tmp/deep_copilot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_copilot-0.0.5.tar", last modified: Wed May 17 11:03:39 2023, max compression
+gzip compressed data, was "deep_copilot-0.0.6.tar", last modified: Wed May 17 11:20:27 2023, max compression
```

## Comparing `deep_copilot-0.0.5.tar` & `deep_copilot-0.0.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.926931 deep_copilot-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11558 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 11:03:39.925931 deep_copilot-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.915931 deep_copilot-0.0.5/deep_copilot/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 07:53:29.000000 deep_copilot-0.0.5/deep_copilot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.917931 deep_copilot-0.0.5/deep_copilot/audio_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2022-10-11 01:39:00.000000 deep_copilot-0.0.5/deep_copilot/audio_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-05-17 09:05:05.000000 deep_copilot-0.0.5/deep_copilot/audio_tools/base_audio_tools.py
--rw-r--r--   0 root         (0) root         (0)     8546 2022-10-11 06:47:07.000000 deep_copilot-0.0.5/deep_copilot/audio_tools/vad_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.918931 deep_copilot-0.0.5/deep_copilot/command_tools/
--rw-r--r--   0 root         (0) root         (0)      129 2022-09-23 08:46:31.000000 deep_copilot-0.0.5/deep_copilot/command_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      303 2022-09-23 03:56:36.000000 deep_copilot-0.0.5/deep_copilot/command_tools/compat.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-05-17 09:18:16.000000 deep_copilot-0.0.5/deep_copilot/command_tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.918931 deep_copilot-0.0.5/deep_copilot/date_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2022-10-10 08:58:10.000000 deep_copilot-0.0.5/deep_copilot/date_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-05-17 09:05:05.000000 deep_copilot-0.0.5/deep_copilot/date_tools/datetimeutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.918931 deep_copilot-0.0.5/deep_copilot/excel_tools/
--rw-r--r--   0 root         (0) root         (0)      129 2022-09-16 08:29:18.000000 deep_copilot-0.0.5/deep_copilot/excel_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1643 2022-09-27 07:15:50.000000 deep_copilot-0.0.5/deep_copilot/excel_tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.919931 deep_copilot-0.0.5/deep_copilot/faiss_tools/
--rw-r--r--   0 root         (0) root         (0)      136 2023-03-30 06:39:27.000000 deep_copilot-0.0.5/deep_copilot/faiss_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-01-03 13:34:50.000000 deep_copilot-0.0.5/deep_copilot/faiss_tools/faiss_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.919931 deep_copilot-0.0.5/deep_copilot/hanlp_tools/
--rw-r--r--   0 root         (0) root         (0)      129 2022-11-03 11:34:56.000000 deep_copilot-0.0.5/deep_copilot/hanlp_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/hanlp_tools/hanlp_copilot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.920931 deep_copilot-0.0.5/deep_copilot/log_tools/
--rw-r--r--   0 root         (0) root         (0)      128 2022-09-06 09:29:11.000000 deep_copilot-0.0.5/deep_copilot/log_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/log_tools/log_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.920931 deep_copilot-0.0.5/deep_copilot/misc_tools/
--rw-r--r--   0 root         (0) root         (0)      129 2022-11-02 07:19:29.000000 deep_copilot-0.0.5/deep_copilot/misc_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5169 2023-02-13 06:44:39.000000 deep_copilot-0.0.5/deep_copilot/misc_tools/es_tools.py
--rw-r--r--   0 root         (0) root         (0)     6659 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/misc_tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.921931 deep_copilot-0.0.5/deep_copilot/mysql_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 08:03:31.000000 deep_copilot-0.0.5/deep_copilot/mysql_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12529 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/mysql_tools/mysql_copilot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.921931 deep_copilot-0.0.5/deep_copilot/path_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2022-11-18 08:11:56.000000 deep_copilot-0.0.5/deep_copilot/path_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3406 2022-11-18 08:17:40.000000 deep_copilot-0.0.5/deep_copilot/path_tools/path_copilot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.922931 deep_copilot-0.0.5/deep_copilot/seed_tools/
--rw-r--r--   0 root         (0) root         (0)      129 2022-09-07 03:30:37.000000 deep_copilot-0.0.5/deep_copilot/seed_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/seed_tools/seed_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.922931 deep_copilot-0.0.5/deep_copilot/string_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2022-10-12 06:01:05.000000 deep_copilot-0.0.5/deep_copilot/string_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3530 2023-03-07 08:42:48.000000 deep_copilot-0.0.5/deep_copilot/string_tools/string_copilot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.924931 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2022-09-23 03:49:41.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1095 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/base_image_tools.py
--rw-r--r--   0 root         (0) root         (0)     7517 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/base_video_tools.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/ffmpeg_tools.py
--rw-r--r--   0 root         (0) root         (0)     8461 2022-05-18 08:51:21.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/ffmpyutil.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/key_frame_extraction_tools.py
--rw-r--r--   0 root         (0) root         (0)      690 2022-09-23 05:56:01.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/moviepy_tools.py
--rw-r--r--   0 root         (0) root         (0)     6704 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/opencv_tools.py
--rw-r--r--   0 root         (0) root         (0)     2231 2022-05-26 07:58:31.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/sceneutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.925931 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-30 06:39:27.000000 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5552 2023-05-17 09:28:11.000000 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/chatgpt_tools.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/t5_model_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.916931 deep_copilot-0.0.5/deep_copilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1953 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.5/deep_copilot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      289 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-05-17 08:17:49.000000 deep_copilot-0.0.5/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 11:03:39.926931 deep_copilot-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2117 2023-05-17 09:16:07.000000 deep_copilot-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.953408 deep_copilot-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-17 07:38:12.000000 deep_copilot-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-05-17 07:38:12.000000 deep_copilot-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      116 2023-05-17 07:38:12.000000 deep_copilot-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 11:20:27.953408 deep_copilot-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-17 07:38:12.000000 deep_copilot-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.943408 deep_copilot-0.0.6/deep_copilot/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 07:53:29.000000 deep_copilot-0.0.6/deep_copilot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.945407 deep_copilot-0.0.6/deep_copilot/audio_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-10-11 01:39:00.000000 deep_copilot-0.0.6/deep_copilot/audio_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-05-17 09:05:05.000000 deep_copilot-0.0.6/deep_copilot/audio_tools/base_audio_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8546 2022-10-11 06:47:07.000000 deep_copilot-0.0.6/deep_copilot/audio_tools/vad_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.946408 deep_copilot-0.0.6/deep_copilot/command_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-23 08:46:31.000000 deep_copilot-0.0.6/deep_copilot/command_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      303 2022-09-23 03:56:36.000000 deep_copilot-0.0.6/deep_copilot/command_tools/compat.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-05-17 09:18:16.000000 deep_copilot-0.0.6/deep_copilot/command_tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.946408 deep_copilot-0.0.6/deep_copilot/date_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-10-10 08:58:10.000000 deep_copilot-0.0.6/deep_copilot/date_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-05-17 09:05:05.000000 deep_copilot-0.0.6/deep_copilot/date_tools/datetimeutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.946408 deep_copilot-0.0.6/deep_copilot/excel_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-16 08:29:18.000000 deep_copilot-0.0.6/deep_copilot/excel_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2022-09-27 07:15:50.000000 deep_copilot-0.0.6/deep_copilot/excel_tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.947408 deep_copilot-0.0.6/deep_copilot/faiss_tools/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-03-30 06:39:27.000000 deep_copilot-0.0.6/deep_copilot/faiss_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-01-03 13:34:50.000000 deep_copilot-0.0.6/deep_copilot/faiss_tools/faiss_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.947408 deep_copilot-0.0.6/deep_copilot/hanlp_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-11-03 11:34:56.000000 deep_copilot-0.0.6/deep_copilot/hanlp_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-17 08:59:59.000000 deep_copilot-0.0.6/deep_copilot/hanlp_tools/hanlp_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.948408 deep_copilot-0.0.6/deep_copilot/log_tools/
+-rw-r--r--   0 root         (0) root         (0)      128 2022-09-06 09:29:11.000000 deep_copilot-0.0.6/deep_copilot/log_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/log_tools/log_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.948408 deep_copilot-0.0.6/deep_copilot/misc_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-11-02 07:19:29.000000 deep_copilot-0.0.6/deep_copilot/misc_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5169 2023-02-13 06:44:39.000000 deep_copilot-0.0.6/deep_copilot/misc_tools/es_tools.py
+-rw-r--r--   0 root         (0) root         (0)     6659 2023-05-17 08:59:59.000000 deep_copilot-0.0.6/deep_copilot/misc_tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.949408 deep_copilot-0.0.6/deep_copilot/mysql_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 08:03:31.000000 deep_copilot-0.0.6/deep_copilot/mysql_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12529 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/mysql_tools/mysql_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.949408 deep_copilot-0.0.6/deep_copilot/path_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-11-18 08:11:56.000000 deep_copilot-0.0.6/deep_copilot/path_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2022-11-18 08:17:40.000000 deep_copilot-0.0.6/deep_copilot/path_tools/path_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.950408 deep_copilot-0.0.6/deep_copilot/seed_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-07 03:30:37.000000 deep_copilot-0.0.6/deep_copilot/seed_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-05-17 08:59:59.000000 deep_copilot-0.0.6/deep_copilot/seed_tools/seed_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.950408 deep_copilot-0.0.6/deep_copilot/string_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-10-12 06:01:05.000000 deep_copilot-0.0.6/deep_copilot/string_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3530 2023-03-07 08:42:48.000000 deep_copilot-0.0.6/deep_copilot/string_tools/string_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.952408 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-09-23 03:49:41.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/base_image_tools.py
+-rw-r--r--   0 root         (0) root         (0)     7517 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/base_video_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/ffmpeg_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8461 2022-05-18 08:51:21.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/ffmpyutil.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/key_frame_extraction_tools.py
+-rw-r--r--   0 root         (0) root         (0)      690 2022-09-23 05:56:01.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/moviepy_tools.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-05-17 08:51:50.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/opencv_tools.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2022-05-26 07:58:31.000000 deep_copilot-0.0.6/deep_copilot/video_and_image_tools/sceneutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.953408 deep_copilot-0.0.6/deep_copilot/zero_short_model_tools/
+-rw-r--r--   0 root         (0) root         (0)      134 2023-03-30 06:39:27.000000 deep_copilot-0.0.6/deep_copilot/zero_short_model_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-17 09:28:11.000000 deep_copilot-0.0.6/deep_copilot/zero_short_model_tools/chatgpt_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-05-17 08:59:59.000000 deep_copilot-0.0.6/deep_copilot/zero_short_model_tools/t5_model_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:20:27.944408 deep_copilot-0.0.6/deep_copilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 11:20:27.000000 deep_copilot-0.0.6/deep_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-05-17 11:20:27.000000 deep_copilot-0.0.6/deep_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 11:20:27.000000 deep_copilot-0.0.6/deep_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.6/deep_copilot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      289 2023-05-17 11:20:27.000000 deep_copilot-0.0.6/deep_copilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 11:20:27.000000 deep_copilot-0.0.6/deep_copilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-17 11:03:46.000000 deep_copilot-0.0.6/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 11:20:27.953408 deep_copilot-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-17 09:16:07.000000 deep_copilot-0.0.6/setup.py
```

### Comparing `deep_copilot-0.0.5/CONTRIBUTING.md` & `deep_copilot-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/LICENSE` & `deep_copilot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/PKG-INFO` & `deep_copilot-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_copilot
-Version: 0.0.5
+Version: 0.0.6
 Summary: gyw toolkits
 Home-page: https://github.com/612twilight/deep_copilot/tree/master/
 Author: gyw
 Author-email: 240590367@qqq.com
 License: Apache Software License 2.0
 Keywords: anything not for deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deep_copilot-0.0.5/README.md` & `deep_copilot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/audio_tools/base_audio_tools.py` & `deep_copilot-0.0.6/deep_copilot/audio_tools/base_audio_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/audio_tools/vad_tools.py` & `deep_copilot-0.0.6/deep_copilot/audio_tools/vad_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/command_tools/tools.py` & `deep_copilot-0.0.6/deep_copilot/command_tools/tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/date_tools/datetimeutil.py` & `deep_copilot-0.0.6/deep_copilot/date_tools/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/excel_tools/tools.py` & `deep_copilot-0.0.6/deep_copilot/excel_tools/tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/faiss_tools/faiss_tools.py` & `deep_copilot-0.0.6/deep_copilot/faiss_tools/faiss_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/hanlp_tools/hanlp_copilot.py` & `deep_copilot-0.0.6/deep_copilot/hanlp_tools/hanlp_copilot.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/log_tools/log_tool.py` & `deep_copilot-0.0.6/deep_copilot/log_tools/log_tool.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/misc_tools/es_tools.py` & `deep_copilot-0.0.6/deep_copilot/misc_tools/es_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/misc_tools/tools.py` & `deep_copilot-0.0.6/deep_copilot/misc_tools/tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/mysql_tools/mysql_copilot.py` & `deep_copilot-0.0.6/deep_copilot/mysql_tools/mysql_copilot.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/path_tools/path_copilot.py` & `deep_copilot-0.0.6/deep_copilot/path_tools/path_copilot.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/seed_tools/seed_tool.py` & `deep_copilot-0.0.6/deep_copilot/seed_tools/seed_tool.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/string_tools/string_copilot.py` & `deep_copilot-0.0.6/deep_copilot/string_tools/string_copilot.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/base_image_tools.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/base_image_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/base_video_tools.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/base_video_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/ffmpeg_tools.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/ffmpeg_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/ffmpyutil.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/ffmpyutil.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/key_frame_extraction_tools.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/key_frame_extraction_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/moviepy_tools.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/moviepy_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/opencv_tools.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/opencv_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/video_and_image_tools/sceneutil.py` & `deep_copilot-0.0.6/deep_copilot/video_and_image_tools/sceneutil.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/chatgpt_tools.py` & `deep_copilot-0.0.6/deep_copilot/zero_short_model_tools/chatgpt_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/t5_model_tools.py` & `deep_copilot-0.0.6/deep_copilot/zero_short_model_tools/t5_model_tools.py`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/deep_copilot.egg-info/PKG-INFO` & `deep_copilot-0.0.6/deep_copilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-copilot
-Version: 0.0.5
+Version: 0.0.6
 Summary: gyw toolkits
 Home-page: https://github.com/612twilight/deep_copilot/tree/master/
 Author: gyw
 Author-email: 240590367@qqq.com
 License: Apache Software License 2.0
 Keywords: anything not for deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deep_copilot-0.0.5/deep_copilot.egg-info/SOURCES.txt` & `deep_copilot-0.0.6/deep_copilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.5/setup.py` & `deep_copilot-0.0.6/setup.py`

 * *Files identical despite different names*

