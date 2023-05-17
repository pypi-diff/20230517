# Comparing `tmp/nlptoolssna-0.8.8.tar.gz` & `tmp/nlptoolssna-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.8.8.tar", last modified: Sat May 13 13:46:27 2023, max compression
+gzip compressed data, was "nlptoolssna-0.8.9.tar", last modified: Wed May 17 16:56:42 2023, max compression
```

## Comparing `nlptoolssna-0.8.8.tar` & `nlptoolssna-0.8.9.tar`

### file list

```diff
@@ -1,84 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.599743 nlptoolssna-0.8.8/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-13 13:46:27.599743 nlptoolssna-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.494364 nlptoolssna-0.8.8/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.466299 nlptoolssna-0.8.8/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.469301 nlptoolssna-0.8.8/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.495365 nlptoolssna-0.8.8/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.8/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.502366 nlptoolssna-0.8.8/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.8/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.8/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.8/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.8/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.510925 nlptoolssna-0.8.8/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.511926 nlptoolssna-0.8.8/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.8/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.518925 nlptoolssna-0.8.8/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.519925 nlptoolssna-0.8.8/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.8/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.8/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.521926 nlptoolssna-0.8.8/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.8/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.8/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.528643 nlptoolssna-0.8.8/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.8.8/docs/source/api/utils/implication.rst
--rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.8.8/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.8.8/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.8.8/docs/source/api/utils/text_transliteration.rst
--rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.8.8/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.8.8/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.8/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.8/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.8.8/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.8/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.535820 nlptoolssna-0.8.8/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.540833 nlptoolssna-0.8.8/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.8/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-05-11 20:56:17.000000 nlptoolssna-0.8.8/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.8.8/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.552821 nlptoolssna-0.8.8/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.8/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4142 2023-05-11 20:59:35.000000 nlptoolssna-0.8.8/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5057 2023-05-11 20:57:32.000000 nlptoolssna-0.8.8/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.8.8/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1336 2023-05-11 21:00:06.000000 nlptoolssna-0.8.8/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-11 20:58:53.000000 nlptoolssna-0.8.8/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.555823 nlptoolssna-0.8.8/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.8/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.566821 nlptoolssna-0.8.8/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.8/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.8/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     6376 2023-05-08 18:11:31.000000 nlptoolssna-0.8.8/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.8/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.8.8/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.578199 nlptoolssna-0.8.8/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.8/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    27982 2023-05-13 13:44:33.000000 nlptoolssna-0.8.8/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0    10287 2023-05-11 20:50:47.000000 nlptoolssna-0.8.8/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     7556 2023-05-11 20:46:42.000000 nlptoolssna-0.8.8/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0     9283 2023-05-08 19:13:30.000000 nlptoolssna-0.8.8/nlptools/utils/text_transliteration.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.8/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.593777 nlptoolssna-0.8.8/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-13 13:46:27.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1758 2023-05-13 13:46:27.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 13:46:27.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-13 13:46:27.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-13 13:46:27.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 13:46:27.000000 nlptoolssna-0.8.8/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-13 13:46:27.602538 nlptoolssna-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-05-11 21:37:10.000000 nlptoolssna-0.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:46:27.597753 nlptoolssna-0.8.8/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.8/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.186373 nlptoolssna-0.8.9/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-17 16:56:42.186373 nlptoolssna-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.027289 nlptoolssna-0.8.9/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.9/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:41.994068 nlptoolssna-0.8.9/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:41.994968 nlptoolssna-0.8.9/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.030684 nlptoolssna-0.8.9/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.9/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.036122 nlptoolssna-0.8.9/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.9/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.9/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.9/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.9/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.047019 nlptoolssna-0.8.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.048021 nlptoolssna-0.8.9/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.9/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.054187 nlptoolssna-0.8.9/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.056026 nlptoolssna-0.8.9/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.9/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.9/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.058998 nlptoolssna-0.8.9/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.9/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.9/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.065573 nlptoolssna-0.8.9/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.8.9/docs/source/api/utils/implication.rst
+-rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.8.9/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.8.9/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.8.9/docs/source/api/utils/text_transliteration.rst
+-rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.8.9/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.8.9/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.9/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.8.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.9/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.071165 nlptoolssna-0.8.9/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.077738 nlptoolssna-0.8.9/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.9/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     9183 2023-05-13 17:55:55.000000 nlptoolssna-0.8.9/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.8.9/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.093463 nlptoolssna-0.8.9/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.9/nlptools/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.107226 nlptoolssna-0.8.9/nlptools/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-05-17 16:50:20.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/eval.py
+-rw-rw-rw-   0        0        0     1288 2023-05-17 16:49:58.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/infer.py
+-rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/process.py
+-rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/train.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.115116 nlptoolssna-0.8.9/nlptools/arabiner/data/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/data/__init__.py
+-rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.8.9/nlptools/arabiner/data/datasets.py
+-rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/data/transforms.py
+-rw-rw-rw-   0        0        0     4149 2023-05-17 07:25:34.000000 nlptoolssna-0.8.9/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-05-17 07:25:45.000000 nlptoolssna-0.8.9/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3646 2023-05-17 16:45:01.000000 nlptoolssna-0.8.9/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1328 2023-05-17 07:12:53.000000 nlptoolssna-0.8.9/nlptools/arabiner/infer.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.126987 nlptoolssna-0.8.9/nlptools/arabiner/nn/
+-rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/BaseModel.py
+-rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/BertNestedTagger.py
+-rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/BertSeqTagger.py
+-rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-05-17 07:25:57.000000 nlptoolssna-0.8.9/nlptools/arabiner/transforms.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.136378 nlptoolssna-0.8.9/nlptools/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3649 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/metrics.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.139394 nlptoolssna-0.8.9/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.9/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.151940 nlptoolssna-0.8.9/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.9/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.9/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.8.9/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.9/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.8.9/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.167852 nlptoolssna-0.8.9/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.9/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.8.9/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0    10287 2023-05-11 20:50:47.000000 nlptoolssna-0.8.9/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     7600 2023-05-15 14:27:42.000000 nlptoolssna-0.8.9/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.8.9/nlptools/utils/text_transliteration.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.9/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.182654 nlptoolssna-0.8.9/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2308 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      144 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-17 16:56:42.188212 nlptoolssna-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2023-05-17 07:09:09.000000 nlptoolssna-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.185373 nlptoolssna-0.8.9/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.8.8/CONTRIBUTING.rst` & `nlptoolssna-0.8.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/LICENSE` & `nlptoolssna-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/PKG-INFO` & `nlptoolssna-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.8/README.rst` & `nlptoolssna-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/Makefile` & `nlptoolssna-0.8.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/build/html/_images/download.png` & `nlptoolssna-0.8.9/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/build/html/_static/download.png` & `nlptoolssna-0.8.9/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/make.bat` & `nlptoolssna-0.8.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/source/_static/download.png` & `nlptoolssna-0.8.9/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/source/conf.py` & `nlptoolssna-0.8.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/docs/source/installation.rst` & `nlptoolssna-0.8.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/nlptools/arabiner/data.py` & `nlptoolssna-0.8.9/nlptools/arabiner/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from torch.utils.data import DataLoader
 from torchtext.vocab import vocab
 from collections import Counter, namedtuple
 import logging
 import re
 import itertools
