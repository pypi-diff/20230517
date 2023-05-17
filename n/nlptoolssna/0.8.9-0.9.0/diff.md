# Comparing `tmp/nlptoolssna-0.8.9.tar.gz` & `tmp/nlptoolssna-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.8.9.tar", last modified: Wed May 17 16:56:42 2023, max compression
+gzip compressed data, was "nlptoolssna-0.9.0.tar", last modified: Wed May 17 17:03:35 2023, max compression
```

## Comparing `nlptoolssna-0.8.9.tar` & `nlptoolssna-0.9.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.186373 nlptoolssna-0.8.9/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-17 16:56:42.186373 nlptoolssna-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.027289 nlptoolssna-0.8.9/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.9/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:41.994068 nlptoolssna-0.8.9/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:41.994968 nlptoolssna-0.8.9/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.030684 nlptoolssna-0.8.9/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.9/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.036122 nlptoolssna-0.8.9/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.9/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.9/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.9/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.9/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.9/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.047019 nlptoolssna-0.8.9/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.048021 nlptoolssna-0.8.9/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.9/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.054187 nlptoolssna-0.8.9/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.056026 nlptoolssna-0.8.9/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.9/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.9/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.058998 nlptoolssna-0.8.9/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.9/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.9/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.065573 nlptoolssna-0.8.9/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.8.9/docs/source/api/utils/implication.rst
--rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.8.9/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.8.9/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.8.9/docs/source/api/utils/text_transliteration.rst
--rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.8.9/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.8.9/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.9/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.9/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.8.9/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.9/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.071165 nlptoolssna-0.8.9/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.077738 nlptoolssna-0.8.9/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.9/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     9183 2023-05-13 17:55:55.000000 nlptoolssna-0.8.9/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.8.9/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.093463 nlptoolssna-0.8.9/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.9/nlptools/arabiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.107226 nlptoolssna-0.8.9/nlptools/arabiner/bin/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-05-17 16:50:20.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/eval.py
--rw-rw-rw-   0        0        0     1288 2023-05-17 16:49:58.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/infer.py
--rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/process.py
--rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.8.9/nlptools/arabiner/bin/train.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.115116 nlptoolssna-0.8.9/nlptools/arabiner/data/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/data/__init__.py
--rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.8.9/nlptools/arabiner/data/datasets.py
--rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/data/transforms.py
--rw-rw-rw-   0        0        0     4149 2023-05-17 07:25:34.000000 nlptoolssna-0.8.9/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-05-17 07:25:45.000000 nlptoolssna-0.8.9/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3646 2023-05-17 16:45:01.000000 nlptoolssna-0.8.9/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1328 2023-05-17 07:12:53.000000 nlptoolssna-0.8.9/nlptools/arabiner/infer.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.126987 nlptoolssna-0.8.9/nlptools/arabiner/nn/
--rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/BaseModel.py
--rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/BertNestedTagger.py
--rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/BertSeqTagger.py
--rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/nn/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-05-17 07:25:57.000000 nlptoolssna-0.8.9/nlptools/arabiner/transforms.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.136378 nlptoolssna-0.8.9/nlptools/arabiner/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/data.py
--rw-rw-rw-   0        0        0     3649 2023-05-17 16:42:37.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/helpers.py
--rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.8.9/nlptools/arabiner/utils/metrics.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.139394 nlptoolssna-0.8.9/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.9/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.151940 nlptoolssna-0.8.9/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.9/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.9/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.8.9/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.9/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.8.9/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.167852 nlptoolssna-0.8.9/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.9/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.8.9/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0    10287 2023-05-11 20:50:47.000000 nlptoolssna-0.8.9/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     7600 2023-05-15 14:27:42.000000 nlptoolssna-0.8.9/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.8.9/nlptools/utils/text_transliteration.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.9/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.182654 nlptoolssna-0.8.9/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2308 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      144 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 16:56:41.000000 nlptoolssna-0.8.9/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-17 16:56:42.188212 nlptoolssna-0.8.9/setup.cfg
--rw-rw-rw-   0        0        0     2095 2023-05-17 07:09:09.000000 nlptoolssna-0.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:56:42.185373 nlptoolssna-0.8.9/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.9/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.344684 nlptoolssna-0.9.0/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-17 17:03:35.345683 nlptoolssna-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.168225 nlptoolssna-0.9.0/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.9.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.120750 nlptoolssna-0.9.0/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.122625 nlptoolssna-0.9.0/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.171779 nlptoolssna-0.9.0/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.0/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.181297 nlptoolssna-0.9.0/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.0/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.9.0/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.0/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.0/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.9.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.196725 nlptoolssna-0.9.0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.198727 nlptoolssna-0.9.0/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.0/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.234224 nlptoolssna-0.9.0/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.236786 nlptoolssna-0.9.0/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.9.0/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.9.0/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.239349 nlptoolssna-0.9.0/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.9.0/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.9.0/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.249825 nlptoolssna-0.9.0/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.9.0/docs/source/api/utils/implication.rst
+-rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.9.0/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.9.0/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.9.0/docs/source/api/utils/text_transliteration.rst
+-rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.9.0/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.9.0/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.9.0/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.9.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.9.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.9.0/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.258499 nlptoolssna-0.9.0/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.267905 nlptoolssna-0.9.0/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.9.0/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     9187 2023-05-17 17:03:21.000000 nlptoolssna-0.9.0/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.9.0/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.279456 nlptoolssna-0.9.0/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.9.0/nlptools/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.288064 nlptoolssna-0.9.0/nlptools/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-05-17 16:50:20.000000 nlptoolssna-0.9.0/nlptools/arabiner/bin/eval.py
+-rw-rw-rw-   0        0        0     1288 2023-05-17 16:49:58.000000 nlptoolssna-0.9.0/nlptools/arabiner/bin/infer.py
+-rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.9.0/nlptools/arabiner/bin/process.py
+-rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.9.0/nlptools/arabiner/bin/train.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.293324 nlptoolssna-0.9.0/nlptools/arabiner/data/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/data/__init__.py
+-rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.9.0/nlptools/arabiner/data/datasets.py
+-rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/data/transforms.py
+-rw-rw-rw-   0        0        0     4149 2023-05-17 07:25:34.000000 nlptoolssna-0.9.0/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-05-17 07:25:45.000000 nlptoolssna-0.9.0/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3646 2023-05-17 16:45:01.000000 nlptoolssna-0.9.0/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1328 2023-05-17 07:12:53.000000 nlptoolssna-0.9.0/nlptools/arabiner/infer.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.300664 nlptoolssna-0.9.0/nlptools/arabiner/nn/
+-rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/nn/BaseModel.py
+-rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.9.0/nlptools/arabiner/nn/BertNestedTagger.py
+-rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.9.0/nlptools/arabiner/nn/BertSeqTagger.py
+-rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/nn/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-05-17 07:25:57.000000 nlptoolssna-0.9.0/nlptools/arabiner/transforms.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.307465 nlptoolssna-0.9.0/nlptools/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.9.0/nlptools/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3649 2023-05-17 16:42:37.000000 nlptoolssna-0.9.0/nlptools/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.9.0/nlptools/arabiner/utils/metrics.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.309635 nlptoolssna-0.9.0/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.9.0/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.317544 nlptoolssna-0.9.0/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.9.0/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.9.0/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.9.0/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.9.0/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.9.0/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.328390 nlptoolssna-0.9.0/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.9.0/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.9.0/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0    10287 2023-05-11 20:50:47.000000 nlptoolssna-0.9.0/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     7600 2023-05-15 14:27:42.000000 nlptoolssna-0.9.0/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.9.0/nlptools/utils/text_transliteration.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.9.0/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.340485 nlptoolssna-0.9.0/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-17 17:03:34.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2308 2023-05-17 17:03:35.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:03:34.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-17 17:03:34.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      144 2023-05-17 17:03:34.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 17:03:34.000000 nlptoolssna-0.9.0/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-17 17:03:35.347145 nlptoolssna-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2023-05-17 07:09:09.000000 nlptoolssna-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:03:35.343685 nlptoolssna-0.9.0/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.9.0/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.8.9/CONTRIBUTING.rst` & `nlptoolssna-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/LICENSE` & `nlptoolssna-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/PKG-INFO` & `nlptoolssna-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.9/README.rst` & `nlptoolssna-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/Makefile` & `nlptoolssna-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/build/html/_images/download.png` & `nlptoolssna-0.9.0/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/build/html/_static/download.png` & `nlptoolssna-0.9.0/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/make.bat` & `nlptoolssna-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/source/_static/download.png` & `nlptoolssna-0.9.0/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/source/conf.py` & `nlptoolssna-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/docs/source/installation.rst` & `nlptoolssna-0.9.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.9.0/nlptools/DataDownload/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 import requests  
 import zipfile
 from tqdm import tqdm
 import tarfile
 urls = {
     'morph': 'https://portal.sina.birzeit.edu/ALMA27012000.pickle',
-    'ner': 'http://portal.sina.birzeit.edu/Wj27012000.zip'
+    'ner': 'https://portal.sina.birzeit.edu/Wj27012000.tar.gz'
 }
 
 #     'salma': 'http://portal.sina.birzeit.edu/SALMA27012000.zip',
 #     'salma2021': 'http://portal.sina.birzeit.edu/SALMA_v2.zip'
 #
