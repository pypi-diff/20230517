# Comparing `tmp/shallowpavlov-0.0.1.tar.gz` & `tmp/shallowpavlov-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shallowpavlov-0.0.1.tar", last modified: Wed May 17 15:29:04 2023, max compression
+gzip compressed data, was "shallowpavlov-1.0.0rc1.tar", last modified: Wed May 10 21:52:53 2023, max compression
```

## Comparing `shallowpavlov-0.0.1.tar` & `shallowpavlov-1.0.0rc1.tar`

### file list

```diff
@@ -1,387 +1,387 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.040868 shallowpavlov-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-17 15:29:04.040868 shallowpavlov-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.920863 shallowpavlov-0.0.1/deeppavlov/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.920863 shallowpavlov-0.0.1/deeppavlov/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.924863 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/boolqa_rubert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.928863 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/insults_kaggle_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/paraphraser_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/query_pr.json
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_convers_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/sentiment_twitter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.932863 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.932863 shallowpavlov-0.0.1/deeppavlov/configs/cv/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/cv/cv_tfidf_autofaq.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.932863 shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/bpr_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.932863 shallowpavlov-0.0.1/deeppavlov/configs/embedder/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/embedder/bert_embedder.json
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/embedder/bert_sentence_embedder.json
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/embedder/tfidf_vectorizer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.936864 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_detection_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_detection_ru.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_extraction_en.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_extraction_ru.json
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_linking_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_linking_ru.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.936864 shallowpavlov-0.0.1/deeppavlov/configs/faq/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/faq/fasttext_avg_autofaq.json
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/faq/fasttext_tfidf_autofaq.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/faq/tfidf_autofaq.json
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/faq/tfidf_logreg_autofaq.json
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/faq/tfidf_logreg_en_faq.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.940864 shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/nq_croped_fid.json
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/nq_fid.json
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/tqa_fid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.940864 shallowpavlov-0.0.1/deeppavlov/configs/kbqa/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/kbqa/kbqa_cq_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/kbqa/kbqa_cq_ru.json
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/kbqa/wiki_parser.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.944864 shallowpavlov-0.0.1/deeppavlov/configs/ner/
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_collection3_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_conll2003_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_ontonotes_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_bert_probas.json
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.944864 shallowpavlov-0.0.1/deeppavlov/configs/odqa/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/odqa/en_odqa_bpr_croped_fid.json
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/odqa/en_odqa_infer_wiki.json
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.948864 shallowpavlov-0.0.1/deeppavlov/configs/paramsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/paramsearch/tfidf_logreg_autofaq_psearch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.948864 shallowpavlov-0.0.1/deeppavlov/configs/ranking/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ranking/rel_ranking_bert_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/ranking/rel_ranking_bert_ru.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.948864 shallowpavlov-0.0.1/deeppavlov/configs/regressors/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/regressors/translation_ranker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.948864 shallowpavlov-0.0.1/deeppavlov/configs/relation_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/relation_extraction/re_docred.json
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/relation_extraction/re_rured.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.952864 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.952864 shallowpavlov-0.0.1/deeppavlov/configs/sentence_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.956864 shallowpavlov-0.0.1/deeppavlov/configs/spelling_correction/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.956864 shallowpavlov-0.0.1/deeppavlov/configs/squad/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/squad/qa_multisberquad_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/squad/qa_squad2_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_ru_bert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.956864 shallowpavlov-0.0.1/deeppavlov/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.960865 shallowpavlov-0.0.1/deeppavlov/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/commands/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/commands/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.964865 shallowpavlov-0.0.1/deeppavlov/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/log_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/metrics_registry.json
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/metrics_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/params_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/prints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/registry.json
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/common/requirements_registry.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.964865 shallowpavlov-0.0.1/deeppavlov/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/data/data_fitting_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/data/data_learning_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/data/dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/data/simple_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.968865 shallowpavlov-0.0.1/deeppavlov/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/lr_scheduled_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/models/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.968865 shallowpavlov-0.0.1/deeppavlov/core/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/trainers/fit_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/trainers/nn_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/trainers/torch_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/core/trainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.972865 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/basic_classification_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/multitask_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/siamese_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/sqlite_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/squad_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_iterators/typos_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.980865 shallowpavlov-0.0.1/deeppavlov/dataset_readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/basic_classification_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/boolqa_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/conll2003_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/docred_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/faq_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/huggingface_dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/imdb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/line_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/odqa_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/paraphraser_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/rel_ranking_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/rured_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/sq_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/squad_dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/typos_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/dataset_readers/ubuntu_v2_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.984866 shallowpavlov-0.0.1/deeppavlov/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/elmo_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/fmeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/google_bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/log_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/mse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/record_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/roc_auc_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/metrics/squad_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.984866 shallowpavlov-0.0.1/deeppavlov/models/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.988866 shallowpavlov-0.0.1/deeppavlov/models/api_requester/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/api_requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/api_requester/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/api_requester/api_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.988866 shallowpavlov-0.0.1/deeppavlov/models/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/cos_sim_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/proba2labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/re_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/torch_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/torch_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/classifiers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.992866 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19171 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/biencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/bpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/logit_ranker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/pop_ranker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/tfidf_ranker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.996866 shallowpavlov-0.0.1/deeppavlov/models/embedders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/embedders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/embedders/abstract_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/embedders/fasttext_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/embedders/tfidf_weighted_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/embedders/transformers_embedder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.996866 shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/entity_detection_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28934 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/entity_linking.py
--rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/ner_chunker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.000866 shallowpavlov-0.0.1/deeppavlov/models/kbqa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/query_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/query_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/rel_ranking_infer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/sentence_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/template_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    32714 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/tree_to_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/type_define.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26135 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/kbqa/wiki_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.008867 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/ner_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/odqa_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/one_hotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/re_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/response_base_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/sentseg_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/squad_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/str_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/str_token_reverser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/str_utf8_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/preprocessors/transformers_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.008867 shallowpavlov-0.0.1/deeppavlov/models/ranking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/ranking/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.008867 shallowpavlov-0.0.1/deeppavlov/models/relation_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/relation_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/relation_extraction/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/relation_extraction/relation_extraction_bert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.008867 shallowpavlov-0.0.1/deeppavlov/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/sklearn/sklearn_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.008867 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.012867 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/brillmoore/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/brillmoore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/brillmoore/error_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.012867 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/electors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/electors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/electors/kenlm_elector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/electors/top1_elector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.012867 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33386 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    20586 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.016867 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/nltk_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/ru_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/spacy_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/split_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/tokenizers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.020867 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/fusion_in_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_bert_ranker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_generative_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_squad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.020867 shallowpavlov-0.0.1/deeppavlov/models/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/vectorizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/paramsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.028867 shallowpavlov-0.0.1/deeppavlov/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/datasets.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/en_core_web_sm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/fasttext.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/hdt.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/kenlm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/lxml.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/opt_einsum.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/rapidfuzz.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/ru_core_news_sm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/sacremoses.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/slovnet.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/sortedcontainers.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/torchcrf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/transformers.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/transformers_3.0.2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/udapi.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/requirements/whapi.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.028867 shallowpavlov-0.0.1/deeppavlov/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.028867 shallowpavlov-0.0.1/deeppavlov/utils/agent/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/agent/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/agent/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/agent/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.032868 shallowpavlov-0.0.1/deeppavlov/utils/connector/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/connector/dialog_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.032868 shallowpavlov-0.0.1/deeppavlov/utils/pip_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/pip_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/pip_wrapper/pip_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.032868 shallowpavlov-0.0.1/deeppavlov/utils/server/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/server/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.032868 shallowpavlov-0.0.1/deeppavlov/utils/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/settings/dialog_logger_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/settings/log_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/settings/server_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.036868 shallowpavlov-0.0.1/deeppavlov/utils/socket/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/socket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/utils/socket/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.036868 shallowpavlov-0.0.1/deeppavlov/vocabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/vocabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/vocabs/typos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/deeppavlov/vocabs/wiki_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:29:04.040868 shallowpavlov-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.036868 shallowpavlov-0.0.1/shallowpavlov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-17 15:29:03.000000 shallowpavlov-0.0.1/shallowpavlov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-05-17 15:29:03.000000 shallowpavlov-0.0.1/shallowpavlov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:29:03.000000 shallowpavlov-0.0.1/shallowpavlov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-17 15:29:03.000000 shallowpavlov-0.0.1/shallowpavlov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 15:29:03.000000 shallowpavlov-0.0.1/shallowpavlov.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.036868 shallowpavlov-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    33328 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/tests/test_quick_start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:03.916863 shallowpavlov-0.0.1/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:29:04.040868 shallowpavlov-0.0.1/utils/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/utils/prepare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/utils/prepare/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/utils/prepare/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-17 15:25:39.000000 shallowpavlov-0.0.1/utils/prepare/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.532681 shallowpavlov-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-10 21:52:53.532681 shallowpavlov-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.440678 shallowpavlov-1.0.0rc1/deeppavlov/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.440678 shallowpavlov-1.0.0rc1/deeppavlov/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.444679 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/boolqa_rubert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.448679 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/insults_kaggle_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/paraphraser_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/query_pr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_convers_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/sentiment_twitter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.448679 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.448679 shallowpavlov-1.0.0rc1/deeppavlov/configs/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/cv/cv_tfidf_autofaq.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.452679 shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/bpr_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.452679 shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/bert_embedder.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/bert_sentence_embedder.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/tfidf_vectorizer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.452679 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_detection_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_detection_ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_extraction_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_extraction_ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_linking_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_linking_ru.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.456679 shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/fasttext_avg_autofaq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/fasttext_tfidf_autofaq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/tfidf_autofaq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/tfidf_logreg_autofaq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/tfidf_logreg_en_faq.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.456679 shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/nq_croped_fid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/nq_fid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/tqa_fid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.456679 shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/kbqa_cq_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/kbqa_cq_ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/wiki_parser.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.460679 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_collection3_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_conll2003_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_ontonotes_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_bert_probas.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.460679 shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/en_odqa_bpr_croped_fid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/en_odqa_infer_wiki.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.460679 shallowpavlov-1.0.0rc1/deeppavlov/configs/paramsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/paramsearch/tfidf_logreg_autofaq_psearch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.464679 shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/rel_ranking_bert_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/rel_ranking_bert_ru.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.464679 shallowpavlov-1.0.0rc1/deeppavlov/configs/regressors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/regressors/translation_ranker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.464679 shallowpavlov-1.0.0rc1/deeppavlov/configs/relation_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/relation_extraction/re_docred.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/relation_extraction/re_rured.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.468679 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.468679 shallowpavlov-1.0.0rc1/deeppavlov/configs/sentence_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.468679 shallowpavlov-1.0.0rc1/deeppavlov/configs/spelling_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.468679 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/qa_multisberquad_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/qa_squad2_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_ru_bert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.468679 shallowpavlov-1.0.0rc1/deeppavlov/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.472679 shallowpavlov-1.0.0rc1/deeppavlov/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/commands/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/commands/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.472679 shallowpavlov-1.0.0rc1/deeppavlov/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/log_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/metrics_registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/metrics_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/params_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/common/requirements_registry.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.476679 shallowpavlov-1.0.0rc1/deeppavlov/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/data/data_fitting_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/data/data_learning_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/data/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/data/simple_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.476679 shallowpavlov-1.0.0rc1/deeppavlov/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/lr_scheduled_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/models/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.476679 shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/fit_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/nn_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/torch_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.480679 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/basic_classification_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/multitask_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/siamese_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/sqlite_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/squad_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/typos_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.484680 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/basic_classification_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/boolqa_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/conll2003_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/docred_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/faq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/huggingface_dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/imdb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/odqa_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/paraphraser_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/rel_ranking_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/rured_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/sq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/squad_dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/typos_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/ubuntu_v2_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.488680 shallowpavlov-1.0.0rc1/deeppavlov/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/elmo_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/fmeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/google_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/log_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/mse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/record_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/roc_auc_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/metrics/squad_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.492680 shallowpavlov-1.0.0rc1/deeppavlov/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.492680 shallowpavlov-1.0.0rc1/deeppavlov/models/api_requester/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/api_requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/api_requester/api_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/api_requester/api_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.492680 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/cos_sim_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/proba2labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/re_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/torch_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/torch_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.496680 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19171 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/biencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/bpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/logit_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/pop_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/tfidf_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.496680 shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/abstract_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/fasttext_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/tfidf_weighted_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/transformers_embedder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.496680 shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/entity_detection_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28934 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/entity_linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/ner_chunker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.500680 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/query_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/query_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/rel_ranking_infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/sentence_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/template_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32714 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/tree_to_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/type_define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26135 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/wiki_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/ner_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/odqa_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/one_hotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/re_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/response_base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/sentseg_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/squad_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/str_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/str_token_reverser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/str_utf8_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/transformers_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/ranking/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/relation_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/relation_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/relation_extraction/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/relation_extraction/relation_extraction_bert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/sklearn/sklearn_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/brillmoore/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/brillmoore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/brillmoore/error_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.508680 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/electors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/electors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/electors/kenlm_elector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/electors/top1_elector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.512680 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33386 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20586 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.512680 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/nltk_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/ru_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/split_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.516680 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/fusion_in_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_bert_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_generative_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_squad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.516680 shallowpavlov-1.0.0rc1/deeppavlov/models/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/vectorizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/paramsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.524680 shallowpavlov-1.0.0rc1/deeppavlov/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/datasets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/en_core_web_sm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/fasttext.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/hdt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/kenlm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/lxml.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/opt_einsum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/rapidfuzz.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/ru_core_news_sm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/sacremoses.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/slovnet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/sortedcontainers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/torchcrf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/transformers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/transformers_3.0.2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/udapi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/requirements/whapi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.524680 shallowpavlov-1.0.0rc1/deeppavlov/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.524680 shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.524680 shallowpavlov-1.0.0rc1/deeppavlov/utils/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/connector/dialog_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.524680 shallowpavlov-1.0.0rc1/deeppavlov/utils/pip_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/pip_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/pip_wrapper/pip_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.528680 shallowpavlov-1.0.0rc1/deeppavlov/utils/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/server/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.528680 shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/dialog_logger_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/log_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/server_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.528680 shallowpavlov-1.0.0rc1/deeppavlov/utils/socket/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/utils/socket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.528680 shallowpavlov-1.0.0rc1/deeppavlov/vocabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/vocabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/vocabs/typos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-10 21:49:25.000000 shallowpavlov-1.0.0rc1/deeppavlov/vocabs/wiki_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:52:53.532681 shallowpavlov-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.528680 shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-10 21:52:53.000000 shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-05-10 21:52:53.000000 shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:52:53.000000 shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 21:52:53.000000 shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 21:52:53.000000 shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.528680 shallowpavlov-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    33328 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/tests/test_quick_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.436679 shallowpavlov-1.0.0rc1/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:52:53.532681 shallowpavlov-1.0.0rc1/utils/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/utils/prepare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/utils/prepare/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/utils/prepare/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-10 21:49:26.000000 shallowpavlov-1.0.0rc1/utils/prepare/upload.py
```

### Comparing `shallowpavlov-0.0.1/LICENSE` & `shallowpavlov-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/PKG-INFO` & `shallowpavlov-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shallowpavlov
-Version: 0.0.1
+Version: 1.0.0rc1
 Summary: An open source library for building end-to-end dialog systems and training chatbots.
 Home-page: https://github.com/deepmipt/DeepPavlov
 Download-URL: https://github.com/deepmipt/DeepPavlov/archive/1.0.0rc1.tar.gz
 Author: Neural Networks and Deep Learning lab, MIPT
 Author-email: info@deeppavlov.ai
 License: Apache License, Version 2.0
 Keywords: NLP,NER,SQUAD,Intents,Chatbot
