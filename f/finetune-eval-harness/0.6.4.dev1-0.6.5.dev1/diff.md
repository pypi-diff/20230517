# Comparing `tmp/finetune_eval_harness-0.6.4.dev1.tar.gz` & `tmp/finetune_eval_harness-0.6.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetune_eval_harness-0.6.4.dev1.tar", last modified: Tue May 16 23:43:36 2023, max compression
+gzip compressed data, was "finetune_eval_harness-0.6.5.dev1.tar", last modified: Wed May 17 20:08:08 2023, max compression
```

## Comparing `finetune_eval_harness-0.6.4.dev1.tar` & `finetune_eval_harness-0.6.5.dev1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:43:36.490509 finetune_eval_harness-0.6.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 23:43:36.490509 finetune_eval_harness-0.6.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:43:36.490509 finetune_eval_harness-0.6.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:43:36.478509 finetune_eval_harness-0.6.4.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:43:36.482509 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:43:36.482509 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)    54569 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/process_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:43:36.490509 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/dutch_social.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/eur_lux.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/flue.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/german_europarl.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/german_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/german_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/germeval2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/germeval2018.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/gnad10.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/greek_legal.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/mapa.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/rucola.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/task_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 23:43:35.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:43:36.482509 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 23:43:36.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-16 23:43:36.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 23:43:36.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 23:43:36.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 23:43:36.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 23:43:36.000000 finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:08:08.313394 finetune_eval_harness-0.6.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 20:08:08.309394 finetune_eval_harness-0.6.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:08:08.313394 finetune_eval_harness-0.6.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:08:08.305394 finetune_eval_harness-0.6.5.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:08:08.305394 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:08:08.309394 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54631 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/process_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:08:08.309394 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/dutch_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/eur_lux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/flue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/german_europarl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/german_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/german_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/germeval2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/germeval2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/gnad10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/greek_legal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/mapa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/rucola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/task_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 20:08:06.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:08:08.305394 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 20:08:08.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-17 20:08:08.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 20:08:08.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 20:08:08.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 20:08:08.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 20:08:08.000000 finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/top_level.txt
```

### Comparing `finetune_eval_harness-0.6.4.dev1/LICENSE` & `finetune_eval_harness-0.6.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/PKG-INFO` & `finetune_eval_harness-0.6.5.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetune_eval_harness
-Version: 0.6.4.dev1
+Version: 0.6.5.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
```

### Comparing `finetune_eval_harness-0.6.4.dev1/README.md` & `finetune_eval_harness-0.6.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/setup.py` & `finetune_eval_harness-0.6.5.dev1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "finetune_eval_harness",
-    version="0.6.4.dev1",
+    version="0.6.5.dev1",
     description="Finetune_Eval_Harness",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="MIT",
     author="DFKI Berlin",
     author_email="akga01@dfki.de",
-    #url="https://github.com/malteos/finetune-evaluation-harness",
-    #package_dir={"":""},
-    # packages=[
-    #         'hf_scripts', 
-    #         'tasks',
-    #         'templates',
-    #         'tests',
-    # ],
-    # scripts = [
-    #     'process_args.py',
-    #     'main.py'
-    # ],
     package_dir={"": "src"},
     packages=find_packages("src"),
     entry_points={"console_scripts": ["finetune-eval-harness=finetune_eval_harness.main:main"]},
     python_requires=">=3.8.0",
     install_requires=[
         'pyarrow==6.0.1',
         'wandb',
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/__init__.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,21 +25,26 @@
     germeval2018,
     gnad10,
     ner,
     qa,
     german_quad,
 )
 '''
+
+'''
 import sys 
 sys.path.append('../')
-#from . import process_args
-#from . import main
 from src.finetune_eval_harness.tasks.task_registry import get_all_tasks, get_all_task_types, get_dataset_information
-#from .process_args import process_arguments
-#import src.finetune_eval.process_args as process_args
 
-
-#import src.finetune_eval.main as main
 import src.finetune_eval_harness.tasks
 import src.finetune_eval_harness.hf_scripts
 import src.finetune_eval_harness.tasks as tasks
 import src.finetune_eval_harness.hf_scripts as hf_scripts
