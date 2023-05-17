# Comparing `tmp/musiclang-0.8.8.tar.gz` & `tmp/musiclang-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclang-0.8.8.tar", last modified: Tue May  2 17:29:27 2023, max compression
+gzip compressed data, was "musiclang-0.8.9.tar", last modified: Wed May  3 09:47:14 2023, max compression
```

## Comparing `musiclang-0.8.8.tar` & `musiclang-0.8.9.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.201292 musiclang-0.8.8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-05-02 17:29:24.000000 musiclang-0.8.8/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2023-05-02 17:29:27.201292 musiclang-0.8.8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3653 2023-05-02 17:29:24.000000 musiclang-0.8.8/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.177292 musiclang-0.8.8/musiclang/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.177292 musiclang-0.8.8/musiclang/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.181292 musiclang-0.8.8/musiclang/analyze/augmented_net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/chord_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/feature_representation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8996 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/inference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/input_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/keydistance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/output_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/score_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/augmented_net/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/midi_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12879 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16589 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/pattern_analyzer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/pattern_sampler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/roman_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/score_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/score_formatter_elements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8592 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/to_musiclang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/analyze/voice_separation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/library.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.181292 musiclang-0.8.8/musiclang/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.181292 musiclang-0.8.8/musiclang/predict/arranger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/arranger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/arranger/arranger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/arranger/arranger_trainer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/arranger/melody_arranger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6092 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/arranger/melody_arranger_trainer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.181292 musiclang-0.8.8/musiclang/predict/composer/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/composer/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8883 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/composer/auto_composer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/composer/composer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/composer/harmony.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.181292 musiclang-0.8.8/musiclang/predict/predictors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/predictors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/predictors/hugging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/predictors/windowed.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.185292 musiclang-0.8.8/musiclang/predict/tokenizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/tokenizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/predict/tokenizers/chord_tokenizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.185292 musiclang-0.8.8/musiclang/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/base_transformer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.185292 musiclang-0.8.8/musiclang/transform/chord/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/chord/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/chord/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/arrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/patternator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18039 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/composing/voice_leading.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/dynamics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/dynamics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/dynamics/dynamizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/features/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/features/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/features/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/generators/rythm_generator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/mask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/melody/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/melody/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/melody/basics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/melody/continuation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/melody/filler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/merger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/note/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/note/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/note/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/orchestrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/orchestrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/orchestrations/epic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/orchestrations/nocturne.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/score/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/score/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/score/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.189292 musiclang-0.8.8/musiclang/transform/score_merger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/score_merger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/score_merger/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.193292 musiclang-0.8.8/musiclang/transform/structure_graphs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/structure_graphs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/structure_graphs/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/transformer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/transform/utils_random.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.193292 musiclang-0.8.8/musiclang/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.193292 musiclang-0.8.8/musiclang/write/arrange_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/arrange_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/arrange_utils/arrange_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/arrange_utils/skyline_algorithm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43763 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/element.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.193292 musiclang-0.8.8/musiclang/write/elements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/bar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/beat.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/element.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/free_text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/rhythm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/time_signature.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/tonality.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/voice_leading.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/elements/voicing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13661 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14138 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27070 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/note_pitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8474 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/ornementation.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.193292 musiclang-0.8.8/musiclang/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/out/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12085 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/out/midi_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/out/to_code.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/out/to_midi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/out/to_mxl.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.193292 musiclang-0.8.8/musiclang/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5393 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/pitches/pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/musiclang/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/properties/note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/musiclang/write/rhythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/rhythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/rhythm/metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/rhythm/score_rythm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/rhythm/utils_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37418 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/score.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/musiclang/write/sequence/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/sequence/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/sequence/sequence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/sequence/sequence_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/musiclang/write/time_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/time_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/time_utils/time_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-05-02 17:29:24.000000 musiclang-0.8.8/musiclang/write/tonality.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.177292 musiclang-0.8.8/musiclang.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2023-05-02 17:29:27.000000 musiclang-0.8.8/musiclang.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6212 2023-05-02 17:29:27.000000 musiclang-0.8.8/musiclang.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 17:29:27.000000 musiclang-0.8.8/musiclang.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-02 17:29:27.000000 musiclang-0.8.8/musiclang.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-02 17:29:27.000000 musiclang-0.8.8/musiclang.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      995 2023-05-02 17:29:25.000000 musiclang-0.8.8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-02 17:29:27.201292 musiclang-0.8.8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2023-05-02 17:29:25.000000 musiclang-0.8.8/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/tests/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/analyze/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/analyze/test_analyze.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/analyze/test_score_formatter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/tests/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/composing/test_counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/composing/test_project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/composing/test_voice_leading.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/tests/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/predict/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/predict/test_auto_composer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/tests/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/transform/test_mask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/transform/test_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/transform/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/transform/test_transform_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/transform/test_transforms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.197292 musiclang-0.8.8/tests/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.201292 musiclang-0.8.8/tests/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/out/test_to_midi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.201292 musiclang-0.8.8/tests/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/pitches/test_pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.201292 musiclang-0.8.8/tests/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/properties/test_note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:27.201292 musiclang-0.8.8/tests/write/rythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/rythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/rythm/test_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_absolute_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_bass_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_chord_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_chromatic_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_drum_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_extensions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5994 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_score.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-05-02 17:29:24.000000 musiclang-0.8.8/tests/write/test_tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-05-03 09:47:11.000000 musiclang-0.8.9/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2023-05-03 09:47:14.968462 musiclang-0.8.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3653 2023-05-03 09:47:11.000000 musiclang-0.8.9/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.952462 musiclang-0.8.9/musiclang/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.952462 musiclang-0.8.9/musiclang/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/analyze/augmented_net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/chord_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/feature_representation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8996 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/inference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/input_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/keydistance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/output_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/score_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/augmented_net/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/midi_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12879 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16589 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/pattern_analyzer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/pattern_sampler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/roman_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/score_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/score_formatter_elements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8592 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/to_musiclang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/analyze/voice_separation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/library.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/arranger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/arranger_trainer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/melody_arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6092 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/arranger/melody_arranger_trainer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/composer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8888 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/auto_composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/composer/harmony.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/predictors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/predictors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/predictors/hugging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/predictors/windowed.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/predict/tokenizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/tokenizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/predict/tokenizers/chord_tokenizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/base_transformer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.956462 musiclang-0.8.9/musiclang/transform/chord/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/chord/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/chord/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/arrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/patternator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18039 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/composing/voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/dynamics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/dynamics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/dynamics/dynamizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/features/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/features/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/features/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/generators/rythm_generator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/mask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/melody/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/basics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/continuation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/melody/filler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/merger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/note/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/note/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/note/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/orchestrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/orchestrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/orchestrations/epic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/orchestrations/nocturne.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/score/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/score_merger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score_merger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/score_merger/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/transform/structure_graphs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/structure_graphs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/structure_graphs/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/transformer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/transform/utils_random.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.960462 musiclang-0.8.9/musiclang/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/arrange_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/arrange_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/arrange_utils/arrange_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/arrange_utils/skyline_algorithm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43763 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4651 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/element.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/elements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/bar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/beat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/element.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/free_text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/rhythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/time_signature.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/tonality.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/voice_leading.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/elements/voicing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13661 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14138 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27070 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/note_pitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8474 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/ornementation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12085 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/midi_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/to_code.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/to_midi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/out/to_mxl.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5393 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/pitches/pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/properties/note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/rhythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/score_rythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/rhythm/utils_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37548 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/score.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/sequence/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/sequence/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/sequence/sequence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/sequence/sequence_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/musiclang/write/time_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/time_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/time_utils/time_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-05-03 09:47:11.000000 musiclang-0.8.9/musiclang/write/tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.952462 musiclang-0.8.9/musiclang.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6212 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-03 09:47:14.000000 musiclang-0.8.9/musiclang.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      995 2023-05-03 09:47:13.000000 musiclang-0.8.9/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-03 09:47:14.972462 musiclang-0.8.9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2023-05-03 09:47:13.000000 musiclang-0.8.9/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.964462 musiclang-0.8.9/tests/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/analyze/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/analyze/test_analyze.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/analyze/test_score_formatter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/test_counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/test_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/composing/test_voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/predict/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/predict/test_auto_composer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_mask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_transform_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/transform/test_transforms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/out/test_to_midi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/pitches/test_pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/properties/test_note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:14.968462 musiclang-0.8.9/tests/write/rythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/rythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/rythm/test_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_absolute_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_bass_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_chord_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_chromatic_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_drum_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_extensions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5994 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_score.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-05-03 09:47:11.000000 musiclang-0.8.9/tests/write/test_tonality.py
```

### Comparing `musiclang-0.8.8/LICENSE.md` & `musiclang-0.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/PKG-INFO` & `musiclang-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclang
-Version: 0.8.8
+Version: 0.8.9
 Summary: A python package for music notation and generation
 Home-page: UNKNOWN
 Author: Florian GARDIN
 Author-email: fgardin.pro@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/MusicLang/musiclang/
