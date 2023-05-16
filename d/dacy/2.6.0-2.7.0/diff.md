# Comparing `tmp/dacy-2.6.0.tar.gz` & `tmp/dacy-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dacy-2.6.0.tar", last modified: Tue Apr 11 03:31:37 2023, max compression
+gzip compressed data, was "dacy-2.7.0.tar", last modified: Tue May 16 22:00:23 2023, max compression
```

## Comparing `dacy-2.6.0.tar` & `dacy-2.7.0.tar`

### file list

```diff
@@ -1,210 +1,171 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.334472 dacy-2.6.0/
--rw-r--r--   0 root         (0) root         (0)      461 2023-04-11 03:31:25.000000 dacy-2.6.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      711 2023-04-11 03:31:25.000000 dacy-2.6.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.294472 dacy-2.6.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.298472 dacy-2.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      713 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.298472 dacy-2.6.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     3050 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/mypy.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1068 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     2994 2023-04-11 03:31:25.000000 dacy-2.6.0/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 03:31:25.000000 dacy-2.6.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-11 03:31:25.000000 dacy-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     9467 2023-04-11 03:31:26.000000 dacy-2.6.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5532 2023-04-11 03:31:25.000000 dacy-2.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2372 2023-04-11 03:31:25.000000 dacy-2.6.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 03:31:25.000000 dacy-2.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    21373 2023-04-11 03:31:37.334472 dacy-2.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7076 2023-04-11 03:31:25.000000 dacy-2.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 03:31:25.000000 dacy-2.6.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.302472 dacy-2.6.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.310472 dacy-2.6.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)  1426134 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
--rw-r--r--   0 root         (0) root         (0)    52158 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/asent_analysis.png
--rw-r--r--   0 root         (0) root         (0)    15586 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/asent_prediction.png
--rw-r--r--   0 root         (0) root         (0)    63171 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/dep_parse.png
--rw-r--r--   0 root         (0) root         (0)    61244 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/dep_robustness.png
--rw-r--r--   0 root         (0) root         (0)    15406 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   185775 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/icon_black_text.png
--rw-r--r--   0 root         (0) root         (0)   189414 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   154866 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/icon_no_title.png
--rw-r--r--   0 root         (0) root         (0)    12272 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/ner.png
--rw-r--r--   0 root         (0) root         (0)   103739 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/ner_robustness.png
--rw-r--r--   0 root         (0) root         (0)    77390 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/perf.png
--rw-r--r--   0 root         (0) root         (0)    65393 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/perf_l.png
--rw-r--r--   0 root         (0) root         (0)    69095 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/pos_robustness.png
--rw-r--r--   0 root         (0) root         (0)   661625 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/table_dep.html
--rw-r--r--   0 root         (0) root         (0)   666232 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/table_ent.html
--rw-r--r--   0 root         (0) root         (0)   664139 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/table_perf.html
--rw-r--r--   0 root         (0) root         (0)   662541 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/_static/table_pos.html
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/adv_tutorials.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.310472 dacy-2.6.0/docs/api/
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/api/dacy.datasets.rst
--rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/api/dacy.download.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/api/dacy.score.rst
--rw-r--r--   0 root         (0) root         (0)     3850 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/faq.md
--rw-r--r--   0 root         (0) root         (0)     2295 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      343 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/installation.md
--rw-r--r--   0 root         (0) root         (0)     5118 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     4201 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/performance.general.rst
--rw-r--r--   0 root         (0) root         (0)     6139 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/performance.robustness.rst
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/performance.rst
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.310472 dacy-2.6.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    30779 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/tutorials/basic.ipynb
--rw-r--r--   0 root         (0) root         (0)     5660 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/tutorials/hate-speech.ipynb
--rw-r--r--   0 root         (0) root         (0)    38507 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/tutorials/robustness.ipynb
--rw-r--r--   0 root         (0) root         (0)    21450 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/tutorials/sentiment.ipynb
--rw-r--r--   0 root         (0) root         (0)   108717 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/tutorials/textdescriptives.ipynb
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-11 03:31:25.000000 dacy-2.6.0/docs/tutorials.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.290472 dacy-2.6.0/papers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.314472 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.314472 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
--rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
--rw-r--r--   0 root         (0) root         (0)  2323089 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
--rw-r--r--   0 root         (0) root         (0)     2714 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
--rw-r--r--   0 root         (0) root         (0)     2848 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-11 03:31:25.000000 dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
--rw-r--r--   0 root         (0) root         (0)     4807 2023-04-11 03:31:26.000000 dacy-2.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 03:31:37.334472 dacy-2.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.290472 dacy-2.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.318472 dacy-2.6.0/src/dacy/
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.318472 dacy-2.6.0/src/dacy/datasets/
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/constants.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/dane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.318472 dacy-2.6.0/src/dacy/datasets/lookup_tables/
--rw-r--r--   0 root         (0) root         (0)      578 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/lookup_tables/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/lookup_tables/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126210 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/lookup_tables/names.csv
--rw-r--r--   0 root         (0) root         (0)     4546 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/datasets/names.py
--rw-r--r--   0 root         (0) root         (0)     4146 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.318472 dacy-2.6.0/src/dacy/hate_speech/
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/hate_speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3874 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/hate_speech/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.318472 dacy-2.6.0/src/dacy/ner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/ner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/ner/fine_grained.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/ner/wrapped_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.322472 dacy-2.6.0/src/dacy/score/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/score/input_length.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/score/score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.322472 dacy-2.6.0/src/dacy/sentiment/
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/sentiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5408 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/sentiment/wrapped_models.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-11 03:31:25.000000 dacy-2.6.0/src/dacy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.318472 dacy-2.6.0/src/dacy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21373 2023-04-11 03:31:37.000000 dacy-2.6.0/src/dacy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6392 2023-04-11 03:31:37.000000 dacy-2.6.0/src/dacy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:31:37.000000 dacy-2.6.0/src/dacy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      261 2023-04-11 03:31:37.000000 dacy-2.6.0/src/dacy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      659 2023-04-11 03:31:37.000000 dacy-2.6.0/src/dacy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 03:31:37.000000 dacy-2.6.0/src/dacy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8076 2023-04-11 03:31:25.000000 dacy-2.6.0/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.322472 dacy-2.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_datasets.py
--rw-r--r--   0 root         (0) root         (0)      360 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_hate_speech.py
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_ner.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_score.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_sentiment.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-11 03:31:25.000000 dacy-2.6.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.322472 dacy-2.6.0/training/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.322472 dacy-2.6.0/training/ner_fine_grained/
--rw-r--r--   0 root         (0) root         (0)     5832 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.322472 dacy-2.6.0/training/ner_fine_grained/configs/
--rw-r--r--   0 root         (0) root         (0)     3260 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     2811 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     2819 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/configs/config_small.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/environment_setup.sh
--rw-r--r--   0 root         (0) root         (0)      829 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)    12576 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/project.yml
--rw-r--r--   0 root         (0) root         (0)      259 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/server_setup.sh
--rw-r--r--   0 root         (0) root         (0)     3428 2023-04-11 03:31:25.000000 dacy-2.6.0/training/ner_fine_grained/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)     3495 2023-04-11 03:31:25.000000 dacy-2.6.0/training/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.326472 dacy-2.6.0/training/v0.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.326472 dacy-2.6.0/training/v0.0.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4458 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/configs/config_-l-ctra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4449 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/configs/config_conv_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4467 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/configs/config_electra_small.cfg
--rw-r--r--   0 root         (0) root         (0)     4432 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4440 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/configs/config_medium.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.326472 dacy-2.6.0/training/v0.0.0/img/
--rw-r--r--   0 root         (0) root         (0)    40449 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/img/perf_training.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.326472 dacy-2.6.0/training/v0.0.0/metrics/
--rw-r--r--   0 root         (0) root         (0)     3582 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/metrics/dane_-l-ctra_cased.json
--rw-r--r--   0 root         (0) root         (0)     3594 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/metrics/dane_-l-ctra_uncased.json
--rw-r--r--   0 root         (0) root         (0)     3591 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/metrics/dane_conv_small.json
--rw-r--r--   0 root         (0) root         (0)     3638 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/metrics/dane_electra.json
--rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/metrics/dane_large.json
--rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/metrics/dane_medium.json
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/orth_variants.json
--rw-r--r--   0 root         (0) root         (0)     9596 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/project.yml
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.0.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.326472 dacy-2.6.0/training/v0.1.0/
--rw-r--r--   0 root         (0) root         (0)     6617 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.330472 dacy-2.6.0/training/v0.1.0/configs/
--rw-r--r--   0 root         (0) root         (0)     4633 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4635 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/configs/config_small.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.330472 dacy-2.6.0/training/v0.1.0/metrics/
--rw-r--r--   0 root         (0) root         (0)   237018 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236140 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   237616 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5506 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5502 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5595 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5454 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5629 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15843 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.0/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.330472 dacy-2.6.0/training/v0.1.1/
--rw-r--r--   0 root         (0) root         (0)     7458 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.334472 dacy-2.6.0/training/v0.1.1/configs/
--rw-r--r--   0 root         (0) root         (0)     4619 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/configs/config_large.cfg
--rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/configs/config_medium.cfg
--rw-r--r--   0 root         (0) root         (0)     4621 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/configs/config_small.cfg
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/danish_augmenter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:37.334472 dacy-2.6.0/training/v0.1.1/metrics/
--rw-r--r--   0 root         (0) root         (0)   236308 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_augmented_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   236675 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_augmented_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)   238715 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_augmented_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5488 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_best_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5522 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_best_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5592 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_best_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_last_dacy_large_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5485 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_last_dacy_medium_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)     5601 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/metrics/dane_last_dacy_small_trf-0.1.0.json
--rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/project.yml
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/update_meta_json.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 03:31:25.000000 dacy-2.6.0/training/v0.1.1/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.881512 dacy-2.7.0/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-05-16 22:00:10.000000 dacy-2.7.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      711 2023-05-16 22:00:10.000000 dacy-2.7.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.841512 dacy-2.7.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.841512 dacy-2.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      713 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.841512 dacy-2.7.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      918 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/mypy.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-05-16 22:00:10.000000 dacy-2.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-05-16 22:00:10.000000 dacy-2.7.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-16 22:00:10.000000 dacy-2.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    11135 2023-05-16 22:00:12.000000 dacy-2.7.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-05-16 22:00:10.000000 dacy-2.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-05-16 22:00:10.000000 dacy-2.7.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-16 22:00:10.000000 dacy-2.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20005 2023-05-16 22:00:23.881512 dacy-2.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-05-16 22:00:10.000000 dacy-2.7.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-16 22:00:10.000000 dacy-2.7.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.845512 dacy-2.7.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.853512 dacy-2.7.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)  1426134 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png
+-rw-r--r--   0 root         (0) root         (0)    52158 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/asent_analysis.png
+-rw-r--r--   0 root         (0) root         (0)    15586 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/asent_prediction.png
+-rw-r--r--   0 root         (0) root         (0)    63171 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/dep_parse.png
+-rw-r--r--   0 root         (0) root         (0)    61244 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/dep_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   185775 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/icon_black_text.png
+-rw-r--r--   0 root         (0) root         (0)   189414 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   154866 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/icon_no_title.png
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/ner.png
+-rw-r--r--   0 root         (0) root         (0)   103739 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/ner_robustness.png
+-rw-r--r--   0 root         (0) root         (0)    77390 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/perf.png
+-rw-r--r--   0 root         (0) root         (0)    65393 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/perf_l.png
+-rw-r--r--   0 root         (0) root         (0)    69095 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/pos_robustness.png
+-rw-r--r--   0 root         (0) root         (0)   661625 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/table_dep.html
+-rw-r--r--   0 root         (0) root         (0)   666232 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/table_ent.html
+-rw-r--r--   0 root         (0) root         (0)   664139 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/table_perf.html
+-rw-r--r--   0 root         (0) root         (0)   662541 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/_static/table_pos.html
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/adv_tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.857512 dacy-2.7.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/api/dacy.datasets.rst
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/api/dacy.download.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/api/dacy.score.rst
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/faq.md
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)     7674 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/performance.general.rst
+-rw-r--r--   0 root         (0) root         (0)     6139 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/performance.robustness.rst
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/performance.rst
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.857512 dacy-2.7.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    36112 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/tutorials/basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/tutorials/hate-speech.ipynb
+-rw-r--r--   0 root         (0) root         (0)    38507 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/tutorials/robustness.ipynb
+-rw-r--r--   0 root         (0) root         (0)    21450 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/tutorials/sentiment.ipynb
+-rw-r--r--   0 root         (0) root         (0)   108717 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/tutorials/textdescriptives.ipynb
+-rw-r--r--   0 root         (0) root         (0)      598 2023-05-16 22:00:10.000000 dacy-2.7.0/docs/tutorials.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.833512 dacy-2.7.0/papers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.861512 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.865512 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py
+-rw-r--r--   0 root         (0) root         (0)  2323089 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-05-16 22:00:10.000000 dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-05-16 22:00:12.000000 dacy-2.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 22:00:23.881512 dacy-2.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.837512 dacy-2.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.865512 dacy-2.7.0/src/dacy/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.869512 dacy-2.7.0/src/dacy/datasets/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/dane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.869512 dacy-2.7.0/src/dacy/datasets/lookup_tables/
+-rw-r--r--   0 root         (0) root         (0)      578 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/lookup_tables/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/lookup_tables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126210 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/lookup_tables/names.csv
+-rw-r--r--   0 root         (0) root         (0)     4546 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/datasets/names.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.869512 dacy-2.7.0/src/dacy/hate_speech/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/hate_speech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/hate_speech/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.869512 dacy-2.7.0/src/dacy/ner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/ner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/ner/fine_grained.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/ner/wrapped_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.869512 dacy-2.7.0/src/dacy/score/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/score/input_length.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/score/score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.869512 dacy-2.7.0/src/dacy/sentiment/
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/sentiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5408 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/sentiment/wrapped_models.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-05-16 22:00:10.000000 dacy-2.7.0/src/dacy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.865512 dacy-2.7.0/src/dacy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20005 2023-05-16 22:00:23.000000 dacy-2.7.0/src/dacy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-05-16 22:00:23.000000 dacy-2.7.0/src/dacy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 22:00:23.000000 dacy-2.7.0/src/dacy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      261 2023-05-16 22:00:23.000000 dacy-2.7.0/src/dacy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-16 22:00:23.000000 dacy-2.7.0/src/dacy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-16 22:00:23.000000 dacy-2.7.0/src/dacy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8076 2023-05-16 22:00:10.000000 dacy-2.7.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.873512 dacy-2.7.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_datasets.py
+-rw-r--r--   0 root         (0) root         (0)      360 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_hate_speech.py
+-rw-r--r--   0 root         (0) root         (0)      373 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_score.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-16 22:00:10.000000 dacy-2.7.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.873512 dacy-2.7.0/training/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.873512 dacy-2.7.0/training/main/
+-rw-r--r--   0 root         (0) root         (0)     7525 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.877512 dacy-2.7.0/training/main/configs/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/assemble.cfg
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/assemble_coref.cfg
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/cluster.cfg
+-rw-r--r--   0 root         (0) root         (0)     6302 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/config.cfg
+-rw-r--r--   0 root         (0) root         (0)     6409 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/config_small.cfg
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/further_train.cfg
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/configs/span_resolver.cfg
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.877512 dacy-2.7.0/training/main/scripts/
+-rw-r--r--   0 root         (0) root         (0)    10379 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/add_readme_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    10824 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/combine.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/create_ddt_compatible_splits_for_cdt.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/create_kb.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/custom_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/evaluate_coref.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/prep_span_data.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/scripts/update_description.py
+-rw-r--r--   0 root         (0) root         (0)    27478 2023-05-16 22:00:10.000000 dacy-2.7.0/training/main/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.881512 dacy-2.7.0/training/ner_fine_grained/
+-rw-r--r--   0 root         (0) root         (0)     5832 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 22:00:23.881512 dacy-2.7.0/training/ner_fine_grained/configs/
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/configs/config_large.cfg
+-rw-r--r--   0 root         (0) root         (0)     2811 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/configs/config_medium.cfg
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/configs/config_small.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/environment_setup.sh
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)    12576 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/project.yml
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/server_setup.sh
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-05-16 22:00:10.000000 dacy-2.7.0/training/ner_fine_grained/update_meta_json.py
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-16 22:00:10.000000 dacy-2.7.0/training/readme.md
```

### Comparing `dacy-2.6.0/.cruft.json` & `dacy-2.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/ISSUE_TEMPLATE/01_bugs.md` & `dacy-2.7.0/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/ISSUE_TEMPLATE/config.yml` & `dacy-2.7.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/dependabot.yml` & `dacy-2.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/check_for_rej.yml` & `dacy-2.7.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/cruft.yml` & `dacy-2.7.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/dependabot_automerge.yml` & `dacy-2.7.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/documentation.yml` & `dacy-2.7.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/mypy.yml` & `dacy-2.7.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/pre-commit.yml` & `dacy-2.7.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/release.yml` & `dacy-2.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/stalebot.yml` & `dacy-2.7.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/.github/workflows/tests.yml` & `dacy-2.7.0/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         if: steps.cache_venv.outputs.cache-hit != 'true'
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         shell: bash
         run: |