+'''
+
+import sys
+sys.path.append('./')
+import tasks
+from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types, get_dataset_information
+
+sys.path.append('../')
+import hf_scripts
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,18 @@
     train_batch_size: int = field(
         default=2, metadata={"help": "Size of train batch size"}
     )
     label_value: Optional[str] = field(
         default=None, metadata={"help": "label from the original dataset"}
     )
     special_task_type: Optional[str] = field(
-        default=None, 
-        metadata={"help": "Is this some special task (eg multi-label classification). Use: multi_label_classification"}   
+        default=None,
+        metadata={
+            "help": "Is this some special task (eg multi-label classification). Use: multi_label_classification"
+        },
     )
     remove_labels: Optional[List[str]] = field(
         default=None,
         metadata={
             "help": "Labels which have to removed (please verify these from the original dataset)"
         },
     )
@@ -229,29 +231,31 @@
     )
     doc_stride: int = field(
         default=16,
         metadata={
             "help": "When splitting up a long document into chunks, how much stride to take between chunks."
         },
     )
-    is_subset: bool = field(default = False, metadata={"help": "Take subset of the datset"})
+    is_subset: bool = field(
+        default=False, metadata={"help": "Take subset of the datset"}
+    )
     train_file: Optional[str] = field(
         default=None,
         metadata={"help": "A csv or a json file containing the training data."},
     )
     validation_file: Optional[str] = field(
         default=None,
         metadata={"help": "A csv or a json file containing the validation data."},
     )
     test_file: Optional[str] = field(
         default=None,
         metadata={"help": "A csv or a json file containing the test data."},
     )
 
-    '''
+    """
     def __post_init__(self):
         if self.task_name is not None:
             self.task_name = self.task_name.lower()
             if self.task_name not in task_to_keys.keys():
                 raise ValueError(
                     "Unknown task, you should pick one in "
                     + ",".join(task_to_keys.keys())
@@ -268,8 +272,8 @@
                 "csv",
                 "json",
             ], "`train_file` should be a csv or a json file."
             validation_extension = self.validation_file.split(".")[-1]
             assert (
                 validation_extension == train_extension
             ), "`validation_file` should have the same extension (csv or json) as `train_file`."
-    '''
+    """
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/model_args.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/model_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/trainer.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/trainer.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import sys
-sys.path.append('../')
+
+sys.path.append("../")
 import numpy as np
 from dataclasses import dataclass, field
 from . import trainer_qa
 from . import hgf_fine_tune_class, hgf_fine_tune_ner, hgf_fine_tune_qa
 from .model_args import ModelArguments
 from .data_trainining_args import DataTrainingArguments
 from .initial_arguments import InitialArguments
@@ -29,15 +30,26 @@
 from peft import (
     get_peft_model,
     LoraConfig,
 )
 from peft import PrefixTuningConfig, PromptEncoderConfig, PromptTuningConfig, TaskType
 from peft.utils.other import fsdp_auto_wrap_policy
 from os import path
-from src.finetune_eval_harness.tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY 
+
+sys.path.append("./")
+from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types
+
+
+# from src.finetune_eval_harness.tasks.task_registry import (
+#     get_all_tasks,
+#     TASK_REGISTRY,
+#     TASK_TYPE_REGISTRY,
+# )
+
+
 import json
 from typing import Any, Dict
 from . import utils_qa
 from datasets import load_dataset, DatasetDict
 
 """
 File containing utlility functions used over all the hf_scripts folder for all the tasks
@@ -100,14 +112,15 @@
 
     data_args.results_log_path = init_args.results_logging_dir
     training_args.do_train = True
     training_args.do_eval = True
     training_args.overwrite_output_dir = True
     return (training_args, data_args)
 
+
 '''
 def parse_hf_arguments(args):
     """
     method to parse arguments in each of the hf script for each task
 
     Args:
         args: command line arguments passed while while running the main.py file
