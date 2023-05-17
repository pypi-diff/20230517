# Comparing `tmp/text2story-1.2.4.tar.gz` & `tmp/text2story-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.2.4.tar", last modified: Wed May 17 10:09:49 2023, max compression
+gzip compressed data, was "text2story-1.2.5.tar", last modified: Wed May 17 10:12:53 2023, max compression
```

## Comparing `text2story-1.2.4.tar` & `text2story-1.2.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.105173 text2story-1.2.4/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.2.4/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.2.4/MANIFEST.in
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9809 2023-05-17 10:09:49.105173 text2story-1.2.4/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8610 2023-03-31 14:16:09.000000 text2story-1.2.4/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      114 2023-03-29 13:58:48.000000 text2story-1.2.4/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1576 2023-05-17 10:09:49.105173 text2story-1.2.4/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       70 2023-03-29 13:48:56.000000 text2story-1.2.4/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.089173 text2story-1.2.4/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.089173 text2story-1.2.4/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.093173 text2story-1.2.4/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.085173 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.093173 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.093173 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-16 12:34:10.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/ALLENNLP/preprocess.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.093173 text2story-1.2.4/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2023-04-28 09:04:12.000000 text2story-1.2.4/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.2.4/text2story/annotators/SPARKNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2199 2023-04-05 14:48:57.000000 text2story-1.2.4/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.097173 text2story-1.2.4/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.2.4/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2022-11-04 13:39:56.000000 text2story-1.2.4/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.101173 text2story-1.2.4/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.2.4/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.2.4/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5281 2023-05-03 09:45:52.000000 text2story-1.2.4/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.101173 text2story-1.2.4/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.2.4/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.105173 text2story-1.2.4/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.2.4/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22674 2023-03-27 13:07:12.000000 text2story-1.2.4/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.2.4/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.105173 text2story-1.2.4/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.2.4/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.2.4/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.2.4/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.2.4/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.105173 text2story-1.2.4/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.2.4/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.105173 text2story-1.2.4/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.2.4/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8324 2023-05-17 09:59:45.000000 text2story-1.2.4/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.105173 text2story-1.2.4/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.2.4/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14759 2023-03-31 13:18:54.000000 text2story-1.2.4/text2story/viz/bubble_tikz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:09:49.089173 text2story-1.2.4/text2story.egg-info/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9809 2023-05-17 10:09:49.000000 text2story-1.2.4/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2678 2023-05-17 10:09:49.000000 text2story-1.2.4/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-17 10:09:49.000000 text2story-1.2.4/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2023-05-17 10:09:49.000000 text2story-1.2.4/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-05-17 10:09:49.000000 text2story-1.2.4/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-03-29 13:58:12.000000 text2story-1.2.4/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.2.5/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.2.5/MANIFEST.in
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-17 10:12:53.891648 text2story-1.2.5/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8575 2023-05-17 10:11:38.000000 text2story-1.2.5/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      114 2023-03-29 13:58:48.000000 text2story-1.2.5/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1576 2023-05-17 10:12:53.895648 text2story-1.2.5/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       70 2023-03-29 13:48:56.000000 text2story-1.2.5/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.883648 text2story-1.2.5/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.883648 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-16 12:34:10.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/ALLENNLP/preprocess.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2023-04-28 09:04:12.000000 text2story-1.2.5/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.2.5/text2story/annotators/SPARKNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2199 2023-04-05 14:48:57.000000 text2story-1.2.5/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.2.5/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2022-11-04 13:39:56.000000 text2story-1.2.5/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.2.5/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.2.5/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5281 2023-05-03 09:45:52.000000 text2story-1.2.5/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.2.5/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.2.5/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22674 2023-03-27 13:07:12.000000 text2story-1.2.5/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.2.5/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.2.5/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.2.5/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.2.5/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.2.5/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.2.5/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.2.5/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8324 2023-05-17 09:59:45.000000 text2story-1.2.5/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.891648 text2story-1.2.5/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.2.5/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14759 2023-03-31 13:18:54.000000 text2story-1.2.5/text2story/viz/bubble_tikz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-17 10:12:53.887648 text2story-1.2.5/text2story.egg-info/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-17 10:12:53.000000 text2story-1.2.5/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2678 2023-05-17 10:12:53.000000 text2story-1.2.5/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-17 10:12:53.000000 text2story-1.2.5/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2023-05-17 10:12:53.000000 text2story-1.2.5/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-05-17 10:12:53.000000 text2story-1.2.5/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-03-29 13:58:12.000000 text2story-1.2.5/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.2.4/LICENSE` & `text2story-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/PKG-INFO` & `text2story-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.2.4
+Version: 1.2.5
 Summary: It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
 Home-page: https://www.inesctec.pt/pt/centros/liaad
 Author: LIAAD lab
 License: GNU Public Licence
 Keywords: natural-language-processing,nlp,natural-language-understanding,deep-learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -96,15 +96,15 @@
 
 t2s.start('en') # Load the pipelines in en language
 
 text = 'On Friday morning, Max Healthcare, which runs 10 private hospitals around Delhi, put out an "SOS" message, saying it had less than an hour\'s supply remaining at two of its sites. The shortage was later resolved.'
 
 doc = t2s.Narrative('en', text, '2020-05-30')
 