-          python -m venv .venv
+          python3 -m venv .venv
           if [ "${{ matrix.os }}" == "windows-latest" ]; then
             source .venv/Scripts/activate
           else
             source .venv/bin/activate
           fi
-          python -m pip install --upgrade pip
+          python3 -m pip install --upgrade pip
           pip install -e .[tests]
 
       - name: Run and write pytest
         shell: bash
         run: |
           if [ "${{ matrix.os }}" == "windows-latest" ]; then
             source .venv/Scripts/activate
```

### Comparing `dacy-2.6.0/.gitignore` & `dacy-2.7.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -130,20 +130,24 @@
 
 # training
 data
 *.conllu
 *.spacy
 corpus/*
 training/*/training/*
+training/*/assets/*
+training/*/corpus/*
 training/*/wandb/*
 training/*/packages/*
 training/*/hub/*
+training/*/metrics/*
 
 # Removing data
 data
+*.zip
 
 # project specific
 *.lock
 
 # mac
 .DS_store
 
@@ -158,8 +162,8 @@
 .Rhistory
 
 # Documentation
 _build/*
 
 # tutorials:
 tutorials/BenchmarkFairness.ipynb
-tutorials/*.py
+tutorials/*.py
```

### Comparing `dacy-2.6.0/.pre-commit-config.yaml` & `dacy-2.7.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 repos:
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.265
     hooks:
       - id: ruff
         args:
           [
             "--extend-select",
             "F401",
             "--extend-select",
             "F841",
             "--fix",
             "--exit-non-zero-on-fix",
           ]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
 
   - repo: https://github.com/repo-helper/pyproject-parser
-    rev: v0.7.0
+    rev: v0.9.0b2
     hooks:
       - id: check-pyproject
```

### Comparing `dacy-2.6.0/CHANGELOG.md` & `dacy-2.7.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.7.0 (2023-05-16)
+### Feature
+* Added version 0.2.0 models ([`5d4fc7d`](https://github.com/centre-for-humanities-computing/DaCy/commit/5d4fc7de635050423d9282795b67446259425bef))
+
+### Fix
+* Ensure that model download is handled correctly ([`2b48f4d`](https://github.com/centre-for-humanities-computing/DaCy/commit/2b48f4dacbd2fd06598421595d858677f1829826))
+* Removed unused package ([`c1f8681`](https://github.com/centre-for-humanities-computing/DaCy/commit/c1f86811748465413319dfc4f49483e3f913053c))
+
+### Documentation
+* Updated readme ([`0ce3862`](https://github.com/centre-for-humanities-computing/DaCy/commit/0ce3862170afe6f3442a39cd0bd8676917bb2e80))
+* Fixed news listing ([`9ea806d`](https://github.com/centre-for-humanities-computing/DaCy/commit/9ea806dbaae221d10f7f4ba5870eb3bdc29b412c))
+* Fix rendering of links ([`a7a9d96`](https://github.com/centre-for-humanities-computing/DaCy/commit/a7a9d964aa7be8f6fb77621dedaaca46b7691cf4))
+* Added coref and NED ([`4d20f71`](https://github.com/centre-for-humanities-computing/DaCy/commit/4d20f7167fa91fe557d71b32f6be8818e4ebb1d3))
+* Added news ([`de76d12`](https://github.com/centre-for-humanities-computing/DaCy/commit/de76d129da43176b13b0e8305b24e4b211554ab6))
+* Added missing links to readme ([`6ea8d4b`](https://github.com/centre-for-humanities-computing/DaCy/commit/6ea8d4b6308d9721e4be2de7a98515a7872d7431))
+* Hide downloads from output ([`efeae63`](https://github.com/centre-for-humanities-computing/DaCy/commit/efeae639a5f8e44ab18a18d3ff2262826c251427))
+* Update docs to hide downloads ([`0ee0a51`](https://github.com/centre-for-humanities-computing/DaCy/commit/0ee0a516b6faebf729eba8265e1f39a0de7c31e2))
+
 ## v2.6.0 (2023-04-11)
 ### Feature
 * Added fine-grained ner component ([`4977687`](https://github.com/centre-for-humanities-computing/DaCy/commit/497768716f6b47f2addf5565f43ac1e0605a8f3d))
 
 ### Fix
 * Updates pandas version ([`09c438a`](https://github.com/centre-for-humanities-computing/DaCy/commit/09c438a47a4dcb20c2476a6c131c17edda20092b))
 * Improve UI for the fine-grained NER model ([`1c009c2`](https://github.com/centre-for-humanities-computing/DaCy/commit/1c009c2d093fdb3dc470ad2bcc607ded4dd49652))
```

### Comparing `dacy-2.6.0/CODE_OF_CONDUCT.md` & `dacy-2.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/CONTRIBUTING.md` & `dacy-2.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/LICENSE` & `dacy-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/PKG-INFO` & `dacy-2.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.6.0
+Version: 2.7.0
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
 Author: Lasse Hansen, Emil Jessen
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,16 +235,14 @@
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![documentation](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
 
-[![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
-
 [pypi status]: https://pypi.org/project/dacy/
 [documentation]: https://centre-for-humanities-computing.github.io/dacy/
 [tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 
 <!-- start short-description -->
@@ -263,70 +261,56 @@
 To use the model you first have to download either the small, medium, or large model. To see a list of all available models:
 
 ```python
 import dacy
 for model in dacy.models():
     print(model)
 # ...
-# da_dacy_small_trf-0.1.0
-# da_dacy_medium_trf-0.1.0
-# da_dacy_large_trf-0.1.0
+# da_dacy_small_trf-0.2.0
+# da_dacy_medium_trf-0.2.0
+# da_dacy_large_trf-0.2.0
 ```
 
 To download and load a model simply execute:
 ```python
-nlp = dacy.load("da_dacy_medium_trf-0.1.0")
-# or equivalently
+nlp = dacy.load("da_dacy_medium_trf-0.2.0")
+# or equivalently (always loads the latest version)
 nlp = dacy.load("medium")
 ```
 
-Which will download the model to the `.dacy` directory in your home directory. 
-
-
-To download the model to a specific directory:
-```python
-dacy.download_model("da_dacy_medium_trf-0.1.0", your_save_path)
-nlp = dacy.load_model("da_dacy_medium_trf-0.1.0", your_save_path)
-```
-
-
 To see more examples, see the [documentation].
 
 # 📖 Documentation
 
 | Documentation              |                                                                                             |
 | -------------------------- | ------------------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use DaCy and its features.                                |
 | 🦾 **[Performance]**        | A detailed description of the performance of DaCy and comparison with similar Danish models |
-| 😎 **[Demo]**               | A simple Streamlit demo to try out the augmenters.                                          |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                                 |
 | 🎛 **[API References]**     | The detailed reference for DaCy's API. Including function documentation                     |
 | 🙋 **[FAQ]**                | Frequently asked questions                                                                  |
 
 
 [Installation]: https://centre-for-humanities-computing.github.io/DaCy/installation.html
 [Getting started]: https://centre-for-humanities-computing.github.io/DaCy/using_dacy.html
 [api references]: https://centre-for-humanities-computing.github.io/DaCy/
-[Demo]: https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.
 [News and changelog]: https://centre-for-humanities-computing.github.io/DaCy/news.html
 [FAQ]: https://centre-for-humanities-computing.github.io/DaCy/faq.html
 [Performance]: https://centre-for-humanities-computing.github.io/DaCy/performance.html
 
 
 
 
 
 <br /> 
 
 <details>
   <summary> Training and reproduction </summary>
 
-The folder `training` contains a range of folders with a SpaCy project for each model version. This allows for the reproduction of the results. The SpaCy project folders also include the evaluation metrics and scripts for acquiring the required data. For more information, please see the readme's in the respective training folders.
-
-The folders include v0.0.0, v0.1.0, v0.1.1 and ner_fine_grained. The former 3 refer to the training of the main DaCy models, trained and evaluated on the DaNE dataset, whereas the latter contains the project for the fine-grained NER models trained on the [DANSK dataset](https://huggingface.co/datasets/chcaa/DANSK). Please refer to the available README's located within each training folder for more information.
+The folder `training` contains a range of folders with a SpaCy project for each model version. This allows for the reproduction of the results.
 
 Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
 
 </details>
 
 <br /> 
 
@@ -346,7 +330,9 @@
 [Documentation]: https://centre-for-humanities-computing.github.io/dacy/index.html
 [Installation]: https://centre-for-humanities-computing.github.io/dacy/installation.html
 [Tutorials]: https://centre-for-humanities-computing.github.io/dacy/tutorials.html
 [API Reference]: https://centre-for-humanities-computing.github.io/dacy/references.html
 [FAQ]: https://centre-for-humanities-computing.github.io/dacy/faq.html
 [github issue tracker]: https://github.com/centre-for-humanities-computing/dacy/issues
 [github discussions]: https://github.com/centre-for-humanities-computing/dacy/discussions
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/project/dacy/
```

### Comparing `dacy-2.6.0/README.md` & `dacy-2.7.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![documentation](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
 
-[![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
-
 [pypi status]: https://pypi.org/project/dacy/
 [documentation]: https://centre-for-humanities-computing.github.io/dacy/
 [tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 
 <!-- start short-description -->
@@ -32,70 +30,56 @@
 To use the model you first have to download either the small, medium, or large model. To see a list of all available models:
 
 ```python
 import dacy
 for model in dacy.models():
     print(model)
 # ...
-# da_dacy_small_trf-0.1.0
-# da_dacy_medium_trf-0.1.0
-# da_dacy_large_trf-0.1.0
+# da_dacy_small_trf-0.2.0
+# da_dacy_medium_trf-0.2.0
+# da_dacy_large_trf-0.2.0
 ```
 
 To download and load a model simply execute:
 ```python
-nlp = dacy.load("da_dacy_medium_trf-0.1.0")
-# or equivalently
+nlp = dacy.load("da_dacy_medium_trf-0.2.0")
+# or equivalently (always loads the latest version)
 nlp = dacy.load("medium")
 ```
 
-Which will download the model to the `.dacy` directory in your home directory. 
-
-
-To download the model to a specific directory:
-```python
-dacy.download_model("da_dacy_medium_trf-0.1.0", your_save_path)
-nlp = dacy.load_model("da_dacy_medium_trf-0.1.0", your_save_path)
-```
-
-
 To see more examples, see the [documentation].
 
 # 📖 Documentation
 
 | Documentation              |                                                                                             |
 | -------------------------- | ------------------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use DaCy and its features.                                |
 | 🦾 **[Performance]**        | A detailed description of the performance of DaCy and comparison with similar Danish models |
-| 😎 **[Demo]**               | A simple Streamlit demo to try out the augmenters.                                          |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                                 |
 | 🎛 **[API References]**     | The detailed reference for DaCy's API. Including function documentation                     |
 | 🙋 **[FAQ]**                | Frequently asked questions                                                                  |
 
 
 [Installation]: https://centre-for-humanities-computing.github.io/DaCy/installation.html
 [Getting started]: https://centre-for-humanities-computing.github.io/DaCy/using_dacy.html
 [api references]: https://centre-for-humanities-computing.github.io/DaCy/
-[Demo]: https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.
 [News and changelog]: https://centre-for-humanities-computing.github.io/DaCy/news.html
 [FAQ]: https://centre-for-humanities-computing.github.io/DaCy/faq.html
 [Performance]: https://centre-for-humanities-computing.github.io/DaCy/performance.html
 
 
 
 
 
 <br /> 
 
 <details>
   <summary> Training and reproduction </summary>
 
-The folder `training` contains a range of folders with a SpaCy project for each model version. This allows for the reproduction of the results. The SpaCy project folders also include the evaluation metrics and scripts for acquiring the required data. For more information, please see the readme's in the respective training folders.
-
-The folders include v0.0.0, v0.1.0, v0.1.1 and ner_fine_grained. The former 3 refer to the training of the main DaCy models, trained and evaluated on the DaNE dataset, whereas the latter contains the project for the fine-grained NER models trained on the [DANSK dataset](https://huggingface.co/datasets/chcaa/DANSK). Please refer to the available README's located within each training folder for more information.
+The folder `training` contains a range of folders with a SpaCy project for each model version. This allows for the reproduction of the results.
 
 Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
 
 </details>
 
 <br /> 
 
@@ -115,7 +99,9 @@
 [Documentation]: https://centre-for-humanities-computing.github.io/dacy/index.html
 [Installation]: https://centre-for-humanities-computing.github.io/dacy/installation.html
 [Tutorials]: https://centre-for-humanities-computing.github.io/dacy/tutorials.html
 [API Reference]: https://centre-for-humanities-computing.github.io/dacy/references.html
 [FAQ]: https://centre-for-humanities-computing.github.io/dacy/faq.html
 [github issue tracker]: https://github.com/centre-for-humanities-computing/dacy/issues
 [github discussions]: https://github.com/centre-for-humanities-computing/dacy/discussions
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/project/dacy/
```

#### html2text {}

```diff
@@ -3,70 +3,54 @@
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status] [![pip
 downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/
 dacy/) [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi
 status] [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 [black] [![documentation](https://github.com/centre-for-humanities-computing/
 dacy/actions/workflows/documentation.yml/badge.svg)][documentation] [![Tests]
 (https://github.com/centre-for-humanities-computing/dacy/actions/workflows/
-tests.yml/badge.svg)][tests] [![Demo](https://img.shields.io/badge/Try%20the-
-Demo-important)](https://huggingface.co/chcaa/
-da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
-[pypi status]: https://pypi.org/project/dacy/ [documentation]: https://centre-
-for-humanities-computing.github.io/dacy/ [tests]: https://github.com/centre-
-for-humanities-computing/dacy/actions?workflow=Tests [black]: https://
-github.com/psf/black  DaCy is a Danish natural language preprocessing framework
-made with SpaCy. Its largest pipeline has achieved State-of-the-Art performance
-on Named entity recognition, part-of-speech tagging and dependency parsing for
-Danish. Feel free to try out the [demo](https://huggingface.co/chcaa/
+tests.yml/badge.svg)][tests] [pypi status]: https://pypi.org/project/dacy/
+[documentation]: https://centre-for-humanities-computing.github.io/dacy/
+[tests]: https://github.com/centre-for-humanities-computing/dacy/
+actions?workflow=Tests [black]: https://github.com/psf/black  DaCy is a Danish
+natural language preprocessing framework made with SpaCy. Its largest pipeline
+has achieved State-of-the-Art performance on Named entity recognition, part-of-
+speech tagging and dependency parsing for Danish. Feel free to try out the
+[demo](https://huggingface.co/chcaa/
 da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.).
 This repository contains material for using DaCy, reproducing the results and
 guides on usage of the package. Furthermore, it also contains behavioural tests
 for biases and robustness of Danish NLP pipelines.  ## ð§ Installation You
 can install `dacy` via [pip] from [PyPI]: ```bash pip install dacy ``` ##
 ð©âð» Usage To use the model you first have to download either the small,
 medium, or large model. To see a list of all available models: ```python import
-dacy for model in dacy.models(): print(model) # ... # da_dacy_small_trf-0.1.0 #
-da_dacy_medium_trf-0.1.0 # da_dacy_large_trf-0.1.0 ``` To download and load a
-model simply execute: ```python nlp = dacy.load("da_dacy_medium_trf-0.1.0") #
-or equivalently nlp = dacy.load("medium") ``` Which will download the model to
-the `.dacy` directory in your home directory. To download the model to a
-specific directory: ```python dacy.download_model("da_dacy_medium_trf-0.1.0",
-your_save_path) nlp = dacy.load_model("da_dacy_medium_trf-0.1.0",
-your_save_path) ``` To see more examples, see the [documentation]. # ð
-Documentation | Documentation | | | -------------------------- | --------------
------------------------------------------------------------------------------ |
-| ð **[Getting started]** | Guides and instructions on how to use DaCy and
-its features. | | ð¦¾ **[Performance]** | A detailed description of the
-performance of DaCy and comparison with similar Danish models | | ð **
-[Demo]** | A simple Streamlit demo to try out the augmenters. | | ð° **[News
+dacy for model in dacy.models(): print(model) # ... # da_dacy_small_trf-0.2.0 #
+da_dacy_medium_trf-0.2.0 # da_dacy_large_trf-0.2.0 ``` To download and load a
+model simply execute: ```python nlp = dacy.load("da_dacy_medium_trf-0.2.0") #
+or equivalently (always loads the latest version) nlp = dacy.load("medium") ```
+To see more examples, see the [documentation]. # ð Documentation |
+Documentation | | | -------------------------- | ------------------------------
+------------------------------------------------------------- | | ð **
+[Getting started]** | Guides and instructions on how to use DaCy and its
+features. | | ð¦¾ **[Performance]** | A detailed description of the
+performance of DaCy and comparison with similar Danish models | | ð° **[News
 and changelog]** | New additions, changes and version history. | | ð **[API
 References]** | The detailed reference for DaCy's API. Including function
 documentation | | ð **[FAQ]** | Frequently asked questions | [Installation]:
 https://centre-for-humanities-computing.github.io/DaCy/installation.html
 [Getting started]: https://centre-for-humanities-computing.github.io/DaCy/
 using_dacy.html [api references]: https://centre-for-humanities-
-computing.github.io/DaCy/ [Demo]: https://huggingface.co/chcaa/
-da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.
-[News and changelog]: https://centre-for-humanities-computing.github.io/DaCy/
-news.html [FAQ]: https://centre-for-humanities-computing.github.io/DaCy/
-faq.html [Performance]: https://centre-for-humanities-computing.github.io/DaCy/
-performance.html
+computing.github.io/DaCy/ [News and changelog]: https://centre-for-humanities-
+computing.github.io/DaCy/news.html [FAQ]: https://centre-for-humanities-
+computing.github.io/DaCy/faq.html [Performance]: https://centre-for-humanities-
+computing.github.io/DaCy/performance.html
   Training and reproduction  The folder `training` contains a range of folders
 with a SpaCy project for each model version. This allows for the reproduction
-of the results. The SpaCy project folders also include the evaluation metrics
-and scripts for acquiring the required data. For more information, please see
-the readme's in the respective training folders. The folders include v0.0.0,
-v0.1.0, v0.1.1 and ner_fine_grained. The former 3 refer to the training of the
-main DaCy models, trained and evaluated on the DaNE dataset, whereas the latter
-contains the project for the fine-grained NER models trained on the [DANSK
-dataset](https://huggingface.co/datasets/chcaa/DANSK). Please refer to the
-available README's located within each training folder for more information.
-Want to learn more about how DaCy initially came to be, check out this [blog
-post](https://www.centre-for-humanities-computing.com/post/new-fast-and-
-efficient-state-of-the-art-in-danish-nlp/).
+of the results. Want to learn more about how DaCy initially came to be, check
+out this [blog post](https://www.centre-for-humanities-computing.com/post/new-
+fast-and-efficient-state-of-the-art-in-danish-nlp/).
 # ð¬ Where to ask questions To ask report issues or request features, please
 use the [GitHub Issue Tracker](https://github.com/centre-for-humanities-
 computing/DaCy/issues). Questions related to SpaCy are kindly referred to the
 SpaCy GitHub or forum. Otherwise, please use the discussion Forums. | Type | |
 | ------------------------------ | ---------------------- | | ð **FAQ** |
 [FAQ] | | ð¨ **Bug Reports** | [GitHub Issue Tracker] | | ð **Feature
 Requests & Ideas** | [GitHub Issue Tracker] | | ð©âð» **Usage Questions**
@@ -74,8 +58,9 @@
 [Documentation]: https://centre-for-humanities-computing.github.io/dacy/
 index.html [Installation]: https://centre-for-humanities-computing.github.io/
 dacy/installation.html [Tutorials]: https://centre-for-humanities-
 computing.github.io/dacy/tutorials.html [API Reference]: https://centre-for-
 humanities-computing.github.io/dacy/references.html [FAQ]: https://centre-for-
 humanities-computing.github.io/dacy/faq.html [github issue tracker]: https://
 github.com/centre-for-humanities-computing/dacy/issues [github discussions]:
-https://github.com/centre-for-humanities-computing/dacy/discussions
+https://github.com/centre-for-humanities-computing/dacy/discussions [pip]:
+https://pypi.org/project/pip/ [PyPI]: https://pypi.org/project/dacy/
```

### Comparing `dacy-2.6.0/citation.cff` & `dacy-2.7.0/citation.cff`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png` & `dacy-2.7.0/docs/_static/DALL-E_2022-07-27_A_minimalistic_2d_depiction_of_a_danish_cream_pastry.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/asent_analysis.png` & `dacy-2.7.0/docs/_static/asent_analysis.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/asent_prediction.png` & `dacy-2.7.0/docs/_static/asent_prediction.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/dep_parse.png` & `dacy-2.7.0/docs/_static/dep_parse.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/dep_robustness.png` & `dacy-2.7.0/docs/_static/dep_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/favicon.ico` & `dacy-2.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/icon.png` & `dacy-2.7.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/icon_black_text.png` & `dacy-2.7.0/docs/_static/icon_black_text.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/icon_dark.png` & `dacy-2.7.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/icon_no_title.png` & `dacy-2.7.0/docs/_static/icon_no_title.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/ner.png` & `dacy-2.7.0/docs/_static/ner.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/ner_robustness.png` & `dacy-2.7.0/docs/_static/ner_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/perf.png` & `dacy-2.7.0/docs/_static/perf.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/perf_l.png` & `dacy-2.7.0/docs/_static/perf_l.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/pos_robustness.png` & `dacy-2.7.0/docs/_static/pos_robustness.png`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/table_dep.html` & `dacy-2.7.0/docs/_static/table_dep.html`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/table_ent.html` & `dacy-2.7.0/docs/_static/table_ent.html`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/table_perf.html` & `dacy-2.7.0/docs/_static/table_perf.html`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/_static/table_pos.html` & `dacy-2.7.0/docs/_static/table_pos.html`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/conf.py` & `dacy-2.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/faq.md` & `dacy-2.7.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/index.md` & `dacy-2.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/performance.general.rst` & `dacy-2.7.0/docs/performance.general.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/performance.robustness.rst` & `dacy-2.7.0/docs/performance.robustness.rst`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/tutorials/basic.ipynb` & `dacy-2.7.0/docs/tutorials/basic.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9663743268289708%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': {insert: [(0, 'da_dacy_small_trf-0.2.0\\n'), (1, "*

 * *            "'da_dacy_medium_trf-0.2.0\\n'), (2, 'da_dacy_large_trf-0.2.0\\n')], delete: [2, 1, "*

 * *            "0]}}}}, 3: {'outputs': [], 'source': {insert: [(0, '# get the latest medium "*

 * *            "model:\\n')], delete: [0]}}, 5: {'outputs': [], 'source': ['doc = "*

 * *            'nlp("DaCy-pakken er en hurtig og effektiv pipeline til dansk '*

 * *            'sprogprocessering.")\']}, 6: {\'source\': {insert: [(1, "Nam […]*

```diff
@@ -28,17 +28,17 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "da_dacy_small_trf-0.1.0\n",
-                        "da_dacy_medium_trf-0.1.0\n",
-                        "da_dacy_large_trf-0.1.0\n",
+                        "da_dacy_small_trf-0.2.0\n",
+                        "da_dacy_medium_trf-0.2.0\n",
+                        "da_dacy_large_trf-0.2.0\n",
                         "small\n",
                         "medium\n",
                         "large\n",
                         "da_dacy_small_ner_fine_grained-0.1.0\n",
                         "da_dacy_medium_ner_fine_grained-0.1.0\n",
                         "da_dacy_large_ner_fine_grained-0.1.0\n"
                     ]
@@ -69,30 +69,17 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "tags": [
                     "hide-output"
                 ]
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:887: UserWarning: [W095] Model 'da_dacy_medium_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.5.1). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
-                        "  warnings.warn(warn_msg)\n",
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/util.py:887: UserWarning: [W095] Model 'da_dacy_small_trf' (0.1.0) was trained with spaCy v3.1 and may not be 100% compatible with the current version (3.5.1). If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spaCy version. For more details and available updates, run: python -m spacy validate\n",
-                        "  warnings.warn(warn_msg)\n",
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy_transformers/pipeline_component.py:402: UserWarning: Automatically converting a transformer component from spacy-transformers v1.0 to v1.1+. If you see errors or degraded performance, download a newer compatible model or retrain your custom model with the current spacy-transformers version. For more details and available updates, run: python -m spacy validate\n",
-                        "  warnings.warn(warn_msg)\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "# get the latest small model:\n",
+                "# get the latest medium model:\n",
                 "nlp = dacy.load(\"small\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -108,50 +95,39 @@
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/au561649/.virtualenvs/dacy/lib/python3.10/site-packages/spacy/pipeline/attributeruler.py:150: UserWarning: [W036] The component 'matcher' does not have any patterns defined.\n",
-                        "  matches = self.matcher(doc, allow_missing=True, as_spans=False)\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "doc = nlp(\n",
-                "    \"DaCy er en hurtig og effektiv pipeline til dansk sprogprocessering.\"\n",
-                ")"
+                "doc = nlp(\"DaCy-pakken er en hurtig og effektiv pipeline til dansk sprogprocessering.\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Named Entity Recognition\n",
-                "Named Entity Recognition (NER)is the task of identifying named entities in a text. A named entity is a \u201creal-world object\u201d that's assigned a name - for example, a person, a country, a product or a book title. \n",
+                "Named Entity Recognition (NER) is the task of identifying named entities in a text. A named entity is a \u201creal-world object\u201d that's assigned a name - for example, a person, a country, a product or a book title. \n",
                 "DaCy can recognize organizations, persons, and location, as well as other miscellaneous entities."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "DaCy : PER\n",
+                        "DaCy-pakken : MISC\n",
                         "dansk : MISC\n"
                     ]
                 }
             ],
             "source": [
                 "for entity in doc.ents:\n",
                 "    print(entity, \":\", entity.label_)"
@@ -171,21 +147,25 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<span class=\"tex2jax_ignore\"><div class=\"entities\" style=\"line-height: 2.5; direction: ltr\">\n",
                             "<mark class=\"entity\" style=\"background: #ddd; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 1; border-radius: 0.35em;\">\n",
-                            "    DaCy\n",
-                            "    <span style=\"font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; vertical-align: middle; margin-left: 0.5rem\">PER</span>\n",
+                            "    DaCy-pakken\n",
+                            "    <span style=\"font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; vertical-align: middle; margin-left: 0.5rem\">MISC\n",
+                            " <a style=\"text-decoration: none; color: inherit; font-weight: normal\" href=\"#\">NIL</a>\n",
+                            "</span>\n",
                             "</mark>\n",
                             " er en hurtig og effektiv pipeline til \n",
                             "<mark class=\"entity\" style=\"background: #ddd; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 1; border-radius: 0.35em;\">\n",
                             "    dansk\n",
-                            "    <span style=\"font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; vertical-align: middle; margin-left: 0.5rem\">MISC</span>\n",
+                            "    <span style=\"font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; vertical-align: middle; margin-left: 0.5rem\">MISC\n",
+                            " <a style=\"text-decoration: none; color: inherit; font-weight: normal\" href=\"#\">Q35</a>\n",
+                            "</span>\n",
                             "</mark>\n",
                             " sprogprocessering.</div></span>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
@@ -209,14 +189,44 @@
                 "\n",
                 "To do this you can simply load the model using:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<spacy_wrap.pipeline_component_tok_clf.TokenClassificationTransformer at 0x1758db040>"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# load the small dacy model excluding the NER component\n",
+                "nlp = dacy.load(\"small\", exclude=[\"ner\"])\n",
+                "# or use an empty spacy model if you only want to do NER\n",
+                "# nlp = spacy.blank(\"da\")\n",
+                "\n",
+                "# add the ner component from the state-of-the-art model\n",
+                "nlp.add_pipe(\"dacy/ner\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<span class=\"tex2jax_ignore\"><div class=\"entities\" style=\"line-height: 2.5; direction: ltr\">Denne \n",
                             "<mark class=\"entity\" style=\"background: #ddd; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 1; border-radius: 0.35em;\">\n",
@@ -240,42 +250,130 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "# load the small dacy model excluding the NER component\n",
-                "nlp = dacy.load(\"small\", exclude=[\"ner\"])\n",
-                "# or use an empty spacy model if you only want to do NER\n",
-                "# nlp = spacy.blank(\"da\")\n",
-                "\n",
-                "# add the ner component from the state-of-the-art model\n",
-                "nlp.add_pipe(\"dacy/ner\")\n",
-                "\n",
                 "doc = nlp(\"Denne NER model er tr\u00e6net af Dan fra Alexandra Instituttet\")\n",
                 "\n",
                 "displacy.render(doc, style=\"ent\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "```{warn}\n",
+                "```{warning}\n",
                 "Note that this will add an additonal model to your pipeline, which will slow down the inference speed.\n",
                 "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Named Entity Linking\n",
+                "As you probably already saw the named entities are annotated with a unique identifier. This is because DaCy also supports named entity linking.\n",
+                "\n",
+                "[Named entity linking](https://en.wikipedia.org/wiki/Entity_linking) is the task of linking a named entity to a knowledge base. This is done by assigning a unique identifier to each entity. This allows us to link entities to other entities and extract information from the knowledge base. For example, we can link the entity \"Barack Obama\" to the Wikipedia or wikidata page about Barack Obama. Named entity linking is also known as named entity disambiguation, though this term could also refer to the task of distinguishing between entities with the same name without linking to a knowledge base.\n",
+                "\n",
+                "```{admonition} Beta feature\n",
+                "Named entity linking is currently in beta and is not yet fully tested. If you find any bugs please report them on [github](https://github.com/centre-for-humanities-computing/DaCy/issues).\n",
+                "We are working on expanding the knowledge-base as well as correcting the annotations, which currently annotates unknown persons using the QID for the correspondig name. For instance in the sentence *Rutechef Ivan Madsen: \"Jeg ved ikke hvorfor...* the name *Ivan Madsen* is annotated using two QID's Q830350 (Ivan, male name) and Q16876242 (Madsen, family name), which we believe is incorrect as the person is not referring to the last name *Madsen*, but rather the person with the full name *Ivan Madsen*.\n",
+                "The knowledge is also currently limited and thus while the links you do obtain are often correct the model will often not be able to link all entities to the knowledge base.\n",
+                "```\n",
+                "\n",
+                "In DaCy the `small`, `medium`, and `large` model slhave a named entity linking component. This component uses a neural entity linking to match the entity to a specifc entity in the knowledge base. The knowledge base DaCy uses is currently a combination of Danish and English Wikidata."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<span class=\"tex2jax_ignore\"><div class=\"entities\" style=\"line-height: 2.5; direction: ltr\">\n",
+                            "<mark class=\"entity\" style=\"background: #ff9561; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 1; border-radius: 0.35em;\">\n",
+                            "    Danmarks\n",
+                            "    <span style=\"font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; vertical-align: middle; margin-left: 0.5rem\">LOC\n",
+                            " <a style=\"text-decoration: none; color: inherit; font-weight: normal\" href=\"#\">Q35</a>\n",
+                            "</span>\n",
+                            "</mark>\n",
+                            " dronning bor i \n",
+                            "<mark class=\"entity\" style=\"background: #ff9561; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 1; border-radius: 0.35em;\">\n",
+                            "    K\u00f8benhavn\n",
+                            "    <span style=\"font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; vertical-align: middle; margin-left: 0.5rem\">LOC\n",
+                            " <a style=\"text-decoration: none; color: inherit; font-weight: normal\" href=\"#\">Q1748</a>\n",
+                            "</span>\n",
+                            "</mark>\n",
+                            "</div></span>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Danmarks : Q35\n",
+                        "country in Northern Europe\n",
+                        "nordeurop\u00e6isk land\n",
+                        " \n",
+                        "K\u00f8benhavn : Q1748\n",
+                        "capital city of Denmark\n",
+                        "Danmarks hovedstad\n",
+                        " \n"
+                    ]
+                }
+            ],
+            "source": [
+                "from wikidata.client import Client\n",
+                "\n",
+                "nlp = dacy.load(\"small\")\n",
+                "text = \"Danmarks dronning bor i K\u00f8benhavn\"\n",
+                "\n",
+                "doc = nlp(text)\n",
+                "\n",
+                "displacy.render(doc, style=\"ent\")\n",
+                "\n",
+                "\n",
+                "client = Client() # start wikidata client\n",
+                "for entity in doc.ents:\n",
+                "    print(entity, \":\", entity.kb_id_)\n",
+                "\n",
+                "    # print the short description derived from wikidata\n",
+                "    wikidata_entry  = client.get(entity.kb_id_, load=True)\n",
+                "    print(wikidata_entry.description.get(\"en\"))\n",
+                "    print(wikidata_entry.description.get(\"da\"))\n",
+                "    print(\" \")\n",
+                "        \n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "You can even do more things e.g. extract the information from the knowledge base such as images, associated wikipedia article and so on."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Fine-grained NER\n",
                 "\n",
                 "DaCy also features models with a more fine-grained Named Entity Recognition component.\n",
                 "This has been trained on the [DANSK](https://huggingface.co/datasets/chcaa/DANSK).\n",
                 "This allows for the detection of 18 classes - namely the following Named Entities:\n",
                 "\n",
                 "|  Tag        |             Description                                         |\n",
@@ -305,45 +403,45 @@
                 "| CARDINAL | Numerals that do no fall under another type |\n",
                 "\n",
                 "The fine-grained NER component may be utilized in an existing pipeline in the following fashion:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 9,
             "metadata": {
                 "tags": [
                     "hide-output"
                 ]
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<spacy.pipeline.ner.EntityRecognizer at 0x29cc06ab0>"
+                            "<spacy.pipeline.ner.EntityRecognizer at 0x177f79d90>"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# load the small dacy model excluding the NER component\n",
                 "nlp = dacy.load(\"small\", exclude=[\"ner\"])\n",
                 "\n",
                 "# add the ner component from the state-of-the-art fine-grained model\n",
                 "nlp.add_pipe(\"dacy/ner-fine-grained\", config={\"size\": \"small\"})\n",
-                "# or if you only want to do NER\n",
+                "# or if you only want to do just NER\n",
                 "# nlp = dacy.load(\"da_dacy_small_ner_fine_grained-0.1.0\")\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<span class=\"tex2jax_ignore\"><div class=\"entities\" style=\"line-height: 2.5; direction: ltr\">Denne model samt \n",
                             "<mark class=\"entity\" style=\"background: #e4e7d2; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 1; border-radius: 0.35em;\">\n",
@@ -390,51 +488,52 @@
                 "[Part-of-speech tagging](https://en.wikipedia.org/wiki/Part-of-speech_tagging) (POS) is the task of assigning a part of speech to each word in a text. The part of speech is the grammatical role of a word in a sentence. For example, the word \u201crun\u201d is a verb, and the word \u201cbook\u201d is a noun. \n",
                 "\n",
                 "After tokenization, DaCy can parse and tag a given Doc. This is where the trained pipeline and its statistical models come in, which enable spaCy to make predictions of which tag or label most likely applies in this context. A trained component includes data that is produced by showing a system enough examples for it to make predictions that generalize across the language \u2013 for example, a word following \u201cthe\u201d in English is most likely a noun."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Token POS-tag\n",
                         "Denne:\t DET\n",
                         "model:\t NOUN\n",
                         "samt:\t CCONJ\n",
                         "3:\t NUM\n",
                         "andre:\t PRON\n",
                         "blev:\t AUX\n",
                         "tr\u00e6net:\t VERB\n",
-                        "d.:\t DET\n",
+                        "d.:\t ADV\n",
                         "7.:\t ADJ\n",
                         "marts:\t NOUN\n",
                         "af:\t ADP\n",
                         "Center:\t NOUN\n",
                         "for:\t ADP\n",
                         "Humantities:\t PROPN\n",
-                        "Computing:\t X\n",
+                        "Computing:\t PROPN\n",
                         "i:\t ADP\n",
                         "Aarhus:\t PROPN\n",
                         "kommune:\t NOUN\n"
                     ]
                 }
             ],
             "source": [
                 "print(\"Token POS-tag\")\n",
                 "for token in doc:\n",
                 "    print(f\"{token}:\\t {token.pos_}\")\n",
                 "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```{seealso}\n",
                 "For more on Part-of-speech tagging see SpaCy's [documentation](https://spacy.io/usage/linguistic-features#pos-tagging).\n",
                 "````\n"
             ]
@@ -456,21 +555,21 @@
                 "```{seealso}\n",
                 "For more on Dependency parsing see SpaCy's [documentation](https://spacy.io/usage/linguistic-features#dependency-parse).\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<span class=\"tex2jax_ignore\"><svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" xml:lang=\"da\" id=\"f6f16117a7124226b425ab278fbb8fb2-0\" class=\"displacy\" width=\"1450\" height=\"487.0\" direction=\"ltr\" style=\"max-width: none; height: 487.0px; color: #000000; background: #ffffff; font-family: Arial; direction: ltr\">\n",
+                            "<span class=\"tex2jax_ignore\"><svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" xml:lang=\"da\" id=\"66d5b791ef05478889e96bb1fb3441cb-0\" class=\"displacy\" width=\"1450\" height=\"487.0\" direction=\"ltr\" style=\"max-width: none; height: 487.0px; color: #000000; background: #ffffff; font-family: Arial; direction: ltr\">\n",
                             "<text class=\"displacy-token\" fill=\"currentColor\" text-anchor=\"middle\" y=\"397.0\">\n",
                             "    <tspan class=\"displacy-word\" fill=\"currentColor\" x=\"50\">DaCy</tspan>\n",
                             "    <tspan class=\"displacy-tag\" dy=\"2em\" fill=\"currentColor\" x=\"50\">PROPN</tspan>\n",
                             "</text>\n",
                             "\n",
                             "<text class=\"displacy-token\" fill=\"currentColor\" text-anchor=\"middle\" y=\"397.0\">\n",
                             "    <tspan class=\"displacy-word\" fill=\"currentColor\" x=\"225\">er</tspan>\n",
@@ -504,65 +603,65 @@
                             "\n",
                             "<text class=\"displacy-token\" fill=\"currentColor\" text-anchor=\"middle\" y=\"397.0\">\n",
                             "    <tspan class=\"displacy-word\" fill=\"currentColor\" x=\"1275\">fritekst.</tspan>\n",
                             "    <tspan class=\"displacy-tag\" dy=\"2em\" fill=\"currentColor\" x=\"1275\">NOUN</tspan>\n",
                             "</text>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-0\" stroke-width=\"2px\" d=\"M70,352.0 C70,2.0 750.0,2.0 750.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-0\" stroke-width=\"2px\" d=\"M70,352.0 C70,2.0 750.0,2.0 750.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-0\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">nsubj</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-0\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">nsubj</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M70,354.0 L62,342.0 78,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-1\" stroke-width=\"2px\" d=\"M245,352.0 C245,89.5 745.0,89.5 745.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-1\" stroke-width=\"2px\" d=\"M245,352.0 C245,89.5 745.0,89.5 745.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-1\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">cop</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-1\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">cop</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M245,354.0 L237,342.0 253,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-2\" stroke-width=\"2px\" d=\"M420,352.0 C420,177.0 740.0,177.0 740.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-2\" stroke-width=\"2px\" d=\"M420,352.0 C420,177.0 740.0,177.0 740.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-2\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">det</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-2\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">det</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M420,354.0 L412,342.0 428,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-3\" stroke-width=\"2px\" d=\"M595,352.0 C595,264.5 735.0,264.5 735.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-3\" stroke-width=\"2px\" d=\"M595,352.0 C595,264.5 735.0,264.5 735.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-3\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">amod</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-3\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">amod</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M595,354.0 L587,342.0 603,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-4\" stroke-width=\"2px\" d=\"M945,352.0 C945,177.0 1265.0,177.0 1265.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-4\" stroke-width=\"2px\" d=\"M945,352.0 C945,177.0 1265.0,177.0 1265.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-4\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">case</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-4\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">case</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M945,354.0 L937,342.0 953,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-5\" stroke-width=\"2px\" d=\"M1120,352.0 C1120,264.5 1260.0,264.5 1260.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-5\" stroke-width=\"2px\" d=\"M1120,352.0 C1120,264.5 1260.0,264.5 1260.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-5\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">amod</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-5\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">amod</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M1120,354.0 L1112,342.0 1128,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "\n",
                             "<g class=\"displacy-arrow\">\n",
-                            "    <path class=\"displacy-arc\" id=\"arrow-f6f16117a7124226b425ab278fbb8fb2-0-6\" stroke-width=\"2px\" d=\"M770,352.0 C770,89.5 1270.0,89.5 1270.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
+                            "    <path class=\"displacy-arc\" id=\"arrow-66d5b791ef05478889e96bb1fb3441cb-0-6\" stroke-width=\"2px\" d=\"M770,352.0 C770,89.5 1270.0,89.5 1270.0,352.0\" fill=\"none\" stroke=\"currentColor\"/>\n",
                             "    <text dy=\"1.25em\" style=\"font-size: 0.8em; letter-spacing: 1px\">\n",
-                            "        <textPath xlink:href=\"#arrow-f6f16117a7124226b425ab278fbb8fb2-0-6\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">nmod</textPath>\n",
+                            "        <textPath xlink:href=\"#arrow-66d5b791ef05478889e96bb1fb3441cb-0-6\" class=\"displacy-label\" startOffset=\"50%\" side=\"left\" fill=\"currentColor\" text-anchor=\"middle\">nmod</textPath>\n",
                             "    </text>\n",
                             "    <path class=\"displacy-arrowhead\" d=\"M1270.0,354.0 L1278.0,342.0 1262.0,342.0\" fill=\"currentColor\"/>\n",
                             "</g>\n",
                             "</svg></span>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
@@ -586,15 +685,15 @@
             "source": [
                 "# Sentence Segmentation\n",
                 "Sentence segmentation is the task of splitting a text into sentences. In DaCy this is done using the dependency parser. This makes it very accurate and allows for the detection of sentences that are not separated by a punctuations."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "S\u00e6tnings segmentering er en vigtig del af sprogprocessering\n",
@@ -618,15 +717,15 @@
                 "[Noun chunks](https://en.wikipedia.org/wiki/Noun_phrase) are \"base noun phrases\" \u2013 flat phrases that have a noun as their head. For example, \"the big yellow taxi\" and \"the quick brown fox\" are noun chunks. Noun chunks are \"noun-like\" words, such as a noun, a pronoun, a proper noun, or a noun phrase, that function as the head of a noun phrase.\n",
                 "\n",
                 "Noun chunks are for example used for information extraction, and for finding subjects and objects of verbs."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "DaCy\n",
@@ -658,15 +757,15 @@
                 "[Lemmatization](https://en.wikipedia.org/wiki/Lemmatisation) is the task of grouping together the inflected forms of a word so they can be analysed as a single item. For example, the verb \u201cto run\u201d has the base form \u201crun\u201d, and the verb \u201cran\u201d has the base form \u201crun\u201d.\n",
                 "\n",
                 "Lemmatization is for example used for text normalization before training a machine learning model to reduce the number of unique tokens in the training data."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Normalisering Normalisering\n",
@@ -683,14 +782,65 @@
             ],
             "source": [
                 "doc = nlp(\"Normalisering af tekst kan v\u00e6re en god id\u00e9.\")\n",
                 "\n",
                 "for token in doc:\n",
                 "    print(token, token.lemma_)"
             ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Coreference Resolution"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "[Coreference resolution](https://en.wikipedia.org/wiki/Coreference) is the task of finding all expressions that refer to the same entity in a text. For example, in the sentence \u201cThe dog chased the ball because it was shiny\u201d, \u201cit\u201d is referring to the \u201cball\u201d.\n",
+                "\n",
+                "\n",
+                "Coreference resolution is for example used for question answering, summarization, conversational agents/chatbots and information extraction where such resolved references can lead to a better semantic representation.\n",
+                "\n",
+                "```{admonition} Beta feature\n",
+                "Coreference resolution is currently an experimental feature from spaCy. This is thus only a beta feature in DaCy. We are currently working on improving the performance of the model.\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Coreference clusters:\n",
+                        "{'coref_clusters_1': [minkavler Henning Christensen, han, han, hans]}\n"
+                    ]
+                }
+            ],
+            "source": [
+                "text = \"Den 4. november 2020 fik minkavler Henning Christensen og hele familien et chok. Efter et pressem\u00f8de, fik han at vide at alle mink i Danmark skulle aflives. Dermed fik han fjernet hans livsgrundlag\"\n",
+                "doc = nlp(text)\n",
+                "print(\"Coreference clusters:\")\n",
+                "print(doc.spans)\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "dacy",
             "language": "python",
             "name": "python3"
```

### Comparing `dacy-2.6.0/docs/tutorials/hate-speech.ipynb` & `dacy-2.7.0/docs/tutorials/hate-speech.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/tutorials/robustness.ipynb` & `dacy-2.7.0/docs/tutorials/robustness.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/tutorials/sentiment.ipynb` & `dacy-2.7.0/docs/tutorials/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/tutorials/textdescriptives.ipynb` & `dacy-2.7.0/docs/tutorials/textdescriptives.ipynb`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/docs/tutorials.md` & `dacy-2.7.0/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_daluke.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_danlp.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_flair.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_nerda.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_polyglot.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/apply_fns/apply_fn_utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/augmentation_robustness.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/dacy_paper_replication.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/readme.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/requirement.txt`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd` & `dacy-2.7.0/papers/DaCy-A-Unified-Framework-for-Danish-NLP/robustness.Rmd`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/pyproject.toml` & `dacy-2.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dacy"
-version = "2.6.0"
+version = "2.7.0"
 description = "A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish"
 authors = [
   {name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}, 
   {name = "Lasse Hansen"},
   {name = "Emil Jessen"}
 ]
 
@@ -31,51 +31,53 @@
     "nlp",
     "danish",
     "spacy-universe",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "spacy-wrap>=1.4.1,<1.5.0",
-    "spacy>=3.2.0,<3.6.0",
+    "spacy-experimental >= 0.6.2",
+    "spacy[transformers]>=3.2.0,<3.6.0",
     "pandas>=1.0.0,<2.0.0",
     "wasabi>=0.8.2,<0.11.0",
     "tqdm>=4.42.1,<4.66.0",
-    "sentencepiece>=0.1.96,<0.2.0",
 ]
 
 
 [project.urls]
 homepage = "https://centre-for-humanities-computing.github.io/DaCy/"
 documentation = "https://centre-for-humanities-computing.github.io/DaCy/"
 repository = "https://github.com/centre-for-humanities-computing/DaCy"
 [project.license]
 file = "LICENSE"
 name = "Apache License 2.0"
 [project.optional-dependencies]
 dev = [
   "cruft",
   "mypy",  
-  "pre-commit==2.20.0,<3.2.2",
-  "ruff==0.0.261", # important that these match the pre-commit hooks
+  "pre-commit==3.3.1",
+  "ruff==0.0.267", # important that these match the pre-commit hooks
   "black[jupyter]==23.3.0", # important that these match the pre-commit hooks
 ]
 tests = [
   "pytest>=7.1.2,<7.4.0",
   "pytest-cov>=3.0.0,<3.1.0",
-  "pytest-xdist>=3.0.0,<3.3.0",
+  "pytest-xdist>=3.0.0,<3.4.0",
   "pytest-instafail>=0.4.2,<0.6.0",
 ]
 docs = [
-    "sphinx>=5.3.0,<5.4.0",
+    "sphinx>=5.3.0,<7.1.0",
     "furo>=2022.12.7,< 2022.12.8",  # theme
-    "sphinx-copybutton>=0.5.1,<0.5.2",
-    "sphinxext-opengraph>=0.7.3,<0.8.2",
-    "sphinx_design>=0.3.0,<0.3.1",
+    "sphinx-copybutton>=0.5.1,<0.5.3",
+    "sphinxext-opengraph>=0.7.3,<0.8.3",
+    "sphinx_design>=0.3.0,<0.4.2",
     "sphinx_togglebutton>=0.2.3,<0.4.0",
     "myst-nb>=0.6.0,<1.17.0",  # for rendering notebooks
+    # for named entity linking
+    "wikidata>=0.7.0",
     # for tutorials
     "jupyter>=1.0.0,<1.1.0",
     # sentiment analysis
     "asent>=0.4.2,<0.8.0",
     "augmenty>=1.0.2,<1.4.0",
     # for the textdescriptives tutorial
     "textdescriptives>=2.1.0,<3.0.0",
@@ -177,17 +179,15 @@
   "venv",
   "__init__.py",
   ".venv",
   ".env",
   ".git",
   "__pycache__",
   "dev/**",
-  "training/v0.0.0/**",
-  "training/v0.1.0/**",
-  "training/v0.1.1/**",
+  "training/main/**",
   "training/ner_fine_grained/**",
   "papers/DaCy-A-Unified-Framework-for-Danish-NLP/**"
 ]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 target-version = "py38"
```

### Comparing `dacy-2.6.0/src/dacy/datasets/dane.py` & `dacy-2.7.0/src/dacy/datasets/dane.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/datasets/lookup_tables/README.md` & `dacy-2.7.0/src/dacy/datasets/lookup_tables/README.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/datasets/lookup_tables/names.csv` & `dacy-2.7.0/src/dacy/datasets/lookup_tables/names.csv`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/datasets/names.py` & `dacy-2.7.0/src/dacy/datasets/names.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/download.py` & `dacy-2.7.0/src/dacy/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Functions for downloading DaCy models."""
 import os
-from distutils.version import StrictVersion
 from importlib.metadata import version
 from pathlib import Path
 
 from spacy.util import get_installed_models
 from tqdm import tqdm
 
-versions = ["1.1.2", "1.0.0", "1.3.3", "1.0.12", "1.0.2"]
-versions.sort(key=StrictVersion)
 DACY_DEFAULT_PATH = Path.home() / ".dacy"
 
 DEFAULT_CACHE_DIR = os.getenv(
     "DACY_CACHE_DIR",
     DACY_DEFAULT_PATH,
 )
 
 models_url = {
-    "da_dacy_small_trf-0.1.0": "https://huggingface.co/chcaa/da_dacy_small_trf/resolve/a3da03433d42538fca37847e3c73503d8e029088/da_dacy_small_trf-any-py3-none-any.whl",
-    "da_dacy_medium_trf-0.1.0": "https://huggingface.co/chcaa/da_dacy_medium_trf/resolve/61a54ab9e9ab437f5c603c023d4238ecc5bb8eb5/da_dacy_medium_trf-any-py3-none-any.whl",
-    "da_dacy_large_trf-0.1.0": "https://huggingface.co/chcaa/da_dacy_large_trf/resolve/5cfbb2bccf8e9509126e32fa3c537cc3c062aec2/da_dacy_large_trf-any-py3-none-any.whl",
+    "da_dacy_small_trf-0.2.0": "https://huggingface.co/chcaa/da_dacy_small_trf/resolve/0eadea074d5f637e76357c46bbd56451471d0154/da_dacy_small_trf-any-py3-none-any.whl",
+    "da_dacy_medium_trf-0.2.0": "https://huggingface.co/chcaa/da_dacy_medium_trf/resolve/e7dba91f855a1d26679dc1ef3aa49f7874b50543/da_dacy_medium_trf-any-py3-none-any.whl",
+    "da_dacy_large_trf-0.2.0": "https://huggingface.co/chcaa/da_dacy_large_trf/resolve/963232f378190476503a1bfc35b520cb142e9e41/da_dacy_large_trf-any-py3-none-any.whl",
     "small": None,
     "medium": None,
     "large": None,
     "da_dacy_small_ner_fine_grained-0.1.0": "https://huggingface.co/chcaa/da_dacy_small_ner_fine_grained/resolve/43fedc5a1b1c1d193f461d13225f217f2ced507d/da_dacy_small_ner_fine_grained-any-py3-none-any.whl",
     "da_dacy_medium_ner_fine_grained-0.1.0": "https://huggingface.co/chcaa/da_dacy_medium_ner_fine_grained/resolve/4bfc4397b720acdb6428d64f18e90bfd439c80fc/da_dacy_medium_ner_fine_grained-any-py3-none-any.whl",
     "da_dacy_large_ner_fine_grained-0.1.0": "https://huggingface.co/chcaa/da_dacy_large_ner_fine_grained/resolve/08f973a1ff57120268bf30d3b7e7c4656ed25a58/da_dacy_large_ner_fine_grained-any-py3-none-any.whl",
 }
@@ -36,15 +33,15 @@
         model: string indicating the model
 
     Returns:
         str: latest version of the model
     """
     if model in {"small", "medium", "large"}:
         model = f"da_dacy_{model}_trf"
-    versions = [mdl.split("-")[-1] for mdl in models_url if "ner_fine_grained" in mdl]
+    versions = [mdl.split("-")[-1] for mdl in models_url if mdl.startswith(model)]
     versions = sorted(
         versions,
         key=lambda s: [int(u) for u in s.split(".")],
         reverse=True,
     )
     return versions[0]
 
@@ -112,13 +109,11 @@
     if model not in models_url:
         raise ValueError(
             f"The model '{model}' is not available in DaCy. Please use dacy.models() to see a"
             + " list of all models",
         )
 
     mdl = model.split("-")[0]
-    if mdl in get_installed_models() and not force:
-        if version(mdl) == mdl_version:
-            return mdl
-    else:
-        install(models_url[model])
+    if mdl in get_installed_models() and not force and version(mdl) == mdl_version:
+        return mdl
+    install(models_url[model])
     return mdl
```

### Comparing `dacy-2.6.0/src/dacy/hate_speech/wrapped_models.py` & `dacy-2.7.0/src/dacy/hate_speech/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/load.py` & `dacy-2.7.0/src/dacy/load.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functionality for loading and locating DaCy models."""
+import warnings
 from pathlib import Path
 from typing import Any, Union
 
 import spacy
 from spacy.language import Language
-from wasabi import msg
 
 from .download import DEFAULT_CACHE_DIR, download_model, models_url
 
 
 def load(
     model: str,
     force: bool = False,
@@ -51,15 +51,15 @@
         str: path to the location of DaCy models
 
     Example:
         >>> import dacy
         >>> dacy.where_is_my_dacy()
     """
     if verbose is True:
-        msg.info(
+        warnings.warn(  # noqa: B028
             "DaCy pipelines above and including version 0.1.0 are installed as a "
             + "python module and are thus located in your python environment under "
             + "the respective names. To get a list of installed models use "
             + "spacy.util.get_installed_models()",
         )
     return DEFAULT_CACHE_DIR
```

### Comparing `dacy-2.6.0/src/dacy/ner/fine_grained.py` & `dacy-2.7.0/src/dacy/ner/fine_grained.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
         nlp: The spaCy language pipeline
         name: The name of the component
         size: The size of the model to use. Can be "small", "medium" or "large"
         transformer_name: The name of the transformer component which the NER moel will listen to
         version: The version of the model to use. If None, the latest version will be used
     """
     if version is None:
-        version = dacy.get_latest_version("da_dacy_{size}_ner_fine_grained")
+        version = dacy.get_latest_version(f"da_dacy_{size}_ner_fine_grained")
     nlp_ner = dacy.load(f"da_dacy_{size}_ner_fine_grained-{version}")
     nlp.add_pipe(factory_name="transformer", name=transformer_name, source=nlp_ner)
     name_, component = nlp_ner.components[-1]
     component.tok2vec.layers[0].layers[0].upstream_name = transformer_name  # type: ignore
     component.name = name  # type: ignore
     return component
```

### Comparing `dacy-2.6.0/src/dacy/ner/wrapped_models.py` & `dacy-2.7.0/src/dacy/ner/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/score/input_length.py` & `dacy-2.7.0/src/dacy/score/input_length.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/score/score.py` & `dacy-2.7.0/src/dacy/score/score.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/sentiment/wrapped_models.py` & `dacy-2.7.0/src/dacy/sentiment/wrapped_models.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy/utils.py` & `dacy-2.7.0/src/dacy/utils.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/src/dacy.egg-info/PKG-INFO` & `dacy-2.7.0/src/dacy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dacy
-Version: 2.6.0
+Version: 2.7.0
 Summary: A Danish pipeline trained in SpaCy that has achieved State-of-the-Art performance on all dependency parsing, NER and POS-tagging for Danish
 Author: Lasse Hansen, Emil Jessen
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,16 +235,14 @@
 [![PyPI](https://img.shields.io/pypi/v/dacy.svg)][pypi status]
 [![pip downloads](https://img.shields.io/pypi/dm/dacy.svg)](https://pypi.org/project/dacy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/dacy)][pypi status]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![documentation](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/centre-for-humanities-computing/dacy/actions/workflows/tests.yml/badge.svg)][tests]
 
-[![Demo](https://img.shields.io/badge/Try%20the-Demo-important)](https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.)
-
 [pypi status]: https://pypi.org/project/dacy/
 [documentation]: https://centre-for-humanities-computing.github.io/dacy/
 [tests]: https://github.com/centre-for-humanities-computing/dacy/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 
 <!-- start short-description -->
@@ -263,70 +261,56 @@
 To use the model you first have to download either the small, medium, or large model. To see a list of all available models:
 
 ```python
 import dacy
 for model in dacy.models():
     print(model)
 # ...
-# da_dacy_small_trf-0.1.0
-# da_dacy_medium_trf-0.1.0
-# da_dacy_large_trf-0.1.0
+# da_dacy_small_trf-0.2.0
+# da_dacy_medium_trf-0.2.0
+# da_dacy_large_trf-0.2.0
 ```
 
 To download and load a model simply execute:
 ```python
-nlp = dacy.load("da_dacy_medium_trf-0.1.0")
-# or equivalently
+nlp = dacy.load("da_dacy_medium_trf-0.2.0")
+# or equivalently (always loads the latest version)
 nlp = dacy.load("medium")
 ```
 
-Which will download the model to the `.dacy` directory in your home directory. 
-
-
-To download the model to a specific directory:
-```python
-dacy.download_model("da_dacy_medium_trf-0.1.0", your_save_path)
-nlp = dacy.load_model("da_dacy_medium_trf-0.1.0", your_save_path)
-```
-
-
 To see more examples, see the [documentation].
 
 # 📖 Documentation
 
 | Documentation              |                                                                                             |
 | -------------------------- | ------------------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use DaCy and its features.                                |
 | 🦾 **[Performance]**        | A detailed description of the performance of DaCy and comparison with similar Danish models |
-| 😎 **[Demo]**               | A simple Streamlit demo to try out the augmenters.                                          |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                                 |
 | 🎛 **[API References]**     | The detailed reference for DaCy's API. Including function documentation                     |
 | 🙋 **[FAQ]**                | Frequently asked questions                                                                  |
 
 
 [Installation]: https://centre-for-humanities-computing.github.io/DaCy/installation.html
 [Getting started]: https://centre-for-humanities-computing.github.io/DaCy/using_dacy.html
 [api references]: https://centre-for-humanities-computing.github.io/DaCy/
-[Demo]: https://huggingface.co/chcaa/da_dacy_medium_trf?text=DaCy+er+en+pipeline+til+anvendelse+af+dansk+sprogteknologi+lavet+af+K.+Enevoldsen%2C+L.+Hansen+og+K.+Nielbo+fra+Center+for+Humanities+Computing.
 [News and changelog]: https://centre-for-humanities-computing.github.io/DaCy/news.html
 [FAQ]: https://centre-for-humanities-computing.github.io/DaCy/faq.html
 [Performance]: https://centre-for-humanities-computing.github.io/DaCy/performance.html
 
 
 
 
 
 <br /> 
 
 <details>
   <summary> Training and reproduction </summary>
 
-The folder `training` contains a range of folders with a SpaCy project for each model version. This allows for the reproduction of the results. The SpaCy project folders also include the evaluation metrics and scripts for acquiring the required data. For more information, please see the readme's in the respective training folders.
-
-The folders include v0.0.0, v0.1.0, v0.1.1 and ner_fine_grained. The former 3 refer to the training of the main DaCy models, trained and evaluated on the DaNE dataset, whereas the latter contains the project for the fine-grained NER models trained on the [DANSK dataset](https://huggingface.co/datasets/chcaa/DANSK). Please refer to the available README's located within each training folder for more information.
+The folder `training` contains a range of folders with a SpaCy project for each model version. This allows for the reproduction of the results.
 
 Want to learn more about how DaCy initially came to be, check out this [blog post](https://www.centre-for-humanities-computing.com/post/new-fast-and-efficient-state-of-the-art-in-danish-nlp/).
 
 </details>
 
 <br /> 
 
@@ -346,7 +330,9 @@
 [Documentation]: https://centre-for-humanities-computing.github.io/dacy/index.html
 [Installation]: https://centre-for-humanities-computing.github.io/dacy/installation.html
 [Tutorials]: https://centre-for-humanities-computing.github.io/dacy/tutorials.html
 [API Reference]: https://centre-for-humanities-computing.github.io/dacy/references.html
 [FAQ]: https://centre-for-humanities-computing.github.io/dacy/faq.html
 [github issue tracker]: https://github.com/centre-for-humanities-computing/dacy/issues
 [github discussions]: https://github.com/centre-for-humanities-computing/dacy/discussions
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/project/dacy/
```

### Comparing `dacy-2.6.0/src/dacy.egg-info/requires.txt` & `dacy-2.7.0/src/dacy.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 spacy-wrap<1.5.0,>=1.4.1
-spacy<3.6.0,>=3.2.0
+spacy-experimental>=0.6.2
+spacy[transformers]<3.6.0,>=3.2.0
 pandas<2.0.0,>=1.0.0
 wasabi<0.11.0,>=0.8.2
 tqdm<4.66.0,>=4.42.1
-sentencepiece<0.2.0,>=0.1.96
 
 [dev]
 cruft
 mypy
-pre-commit<3.2.2,==2.20.0
-ruff==0.0.261
+pre-commit==3.3.1
+ruff==0.0.267
 black[jupyter]==23.3.0
 
 [docs]
-sphinx<5.4.0,>=5.3.0
+sphinx<7.1.0,>=5.3.0
 furo<2022.12.8,>=2022.12.7
-sphinx-copybutton<0.5.2,>=0.5.1
-sphinxext-opengraph<0.8.2,>=0.7.3
-sphinx_design<0.3.1,>=0.3.0
+sphinx-copybutton<0.5.3,>=0.5.1
+sphinxext-opengraph<0.8.3,>=0.7.3
+sphinx_design<0.4.2,>=0.3.0
 sphinx_togglebutton<0.4.0,>=0.2.3
 myst-nb<1.17.0,>=0.6.0
+wikidata>=0.7.0
 jupyter<1.1.0,>=1.0.0
 asent<0.8.0,>=0.4.2
 augmenty<1.4.0,>=1.0.2
 textdescriptives<3.0.0,>=2.1.0
 seaborn<0.13.0,>=0.11.2
 
 [tests]
 pytest<7.4.0,>=7.1.2
 pytest-cov<3.1.0,>=3.0.0
-pytest-xdist<3.3.0,>=3.0.0
+pytest-xdist<3.4.0,>=3.0.0
 pytest-instafail<0.6.0,>=0.4.2
```

### Comparing `dacy-2.6.0/tasks.py` & `dacy-2.7.0/tasks.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/tests/test_datasets.py` & `dacy-2.7.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/tests/test_hate_speech.py` & `dacy-2.7.0/tests/test_hate_speech.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/tests/test_score.py` & `dacy-2.7.0/tests/test_score.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/tests/test_sentiment.py` & `dacy-2.7.0/tests/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/README.md` & `dacy-2.7.0/training/ner_fine_grained/README.md`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/configs/config_large.cfg` & `dacy-2.7.0/training/ner_fine_grained/configs/config_large.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/configs/config_medium.cfg` & `dacy-2.7.0/training/ner_fine_grained/configs/config_medium.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/configs/config_small.cfg` & `dacy-2.7.0/training/ner_fine_grained/configs/config_small.cfg`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/fetch_assets.py` & `dacy-2.7.0/training/ner_fine_grained/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/project.yml` & `dacy-2.7.0/training/ner_fine_grained/project.yml`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/ner_fine_grained/update_meta_json.py` & `dacy-2.7.0/training/ner_fine_grained/update_meta_json.py`

 * *Files identical despite different names*

### Comparing `dacy-2.6.0/training/v0.0.0/configs/config_-l-ctra_small.cfg` & `dacy-2.7.0/training/main/configs/config_small.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,221 +1,296 @@
+# This is intended for training a small encoder - notably it changes the window size to 128 instead of >300
 [paths]
 train = null
 dev = null
 vectors = null
 init_tok2vec = null
+kb = "assets/knowledge_bases/knowledge_base.kb"
 
 [system]
 gpu_allocator = "pytorch"
 seed = 0
 
 [nlp]
 lang = "da"
-pipeline = ["transformer","tagger","parser","ner"]
-batch_size = 512
+pipeline = ["transformer","tagger","morphologizer","trainable_lemmatizer","parser","ner", "coref", "entity_linker"]
+batch_size = 1024
 disabled = []
 before_creation = null
 after_creation = null
 after_pipeline_creation = null
 tokenizer = {"@tokenizers":"spacy.Tokenizer.v1"}
 
 [components]
 
+[components.coref]
+factory = "experimental_coref"
+span_cluster_prefix = "coref_head_clusters"
+
+[components.coref.model]
+@architectures = "spacy-experimental.Coref.v1"
+distance_embedding_size = 20
+dropout = 0.3
+hidden_size = 1024
+depth = 2
+antecedent_limit = 100
+antecedent_batch_size = 512
+
+[components.coref.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 0.5
+upstream = "transformer"
+
+[components.coref.model.tok2vec.pooling]
+@layers = "reduce_mean.v1"
+
+[components.coref.scorer]
+@scorers = "spacy-experimental.coref_scorer.v1"
+span_cluster_prefix = "${components.coref.span_cluster_prefix}"
+
+
+[components.entity_linker]
+factory = "entity_linker"
+get_candidates = {"@misc":"spacy.CandidateGenerator.v1"}
+incl_context = true
+incl_prior = true
+entity_vector_length= 768
+n_sents = 0
+use_gold_ents = true
+    
+
+[components.entity_linker.model]
+@architectures = "spacy.EntityLinker.v2"
+nO = null
+
+[components.entity_linker.model.tok2vec]
+@architectures = "spacy.HashEmbedCNN.v2"
+pretrained_vectors = null
+width = 96
+depth = 2
+embed_size = 2000
+window_size = 1
+maxout_pieces = 3
+subword_features = true
+
+[components.morphologizer]
+factory = "morphologizer"
+extend = false
+overwrite = true
+scorer = {"@scorers":"spacy.morphologizer_scorer.v1"}
+
+[components.morphologizer.model]
+@architectures = "spacy.Tagger.v2"
+nO = null
+normalize = false
+
+[components.morphologizer.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
+pooling = {"@layers":"reduce_mean.v1"}
+upstream = "transformer"
+
 [components.ner]
 factory = "ner"
+incorrect_spans_key = null
 moves = null
+scorer = {"@scorers":"spacy.ner_scorer.v1"}
 update_with_oracle_cut_size = 100
 
 [components.ner.model]
 @architectures = "spacy.TransitionBasedParser.v2"
 state_type = "ner"
 extra_state_tokens = false
-hidden_width = 128
+hidden_width = 64
 maxout_pieces = 2
 use_upper = false
 nO = null
 
 [components.ner.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
 pooling = {"@layers":"reduce_mean.v1"}
-upstream = "*"
+upstream = "transformer"
 
 [components.parser]
 factory = "parser"
 learn_tokens = false
 min_action_freq = 30
 moves = null
+scorer = {"@scorers":"spacy.parser_scorer.v1"}
 update_with_oracle_cut_size = 100
 
 [components.parser.model]
 @architectures = "spacy.TransitionBasedParser.v2"
 state_type = "parser"
-extra_state_tokens = true
+extra_state_tokens = false
 hidden_width = 128
 maxout_pieces = 3
 use_upper = false
 nO = null
 
 [components.parser.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
 pooling = {"@layers":"reduce_mean.v1"}
-upstream = "*"
+upstream = "transformer"
 
 [components.tagger]
 factory = "tagger"
+neg_prefix = "!"
+overwrite = false
+scorer = {"@scorers":"spacy.tagger_scorer.v1"}
 
 [components.tagger.model]
-@architectures = "spacy.Tagger.v1"
+@architectures = "spacy.Tagger.v2"
 nO = null
+normalize = false
 
 [components.tagger.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
 pooling = {"@layers":"reduce_mean.v1"}
-upstream = "*"
+upstream = "transformer"
 
-[components.textcat]
-factory = "textcat"
-threshold = 0.5
-
-[components.textcat.model]
-@architectures = "spacy.TextCatEnsemble.v2"
-nO = null
+[components.trainable_lemmatizer]
+factory = "trainable_lemmatizer"
+backoff = "orth"
+min_tree_freq = 3
+overwrite = false
+scorer = {"@scorers":"spacy.lemmatizer_scorer.v1"}
+top_k = 1
 
-[components.textcat.model.linear_model]
-@architectures = "spacy.TextCatBOW.v1"
-exclusive_classes = true
-ngram_size = 1
-no_output_layer = false
+[components.trainable_lemmatizer.model]
+@architectures = "spacy.Tagger.v2"
 nO = null
+normalize = false
 
-[components.textcat.model.tok2vec]
+[components.trainable_lemmatizer.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
 pooling = {"@layers":"reduce_mean.v1"}
-upstream = "*"
+upstream = "transformer"
 
 [components.transformer]
 factory = "transformer"
 max_batch_items = 4096
 set_extra_annotations = {"@annotation_setters":"spacy-transformers.null_annotation_setter.v1"}
 
 [components.transformer.model]
-@architectures = "spacy-transformers.TransformerModel.v1"
-name = "Maltehb/-l-ctra-danish-electra-small-cased"
+@architectures = "spacy-transformers.TransformerModel.v3"
+name = "replace me"
+mixed_precision = false
 
 [components.transformer.model.get_spans]
 @span_getters = "spacy-transformers.strided_spans.v1"
 window = 128
 stride = 96
 
+[components.transformer.model.grad_scaler_config]
+
 [components.transformer.model.tokenizer_config]
 use_fast = true
 
+[components.transformer.model.transformer_config]
 
 [corpora]
 
 [corpora.dev]
 @readers = "spacy.Corpus.v1"
 path = ${paths.dev}
 max_length = 0
 gold_preproc = false
 limit = 0
 augmenter = null
 
 [corpora.train]
 @readers = "spacy.Corpus.v1"
 path = ${paths.train}
-max_length = 500
+max_length = 0
 gold_preproc = false
 limit = 0
-
-[corpora.train.augmenter]
-@augmenters = "spacy.orth_variants.v1"
-# Percentage of texts that will be augmented / lowercased
-level = 0.1
-lower = 0.5
-
-[corpora.train.augmenter.orth_variants]
-@readers = "srsly.read_json.v1"
-path = "orth_variants.json"
+augmenter = null
 
 [training]
 accumulate_gradient = 3
 dev_corpus = "corpora.dev"
 train_corpus = "corpora.train"
 seed = ${system.seed}
 gpu_allocator = ${system.gpu_allocator}
 dropout = 0.1
-patience = 2500
+patience = 4000
 max_epochs = 0
-max_steps = 400000
-eval_frequency = 600
+max_steps = 40000
+eval_frequency = 200
 frozen_components = []
+annotating_components = []
 before_to_disk = null
 
+
 [training.batcher]
-@batchers = "spacy.batch_by_padded.v1"
-discard_oversize = true
-size = 2000
-buffer = 256
-get_length = null
+@batchers = "spacy.batch_by_sequence.v1"
+size = 1
 
 [training.logger]
-@loggers = "spacy.WandbLogger.v2"
-project_name = "dacy-an-efficient-pipeline-for-danish"
+@loggers = "spacy.WandbLogger.v4"
+project_name = "dacy-v0.2.0"
+model_log_interval = 500
+log_latest_dir = null
+log_best_dir = null
 
 [training.optimizer]
 @optimizers = "Adam.v1"
 beta1 = 0.9
 beta2 = 0.999
 L2_is_weight_decay = true
 L2 = 0.01
 grad_clip = 1.0
-use_averages = false
-eps = 0.00000001
+use_averages = true
+eps = 1e-8
 
 [training.optimizer.learn_rate]
 @schedules = "warmup_linear.v1"
 warmup_steps = 250
-total_steps = 20000
-initial_rate = 0.00005
+total_steps = 40000
+initial_rate = 5e-5
 
 [training.score_weights]
+pos_acc = 0.10
+morph_acc = 0.10
+morph_per_feat = null
+dep_uas = 0.0
+dep_las = 0.20
 dep_las_per_type = null
 sents_p = null
 sents_r = null
-cats_score_desc = null
-cats_micro_p = null
-cats_micro_r = null
-cats_micro_f = null
-cats_macro_p = null
-cats_macro_r = null
-cats_macro_f = null
-cats_macro_auc = null
-cats_f_per_type = null
-cats_macro_auc_per_type = null
-ents_per_type = null
-tag_acc = 0.25
-dep_uas = 0.12
-dep_las = 0.12
-sents_f = 0.0
-cats_score = null
-ents_f = 0.25
+sents_f = 0.04
+lemma_acc = 0.1
+ents_f = 0.29
 ents_p = 0.0
 ents_r = 0.0
+ents_per_type = null
+speed = 0.0
+nel_micro_f = 0.14
+coref_f = 0.20
+coref_p = 0
+coref_r = 0
+
 
 [pretraining]
 
 [initialize]
-vectors = null
+vectors = ${paths.vectors}
 init_tok2vec = ${paths.init_tok2vec}
 vocab_data = null
 lookups = null
 before_init = null
 after_init = null
 
 [initialize.components]
 
+[initialize.components.entity_linker]
+
+[initialize.components.entity_linker.kb_loader]
+@misc = "spacy.KBFromFile.v1"
+kb_path = ${paths.kb}
+
 [initialize.tokenizer]
```

### Comparing `dacy-2.6.0/training/v0.1.0/configs/config_large.cfg` & `dacy-2.7.0/training/main/configs/config.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,226 +1,295 @@
 [paths]
-train = "corpus/da-core-news/train.spacy"
-dev = "corpus/da-core-news/dev.spacy"
+train = null
+dev = null
 vectors = null
-raw = null
 init_tok2vec = null
-vocab_data = null
+kb = "assets/knowledge_bases/knowledge_base.kb"
 
 [system]
 gpu_allocator = "pytorch"
-seed = 1
+seed = 0
 
 [nlp]
 lang = "da"
-pipeline = ["transformer","morphologizer","parser","attribute_ruler","lemmatizer","ner"]
+pipeline = ["transformer","tagger","morphologizer","trainable_lemmatizer","parser","ner", "coref", "entity_linker"]
+batch_size = 1024
 disabled = []
 before_creation = null
 after_creation = null
 after_pipeline_creation = null
-batch_size = 64
 tokenizer = {"@tokenizers":"spacy.Tokenizer.v1"}
 
 [components]
 
-[components.attribute_ruler]
-factory = "attribute_ruler"
-validate = false
-
-[components.lemmatizer]
-factory = "lemmatizer"
-mode = "lookup"
-model = null
-overwrite = false
+[components.coref]
+factory = "experimental_coref"
+span_cluster_prefix = "coref_head_clusters"
+
+[components.coref.model]
+@architectures = "spacy-experimental.Coref.v1"
+distance_embedding_size = 20
+dropout = 0.3
+hidden_size = 1024
+depth = 2
+antecedent_limit = 100
+antecedent_batch_size = 512
+
+[components.coref.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 0.5
+upstream = "transformer"
+
+[components.coref.model.tok2vec.pooling]
+@layers = "reduce_mean.v1"
+
+[components.coref.scorer]
+@scorers = "spacy-experimental.coref_scorer.v1"
+span_cluster_prefix = "${components.coref.span_cluster_prefix}"
+
+
+[components.entity_linker]
+factory = "entity_linker"
+get_candidates = {"@misc":"spacy.CandidateGenerator.v1"}
+incl_context = true
+incl_prior = true
+entity_vector_length= 768
+n_sents = 0
+use_gold_ents = true
+    
+
+[components.entity_linker.model]
+@architectures = "spacy.EntityLinker.v2"
+nO = null
+
+[components.entity_linker.model.tok2vec]
+@architectures = "spacy.HashEmbedCNN.v2"
+pretrained_vectors = null
+width = 96
+depth = 2
+embed_size = 2000
+window_size = 1
+maxout_pieces = 3
+subword_features = true
 
 [components.morphologizer]
 factory = "morphologizer"
+extend = false
+overwrite = true
+scorer = {"@scorers":"spacy.morphologizer_scorer.v1"}
 
 [components.morphologizer.model]
-@architectures = "spacy.Tagger.v1"
+@architectures = "spacy.Tagger.v2"
 nO = null
+normalize = false
 
 [components.morphologizer.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
-upstream = "transformer"
 pooling = {"@layers":"reduce_mean.v1"}
+upstream = "transformer"
 
 [components.ner]
 factory = "ner"
 incorrect_spans_key = null
 moves = null
+scorer = {"@scorers":"spacy.ner_scorer.v1"}
 update_with_oracle_cut_size = 100
 
 [components.ner.model]
 @architectures = "spacy.TransitionBasedParser.v2"
 state_type = "ner"
 extra_state_tokens = false
 hidden_width = 64
 maxout_pieces = 2
 use_upper = false
 nO = null
 
 [components.ner.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
-upstream = "transformer"
 pooling = {"@layers":"reduce_mean.v1"}
+upstream = "transformer"
 
 [components.parser]
 factory = "parser"
 learn_tokens = false
 min_action_freq = 30
 moves = null
+scorer = {"@scorers":"spacy.parser_scorer.v1"}
 update_with_oracle_cut_size = 100
 
 [components.parser.model]
 @architectures = "spacy.TransitionBasedParser.v2"
 state_type = "parser"
 extra_state_tokens = false
-hidden_width = 64
-maxout_pieces = 2
+hidden_width = 128
+maxout_pieces = 3
 use_upper = false
 nO = null
 
 [components.parser.model.tok2vec]
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
+pooling = {"@layers":"reduce_mean.v1"}
 upstream = "transformer"
+
+[components.tagger]
+factory = "tagger"
+neg_prefix = "!"
+overwrite = false
+scorer = {"@scorers":"spacy.tagger_scorer.v1"}
+
+[components.tagger.model]
+@architectures = "spacy.Tagger.v2"
+nO = null
+normalize = false
+
+[components.tagger.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
 pooling = {"@layers":"reduce_mean.v1"}
+upstream = "transformer"
+
+[components.trainable_lemmatizer]
+factory = "trainable_lemmatizer"
+backoff = "orth"
+min_tree_freq = 3
+overwrite = false
+scorer = {"@scorers":"spacy.lemmatizer_scorer.v1"}
+top_k = 1
+
+[components.trainable_lemmatizer.model]
+@architectures = "spacy.Tagger.v2"
+nO = null
+normalize = false
+
+[components.trainable_lemmatizer.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
+pooling = {"@layers":"reduce_mean.v1"}
+upstream = "transformer"
 
 [components.transformer]
 factory = "transformer"
 max_batch_items = 4096
 set_extra_annotations = {"@annotation_setters":"spacy-transformers.null_annotation_setter.v1"}
 
 [components.transformer.model]
-@architectures = "spacy-transformers.TransformerModel.v1"
-name = "xlm-roberta-large"
+@architectures = "spacy-transformers.TransformerModel.v3"
+name = "replace me"
+mixed_precision = false
 
 [components.transformer.model.get_spans]
 @span_getters = "spacy-transformers.strided_spans.v1"
-window = 128
-stride = 96
+window = 400
+stride = 350
+
+[components.transformer.model.grad_scaler_config]
 
 [components.transformer.model.tokenizer_config]
 use_fast = true
-strip_accents = false
+
+[components.transformer.model.transformer_config]
 
 [corpora]
 
 [corpora.dev]
 @readers = "spacy.Corpus.v1"
-limit = 0
+path = ${paths.dev}
 max_length = 0
-path = ${paths:dev}
 gold_preproc = false
+limit = 0
 augmenter = null
 
 [corpora.train]
 @readers = "spacy.Corpus.v1"
-path = ${paths:train}
-max_length = 500
+path = ${paths.train}
+max_length = 0
 gold_preproc = false
 limit = 0
-
-[corpora.train.augmenter]
-@augmenters = "spacy.lower_case.v1"
-level = 0.1
+augmenter = null
 
 [training]
-train_corpus = "corpora.train"
+accumulate_gradient = 3
 dev_corpus = "corpora.dev"
-seed = ${system:seed}
-gpu_allocator = ${system:gpu_allocator}
+train_corpus = "corpora.train"
+seed = ${system.seed}
+gpu_allocator = ${system.gpu_allocator}
 dropout = 0.1
-accumulate_gradient = 3
-patience = 5000
+patience = 4000
 max_epochs = 0
-max_steps = 20000
-eval_frequency = 1000
+max_steps = 40000
+eval_frequency = 200
 frozen_components = []
-before_to_disk = null
 annotating_components = []
+before_to_disk = null
+
 
 [training.batcher]
-@batchers = "spacy.batch_by_padded.v1"
-discard_oversize = true
-get_length = null
-size = 2000
-buffer = 256
+@batchers = "spacy.batch_by_sequence.v1"
+size = 1
 
 [training.logger]
-@loggers = "spacy.WandbLogger.v2"
-project_name = "dacy-an-efficient-pipeline-for-danish"
-
+@loggers = "spacy.WandbLogger.v4"
+project_name = "dacy-v0.2.0"
+model_log_interval = 500
+log_latest_dir = null
+log_best_dir = null
 
 [training.optimizer]
 @optimizers = "Adam.v1"
 beta1 = 0.9
 beta2 = 0.999
 L2_is_weight_decay = true
 L2 = 0.01
 grad_clip = 1.0
 use_averages = true
-eps = 0.00000001
+eps = 1e-8
 
 [training.optimizer.learn_rate]
 @schedules = "warmup_linear.v1"
 warmup_steps = 250
-total_steps = 20000
-initial_rate = 0.00005
+total_steps = 40000
+initial_rate = 5e-5
 
 [training.score_weights]
-pos_acc = 0.08
-morph_acc = 0.08
+pos_acc = 0.10
+morph_acc = 0.10
 morph_per_feat = null
 dep_uas = 0.0
-dep_las = 0.16
+dep_las = 0.20
 dep_las_per_type = null
 sents_p = null
 sents_r = null
-sents_f = 0.02
-lemma_acc = 0.5
-ents_f = 0.16
+sents_f = 0.04
+lemma_acc = 0.1
+ents_f = 0.29
 ents_p = 0.0
 ents_r = 0.0
 ents_per_type = null
+speed = 0.0
+nel_micro_f = 0.14
+coref_f = 0.20
+coref_p = 0
+coref_r = 0
+
 
 [pretraining]
 
 [initialize]
-vocab_data = ${paths.vocab_data}
 vectors = ${paths.vectors}
 init_tok2vec = ${paths.init_tok2vec}
+vocab_data = null
+lookups = null
 before_init = null
 after_init = null
 
 [initialize.components]
 
-[initialize.components.morphologizer]
+[initialize.components.entity_linker]
 
-[initialize.components.morphologizer.labels]
-@readers = "spacy.read_labels.v1"
-path = "corpus/labels/morphologizer.json"
-require = false
-
-[initialize.components.ner]
-
-[initialize.components.ner.labels]
-@readers = "spacy.read_labels.v1"
-path = "corpus/labels/ner.json"
-require = false
-
-[initialize.components.parser]
-
-[initialize.components.parser.labels]
-@readers = "spacy.read_labels.v1"
-path = "corpus/labels/parser.json"
-require = false
-
-[initialize.lookups]
-@misc = "spacy.LookupsDataLoader.v1"
-lang = ${nlp.lang}
-tables = ["lexeme_norm"]
+[initialize.components.entity_linker.kb_loader]
+@misc = "spacy.KBFromFile.v1"
+kb_path = ${paths.kb}
 
 [initialize.tokenizer]
```