@@ -127,15 +140,15 @@
         model_args, data_args, training_args = parser.parse_args_into_dataclasses(
             args=args
         )
 
     return model_args, data_args, training_args
 
 '''
-    
+
 
 def freeze_layers(model_args: ModelArguments, model):
     """
     freeze layers of the model if parameter is passed
 
     Args:
         model_args: object of ModelArguments
@@ -329,15 +342,14 @@
         model: parameter efficent version of AutoModel class
 
     """
 
     task_type_dict = {"SEQ_CLS": TaskType.SEQ_CLS, "TOKEN_CLS": TaskType.TOKEN_CLS}
 
     if data_args.peft_choice == "lora":
-
         peft_config = LoraConfig(
             task_type=task_type_dict[task_type],
             inference_mode="False",
             # target_modules=["query", "value"],
             bias="none",
             r=data_args.r,
             lora_alpha=data_args.lora_alpha,
@@ -422,15 +434,14 @@
     peft_choice: str,
     remaining_params: float,
     problem_description: str,
     per_device_train_batch_size: int,
     label_value: str,
     results_log_path: str,
 ):
-
     """
     method for saving validation metrics if do_eval is True
 
     Args:
         model_name_or_path: name of the model according to HF hub
         trainer: object of the Trainer class
         max_eval_samples: maximum number of eval samples
@@ -476,38 +487,37 @@
         else:
             # file exists read the prev entry, add new one and then write
             with open(log_file_path, "r") as new_file_path:
                 curr_list = json.load(new_file_path)
                 print("curr_list", curr_list)
                 print("metrics", metrics)
                 curr_list = {**curr_list, **metrics}
-                
-                #curr_list = curr_list + [metrics]
+
+                # curr_list = curr_list + [metrics]
 
             with open(log_file_path, "w") as new_file_path:
                 json.dump(curr_list, new_file_path)
 
             new_file_path.close()
 
-        #trainer.log_metrics("eval", metrics)
-        #trainer.save_metrics("eval", metrics)
+        # trainer.log_metrics("eval", metrics)
+        # trainer.save_metrics("eval", metrics)
 
         return metrics
 
 
 def load_save_metrics_predict(
     trainer: Trainer,
     tasks: list,
     predict_datasets: Any,
     label_value: str,
     is_regression: bool,
     output_dir: str,
     label_list: list,
 ):
-
     """
     method for saving evaluation metrics incase do_predict = True
 
     Args:
         model_name_or_path: name of the model according to HF hub
         trainer: object of the Trainer class
         max_eval_samples: maximum number of eval samples
@@ -531,16 +541,18 @@
         predictions = trainer.predict(
             predict_dataset, metric_key_prefix="predict"
         ).predictions
         predictions = (
             np.squeeze(predictions) if is_regression else np.argmax(predictions, axis=1)
         )
 
-        if(os.path.isdir(output_dir)):
-            output_predict_file = os.path.join(output_dir, f"predict_results_{task}.txt")
+        if os.path.isdir(output_dir):
+            output_predict_file = os.path.join(
+                output_dir, f"predict_results_{task}.txt"
+            )
             if trainer.is_world_process_zero():
                 with open(output_predict_file, "w") as writer:
                     writer.write("index\tprediction\n")
                     for index, item in enumerate(predictions):
                         if is_regression:
                             writer.write(f"{index}\t{item:3.3f}\n")
                         else:
@@ -551,15 +563,14 @@
 def save_metrics_predict_ner(
     trainer: Trainer,
     training_args: TrainingArguments,
     predict_dataset: Any,
     output_dir: str,
     label_list: list,
 ):
-
     """
     method for saving prediction metrics for ner
 
     Args:
         model_name_or_path: name of the model according to HF hub
         trainer: object of the Trainer class
         max_eval_samples: maximum number of eval samples
@@ -651,15 +662,14 @@
 
     result["labels"] = result[label_value].copy()
 
     return result
 
 
 def compute_metrics_classification(p: EvalPrediction):
-
     """
     method for computing the classification metrics
     """
 
     preds = p.predictions[0] if isinstance(p.predictions, tuple) else p.predictions
     preds = np.argmax(preds, axis=1)
     return {"accuracy": (preds == p.label_ids).astype(np.float32).mean().item()}
@@ -793,28 +803,27 @@
 
 def load_raw_dataset(
     data_args: DataTrainingArguments,
     training_args: TrainingArguments,
     model_args: ModelArguments,
     logger: Any,
 ):
-
     """
     method for handling the downloading of raw dataset
 
     Args:
         data_args: object of DataTrainingArguments
         training_args: object of TrainingArguments
         model_args: object of ModelArguments
         logger: object of Logger class
 
     """
-    #raw_datasets = {}
-    #raw_datasets["train"]=[]
-    #raw_datasets["test"]=[]
+    # raw_datasets = {}
+    # raw_datasets["train"]=[]
+    # raw_datasets["test"]=[]
 
     raw_datasets = load_dataset(
         data_args.dataset_name,
         data_args.dataset_config_name,
         cache_dir=model_args.cache_dir,
         use_auth_token=True if model_args.use_auth_token else None,
     )
@@ -825,50 +834,48 @@
             "glue",
             data_args.task_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
     if "train" not in raw_datasets:
         train_testvalid = raw_datasets.train_test_split(test=0.1)
-        test_valid = train_testvalid['test']
-        raw_datasets = DatasetDict({
-            'train': train_testvalid['train'],
-            'test': train_testvalid['test']
-        })
+        test_valid = train_testvalid["test"]
+        raw_datasets = DatasetDict(
+            {"train": train_testvalid["train"], "test": train_testvalid["test"]}
+        )
 
     if data_args.is_subset == True:
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
         raw_datasets["train"] = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
-            split=f"train[:3%]",           # use 4% of the train set
+            split=f"train[:3%]",  # use 4% of the train set
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
         raw_datasets["test"] = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
-            split=f"test[:1%]",           # use 1% of the test set
+            split=f"test[:1%]",  # use 1% of the test set
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
     else:
         # Downloading and loading a dataset from the hub.
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
-    
 
     return raw_datasets
 
 
 def load_raw_dataset_ner(data_args: DataTrainingArguments, model_args: ModelArguments):
     """
     download raw dataset
@@ -886,22 +893,22 @@
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
         raw_datasets["train"] = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
-            split=f"train[:3%]",           # use 4% of the train set
+            split=f"train[:3%]",  # use 4% of the train set
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
         raw_datasets["validation"] = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
-            split=f"validation[:1%]",           # use 1% of the test set
+            split=f"validation[:1%]",  # use 1% of the test set
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
 
         # raw_datasets["test"] = load_dataset(
         #     data_args.dataset_name,
         #     data_args.dataset_config_name,
@@ -915,72 +922,70 @@
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
 
-    '''
+    """
     else:
         data_files = {}
         if data_args.train_file is not None:
             data_files["train"] = data_args.train_file
         if data_args.validation_file is not None:
             data_files["validation"] = data_args.validation_file
         if data_args.test_file is not None:
             data_files["test"] = data_args.test_file
         extension = data_args.train_file.split(".")[-1]
         raw_datasets = load_dataset(
             extension, data_files=data_files, cache_dir=model_args.cache_dir
         )
-    '''
+    """
 
     return raw_datasets
 
-def load_raw_dataset_qa(data_args: DataTrainingArguments, model_args: ModelArguments):
 