```

### Comparing `shallowpavlov-0.0.1/README.md` & `shallowpavlov-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/__init__.py` & `shallowpavlov-1.0.0rc1/deeppavlov/__init__.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/__init__.py` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/boolqa_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/boolqa_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/insults_kaggle_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/insults_kaggle_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/paraphraser_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/paraphraser_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/query_pr.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/query_pr.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_convers_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_convers_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/sentiment_twitter.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/sentiment_twitter.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/cv/cv_tfidf_autofaq.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/cv/cv_tfidf_autofaq.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/bpr_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/bpr_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/embedder/bert_embedder.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/bert_embedder.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/embedder/bert_sentence_embedder.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/bert_sentence_embedder.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/embedder/tfidf_vectorizer.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/embedder/tfidf_vectorizer.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_detection_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_detection_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_detection_ru.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_detection_ru.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_extraction_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_extraction_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_extraction_ru.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_extraction_ru.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_linking_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_linking_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/entity_extraction/entity_linking_ru.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/entity_extraction/entity_linking_ru.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/faq/fasttext_avg_autofaq.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/fasttext_avg_autofaq.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/faq/fasttext_tfidf_autofaq.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/fasttext_tfidf_autofaq.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/faq/tfidf_autofaq.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/tfidf_autofaq.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/faq/tfidf_logreg_autofaq.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/tfidf_logreg_autofaq.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/faq/tfidf_logreg_en_faq.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/faq/tfidf_logreg_en_faq.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/nq_croped_fid.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/nq_croped_fid.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980654761904763%*

 * *Differences: {"'chainer'": "{'pipe': {2: {'crop_len': 32}}}",*

 * * "'metadata'": "{'variables': {'MODEL_PATH': "*

 * *               "'{MODELS_PATH}/generative_qa/croped_fusion_in_decoder/natural_questions_32'}}"}*

```diff
@@ -36,15 +36,15 @@
                 "out": [
                     "target_ids"
                 ],
                 "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "torch_generative_qa_croped_fid",