```

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/bin/eval.py` & `nlptoolssna-0.9.0/nlptools/arabiner/bin/eval.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/bin/infer.py` & `nlptoolssna-0.9.0/nlptools/arabiner/bin/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/bin/process.py` & `nlptoolssna-0.9.0/nlptools/arabiner/bin/process.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/bin/train.py` & `nlptoolssna-0.9.0/nlptools/arabiner/bin/train.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/data/datasets.py` & `nlptoolssna-0.9.0/nlptools/arabiner/data/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/data/transforms.py` & `nlptoolssna-0.9.0/nlptools/arabiner/data/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/data.py` & `nlptoolssna-0.9.0/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/datasets.py` & `nlptoolssna-0.9.0/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/helpers.py` & `nlptoolssna-0.9.0/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/infer.py` & `nlptoolssna-0.9.0/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/nn/BaseModel.py` & `nlptoolssna-0.9.0/nlptools/arabiner/nn/BaseModel.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/nn/BertNestedTagger.py` & `nlptoolssna-0.9.0/nlptools/arabiner/nn/BertNestedTagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/transforms.py` & `nlptoolssna-0.9.0/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/utils/data.py` & `nlptoolssna-0.9.0/nlptools/arabiner/utils/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/utils/helpers.py` & `nlptoolssna-0.9.0/nlptools/arabiner/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/arabiner/utils/metrics.py` & `nlptoolssna-0.9.0/nlptools/arabiner/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/data/my_data.pickle` & `nlptoolssna-0.9.0/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/morphology/charsets.py` & `nlptoolssna-0.9.0/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.9.0/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.9.0/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/utils/implication.py` & `nlptoolssna-0.9.0/nlptools/utils/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/utils/jaccard.py` & `nlptoolssna-0.9.0/nlptools/utils/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/utils/parser.py` & `nlptoolssna-0.9.0/nlptools/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptools/utils/text_transliteration.py` & `nlptoolssna-0.9.0/nlptools/utils/text_transliteration.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.9.0/nlptoolssna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.9/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.9.0/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/setup.cfg` & `nlptoolssna-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.9/setup.py` & `nlptoolssna-0.9.0/setup.py`

 * *Files identical despite different names*