+def load_raw_dataset_qa(data_args: DataTrainingArguments, model_args: ModelArguments):
     if data_args.is_subset == True:
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
         raw_datasets["train"] = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
-            split=f"train[:3%]",           # use 4% of the train set
+            split=f"train[:3%]",  # use 4% of the train set
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
         raw_datasets["test"] = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
-            split=f"test[:1%]",           # use 1% of the test set
+            split=f"test[:1%]",  # use 1% of the test set
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
 
     elif data_args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
-        
-    return raw_datasets
 
+    return raw_datasets
 
 
 def preprocess_raw_datasets(
     raw_datasets: Any, data_args: DataTrainingArguments, label_value: str
 ):
-
     """
     method for pre-processing raw datasets
 
     Args:
         data_args: object of DataTrainingArguments
         training_args: object of TrainingArguments
         model_args: object of ModelArguments
@@ -1025,15 +1030,14 @@
         unique_labels = unique_labels | set(label)
     label_list = list(unique_labels)
     label_list.sort()
     return label_list
 
 
 def tokenize_and_align_labels(examples: Dict[str, Any], **fn_kwargs) -> Dict[str, Any]:
-
     """
     returns object of Tokenizer class
 
     Args:
         examples: samples from the dataset
         fn_kwargs: other columns relating to aligning labels for ner
 
@@ -1083,15 +1087,14 @@
 
         labels.append(label_ids)
     tokenized_inputs["labels"] = labels
     return tokenized_inputs
 
 
 def check_tokenizer_instance(tokenizer: AutoTokenizer):
-
     """
     check if tokenizer is PretrainedTokenizer
 
     Args:
         tokenizer: object of AutoTokenizer
 
     Returns:
@@ -1104,15 +1107,14 @@
             "This example script only works for models that have a fast tokenizer. Checkout the big table of models at"
             " https://huggingface.co/transformers/index.html#supported-frameworks to find the model types that meet"
             " this requirement"
         )
 
 
 def generate_b_to_i_label(feature_file_exists: bool, label_list: list):
-
     """
     method to generate b_to_i_label
 
     Args:
         feature_file_exists: boolean value indicating if feature file is there in the hf hub
         label_list: list of labels from the hf dataset
 
@@ -1137,15 +1139,14 @@
 
 def map_train_validation_predict_ds_ner(
     training_args: TrainingArguments,
     data_args: DataTrainingArguments,
     raw_datasets: Any,
     fn_kwargs: Any,
 ):
-
     """
     logic for mapping train, test and validation splits for the ner task
 
     Args:
         training_args: object of TrainingArguments
         data_args: object of DataTrainingArguments
         raw_datasets: datasets object from the hf
@@ -1176,19 +1177,19 @@
                 fn_kwargs=fn_kwargs,
                 load_from_cache_file=not data_args.overwrite_cache,
                 desc="Running tokenizer on train dataset",
             )
 
     if training_args.do_eval:
         if "validation" not in raw_datasets:
-            #raise ValueError("--do_eval requires a validation dataset")
+            # raise ValueError("--do_eval requires a validation dataset")
             eval_dataset = raw_datasets["test"]
         else:
             eval_dataset = raw_datasets["validation"]
-        #eval_dataset = raw_datasets["validation"]
+        # eval_dataset = raw_datasets["validation"]
 
         if data_args.max_eval_samples is not None:
             max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
             eval_dataset = eval_dataset.select(range(max_eval_samples))
         with training_args.main_process_first(
             desc="validation dataset map pre-processing"
         ):
@@ -1196,15 +1197,15 @@
                 tokenize_and_align_labels,
                 batched=True,
                 fn_kwargs=fn_kwargs,
                 num_proc=data_args.preprocessing_num_workers,
                 load_from_cache_file=not data_args.overwrite_cache,
                 desc="Running tokenizer on validation dataset",
             )
-            
+
     return train_dataset, eval_dataset, predict_dataset
 
 
 def generate_label_list(
     raw_datasets: Any, features: Any, ClassLabel: Any, label_column_name: str
 ):
     """
@@ -1236,15 +1237,14 @@
 
     return label_list, label_to_id, feature_file_exists, labels_are_int
 
 
 def prepare_train_features_qa(
     examples: Dict[str, Any], **fn_kwargs_train
 ) -> Dict[str, Any]:
-
     """
     method to prepare train features for qa task
 
     Args:
         examples: instances from the processed dataset
         fn_kwargs: dict containing other fields for preparing train features
 
@@ -1345,15 +1345,14 @@
 
     return tokenized_examples
 
 
 def prepare_features_validation_qa(
     examples: Dict[str, Any], **fn_kwargs_validation
 ) -> Dict[str, Any]:
-
     """
     method to generate features for validation dataset for qa task
 
     Args:
         examples: instances from processed validation dataset
         fn_kwargs_validation: dict containing other fields for processing validation dataset
 
@@ -1417,15 +1416,15 @@
         tokenized_examples["offset_mapping"][i] = [
             (o if sequence_ids[k] == context_index else None)
             for k, o in enumerate(tokenized_examples["offset_mapping"][i])
         ]
 
     return tokenized_examples
 