```

### Comparing `musiclang-0.8.8/README.md` & `musiclang-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/__init__.py` & `musiclang-0.8.9/musiclang/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/__init__.py` & `musiclang-0.8.9/musiclang/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/cache.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/cache.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/chord_vocabulary.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/chord_vocabulary.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/feature_representation.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/feature_representation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/inference.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/inference.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/input_representations.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/input_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/keydistance.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/keydistance.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/models.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/models.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/output_representations.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/output_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/score_parser.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/score_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/augmented_net/utils.py` & `musiclang-0.8.9/musiclang/analyze/augmented_net/utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/constants.py` & `musiclang-0.8.9/musiclang/analyze/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/item.py` & `musiclang-0.8.9/musiclang/analyze/item.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/midi_parser.py` & `musiclang-0.8.9/musiclang/analyze/midi_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/parser.py` & `musiclang-0.8.9/musiclang/analyze/parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/pattern_analyzer.py` & `musiclang-0.8.9/musiclang/analyze/pattern_analyzer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/pattern_sampler.py` & `musiclang-0.8.9/musiclang/analyze/pattern_sampler.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/roman_parser.py` & `musiclang-0.8.9/musiclang/analyze/roman_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/score_formatter.py` & `musiclang-0.8.9/musiclang/analyze/score_formatter.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/score_formatter_elements.py` & `musiclang-0.8.9/musiclang/analyze/score_formatter_elements.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/to_musiclang.py` & `musiclang-0.8.9/musiclang/analyze/to_musiclang.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/analyze/voice_separation.py` & `musiclang-0.8.9/musiclang/analyze/voice_separation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/__init__.py` & `musiclang-0.8.9/musiclang/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/arranger/arranger.py` & `musiclang-0.8.9/musiclang/predict/arranger/arranger.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/arranger/arranger_trainer.py` & `musiclang-0.8.9/musiclang/predict/arranger/arranger_trainer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/arranger/melody_arranger_trainer.py` & `musiclang-0.8.9/musiclang/predict/arranger/melody_arranger_trainer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/composer/auto_composer.py` & `musiclang-0.8.9/musiclang/predict/composer/auto_composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     instrument_dict = {}
     for instrument in instruments:
         clean_instrument = ''.join(instrument.split('__')[:-1])
         instrument_dict[clean_instrument] = instrument_dict.get(clean_instrument, -1) + 1
         index = instrument_dict[clean_instrument]
         real_instruments.append(instrument + f'__{index}')
 