-from arabiner.utils.helpers import load_object
-from arabiner.data.datasets import Token
+from nlptools.arabiner.helpers import load_object
+from nlptools.arabiner.datasets import Token
 
 logger = logging.getLogger(__name__)
 
 
 def conll_to_segments(filename):
     """
     Convert CoNLL files to segments. This return list of segments and each segment is
```

### Comparing `nlptoolssna-0.8.8/nlptools/arabiner/datasets.py` & `nlptoolssna-0.8.9/nlptools/arabiner/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import torch
 from torch.utils.data import Dataset
 from torch.nn.utils.rnn import pad_sequence
-from arabiner.data.transforms import (
+from nlptools.arabiner.data.transforms import (
     BertSeqTransform,
     NestedTagsTransform
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -139,8 +139,8 @@
         masks = torch.cat(masks)
 
         # Pad the tags, do the padding for each tag type
         tags = [torch.nn.ConstantPad1d((0, subwords.shape[-1] - tag.shape[-1]), vocab.get_stoi()["<pad>"])(tag)
                 for tag, vocab in zip(tags, self.vocab.tags[1:])]
         tags = torch.cat(tags)
 
-        return subwords, tags, tokens, masks, valid_len
+        return subwords, tags, tokens, masks, valid_len
```

### Comparing `nlptoolssna-0.8.8/nlptools/arabiner/helpers.py` & `nlptoolssna-0.8.9/nlptools/arabiner/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import logging
 import importlib
 import shutil
 import torch
 import pickle
 import json
-#import random
+import random
 import numpy as np
 from argparse import Namespace
 
 
 def logging_config(log_file=None):
     """
     Initialize custom logger