-    
+
 def train_eval_prediction(
     task_type: str,
     model: Any,
     training_args: TrainingArguments,
     data_args: DataTrainingArguments,
     model_args: ModelArguments,
     train_dataset: Any,
@@ -1438,15 +1437,14 @@
     last_checkpoint: Any,
     label_value: str,
     predict_dataset: Any,
     predict_examples: Any,
     label_list: str,
     is_regression: bool,
 ):
-
     """
     method consisting of training, evaluation and prediction loop logic for each of the task
 
     Args:
         task_type: type of the task
         model: object of AutoModel
         training_args: object of TrainingArguments
@@ -1548,15 +1546,14 @@
                 label_list,
             )
 
     return metrics_eval
 
 
 def map_source_file(task_name: str):
-
     """
     identify the task_type and return the name of the appropriate hf script name
 
     Args:
         task_name: name of the task (classification, ner and qa)
 
     """
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/process_args.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/process_args.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 import sys
 sys.path.append('./')
 from transformers import HfArgumentParser, TrainingArguments
-#from tasks import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
 from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
 import logging
 sys.path.append('../')
-'''
-from hf_scripts.utility_functions import (
-    map_source_file,
-    peft_choice_list,
-    add_labels_data_args,
-)
-from hf_scripts.model_args import ModelArguments
-from hf_scripts.data_trainining_args import DataTrainingArguments
-from hf_scripts.initial_arguments import InitialArguments
-'''
 
 from hf_scripts.utility_functions import (
     map_source_file,
     peft_choice_list,
     add_labels_data_args,
 )
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/__init__.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/task_registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,10 @@
 from typing import List, Union
-from . import (
-    germeval2018,
-    germeval2017,
-    gnad10,
-    german_ner,
-    german_europarl,
-    german_quad,
-    spanish_quad,
-    wiki_cat_es,
-    spanish_conll,
-    flue,
-    spanish_ehealth,
-    szeged_ner,
-    polish_dyk,
-    mapa,
-    eur_lux,
-    ehealth_kd,
-    rucola,
-    klej_dyk,
-    croatian_sentiment,
-    finish_sentiment,
-    swedish_ner,
-    greek_legal,
-    bulgarian_sentiment,
-    czech_subjectivity,
-    danish_misogyny,
-    slovak_sentiment,
-    maltese_sentiment,
-    dutch_social,
-    classification,
-    ner,
-    qa,
-    
-)
+from . import *
 
-''''
 # mapping task to class objects
 TASK_REGISTRY = {
     "germeval2018": germeval2018.GermEval2018,
     "germeval2017": germeval2017.GermEval2017,
     "gnad10": gnad10.Gnad10,
     "german_ner_legal": german_ner.GermanNerLegal,
     "german_europarl": german_europarl.GermanEuroParl,
@@ -101,20 +67,42 @@
     "dutch_social": "classification",
     
 }
 
 ALL_TASKS = sorted(list(TASK_REGISTRY))
 ALL_TASK_TYPES = sorted(list(TASK_TYPE_REGISTRY))
 
+'''
+# returning task class
+def get_task(task_name):
+    try:
+        return TASK_REGISTRY[task_name]
+    except KeyError as exc:
+        print("Available tasks:")
+        print(TASK_REGISTRY)
+        raise KeyError(f"Missing task {task_name}") from exc
 
+'''
 
 # return string names of all the tasks for reference
 def get_all_tasks():
     all_task_str = []
     for key in TASK_REGISTRY:
         all_task_str.append(key)
 
     return all_task_str
 
-'''
+def get_all_task_types():
+    all_task_str = {}
+    for key in TASK_TYPE_REGISTRY:
+        all_task_str[key] = TASK_REGISTRY[key]
+    
+    return all_task_str
+
+def get_dataset_information(dataset_name):
+    #task_obj = TASK_REGISTRY[dataset_name]
+    output_dict = []
+    output_dict.append(TASK_REGISTRY[dataset_name]().get_label_name())
+    output_dict.append(TASK_REGISTRY[dataset_name]().get_dataset_id())
+    output_dict.append(TASK_REGISTRY[dataset_name]().get_url())
 
-from .task_registry import get_all_tasks, TASK_REGISTRY, ALL_TASK_TYPES
+    return output_dict
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 #from tasks.classification import Classification
 from .classification import Classification
 
 _DESCRIPTION = """
