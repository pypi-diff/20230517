# Comparing `tmp/finetune_eval_harness-0.6.2.dev1.tar.gz` & `tmp/finetune_eval_harness-0.6.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetune_eval_harness-0.6.2.dev1.tar", last modified: Tue May 16 22:15:21 2023, max compression
+gzip compressed data, was "finetune_eval_harness-0.6.3.dev1.tar", last modified: Tue May 16 22:34:23 2023, max compression
```

## Comparing `finetune_eval_harness-0.6.2.dev1.tar` & `finetune_eval_harness-0.6.3.dev1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:21.112133 finetune_eval_harness-0.6.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 22:15:21.112133 finetune_eval_harness-0.6.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:15:21.112133 finetune_eval_harness-0.6.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:21.108133 finetune_eval_harness-0.6.2.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:21.108133 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:21.108133 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)    54569 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/process_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:21.112133 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/dutch_social.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/eur_lux.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/flue.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/german_europarl.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/german_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/german_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/germeval2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/germeval2018.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/gnad10.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/greek_legal.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/mapa.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/rucola.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/task_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 22:15:19.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:21.108133 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 22:15:21.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-16 22:15:21.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 22:15:21.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 22:15:21.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 22:15:21.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 22:15:21.000000 finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:34:23.616422 finetune_eval_harness-0.6.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 22:34:23.616422 finetune_eval_harness-0.6.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:34:23.616422 finetune_eval_harness-0.6.3.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:34:23.608422 finetune_eval_harness-0.6.3.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:34:23.608422 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:34:23.612422 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54569 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/process_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:34:23.616422 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/dutch_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/eur_lux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/flue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/german_europarl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/german_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/german_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/germeval2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/germeval2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/gnad10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/greek_legal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/mapa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/rucola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/task_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 22:34:21.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:34:23.612422 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 22:34:23.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-16 22:34:23.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 22:34:23.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 22:34:23.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 22:34:23.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 22:34:23.000000 finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/top_level.txt
```

### Comparing `finetune_eval_harness-0.6.2.dev1/LICENSE` & `finetune_eval_harness-0.6.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/PKG-INFO` & `finetune_eval_harness-0.6.3.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetune_eval_harness
-Version: 0.6.2.dev1
+Version: 0.6.3.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
```

### Comparing `finetune_eval_harness-0.6.2.dev1/README.md` & `finetune_eval_harness-0.6.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/setup.py` & `finetune_eval_harness-0.6.3.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "finetune_eval_harness",
-    version="0.6.2.dev1",
+    version="0.6.3.dev1",
     description="Finetune_Eval_Harness",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="MIT",
     author="DFKI Berlin",
     author_email="akga01@dfki.de",
```

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/__init__.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     german_quad,
 )
 '''
 import sys 
 sys.path.append('../')
 #from . import process_args
 #from . import main
-from src.finetune_eval_harness.tasks.task_registry import get_all_tasks
+from src.finetune_eval_harness.tasks.task_registry import get_all_tasks, get_all_task_types, get_dataset_information
 #from .process_args import process_arguments
 #import src.finetune_eval.process_args as process_args
 
 
 #import src.finetune_eval.main as main
 import src.finetune_eval_harness.tasks
 import src.finetune_eval_harness.hf_scripts
```

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/model_args.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/model_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/trainer.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/trainer.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/process_args.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/process_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/__init__.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/classification.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/dutch_social.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/dutch_social.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/eur_lux.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/eur_lux.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/flue.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/flue.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/german_europarl.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/german_europarl.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/german_ner.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/german_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/germeval2017.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/germeval2017.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/germeval2018.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/germeval2018.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/gnad10.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/gnad10.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/greek_legal.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/greek_legal.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/klej_dyk.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/klej_dyk.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/mapa.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/mapa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/ner.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/rucola.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/rucola.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/spanish_conll.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/spanish_conll.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/swedish_ner.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/swedish_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/szeged_ner.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/szeged_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/task_registry.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/task_registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,8 +85,24 @@
 
 # return string names of all the tasks for reference
 def get_all_tasks():
     all_task_str = []
     for key in TASK_REGISTRY:
         all_task_str.append(key)
 
-    return all_task_str
+    return all_task_str
+
+def get_all_task_types():
+    all_task_str = {}
+    for key in TASK_TYPE_REGISTRY:
+        all_task_str[key] = TASK_REGISTRY[key]
+    
+    return all_task_str
+
+def get_dataset_information(dataset_name):
+    #task_obj = TASK_REGISTRY[dataset_name]
+    output_dict = {}
+    output_dict.append(TASK_REGISTRY[dataset_name]().get_label_name())
+    output_dict.append(TASK_REGISTRY[dataset_name]().get_dataset_id())
+    output_dict.append(TASK_REGISTRY[dataset_name]().get_url())
+
+    return output_dict
```

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/PKG-INFO` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetune-eval-harness
-Version: 0.6.2.dev1
+Version: 0.6.3.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
```

### Comparing `finetune_eval_harness-0.6.2.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt` & `finetune_eval_harness-0.6.3.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