-    return instruments
+    return real_instruments
 
 def auto_compose(melody, harmony, orchestra, voicing, patternator,
                  tonality, solo_instrument, instruments, acc_amp='mf',
                  fixed_bass=True, voice_leading=True
                  ):
     from musiclang.transform import Patternator
```

### Comparing `musiclang-0.8.8/musiclang/predict/composer/composer.py` & `musiclang-0.8.9/musiclang/predict/composer/composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/composer/harmony.py` & `musiclang-0.8.9/musiclang/predict/composer/harmony.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/predictors/hugging.py` & `musiclang-0.8.9/musiclang/predict/predictors/hugging.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/predictors/windowed.py` & `musiclang-0.8.9/musiclang/predict/predictors/windowed.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/predict/tokenizers/chord_tokenizer.py` & `musiclang-0.8.9/musiclang/predict/tokenizers/chord_tokenizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/__init__.py` & `musiclang-0.8.9/musiclang/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/base_transformer.py` & `musiclang-0.8.9/musiclang/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/chord/basics.py` & `musiclang-0.8.9/musiclang/transform/chord/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/arrange.py` & `musiclang-0.8.9/musiclang/transform/composing/arrange.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/counterpoint.py` & `musiclang-0.8.9/musiclang/transform/composing/counterpoint.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/layer.py` & `musiclang-0.8.9/musiclang/transform/composing/layer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/pattern.py` & `musiclang-0.8.9/musiclang/transform/composing/pattern.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/patternator.py` & `musiclang-0.8.9/musiclang/transform/composing/patternator.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/project.py` & `musiclang-0.8.9/musiclang/transform/composing/project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/composing/voice_leading.py` & `musiclang-0.8.9/musiclang/transform/composing/voice_leading.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/dynamics/dynamizer.py` & `musiclang-0.8.9/musiclang/transform/dynamics/dynamizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/features/basics.py` & `musiclang-0.8.9/musiclang/transform/features/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/graph.py` & `musiclang-0.8.9/musiclang/transform/graph.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/library.py` & `musiclang-0.8.9/musiclang/transform/library.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/mask.py` & `musiclang-0.8.9/musiclang/transform/mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/melody/basics.py` & `musiclang-0.8.9/musiclang/transform/melody/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/melody/continuation.py` & `musiclang-0.8.9/musiclang/transform/melody/continuation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/note/basics.py` & `musiclang-0.8.9/musiclang/transform/note/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/orchestrations/epic.py` & `musiclang-0.8.9/musiclang/transform/orchestrations/epic.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/orchestrations/nocturne.py` & `musiclang-0.8.9/musiclang/transform/orchestrations/nocturne.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/pipeline.py` & `musiclang-0.8.9/musiclang/transform/pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/score_merger/basics.py` & `musiclang-0.8.9/musiclang/transform/score_merger/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/structure_graphs/forms.py` & `musiclang-0.8.9/musiclang/transform/structure_graphs/forms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/transformer.py` & `musiclang-0.8.9/musiclang/transform/transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/transform/utils_random.py` & `musiclang-0.8.9/musiclang/transform/utils_random.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/arrange_utils/arrange_utils.py` & `musiclang-0.8.9/musiclang/write/arrange_utils/arrange_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/arrange_utils/skyline_algorithm.py` & `musiclang-0.8.9/musiclang/write/arrange_utils/skyline_algorithm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/chord.py` & `musiclang-0.8.9/musiclang/write/chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/constants.py` & `musiclang-0.8.9/musiclang/write/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/element.py` & `musiclang-0.8.9/musiclang/write/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,21 @@
          Degree
     """
     def __init__(self, val):
         self.val = val
 
 
     def __add__(self, other):
+        from musiclang import Chord, Score
         if isinstance(other, int):
             return Element(self.val + other)
         if isinstance(other, Element):
-            return Element((self.val + other.val) % 7)
+            return self() + other()
+        elif isinstance(Element, (Chord, Score)):
+            return self() + other
         else:
             raise Exception('Cannot add if not type int or Element')
 
     def __repr__(self):
         from .chord import Chord
         return Chord(element=self.val).__repr__()
```

### Comparing `musiclang-0.8.8/musiclang/write/elements/chord.py` & `musiclang-0.8.9/musiclang/write/elements/chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/library.py` & `musiclang-0.8.9/musiclang/write/library.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/melody.py` & `musiclang-0.8.9/musiclang/write/melody.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/note.py` & `musiclang-0.8.9/musiclang/write/note.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/note_pitch.py` & `musiclang-0.8.9/musiclang/write/note_pitch.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/ornementation.py` & `musiclang-0.8.9/musiclang/write/ornementation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/out/constants.py` & `musiclang-0.8.9/musiclang/write/out/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/out/midi_utils.py` & `musiclang-0.8.9/musiclang/write/out/midi_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/out/to_code.py` & `musiclang-0.8.9/musiclang/write/out/to_code.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/out/to_midi.py` & `musiclang-0.8.9/musiclang/write/out/to_midi.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/out/to_mxl.py` & `musiclang-0.8.9/musiclang/write/out/to_mxl.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/pitches/pitches_utils.py` & `musiclang-0.8.9/musiclang/write/pitches/pitches_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/properties/note_properties.py` & `musiclang-0.8.9/musiclang/write/properties/note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/rhythm/metric.py` & `musiclang-0.8.9/musiclang/write/rhythm/metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/rhythm/score_rythm.py` & `musiclang-0.8.9/musiclang/write/rhythm/score_rythm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/rhythm/utils_metric.py` & `musiclang-0.8.9/musiclang/write/rhythm/utils_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/score.py` & `musiclang-0.8.9/musiclang/write/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,17 @@
 
 
         """
         cp = self.copy()
         cp.tags = cp.tags - set(tags)
         return cp
 