+Classification task for Bulagariansentiment dataset
+"""
+
+
+_CITATION = """
 
 """
 
+
 class BulgarianSentiment(Classification):
 
     """
     Class for GermEval 2017 Classification Task
     """
 
 
     DATASET_ID = "sepidmnorozy/Bulgarian_sentiment"  # HF datasets ID
     TASK_NAME = "bulgarian_sentiment"
-    LABEL_NAME = "label"  # column name from HF dataset
+    LABEL_NAME = "label"                            # column name from HF dataset
     HOMEPAGE_URL = "https://huggingface.co/datasets/sepidmnorozy/Bulgarian_sentiment"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
     def get_task_name(self):
         return self.TASK_NAME
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/classification.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 #from tasks.classification import Classification
 from .classification import Classification
 
 
+_DESCRIPTION = """
+Classification task for Croatian sentiment dataset
+"""
+
+
+_CITATION = """
+
+"""
+
 class CroatianSentiment(Classification):
 
     """
     Class for GermEval 2017 Classification Task
     """
 
 
     DATASET_ID = "sepidmnorozy/Croatian_sentiment"  # HF datasets ID
     TASK_NAME = "croatian_sentiment"
-    LABEL_NAME = "label"  # column name from HF dataset
+    LABEL_NAME = "label"                            # column name from HF dataset
     HOMEPAGE_URL = "https://huggingface.co/datasets/sepidmnorozy/Croatian_sentiment"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
     def get_task_name(self):
         return self.TASK_NAME
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 #from tasks.classification import Classification
 from .classification import Classification
 
+_DESCRIPTION = """
+Maltese version of PAWS-X dataset
+"""
 
-class CzechSubjectivity(Classification):
+
+_CITATION = """
+
+
+"""
+
+
+class MalteseSentiment(Classification):
 
     """
     Class for GermEval 2017 Classification Task
     """
 
 
-    DATASET_ID = "pauli31/czech-subjectivity-dataset"  # HF datasets ID
-    TASK_NAME = "czech_subjectivity"
+    DATASET_ID = "amitness/PAWS-X-maltese"  # HF datasets ID
+    TASK_NAME = "maltese_sentiment"
     LABEL_NAME = "label"  # column name from HF dataset
-    HOMEPAGE_URL = "https://huggingface.co/datasets/pauli31/czech-subjectivity-dataset"
+    HOMEPAGE_URL = "https://huggingface.co/datasets/amitness/PAWS-X-maltese"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
     def get_task_name(self):
         return self.TASK_NAME
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 #from tasks.classification import Classification
 from .classification import Classification
 
 
-class DanishMisogyny(Classification):
+DESCRIPTION = """
+
+Classification dataset for slovak sentiment 
+
+"""
+
+
+_CITATION = """
+
+
+
+"""
+
+
+
+
+class SlovakSentiment(Classification):
 
     """
     Class for GermEval 2017 Classification Task
     """
 
 
-    DATASET_ID = "strombergnlp/bajer_danish_misogyny"  # HF datasets ID
-    TASK_NAME = "danish_misogyny"
-    LABEL_NAME = "subtask_A"            # column name from HF dataset
-    HOMEPAGE_URL = "https://huggingface.co/datasets/strombergnlp/bajer_danish_misogyny"
+    DATASET_ID = "sepidmnorozy/Slovak_sentiment"  # HF datasets ID
+    TASK_NAME = "slovak_sentiment"
+    LABEL_NAME = "label"  # column name from HF dataset
+    HOMEPAGE_URL = "https://huggingface.co/datasets/sepidmnorozy/Slovak_sentiment"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
     def get_task_name(self):
         return self.TASK_NAME
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/dutch_social.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/german_europarl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,43 @@
-#from tasks.classification import Classification
+#from tasks.ner import NamedEntityRecognition
 from .classification import Classification
+from .ner import NamedEntityRecognition
 
 
-class DutchSocial(Classification):
+_DESCRIPTION = """
+NER task for german subsplit of the Europarl dataset
+"""
 
-    """
-    Class for GermEval 2017 Classification Task
-    """
 
+_CITATION = """
+
+"""
 
-    DATASET_ID = "dutch_social"  # HF datasets ID
-    TASK_NAME = "dutch_social"
-    LABEL_NAME = "label"  # column name from HF dataset
-    HOMEPAGE_URL = "https://huggingface.co/datasets/dutch_social"
+
+
+class GermanEuroParl(NamedEntityRecognition):
+
+    """
+    Class for German Europarl Task
+    """
+    
+    DATASET_ID = "akash418/german_europarl"
+    TASK_NAME = "german_europarl"
+    HOMEPAGE_URL = "https://huggingface.co/datasets/akash418/german_europarl"
 
     def get_dataset_id(self):
+        """
+        return HF dataset id
+        """
         return self.DATASET_ID
 
     def get_task_name(self):
+        """
+        return task name
+        """
         return self.TASK_NAME
 
-    def get_label_name(self):
-        return self.LABEL_NAME
-
     def get_url(self):
+        """
+        return url
+        """
         return self.HOMEPAGE_URL
-
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 #from tasks.ner import NamedEntityRecognition
-from .classification import Classification
 from .ner import NamedEntityRecognition
 
-class EhealthKd(NamedEntityRecognition):
+class SpanishEhealth(NamedEntityRecognition):
 
     """
     Class for German NER Legal Task
     """
     
     DATASET_ID = "ehealth_kd"  # HF datasets ID
-    TASK_NAME = "ehealth_kd"
-    HOMEPAGE_URL = "https://huggingface.co/datasets/fmmolina/eHealth-KD-Adaptation"
-    LABEL_NAME = "entities"
+    TASK_NAME = "spanish_ehealth"
+    HOMEPAGE_URL = "https://huggingface.co/datasets/ehealth_kd"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
     def get_task_name(self):
         return self.TASK_NAME
 
     def get_url(self):
         return self.HOMEPAGE_URL
     
-    def get_label_name(self):
-        return self.LABEL_NAME
-
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/eur_lux.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/germeval2018.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-#from tasks.classification import Classification
-#from tasks.ner import NamedEntityRecognition
+# from tasks.classification import Classification
 from .classification import Classification
 
+_DESCRIPTION = """
+
+"""
 
 
 _CITATION = """