@@ -94,23 +94,24 @@
     train_config.trainer_config["kwargs"]["loss"] = loss
 
     tagger = load_object(train_config.trainer_config["fn"], train_config.trainer_config["kwargs"])
     tagger.load(os.path.join(model_path, "checkpoints"))
     return tagger, tag_vocab, train_config
 
 
-# def set_seed(seed):
-#     """
-#     Set the seed for random intialization and set
-#     CUDANN parameters to ensure determmihstic results across
-#     multiple runs with the same seed
-#     :param seed: int
-#     """
-#     np.random.seed(seed)
-#     random.seed(seed)
-#     torch.manual_seed(seed)
-#     torch.cuda.manual_seed(seed)
-#     torch.cuda.manual_seed_all(seed)
-
-#     torch.backends.cudnn.deterministic = True
-#     torch.backends.cudnn.benchmark = False
-#     torch.backends.cudnn.enabled = False
+def set_seed(seed):
+    """
+    Set the seed for random intialization and set
+    CUDANN parameters to ensure determmihstic results across
+    multiple runs with the same seed
+
+    :param seed: int
+    """
+    np.random.seed(seed)
+    random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)
+
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.enabled = False
```

### Comparing `nlptoolssna-0.8.8/nlptools/arabiner/infer.py` & `nlptoolssna-0.8.9/nlptools/arabiner/infer.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from nlptools.arabiner.data import get_dataloaders, text2segments
 from nlptools.DataDownload import downloader
 import os
 logger = logging.getLogger(__name__)
 
 
 
-def ner(text, model_path, batch_size=32):
+def ner(text, batch_size=32):
     # Load tagger
-    filename = 'Wj27012000'
+    filename = 'Wj27012000.tar'
     path =downloader.get_appdatadir()
     model_path = os.path.join(path, filename)
     tagger, tag_vocab, train_config = load_checkpoint(model_path)
 
     # Convert text to a tagger dataset and index the tokens in args.text
     dataset, token_vocab = text2segments(text)
```

### Comparing `nlptoolssna-0.8.8/nlptools/arabiner/transforms.py` & `nlptoolssna-0.8.9/nlptools/arabiner/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from transformers import BertTokenizer
 from functools import partial
 import logging
 import re
 import itertools
-import arabiner
+from nlptools.arabiner import datasets
 
 logger = logging.getLogger(__name__)
 
 
 class BertSeqTransform:
     def __init__(self, bert_model, vocab, max_seq_len=512):
         self.tokenizer = BertTokenizer.from_pretrained(bert_model)
@@ -18,15 +18,15 @@
             truncation=True,
         )
         self.max_seq_len = max_seq_len
         self.vocab = vocab
 
     def __call__(self, segment):
         subwords, tags, tokens = list(), list(), list()
-        unk_token = arabiner.data.datasets.Token(text="UNK")
+        unk_token = datasets.Token(text="UNK")
 
         for token in segment:
             token_subwords = self.encoder(token.text)[1:-1]
             subwords += token_subwords
             tags += [self.vocab.tags[0].get_stoi()[token.gold_tag[0]]] + [self.vocab.tags[0].get_stoi()["O"]] * (len(token_subwords) - 1)
             tokens += [token] + [unk_token] * (len(token_subwords) - 1)
 
@@ -59,15 +59,15 @@
             truncation=True,
         )
         self.max_seq_len = max_seq_len
         self.vocab = vocab
 
     def __call__(self, segment):
         tags, tokens, subwords = list(), list(), list()
-        unk_token = arabiner.data.datasets.Token(text="UNK")
+        unk_token = datasets.Token(text="UNK")
 
         # Encode each token and get its subwords and IDs
         for token in segment:
             token.subwords = self.encoder(token.text)[1:-1]
             subwords += token.subwords
             tokens += [token] + [unk_token] * (len(token.subwords ) - 1)
```

### Comparing `nlptoolssna-0.8.8/nlptools/data/my_data.pickle` & `nlptoolssna-0.8.9/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/nlptools/morphology/charsets.py` & `nlptoolssna-0.8.9/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.8.9/nlptools/morphology/morph_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 
         #  elif re.match("^[a-zA-Z]*$", token): 
         #     solution[2] = "Foreign" #pos
 
          else:
             result_token = find_solution(token,language, task)
             