-doc.extract_actors('sparknlp') # Extraction done with just the SPARKNLP tool.
+doc.extract_actors('spacy') # Extraction done with just the SPACY tool.
 
 doc.extract_times() # Extraction done with all tools (same as specifying 'py_heideltime', since we have just one tool to extract timexs)
 
 
 doc.extract_events('allennlp') # Extraction of events with allennlp tool
 doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
 
@@ -140,15 +140,14 @@
          |   narrative.py (Narrative class)
          |   utils.py (Utility functions)
          
         └─ annotators (tools supported by the package to do the extractions)
          |   NLTK
          │   PY_HEIDELTIME
          |   SPACY
-         |   SPARKNLP
 	 |   ALLENNLP
 	 |   CUSTOMPT (A CRF customized model to detect events in the Portuguese language)
          
         └─ brat2viz (tool devoted to create visual representations of ann files)
          |   brat2drs (scripts that do a conversion from a brat stand off format (.ann) to DRS format)
          │   drs2viz (scripts that do a conversion from drs format to a visual representation)
 
@@ -174,15 +173,15 @@
 
 ### Annotators
 All annotators have the same interface: they implement a function called 'extract_' followed by the name of the particular extraction.
 E.g., if they are extracting actors, then they implement a function named 'extract_actors', with two arguments: the language of text and the text itself.
 
 |  Extractions |           Interface                                      |     Supporting tools  |
 |      ---     |             ---                                          |           ---         |
-|     Actor    | extract_actors(lang, text)                               | SPACY, SPARKNLP, NLTK |
+|     Actor    | extract_actors(lang, text)                               | SPACY, NLTK 	  |
 |    Timexs    | extract_timexs(lang, text, publication_time)             |      PY_HEIDELTIME    |
 | ObjectalLink | extract_objectal_links(lang, text, publication_time)     |        ALLENNLP       |
 |     Event    | extract_events(lang, text, publication_time)             | ALLENNLP, CUSTOMPT    |
 | SemanticLink | extract_semantic_role_link(lang, text, publication_time) |        ALLENNLP       |
 
 To **change some model used in the supported tools**, just go to text2story/annotators/ANNOTATOR_TO_BE_CHANGED and change the model in the file: \_\_init\_\_.py.
```

### Comparing `text2story-1.2.4/README.md` & `text2story-1.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 t2s.start('en') # Load the pipelines in en language
 
 text = 'On Friday morning, Max Healthcare, which runs 10 private hospitals around Delhi, put out an "SOS" message, saying it had less than an hour\'s supply remaining at two of its sites. The shortage was later resolved.'
 
 doc = t2s.Narrative('en', text, '2020-05-30')
 