-@inproceedings{germevaltask2017,
-title = {{GermEval 2017: Shared Task on Aspect-based Sentiment in Social Media Customer Feedback}},
-author = {Michael Wojatzki and Eugen Ruppert and Sarah Holschneider and Torsten Zesch and Chris Biemann},
-year = {2017},
-booktitle = {Proceedings of the GermEval 2017 - Shared Task on Aspect-based Sentiment in Social Media Customer Feedback},
-address={Berlin, Germany},
-pages={1--12}
-}
-"""
+@inproceedings{vamvas2020germeval,
+    author    = "Wiegand, Michael, and Siegel, Melanie and Ruppenhofer, Josef",
+    title     = "Overview of the GermEval 2018 Shared Task on the Identification of Offensive Language",
+    booktitle = "Proceedings of the GermEval 2018 Workshop  14th Conference on Natural Language Processing (KONSENS)",
+    address   = "Vienna, SAustria",
+    year      = "2018",
+    month     = "sep",
+    url       = "https://epub.oeaw.ac.at/0xc1aa5576_0x003a10d2.pdf"
+}"""
 
 
-class EurLux(Classification):
+class GermEval2018(Classification):
 
     """
-    Class for GermEval 2017 Classification Task
+    Class for GermEval 2018 Classification Task
     """
 
+    DATASET_ID = "philschmid/germeval18"    # HF datasets ID
+    TASK_NAME = "germeval2018"
+    LABEL_NAME = "multi"                    # column name from HF dataset
+    HOMEPAGE_URL = "https://huggingface.co/datasets/philschmid/germeval18"
 
-    DATASET_ID = "multi_eurlex"  # HF datasets ID
-    TASK_NAME = "eur_lux"
-    LABEL_NAME = "labels"  # column name from HF dataset
-    HOMEPAGE_URL = "https://huggingface.co/datasets/multi_eurlex"
+    def get_task_name(self):
+        return self.TASK_NAME
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
-    def get_task_name(self):
-        return self.TASK_NAME
-
     def get_label_name(self):
         return self.LABEL_NAME
 
     def get_url(self):
         return self.HOMEPAGE_URL
-
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #from tasks.classification import Classification
 from .classification import Classification
 
 
+DESCRIPTION = """
+Classification task for Finish sentiments 
+"""
+
+
+_CITATION = """
+
+"""
+
+
 class FinishSentiment(Classification):
 
     """
     Class for Finish Sentiment Classification
     """
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/german_europarl.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/german_ner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #from tasks.ner import NamedEntityRecognition
-from .classification import Classification
 from .ner import NamedEntityRecognition
 
-class GermanEuroParl(NamedEntityRecognition):
+class GermanNerLegal(NamedEntityRecognition):
 
     """
-    Class for German Europarl Task
+    Class for German NER Legal Task
     """
-
-    DATASET_ID = "akash418/german_europarl"
-    TASK_NAME = "german_europarl"
-    HOMEPAGE_URL = "https://huggingface.co/datasets/akash418/german_europarl"
+    
+    DATASET_ID = "elenanereiss/german-ler"  # HF datasets ID
+    TASK_NAME = "german_ner"
+    HOMEPAGE_URL = "https://huggingface.co/datasets/elenanereiss/german-ler"
 
     def get_dataset_id(self):
-        """
-        return HF dataset id
-        """
         return self.DATASET_ID
 
     def get_task_name(self):
-        """
-        return task name
-        """
         return self.TASK_NAME
 
     def get_url(self):
-        """
-        return url
-        """
         return self.HOMEPAGE_URL
+
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/germeval2017.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/germeval2017.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-#from tasks.classification import Classification
+# from tasks.classification import Classification
 from .classification import Classification
 
 
+_DESCRIPTION = """
+
+Germeval Task 2017: Shared Task on Aspect-based Sentiment in Social Media Customer Feedback
+
+"""
+
+
 _CITATION = """
+
 @inproceedings{germevaltask2017,
 title = {{GermEval 2017: Shared Task on Aspect-based Sentiment in Social Media Customer Feedback}},
 author = {Michael Wojatzki and Eugen Ruppert and Sarah Holschneider and Torsten Zesch and Chris Biemann},
 year = {2017},
 booktitle = {Proceedings of the GermEval 2017 - Shared Task on Aspect-based Sentiment in Social Media Customer Feedback},
 address={Berlin, Germany},
 pages={1--12}
 }
+
 """
 
 
 class GermEval2017(Classification):
 
     """
     Class for GermEval 2017 Classification Task
     """
 
-
     DATASET_ID = "akash418/germeval_2017"  # HF datasets ID
     TASK_NAME = "germeval2017"
     LABEL_NAME = "relevance"  # column name from HF dataset
     HOMEPAGE_URL = "https://huggingface.co/datasets/malteos/germeval2017"
 
     def get_dataset_id(self):
         return self.DATASET_ID