+    def set_duration(self, duration):
+        return Score([c.set_duration(duration) for c in self.chords], tags=set(self.tags))
+
     def remove_tag(self, tag):
         """
         Remove a tag from this object
         Returns a copy of the object
         Parameters
         ----------
         tag: str
```

### Comparing `musiclang-0.8.8/musiclang/write/sequence/sequence.py` & `musiclang-0.8.9/musiclang/write/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/sequence/sequence_utils.py` & `musiclang-0.8.9/musiclang/write/sequence/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/time_utils/time_utils.py` & `musiclang-0.8.9/musiclang/write/time_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang/write/tonality.py` & `musiclang-0.8.9/musiclang/write/tonality.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/musiclang.egg-info/PKG-INFO` & `musiclang-0.8.9/musiclang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclang
-Version: 0.8.8
+Version: 0.8.9
 Summary: A python package for music notation and generation
 Home-page: UNKNOWN
 Author: Florian GARDIN
 Author-email: fgardin.pro@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/MusicLang/musiclang/
```

### Comparing `musiclang-0.8.8/musiclang.egg-info/SOURCES.txt` & `musiclang-0.8.9/musiclang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/pyproject.toml` & `musiclang-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "musiclang"
-version = "0.8.8"
+version = "0.8.9"
 description = "A python package for music notation and generation"
 readme = "README.md"
 authors = [{ name = "Florian GARDIN", email = "fgardin.pro@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `musiclang-0.8.8/setup.py` & `musiclang-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="musiclang",
-    version="0.8.8",
+    version="0.8.9",
     author="Florian GARDIN",
     author_email="fgardin.pro@gmail.com",
     description=("A python package for music notation and generation"
                 ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
```

### Comparing `musiclang-0.8.8/tests/analyze/test_score_formatter.py` & `musiclang-0.8.9/tests/analyze/test_score_formatter.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/composing/test_project.py` & `musiclang-0.8.9/tests/composing/test_project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/composing/test_voice_leading.py` & `musiclang-0.8.9/tests/composing/test_voice_leading.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/predict/test_auto_composer.py` & `musiclang-0.8.9/tests/predict/test_auto_composer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/transform/test_mask.py` & `musiclang-0.8.9/tests/transform/test_mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/transform/test_pipeline.py` & `musiclang-0.8.9/tests/transform/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/transform/test_transforms.py` & `musiclang-0.8.9/tests/transform/test_transforms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/out/test_to_midi.py` & `musiclang-0.8.9/tests/write/out/test_to_midi.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/pitches/test_pitches_utils.py` & `musiclang-0.8.9/tests/write/pitches/test_pitches_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/properties/test_note_properties.py` & `musiclang-0.8.9/tests/write/properties/test_note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/rythm/test_metric.py` & `musiclang-0.8.9/tests/write/rythm/test_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_bass_notes.py` & `musiclang-0.8.9/tests/write/test_bass_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_chord.py` & `musiclang-0.8.9/tests/write/test_chord.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_chord_notes.py` & `musiclang-0.8.9/tests/write/test_chord_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_drum_notes.py` & `musiclang-0.8.9/tests/write/test_drum_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_extensions.py` & `musiclang-0.8.9/tests/write/test_extensions.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_note.py` & `musiclang-0.8.9/tests/write/test_note.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_score.py` & `musiclang-0.8.9/tests/write/test_score.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.8/tests/write/test_tonality.py` & `musiclang-0.8.9/tests/write/test_tonality.py`

 * *Files identical despite different names*