-doc.extract_actors('sparknlp') # Extraction done with just the SPARKNLP tool.
+doc.extract_actors('spacy') # Extraction done with just the SPACY tool.
 
 doc.extract_times() # Extraction done with all tools (same as specifying 'py_heideltime', since we have just one tool to extract timexs)
 
 
 doc.extract_events('allennlp') # Extraction of events with allennlp tool
 doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
 
@@ -114,15 +114,14 @@
          |   narrative.py (Narrative class)
          |   utils.py (Utility functions)
          
         └─ annotators (tools supported by the package to do the extractions)
          |   NLTK
          │   PY_HEIDELTIME
          |   SPACY
-         |   SPARKNLP
 	 |   ALLENNLP
 	 |   CUSTOMPT (A CRF customized model to detect events in the Portuguese language)
          
         └─ brat2viz (tool devoted to create visual representations of ann files)
          |   brat2drs (scripts that do a conversion from a brat stand off format (.ann) to DRS format)
          │   drs2viz (scripts that do a conversion from drs format to a visual representation)
 
@@ -148,15 +147,15 @@
 
 ### Annotators
 All annotators have the same interface: they implement a function called 'extract_' followed by the name of the particular extraction.
 E.g., if they are extracting actors, then they implement a function named 'extract_actors', with two arguments: the language of text and the text itself.
 
 |  Extractions |           Interface                                      |     Supporting tools  |
 |      ---     |             ---                                          |           ---         |
-|     Actor    | extract_actors(lang, text)                               | SPACY, SPARKNLP, NLTK |
+|     Actor    | extract_actors(lang, text)                               | SPACY, NLTK 	  |
 |    Timexs    | extract_timexs(lang, text, publication_time)             |      PY_HEIDELTIME    |
 | ObjectalLink | extract_objectal_links(lang, text, publication_time)     |        ALLENNLP       |
 |     Event    | extract_events(lang, text, publication_time)             | ALLENNLP, CUSTOMPT    |
 | SemanticLink | extract_semantic_role_link(lang, text, publication_time) |        ALLENNLP       |
 
 To **change some model used in the supported tools**, just go to text2story/annotators/ANNOTATOR_TO_BE_CHANGED and change the model in the file: \_\_init\_\_.py.
```

### Comparing `text2story-1.2.4/setup.cfg` & `text2story-1.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = text2story
-version = 1.2.4
+version = 1.2.5
 author = LIAAD lab
 url = https://www.inesctec.pt/pt/centros/liaad
 description = It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = natural-language-processing, nlp, natural-language-understanding, deep-learning
 license = GNU Public Licence