-           
             if result_token == []:
                token_without_al = re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))
                if len(token_without_al) > 5  :
                   result_token = find_solution(token_without_al, language, task)
 
             if result_token == []:
               # try with replace ﻩ with ﺓ
```

### Comparing `nlptoolssna-0.8.8/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.8.9/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/nlptools/utils/implication.py` & `nlptoolssna-0.8.9/nlptools/utils/implication.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #  <w1, w2, implication direction, distance, conflicts, verdict, preferredWord> .
 
 from nlptools.utils.parser import arStrip
 class Implication:
     """
     The implication class computes whether the two Arabic words are the same or not, regardless of how they are diacritized. The output also contains implication direction, distance, number of conflicts, and other outputs. 
     Argd:
-        :obj:`str' word1: input string
-        :obj:`str' word2: input string
+        :obj:`str' word1: input text
+        :obj:`str' word2: input text
 
     """
     # Diacritic Pair Distance Map
     distanceTable = [
     [0, 0, 1, 1, 1, 1, 1, 1, 15, 16, 16, 16, 0, 0, 0, 0 ],
     [0, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
     [1, 101, 0, 101, 101, 101, 101, 101, 101, 101, 101, 101, 0, 0, 0, 0],
@@ -123,15 +123,15 @@
                 self.verdict = "Incompatible"
                 self.direction = -3 # the two words have different letters
                 self.distance = 3000
                 self.conflicts = 0
             
     def get_non_preferred_word(self, word1, word2):
         """
-        Returns the non-preferred word from two given words.
+        This method returns the non-preferred word from two given words.
 
         Args:
             :obj:`str' word1: The first word.
             :obj:`str' word2: The second word.
 
         Returns:
             :obj:`str': The non-preferred word.
@@ -159,15 +159,15 @@
             else:
                 return None
     
 
 
     def get_preferred_word( self , word1,   word2) :
         """
-        Returns the preferred word from two given words.
+        This method returns the preferred word from two given words.
 
         Args:
             :obj:`str' word1: The first word.
             :obj:`str' word2: The second word.
 
         Returns:
             :obj:`str': The preferred word.
@@ -200,21 +200,21 @@
             if word2 != None and (not word2):
                 return  word2
             else:
                 return None
             
     def normalize_alef(word):
         """
-        Normalize the alif (ألف) character in the given word according to certain rules.
+        This method normalizes the alif (ألف) character in the given word.
 
         Args:
             word (:obj:`str`): The input word to be normalized.
 
         Returns:
-            :obj:`str`: The normalized word with alif characters modified based on the rules.
+            :obj:`str`: The normalized word with alif characters modified.
 
         **Example:**
 
         .. highlight:: python
         .. code-block:: python
 
             from nlptools.utils.implication import Implication
@@ -234,15 +234,15 @@
         if word.startswith("ٱ"):
             word = "ا" + word[1:]
         return word
 
 
     def diacritics_syntax_error_in( diacriticsArray ) :
         """
-        Check if the diacritics in the given array are incorrect.
+        This method checks if the diacritics in a given array are incorrect.
 
         Args:
             diacritics_array (:obj:`list`): A list of diacritics to be checked.
 
         Returns:
             :obj:`bool`: True if there is a syntax error in the diacritics, False otherwise.
 
@@ -273,15 +273,15 @@
             
         except :
             return False
         
 
     def wrong_end_diacritic(diac):
         """
-        Check if the given diacritic is a wrong end diacritic.
+        This method checks if the given diacritic is a wrong end diacritic.
 
         Args:
             diac (:obj:`int`): The diacritic value to be checked.
 
         Returns:
             :obj:`bool`: True if the diacritic is one of the follwoing number (85:SHADDAH WITH FATHATAN, 86:SHADDAH WITH KASRTA, 87:SHADDAH WITH DHAMTAN), False if diacritic is greator than or equal0 and diacritic is less than or equal 11.
 
@@ -312,17 +312,15 @@
             return False
         else :
             return diac < 8 or diac > 15
             
     
     def calculate_words_implication(self):
         """
-        Calculate the implication between two words.
-
-        This method updates the verdict, direction, distance, and conflicts attributes of the object based on the implication between the words.
+        This method calculates the implication between two words, and updates the verdict, direction, distance, and conflicts attributes of the object based on the implication between the words.
 
         Returns:
             None
 
         **Example:**
 
         .. highlight:: python
@@ -367,17 +365,15 @@
             else:
                 self.direction = -3 # the two words have different letters
                 self.distance = 3000
                 self.conflicts = 0
 
     def equal_words( self ) :
         """
-        Check if the two words are equal, taking into account the alif as the first letter.
-
-        This method updates the word1Undiac and word2Undiac attributes by removing the first letter, and returns True if the words are equal, False otherwise.
+        This method updates the word1Undiac and word2Undiac attributes by removing the first letter, and returns True if the words are equal, False otherwise. 
 
         Returns:
             :obj:`bool`: True if the words are equal, False otherwise.
 
         **Example:**
 
         .. highlight:: python
@@ -462,19 +458,19 @@
             self.conflictFlags[self.lettersDirection[len(self.lettersDirection) - 1] + 1] = True
             self.distance = self.distance + self.distanceTable[word1Diac][word2Diac]
         return True
 
         
     def calculate_direction(self ): 
         """
-        Calculates the direction of compatibility based on conflict flags.
+        This method calculates the direction of compatibility based on a conflict flags.
 
         Returns:
             :obj:`int`: The direction of compatibility:
-                -1: Incompatible-diacritics
+               -1: Incompatible-diacritics
                 0: Compatible-imply each other
                 1: Compatible-w1 implies w2
                 2: Compatible-w2 implies w1
                 3: Compatible-exactly equal
                 -2147483648: Default value for an invalid direction
         """
         self.conflicts = 0
@@ -488,22 +484,21 @@
             return 1 # Compatible-w1 implies w2
         
         if (self.conflictFlags[2] == False and self.conflictFlags[3] == True ):
             return 2 # Compatible-w2 implies w1
         
         if (self.conflictFlags[4]):
             return 3 # Compatible-exactly equal
-        
         return -2147483648
 
 
 
     def get_diacritics_array(word): 
         """
-        Converts diacritics in a word to digits and returns the array of diacritics.
+        This method converts diacritics in a word to digits and returns the array of diacritics.
 
         Args:
             word (:obj:`str`): The word with diacritics.
 
         Returns:
             :obj:`list`: The array of diacritics converted to digits.
 
@@ -590,15 +585,15 @@
     #     word = word.replace("ٍ", "") #KASRATAN
     #     word = word.replace("ٌ", "") #DAMMATAN
     #     word = word.replace("ّ", "") #SHADDA
     #     return word
 
     def get_letters_array(word):
         """
-        Returns the array of letters from a given word.
+        This method returns the array of letters from a given word.
 
         Args:
             word (:obj:`str`): The word from which to extract the letters.
 
         Returns:
             obj:`list`: The array of letters.
 
@@ -637,15 +632,15 @@
 
 
     def get_word2(self) :
         return self.word2 
 
     def get_result(self):
         """
-        Returns the result of the comparison between two words.
+        This method returns the result of the comparison between two words.
 
         Returns:
             :obj:`str`: The result of the comparison. Can be *Same* or *Different*.
 
         **Example:**
 
         .. highlight:: python
```

### Comparing `nlptoolssna-0.8.8/nlptools/utils/jaccard.py` & `nlptoolssna-0.8.9/nlptools/utils/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/nlptools/utils/parser.py` & `nlptoolssna-0.8.9/nlptools/utils/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import re 
 
-def arStrip(text , diacs=False , smallDiacs=False , shaddah=False , digit=False, alif=False , specialChars=False ):
+def arStrip(text , diacs=True , smallDiacs=True , shaddah=True , digit=True, alif=True , specialChars=True ):
     
     """
     This method removes Arabic diacritics, Quranic annotation signs, shaddah, English and Arabic digits, unify alif with hamzah,
     some special characters, spaces, underscore and Arabic tatwelah from the input text.
 
     Args:
         text (:obj:`str`): Arabic text to be processed.
-        diacs (:obj:`bool`): flag to remove Arabic diacretics [ ًٌٍَُِْ] (default is False).
-        smallDiacs (:obj:`bool`): flag to remove small Quranic annotation signs (default is False).
-        shaddah (:obj:`bool`): flag to remove shaddah (default is False).
-        digit (:obj:`bool`): flag to remove English and Arabic digits (default is False).
-        alif (:obj:`bool`): flag to unify alif with hamzah (default is False).
-        specialChars (:obj:`bool`): flag to remove some special characters (default is False).
+        diacs (:obj:`bool`): flag to remove Arabic diacretics [ ًٌٍَُِْ] (default is True).
+        smallDiacs (:obj:`bool`): flag to remove small Quranic annotation signs (default is True).
+        shaddah (:obj:`bool`): flag to remove shaddah (default is True).
+        digit (:obj:`bool`): flag to remove English and Arabic digits (default is True).
+        alif (:obj:`bool`): flag to unify alif with hamzah (default is True).
+        specialChars (:obj:`bool`): flag to remove some special characters (default is True).
 
     Returns:
         :obj:`str`: processed text with removed diacritics, Quranic annotation signs, shaddah, digits, and special characters.
 
     **Example:**
 
     .. highlight:: python
     .. code-block:: python
 
         from nlptools.utils import parser
-        return parser.arStrip( " مَحًمٌٍُِ" ,True ,True ,True ,True ,False , True )
+        processed_text =parser.arStrip('2023الجو جميلُ' , True , True , True ,  True , False , True )
+        print(processed_text)
 
+        #putput
+        الجو جميل
     """
     try:
         if text: # if the input string is not empty do the following
             #print("in if")
             if diacs == True :
                 text = re.sub(r'[\u064B-\u0650]+', '',text) # Remove all Arabic diacretics [ ًٌٍَُِْ]
                 text = re.sub(r'[\u0652]+', '',text) # Remove SUKUN
@@ -54,57 +57,58 @@
             text = text.replace("ـ" , '') # Remove Arabic tatwelah
             text = text.strip() # Trim input string
     except:
         return text
     return text
     
 
-def remove_punctuation(text):
-    """
-    Removes punctuation marks from the input text.
+# def remove_punctuation(text):
+#     """
+#     Removes punctuation marks from the input text.
     
-    Args:
-      text (:obj:`str`): The input string containing punctuation marks.
+#     Args:
+#       text (:obj:`str`): The input string containing punctuation marks.
     
-    Returns:
-      :obj:`str`: The output string with all punctuation marks removed.
-    **Example:**
+#     Returns:
+#       :obj:`str`: The output string with all punctuation marks removed.
+#     **Example:**
 
-    .. highlight:: python
-    .. code-block:: python
+#     .. highlight:: python
+#     .. code-block:: python
 
-        from nlptools.utils import parser
-        return parser.removePunctuation("te!@#،$%%؟st")
+#         from nlptools.utils import parser
+#         return parser.removePunctuation("te!@#،$%%؟st")
 
-    """
-    outputString = text
-    try:
-        if text:
-            # English Punctuation
-            outputString = re.sub(r'[\u0021-\u002F]+', '',text) # ! " # $ % & ' ( ) * + ,  - . /
-            outputString = re.sub(r'[U+060C]+', '',outputString) # ! " # $ % & ' ( ) * + ,  - . /
-            outputString = re.sub(r'[\u003A-\u0040]+', '',outputString) # : ; < = > ? @ 
-            outputString = re.sub(r'[\u005B-\u0060]+', '',outputString) # [ \ ] ^ _ `
-            outputString = re.sub(r'[\u007B-\u007E]+', '',outputString) # { | } ~
-            # Arabic Punctuation
-            outputString = re.sub(r'[\u060C]+', '',outputString) # ،
-            outputString = re.sub(r'[\u061B]+', '',outputString) # ؛
-            outputString = re.sub(r'[\u061E]+', '',outputString) # ؞
-            outputString = re.sub(r'[\u061F]+', '',outputString) # ؟
-            outputString = re.sub(r'[\u0640]+', '',outputString) # ـ
-            outputString = re.sub(r'[\u0653]+', '',outputString) # ٓ
-            outputString = re.sub(r'[\u065C]+', '',outputString) #  ٬
-            outputString = re.sub(r'[\u066C]+', '',outputString) #  ٜ 
-            outputString = re.sub(r'[\u066A]+', '',outputString) # ٪
-            outputString = re.sub(r'["}"]+', '',outputString) 
-            outputString = re.sub(r'["{"]+', '',outputString) 
-    except:
-        return text
+#     """
+#     outputString = text
+#     try:
+#         if text:
+#             # English Punctuation
+#             outputString = re.sub(r'[\u0021-\u002F]+', '',text) # ! " # $ % & ' ( ) * + ,  - . /
+#             outputString = re.sub(r'[U+060C]+', '',outputString) # ! " # $ % & ' ( ) * + ,  - . /
+#             outputString = re.sub(r'[\u003A-\u0040]+', '',outputString) # : ; < = > ? @ 
+#             outputString = re.sub(r'[\u005B-\u0060]+', '',outputString) # [ \ ] ^ _ `
+#             outputString = re.sub(r'[\u007B-\u007E]+', '',outputString) # { | } ~
+#             # Arabic Punctuation
+#             outputString = re.sub(r'[\u060C]+', '',outputString) # ،
+#             outputString = re.sub(r'[\u061B]+', '',outputString) # ؛
+#             outputString = re.sub(r'[\u061E]+', '',outputString) # ؞
+#             outputString = re.sub(r'[\u061F]+', '',outputString) # ؟
+#             outputString = re.sub(r'[\u0640]+', '',outputString) # ـ
+#             outputString = re.sub(r'[\u0653]+', '',outputString) # ٓ
+#             outputString = re.sub(r'[\u065C]+', '',outputString) #  ٬
+#             outputString = re.sub(r'[\u066C]+', '',outputString) #  ٜ 
+#             outputString = re.sub(r'[\u066A]+', '',outputString) # ٪
+#             outputString = re.sub(r'["}"]+', '',outputString) 
+#             outputString = re.sub(r'["{"]+', '',outputString) 
+#     except:
+#         return text
+
+#     return outputString
 
-    return outputString
 def remove_punctuation(text):
     """
     Removes punctuation marks from the text.
     
     Args:
       text (:obj:`str`): The text containing punctuation marks.
     
@@ -114,25 +118,28 @@
     **Example:**
 
     .. highlight:: python
     .. code-block:: python
     
         from nlptools.utils import parser
         return parser.remove_punctuation("te!@#،$%%؟st")
+
+        #output
+        test
     """
     try:
         if text:
             punctuation_marks = [r'[\u0021-\u002F]+', r'[U+060C]+', r'[\u003A-\u0040]+',
                                  r'[\u005B-\u0060]+', r'[\u007B-\u007E]+', r'[\u060C]+',
                                  r'[\u061B]+', r'[\u061E]+', r'[\u061F]+', r'[\u0640]+',
                                  r'[\u0653]+', r'[\u065C]+', r'[\u066C]+', r'[\u066A]+',
                                  r'["}"]+', r'["{"]+']
             outputString = text
-            for p in punctuation_marks:
-                outputString = re.sub(p, '', outputString)
+            for punctuation in punctuation_marks:
+                outputString = re.sub(punctuation, '', outputString)
     except:
         return text
     return outputString
 
 # def removeEnglish( text ):
 #     """
 #     Removes all Latin characters from the text.
@@ -158,15 +165,15 @@
 #             text = re.sub('[a-zA-Z]+', ' ',text)
 #     except:
 #         return text
 #     return text
 
 def remove_latin(text):
     """
-    Removes all Latin characters from the text.
+    This method removes all Latin characters from the input text.
 
     Args:
         text (:obj:`str`): The text to remove Latin characters from.
 
     Returns:
          outputString (:obj:`str`): The text with all Latin characters removed.
     Note:
@@ -174,19 +181,19 @@
     **Example:**
 
     .. highlight:: python
     .. code-block:: python
 
         from nlptools.utils import parser
         return parser.remove_latin("miojkdujhvaj1546545spkdpoqfoiehwv nWEQFGWERHERTJETAWIKUYFC")
+
+        #output
+        1546545   
     """
     try:
         if text:
             text = re.sub('[a-zA-Z]+', ' ', text)
     except:
         return text
     return text
-# print(removeEnglish("miojkdujhvaj1546545spkdpoqfoiehwv nWEQFGWERHERTJETAWIKUYFC"))
-# print(removePunctuation("te!@#،$%%؟st") )
-# Example
-# print(arStrip( " مَحًمٌٍُِ" ,True ,True ,True ,True ,False , True ))
+
```

### Comparing `nlptoolssna-0.8.8/nlptools/utils/text_transliteration.py` & `nlptoolssna-0.8.9/nlptools/utils/text_transliteration.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,18 +181,24 @@
     **Example:**
 
     .. highlight:: python
     .. code-block:: python
 
         from nlptools.utils import text_transliteration
 
-        return text_transliteration.perform_transliteration( " مَحًمٌٍُِ" ,True ,True ,True ,True ,False , True )        return transliterate.transliterate("مُحَمَدٌ نَـشِيْطٌـ1"  , "ar2bw")
-        return text_transliteration.perform_transliteration("muHamadN"  , "bw2ar")
-        return text_transliteration.perform_transliteration("شَنُعُ۪ـ1"  , "ar2bw")
-        return text_transliteration.perform_transliteration("$aw~aH_2"  , "bw2ar")
+        print(text_transliteration.perform_transliteration("مُحَمَدٌ نَـشِيْطٌـ1"  , "ar2bw"))
+        print(text_transliteration.perform_transliteration("muHamadN"  , "bw2ar"))
+        print(text_transliteration.perform_transliteration("شَنُعُ۪ـ1"  , "ar2bw"))
+        print(text_transliteration.perform_transliteration("$aw~aH_2"  , "bw2ar"))
+
+        #output
+        ('muHamadN na_$iyoTN_1', True)
+        ('مُحَمَدٌ', True)
+        ('$anuE-u_1', True)
+        ('شَوَّح 2', True)
     """
     # to map BW into Arabic  
     if schema == "bw2ar":
         transliterated_text = deque() #Empty deque list
         
         is_all_mapped = True
         for char in text:
@@ -220,21 +226,9 @@
                 is_all_mapped = False   # False if one cjars is not in map
                 transliterated_text.append(char)
             else:
                 transliterated_text.append(char_value)
 
     return ''.join(transliterated_text)  , is_all_mapped
 
-#Examples :
-# print(transliterate("مُحَمَدٌ نَـشِيْطٌـ1"  , "ar2bw")[0])
-# print(transliterate("مُحَمَدٌ نَـشِيْطٌـ1"  , "ar2bw")[1])
-
-# print(transliterate("muHamadN"  , "bw2ar")[0])
-# print(transliterate("muHamadN"  , "bw2ar")[1])
-
-# print(transliterate("شَنُعُ۪ـ1"  , "ar2bw")[0])
-# print(transliterate("شَنُعُ۪ـ1"  , "ar2bw")[1])
-
-# print(transliterate("$aw~aH_2"  , "bw2ar")[0])
-# print(transliterate("$aw~aH_2"  , "bw2ar")[1])
```

### Comparing `nlptoolssna-0.8.8/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.8.9/nlptoolssna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.8/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.8.9/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,30 @@
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
 nlptools/arabiner/data.py
 nlptools/arabiner/datasets.py
 nlptools/arabiner/helpers.py
 nlptools/arabiner/infer.py
 nlptools/arabiner/transforms.py
+nlptools/arabiner/bin/__init__.py
+nlptools/arabiner/bin/eval.py
+nlptools/arabiner/bin/infer.py
+nlptools/arabiner/bin/process.py
+nlptools/arabiner/bin/train.py
+nlptools/arabiner/data/__init__.py
+nlptools/arabiner/data/datasets.py
+nlptools/arabiner/data/transforms.py
+nlptools/arabiner/nn/BaseModel.py
+nlptools/arabiner/nn/BertNestedTagger.py
+nlptools/arabiner/nn/BertSeqTagger.py
+nlptools/arabiner/nn/__init__.py
+nlptools/arabiner/utils/__init__.py
+nlptools/arabiner/utils/data.py
+nlptools/arabiner/utils/helpers.py
+nlptools/arabiner/utils/metrics.py
 nlptools/data/my_data.pickle
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
 nlptools/utils/__init__.py
```

### Comparing `nlptoolssna-0.8.8/setup.cfg` & `nlptoolssna-0.8.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.8/setup.py` & `nlptoolssna-0.8.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 requirements = [
     'six',
     'farasapy',
     'tqdm',
     'requests',
     'regex',
     'pathlib',
-    # 'torch==1.13.1',
-    # 'transformers==4.24.0',
-    # 'torchtext==0.14.0',
-    # 'torchvision==0.14.0',
-    # 'torchdata==0.5.1',
-    # 'seqeval==1.2.2'
+    'torch==1.13.0',
+    'transformers==4.24.0',
+    'torchtext==0.14.0',
+    'torchvision==0.14.0',
+    'seqeval==1.2.2',
+    'natsort==7.1.1'
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Alaa' Omar",
     author_email='alaa.omer2009@gmail.com',
```