@@ -33,8 +41,7 @@
         return self.TASK_NAME
 
     def get_label_name(self):
         return self.LABEL_NAME
 
     def get_url(self):
         return self.HOMEPAGE_URL
-
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/germeval2018.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/klej_dyk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 #from tasks.classification import Classification
 from .classification import Classification
 
 
+_DESCRIPTION = """
+Question Answering dataset consists of almost 5k question-answer pairs obtained from Czy wiesz, section of Polish Wikipedia
+"""
+
+
 _CITATION = """
-@inproceedings{vamvas2020germeval,
-    author    = "Wiegand, Michael, and Siegel, Melanie and Ruppenhofer, Josef",
-    title     = "Overview of the GermEval 2018 Shared Task on the Identification of Offensive Language",
-    booktitle = "Proceedings of the GermEval 2018 Workshop  14th Conference on Natural Language Processing (KONSENS)",
-    address   = "Vienna, SAustria",
-    year      = "2018",
-    month     = "sep",
-    url       = "https://epub.oeaw.ac.at/0xc1aa5576_0x003a10d2.pdf"
-}"""
+
+@misc{11321/39,	
+ title = {Pytania i odpowiedzi z serwisu wikipedyjnego "Czy wiesz", wersja 1.1},	
+ author = {Marci{\'n}czuk, Micha{\l} and Piasecki, Dominik and Piasecki, Maciej and Radziszewski, Adam},	
+ url = {http://hdl.handle.net/11321/39},	
+ note = {{CLARIN}-{PL} digital repository},	
+ year = {2013}	
+}
+
+"""
 
 
-class GermEval2018(Classification):
+
+class KlejDyk(Classification):
 
     """
-    Class for GermEval 2018 Classification Task
+    Class for Klej Dyk Classification Task
     """
 
-    DATASET_ID = "philschmid/germeval18"  # HF datasets ID
-    TASK_NAME = "germeval2018"
-    LABEL_NAME = "multi"  # column name from HF dataset
-    HOMEPAGE_URL = "https://huggingface.co/datasets/philschmid/germeval18"
 
-    def get_task_name(self):
-        return self.TASK_NAME
+    DATASET_ID = "allegro/klej-dyk"  # HF datasets ID
+    TASK_NAME = "klej_dyk"
+    LABEL_NAME = "target"  # column name from HF dataset
+    HOMEPAGE_URL = "https://huggingface.co/datasets/allegro/klej-dyk"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
+    def get_task_name(self):
+        return self.TASK_NAME
+
     def get_label_name(self):
         return self.LABEL_NAME
-    
+
     def get_url(self):
         return self.HOMEPAGE_URL
-    
+
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/gnad10.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/dutch_social.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,36 @@
-#from tasks.classification import Classification
+# from tasks.classification import Classification
 from .classification import Classification
 
-class Gnad10(Classification):
+
+_DESCRIPTION = """
+Classification of social media data in dutch language (See more for data collection from the web page url) 
+"""
+
+
+_CITATION = """
+@data{FK2/MTPTL7_2020, author = {Gupta, Aakash}, publisher = {COVID-19 Data Hub}, title = {{Dutch social media collection}}, year = {2020}, version = {DRAFT VERSION}, doi = {10.5072/FK2/MTPTL7}, url = {https://doi.org/10.5072/FK2/MTPTL7} }
+"""
+
+
+class DutchSocial(Classification):
 
     """
-    Class for GNAD10 Classification Task
+    Class for GermEval 2017 Classification Task
     """
-    
-    DATASET_ID = "gnad10"  # HF datasets ID
-    TASKNAME = "gnad10"
-    LABEL_NAME = "label"
-    HOMEPAGE_URL = "https://huggingface.co/datasets/gnad10"
+
+    DATASET_ID = "dutch_social"  # HF datasets ID
+    TASK_NAME = "dutch_social"
+    LABEL_NAME = "label"  # column name from HF dataset
+    HOMEPAGE_URL = "https://huggingface.co/datasets/dutch_social"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
+    def get_task_name(self):
+        return self.TASK_NAME
+
     def get_label_name(self):
         return self.LABEL_NAME
 
-    def get_task_name(self):
-        return self.TASKNAME
-
     def get_url(self):
-        return self.HOMEPAGE_URL
+        return self.HOMEPAGE_URL
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/ner.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness/tasks/swedish_ner.py` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness/tasks/swedish_ner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 #from tasks.ner import NamedEntityRecognition
 from .ner import NamedEntityRecognition
 
+
+DESCRIPTION = """
+
+emi-manually defined in this case as: Bootstrapped from Swedish Gazetters then manually correcte/reviewed by two independent native speaking swedish annotators
+
+"""
+
+
+_CITATION = """
+
+
+"""
+
+
 class SwedishNer(NamedEntityRecognition):
 
     """
     Class for Swedish NER
     """
     
     DATASET_ID = "swedish_ner_corpus"  # HF datasets ID
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/PKG-INFO` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetune-eval-harness
-Version: 0.6.4.dev1
+Version: 0.6.5.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
```

### Comparing `finetune_eval_harness-0.6.4.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt` & `finetune_eval_harness-0.6.5.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