-                "crop_len": 64,
+                "crop_len": 32,
                 "generate_max_length": 50,
                 "in": [
                     "input_ids",
                     "attention_mask"
                 ],
                 "in_y": [
                     "target_ids"
@@ -96,15 +96,15 @@
             }
         ],
         "variables": {
             "CONFIGS_PATH": "{DEEPPAVLOV_PATH}/configs",
             "DATASET_PATH": "{DOWNLOADS_PATH}/natural_questions",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/generative_qa/croped_fusion_in_decoder/natural_questions",
+            "MODEL_PATH": "{MODELS_PATH}/generative_qa/croped_fusion_in_decoder/natural_questions_32",
             "ROOT_PATH": "~/.deeppavlov",
             "TRANSFORMER": "t5-base"
         }
     },
     "train": {
         "batch_size": 8,
         "class_name": "torch_trainer",
```

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/nq_fid.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/nq_fid.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/generative_qa/tqa_fid.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/generative_qa/tqa_fid.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/kbqa/kbqa_cq_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/kbqa_cq_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/kbqa/kbqa_cq_ru.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/kbqa_cq_ru.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/kbqa/wiki_parser.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/kbqa/wiki_parser.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_collection3_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_collection3_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_conll2003_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_conll2003_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_ontonotes_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_ontonotes_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_bert_probas.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_bert_probas.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/odqa/en_odqa_bpr_croped_fid.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/en_odqa_bpr_croped_fid.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/odqa/en_odqa_infer_wiki.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/en_odqa_infer_wiki.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/paramsearch/tfidf_logreg_autofaq_psearch.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/paramsearch/tfidf_logreg_autofaq_psearch.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ranking/rel_ranking_bert_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/rel_ranking_bert_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/ranking/rel_ranking_bert_ru.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/ranking/rel_ranking_bert_ru.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/regressors/translation_ranker.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/regressors/translation_ranker.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/relation_extraction/re_docred.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/relation_extraction/re_docred.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/relation_extraction/re_rured.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/relation_extraction/re_rured.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/squad/qa_multisberquad_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/qa_multisberquad_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/squad/qa_squad2_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/qa_squad2_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_ru_bert.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_ru_bert.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json` & `shallowpavlov-1.0.0rc1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/commands/infer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/commands/infer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/commands/train.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/commands/train.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/commands/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/commands/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/aliases.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/aliases.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/base.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/base.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/chainer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/chainer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/cross_validation.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/cross_validation.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/errors.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/file.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/file.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/log.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/log.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/log_events.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/log_events.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/metrics_registry.json` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/metrics_registry.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/metrics_registry.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/metrics_registry.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/params.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/params.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/params_search.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/params_search.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/paths.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/paths.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/prints.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/prints.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/registry.json` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/registry.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/registry.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/registry.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/common/requirements_registry.json` & `shallowpavlov-1.0.0rc1/deeppavlov/core/common/requirements_registry.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/data/data_fitting_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/data/data_fitting_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/data/data_learning_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/data/data_learning_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/data/dataset_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/data/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/data/simple_vocab.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/data/simple_vocab.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/data/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/data/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/models/component.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/models/component.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/models/estimator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/models/estimator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/models/lr_scheduled_model.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/models/lr_scheduled_model.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/models/nn_model.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/models/nn_model.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/models/serializable.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/models/serializable.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/models/torch_model.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/models/torch_model.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/trainers/__init__.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/trainers/fit_trainer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/fit_trainer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/trainers/nn_trainer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/nn_trainer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/trainers/torch_trainer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/core/trainers/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/core/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/basic_classification_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/basic_classification_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/multitask_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/multitask_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/siamese_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/siamese_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/sqlite_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/sqlite_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/squad_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/squad_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_iterators/typos_iterator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_iterators/typos_iterator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/basic_classification_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/basic_classification_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/boolqa_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/boolqa_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/conll2003_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/conll2003_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/docred_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/docred_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/faq_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/faq_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/huggingface_dataset_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/huggingface_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/imdb_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/imdb_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/json_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/json_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/line_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/line_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/odqa_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/odqa_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/paraphraser_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/paraphraser_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/rel_ranking_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/rel_ranking_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/rured_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/rured_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/sq_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/sq_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/squad_dataset_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/squad_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/typos_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/typos_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/dataset_readers/ubuntu_v2_reader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/dataset_readers/ubuntu_v2_reader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/deep.py` & `shallowpavlov-1.0.0rc1/deeppavlov/deep.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/download.py` & `shallowpavlov-1.0.0rc1/deeppavlov/download.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/accuracy.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/bleu.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/correlation.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/correlation.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/elmo_metrics.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/elmo_metrics.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/fmeasure.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/fmeasure.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/google_bleu.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/google_bleu.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/log_loss.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/log_loss.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/mse.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/recall_at_k.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/record_metrics.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/record_metrics.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/roc_auc_score.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/roc_auc_score.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/metrics/squad_metrics.py` & `shallowpavlov-1.0.0rc1/deeppavlov/metrics/squad_metrics.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/__init__.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/api_requester/api_requester.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/api_requester/api_requester.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/api_requester/api_router.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/api_requester/api_router.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/classifiers/cos_sim_classifier.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/cos_sim_classifier.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/classifiers/proba2labels.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/proba2labels.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/classifiers/re_bert.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/re_bert.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/classifiers/torch_classification_model.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/torch_classification_model.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/classifiers/torch_nets.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/torch_nets.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/classifiers/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/biencoder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/biencoder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/bpr.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/bpr.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/logit_ranker.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/logit_ranker.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/pop_ranker.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/pop_ranker.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/tfidf_ranker.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/tfidf_ranker.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/doc_retrieval/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/doc_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/embedders/abstract_embedder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/abstract_embedder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/embedders/fasttext_embedder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/fasttext_embedder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/embedders/tfidf_weighted_embedder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/tfidf_weighted_embedder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/embedders/transformers_embedder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/embedders/transformers_embedder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/entity_detection_parser.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/entity_detection_parser.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/entity_linking.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/entity_linking.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/entity_extraction/ner_chunker.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/entity_extraction/ner_chunker.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/query_generator.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/query_generator.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/query_generator_base.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/query_generator_base.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/rel_ranking_infer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/rel_ranking_infer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/sentence_answer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/sentence_answer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/template_matcher.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/template_matcher.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/tree_to_sparql.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/tree_to_sparql.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/type_define.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/type_define.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/kbqa/wiki_parser.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/kbqa/wiki_parser.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/mask.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/mask.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/ner_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/ner_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/odqa_preprocessors.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/odqa_preprocessors.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/one_hotter.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/one_hotter.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/re_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/re_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/response_base_loader.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/response_base_loader.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/sanitizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/sanitizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/sentseg_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/sentseg_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/squad_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/squad_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/str_lower.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/str_lower.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/str_token_reverser.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/str_token_reverser.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/str_utf8_encoder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/str_utf8_encoder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/preprocessors/transformers_preprocessor.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/preprocessors/transformers_preprocessor.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/ranking/metrics.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/ranking/metrics.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/relation_extraction/losses.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/relation_extraction/losses.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/relation_extraction/relation_extraction_bert.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/relation_extraction/relation_extraction_bert.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/sklearn/sklearn_component.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/sklearn/sklearn_component.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/brillmoore/error_model.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/brillmoore/error_model.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/electors/kenlm_elector.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/electors/kenlm_elector.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/electors/top1_elector.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/electors/top1_elector.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/tokenizers/nltk_tokenizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/nltk_tokenizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/tokenizers/ru_tokenizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/ru_tokenizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/tokenizers/spacy_tokenizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/tokenizers/split_tokenizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/split_tokenizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/tokenizers/utils.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/tokenizers/utils.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/crf.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/crf.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/fusion_in_decoder.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/fusion_in_decoder.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_bert_ranker.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_bert_ranker.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_generative_qa.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_generative_qa.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_classifier.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_classifier.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/torch_bert/torch_transformers_squad.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/torch_bert/torch_transformers_squad.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py` & `shallowpavlov-1.0.0rc1/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/paramsearch.py` & `shallowpavlov-1.0.0rc1/deeppavlov/paramsearch.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/settings.py` & `shallowpavlov-1.0.0rc1/deeppavlov/settings.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/agent/messages.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/messages.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/agent/rabbitmq.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/agent/server.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/agent/server.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/connector/dialog_logger.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/connector/dialog_logger.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/pip_wrapper/pip_wrapper.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/pip_wrapper/pip_wrapper.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/server/metrics.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/server/metrics.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/server/server.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/server/server.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/settings/log_config.json` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/log_config.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/settings/server_config.json` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/settings/server_config.json`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/utils/socket/socket.py` & `shallowpavlov-1.0.0rc1/deeppavlov/utils/socket/socket.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/vocabs/typos.py` & `shallowpavlov-1.0.0rc1/deeppavlov/vocabs/typos.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/deeppavlov/vocabs/wiki_sqlite.py` & `shallowpavlov-1.0.0rc1/deeppavlov/vocabs/wiki_sqlite.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/setup.py` & `shallowpavlov-1.0.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return text
 
 
 if __name__ == '__main__':
     setup(
         name='shallowpavlov',
         packages=find_packages(exclude=('tests', 'docs', 'utils')),
-        version='0.0.1',
+        version=__version__,
         description=__description__,
         long_description=readme(),
         long_description_content_type='text/markdown',
         author=__author__,
         author_email=__email__,
         license=__license__,
         url='https://github.com/deepmipt/DeepPavlov',
```

### Comparing `shallowpavlov-0.0.1/shallowpavlov.egg-info/PKG-INFO` & `shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shallowpavlov
-Version: 0.0.1
+Version: 1.0.0rc1
 Summary: An open source library for building end-to-end dialog systems and training chatbots.
 Home-page: https://github.com/deepmipt/DeepPavlov
 Download-URL: https://github.com/deepmipt/DeepPavlov/archive/1.0.0rc1.tar.gz
 Author: Neural Networks and Deep Learning lab, MIPT
 Author-email: info@deeppavlov.ai
 License: Apache License, Version 2.0
 Keywords: NLP,NER,SQUAD,Intents,Chatbot
```

### Comparing `shallowpavlov-0.0.1/shallowpavlov.egg-info/SOURCES.txt` & `shallowpavlov-1.0.0rc1/shallowpavlov.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/tests/test_quick_start.py` & `shallowpavlov-1.0.0rc1/tests/test_quick_start.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/utils/prepare/hashes.py` & `shallowpavlov-1.0.0rc1/utils/prepare/hashes.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/utils/prepare/registry.py` & `shallowpavlov-1.0.0rc1/utils/prepare/registry.py`

 * *Files identical despite different names*

### Comparing `shallowpavlov-0.0.1/utils/prepare/upload.py` & `shallowpavlov-1.0.0rc1/utils/prepare/upload.py`

 * *Files identical despite different names*