```

### Comparing `text2story-1.2.4/text2story/__init__.py` & `text2story-1.2.5/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.2.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.2.5/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.2.5/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.2.5/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.2.5/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.2.5/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.2.5/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.2.5/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.2.5/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.2.5/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/NLTK/__init__.py` & `text2story-1.2.5/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.2.5/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/SPACY/__init__.py` & `text2story-1.2.5/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.2.5/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/annotators/__init__.py` & `text2story-1.2.5/text2story/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/brat2viz/README.md` & `text2story-1.2.5/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.2.5/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.2.5/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/brat2viz/drs2viz/app.py` & `text2story-1.2.5/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.2.5/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.2.5/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/core/annotator.py` & `text2story-1.2.5/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/core/entity_structures.py` & `text2story-1.2.5/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/core/link_structures.py` & `text2story-1.2.5/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/core/narrative.py` & `text2story-1.2.5/text2story/core/narrative.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/core/utils.py` & `text2story-1.2.5/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/experiments/evaluation.py` & `text2story-1.2.5/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/experiments/metrics.py` & `text2story-1.2.5/text2story/experiments/metrics.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/experiments/run_experiments.py` & `text2story-1.2.5/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/experiments/stats.py` & `text2story-1.2.5/text2story/experiments/stats.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/pb-vn2.json` & `text2story-1.2.5/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/read.py` & `text2story-1.2.5/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/read_brat.py` & `text2story-1.2.5/text2story/readers/read_brat.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/read_ecb.py` & `text2story-1.2.5/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/read_framenet.py` & `text2story-1.2.5/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/read_propbank.py` & `text2story-1.2.5/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/token_corpus.py` & `text2story-1.2.5/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/readers/utils.py` & `text2story-1.2.5/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/select/bubble.py` & `text2story-1.2.5/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/select/event.py` & `text2story-1.2.5/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/text2viz/Text2Viz.py` & `text2story-1.2.5/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/text2viz/visualization.py` & `text2story-1.2.5/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/training/participant_concept.py` & `text2story-1.2.5/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story/viz/bubble_tikz.py` & `text2story-1.2.5/text2story/viz/bubble_tikz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.4/text2story.egg-info/PKG-INFO` & `text2story-1.2.5/text2story.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.2.4
+Version: 1.2.5
 Summary: It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
 Home-page: https://www.inesctec.pt/pt/centros/liaad
 Author: LIAAD lab
 License: GNU Public Licence
 Keywords: natural-language-processing,nlp,natural-language-understanding,deep-learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -96,15 +96,15 @@
 
 t2s.start('en') # Load the pipelines in en language
 
 text = 'On Friday morning, Max Healthcare, which runs 10 private hospitals around Delhi, put out an "SOS" message, saying it had less than an hour\'s supply remaining at two of its sites. The shortage was later resolved.'
 
 doc = t2s.Narrative('en', text, '2020-05-30')
 
-doc.extract_actors('sparknlp') # Extraction done with just the SPARKNLP tool.
+doc.extract_actors('spacy') # Extraction done with just the SPACY tool.
 
 doc.extract_times() # Extraction done with all tools (same as specifying 'py_heideltime', since we have just one tool to extract timexs)
 
 
 doc.extract_events('allennlp') # Extraction of events with allennlp tool
 doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
 
@@ -140,15 +140,14 @@
          |   narrative.py (Narrative class)
          |   utils.py (Utility functions)
          
         └─ annotators (tools supported by the package to do the extractions)
          |   NLTK
          │   PY_HEIDELTIME
          |   SPACY
-         |   SPARKNLP
 	 |   ALLENNLP
 	 |   CUSTOMPT (A CRF customized model to detect events in the Portuguese language)
          
         └─ brat2viz (tool devoted to create visual representations of ann files)
          |   brat2drs (scripts that do a conversion from a brat stand off format (.ann) to DRS format)
          │   drs2viz (scripts that do a conversion from drs format to a visual representation)
 
@@ -174,15 +173,15 @@
 
 ### Annotators
 All annotators have the same interface: they implement a function called 'extract_' followed by the name of the particular extraction.
 E.g., if they are extracting actors, then they implement a function named 'extract_actors', with two arguments: the language of text and the text itself.
 
 |  Extractions |           Interface                                      |     Supporting tools  |
 |      ---     |             ---                                          |           ---         |
-|     Actor    | extract_actors(lang, text)                               | SPACY, SPARKNLP, NLTK |
+|     Actor    | extract_actors(lang, text)                               | SPACY, NLTK 	  |
 |    Timexs    | extract_timexs(lang, text, publication_time)             |      PY_HEIDELTIME    |
 | ObjectalLink | extract_objectal_links(lang, text, publication_time)     |        ALLENNLP       |
 |     Event    | extract_events(lang, text, publication_time)             | ALLENNLP, CUSTOMPT    |
 | SemanticLink | extract_semantic_role_link(lang, text, publication_time) |        ALLENNLP       |
 
 To **change some model used in the supported tools**, just go to text2story/annotators/ANNOTATOR_TO_BE_CHANGED and change the model in the file: \_\_init\_\_.py.
```

### Comparing `text2story-1.2.4/text2story.egg-info/SOURCES.txt` & `text2story-1.2.5/text2story.egg-info/SOURCES.txt`

 * *Files identical despite different names*

