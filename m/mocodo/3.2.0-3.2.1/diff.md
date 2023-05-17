# Comparing `tmp/mocodo-3.2.0.tar.gz` & `tmp/mocodo-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocodo-3.2.0.tar", max compression
+gzip compressed data, was "mocodo-3.2.1.tar", max compression
```

## Comparing `mocodo-3.2.0.tar` & `mocodo-3.2.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0     1072 2017-09-06 13:23:36.000000 mocodo-3.2.0/LICENSE
--rw-r--r--   0        0        0     6729 2023-05-15 17:40:57.109268 mocodo-3.2.0/README.md
--rw-r--r--   0        0        0       75 2022-09-05 13:09:15.074760 mocodo-3.2.0/mocodo/__init__.py
--rwxr-xr-x   0        0        0     3798 2022-11-02 08:58:46.486058 mocodo-3.2.0/mocodo/__main__.py
--rwxr-xr-x   0        0        0    16632 2023-01-28 11:18:09.584553 mocodo-3.2.0/mocodo/argument_parser.py
--rwxr-xr-x   0        0        0     8988 2022-09-29 15:13:08.365059 mocodo-3.2.0/mocodo/arrange_bb.py
--rwxr-xr-x   0        0        0     5511 2022-09-22 13:40:19.000000 mocodo-3.2.0/mocodo/arrange_ga.py
--rwxr-xr-x   0        0        0    21404 2023-05-15 13:04:54.384907 mocodo-3.2.0/mocodo/association.py
--rwxr-xr-x   0        0        0     3903 2022-09-05 13:09:15.079105 mocodo-3.2.0/mocodo/attribute.py
--rwxr-xr-x   0        0        0     5886 2023-01-28 11:16:39.787010 mocodo-3.2.0/mocodo/common.py
--rwxr-xr-x   0        0        0     4418 2023-05-15 17:43:30.305592 mocodo-3.2.0/mocodo/constraint.py
--rwxr-xr-x   0        0        0     1437 2022-09-05 13:09:15.080189 mocodo-3.2.0/mocodo/cross.py
--rw-r--r--   0        0        0     1991 2022-09-05 13:09:15.080684 mocodo-3.2.0/mocodo/damerau_levenshtein.py
--rwxr-xr-x   0        0        0     4484 2022-09-05 13:09:15.081151 mocodo-3.2.0/mocodo/diagram_link.py
--rwxr-xr-x   0        0        0     6558 2022-12-12 09:58:24.000000 mocodo-3.2.0/mocodo/entity.py
--rwxr-xr-x   0        0        0      228 2022-09-05 13:09:15.082116 mocodo-3.2.0/mocodo/file_helpers.py
--rwxr-xr-x   0        0        0     1280 2022-09-05 13:09:15.082712 mocodo-3.2.0/mocodo/fitness.py
--rwxr-xr-x   0        0        0     1110 2023-01-28 11:16:39.787918 mocodo-3.2.0/mocodo/font_metrics.py
--rwxr-xr-x   0        0        0     1957 2022-09-05 13:09:15.083736 mocodo-3.2.0/mocodo/grid.py
--rwxr-xr-x   0        0        0    25987 2023-05-15 15:42:56.641165 mocodo-3.2.0/mocodo/leg.py
--rw-r--r--   0        0        0     5334 2022-12-12 12:51:27.098572 mocodo-3.2.0/mocodo/magic_command.py
--rwxr-xr-x   0        0        0    24808 2023-05-15 16:00:16.400968 mocodo-3.2.0/mocodo/mcd.py
--rw-r--r--   0        0        0    11367 2023-05-15 14:17:26.992323 mocodo-3.2.0/mocodo/mcd_to_svg.py
--rwxr-xr-x   0        0        0      630 2022-09-18 17:39:21.116186 mocodo-3.2.0/mocodo/mocodo_error.py
--rwxr-xr-x   0        0        0     4807 2023-05-15 15:25:26.108679 mocodo-3.2.0/mocodo/obfuscate.py
--rwxr-xr-x   0        0        0      542 2022-09-05 13:09:15.088019 mocodo-3.2.0/mocodo/phantom.py
--rwxr-xr-x   0        0        0     1639 2022-09-12 10:44:29.393788 mocodo-3.2.0/mocodo/pluralize_fr.py
--rwxr-xr-x   0        0        0     4535 2023-01-28 11:16:39.790562 mocodo-3.2.0/mocodo/read_template.py
--rwxr-xr-x   0        0        0    35235 2023-01-28 11:16:39.791270 mocodo-3.2.0/mocodo/relations.py
--rw-r--r--   0        0        0      650 2023-05-15 17:14:17.009755 mocodo-3.2.0/mocodo/resources/colors/blank.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.899518 mocodo-3.2.0/mocodo/resources/colors/brewer+1.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.907572 mocodo-3.2.0/mocodo/resources/colors/brewer+2.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.905622 mocodo-3.2.0/mocodo/resources/colors/brewer+3.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903628 mocodo-3.2.0/mocodo/resources/colors/brewer+4.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903285 mocodo-3.2.0/mocodo/resources/colors/brewer+5.json
--rw-r--r--   0        0        0      693 2023-05-15 14:44:57.900653 mocodo-3.2.0/mocodo/resources/colors/brewer+6.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.900431 mocodo-3.2.0/mocodo/resources/colors/brewer+7.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.904370 mocodo-3.2.0/mocodo/resources/colors/brewer+8.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.902137 mocodo-3.2.0/mocodo/resources/colors/brewer+9.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.899761 mocodo-3.2.0/mocodo/resources/colors/brewer-1.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.905982 mocodo-3.2.0/mocodo/resources/colors/brewer-2.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.907245 mocodo-3.2.0/mocodo/resources/colors/brewer-3.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.901837 mocodo-3.2.0/mocodo/resources/colors/brewer-4.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.904980 mocodo-3.2.0/mocodo/resources/colors/brewer-5.json
--rw-r--r--   0        0        0      693 2023-05-15 14:44:57.900217 mocodo-3.2.0/mocodo/resources/colors/brewer-6.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.901531 mocodo-3.2.0/mocodo/resources/colors/brewer-7.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.902965 mocodo-3.2.0/mocodo/resources/colors/brewer-8.json
--rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903848 mocodo-3.2.0/mocodo/resources/colors/brewer-9.json
--rw-r--r--   0        0        0      656 2023-05-15 17:13:10.230401 mocodo-3.2.0/mocodo/resources/colors/bw-alpha.json
--rw-r--r--   0        0        0      660 2023-05-15 14:44:57.899228 mocodo-3.2.0/mocodo/resources/colors/bw.json
--rw-r--r--   0        0        0      706 2023-05-15 17:13:10.207409 mocodo-3.2.0/mocodo/resources/colors/desert.json
--rw-r--r--   0        0        0      658 2023-05-15 17:13:10.207350 mocodo-3.2.0/mocodo/resources/colors/gray.json
--rw-r--r--   0        0        0      686 2023-05-15 17:13:10.206133 mocodo-3.2.0/mocodo/resources/colors/keepsake.json
--rw-r--r--   0        0        0      715 2023-05-15 14:44:57.901018 mocodo-3.2.0/mocodo/resources/colors/mondrian.json
--rw-r--r--   0        0        0      706 2023-05-15 17:13:44.139095 mocodo-3.2.0/mocodo/resources/colors/ocean.json
--rw-r--r--   0        0        0      706 2023-05-15 17:13:07.899644 mocodo-3.2.0/mocodo/resources/colors/pond.json
--rw-r--r--   0        0        0      663 2023-05-15 14:44:57.906877 mocodo-3.2.0/mocodo/resources/colors/wb.json
--rw-r--r--   0        0        0      714 2023-05-15 14:44:57.907841 mocodo-3.2.0/mocodo/resources/colors/xinnian.json
--rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.100146 mocodo-3.2.0/mocodo/resources/font_metrics.json
--rw-r--r--   0        0        0    64345 2022-09-05 13:09:15.100633 mocodo-3.2.0/mocodo/resources/lorem/disparition.txt
--rw-r--r--   0        0        0     3200 2022-09-05 13:09:15.100777 mocodo-3.2.0/mocodo/resources/lorem/four_letter_words.txt
--rw-r--r--   0        0        0     2051 2022-09-05 13:09:15.100888 mocodo-3.2.0/mocodo/resources/lorem/lorem_ipsum.txt
--rw-r--r--   0        0        0      741 2023-05-15 17:23:22.354970 mocodo-3.2.0/mocodo/resources/pristine_sandbox.mcd
--rw-r--r--   0        0        0     3237 2022-12-11 18:28:56.187987 mocodo-3.2.0/mocodo/resources/relation_templates/debug.json
--rw-r--r--   0        0        0     1137 2023-01-28 11:16:39.791612 mocodo-3.2.0/mocodo/resources/relation_templates/dependencies.json
--rw-r--r--   0        0        0      973 2022-12-12 15:29:58.319997 mocodo-3.2.0/mocodo/resources/relation_templates/diagram.json
--rw-r--r--   0        0        0     1362 2022-12-13 17:17:49.267440 mocodo-3.2.0/mocodo/resources/relation_templates/html.json
--rw-r--r--   0        0        0    18311 2022-12-12 15:29:58.320955 mocodo-3.2.0/mocodo/resources/relation_templates/html_verbose.json
--rw-r--r--   0        0        0     7363 2022-12-12 15:29:58.321361 mocodo-3.2.0/mocodo/resources/relation_templates/json.json
--rw-r--r--   0        0        0     1253 2022-12-12 15:29:58.321750 mocodo-3.2.0/mocodo/resources/relation_templates/latex.json
--rw-r--r--   0        0        0      104 2023-01-28 11:16:39.792002 mocodo-3.2.0/mocodo/resources/relation_templates/latex_without_def.json
--rw-r--r--   0        0        0      421 2022-12-12 15:29:58.322622 mocodo-3.2.0/mocodo/resources/relation_templates/markdown.json
--rw-r--r--   0        0        0     1441 2022-12-12 15:29:58.323069 mocodo-3.2.0/mocodo/resources/relation_templates/markdown_data_dict.json
--rw-r--r--   0        0        0    14169 2022-12-12 15:29:58.323618 mocodo-3.2.0/mocodo/resources/relation_templates/markdown_verbose.json
--rw-r--r--   0        0        0     5065 2022-12-12 15:29:58.323968 mocodo-3.2.0/mocodo/resources/relation_templates/mysql.json
--rw-r--r--   0        0        0     5104 2022-12-12 15:29:58.324305 mocodo-3.2.0/mocodo/resources/relation_templates/oracle.json
--rw-r--r--   0        0        0     4918 2022-12-12 15:29:58.324644 mocodo-3.2.0/mocodo/resources/relation_templates/postgresql.json
--rw-r--r--   0        0        0     5311 2022-12-12 15:29:58.325008 mocodo-3.2.0/mocodo/resources/relation_templates/sqlite.json
--rw-r--r--   0        0        0       25 2023-01-28 11:16:39.792840 mocodo-3.2.0/mocodo/resources/relation_templates/text.json
--rw-r--r--   0        0        0      347 2022-12-12 09:58:24.000000 mocodo-3.2.0/mocodo/resources/relation_templates/txt2tags.json
--rw-r--r--   0        0        0     4777 2022-09-05 13:09:15.107446 mocodo-3.2.0/mocodo/resources/res/messages_de.mo
--rw-r--r--   0        0        0     9078 2023-05-15 17:26:46.559028 mocodo-3.2.0/mocodo/resources/res/messages_fr.mo
--rw-r--r--   0        0        0    10357 2023-01-28 11:16:39.793653 mocodo-3.2.0/mocodo/resources/res/messages_fr.po
--rw-r--r--   0        0        0     4048 2022-09-05 13:09:15.109006 mocodo-3.2.0/mocodo/resources/res/messages_zh.mo
--rw-r--r--   0        0        0     1451 2023-05-15 14:49:17.550663 mocodo-3.2.0/mocodo/resources/shapes/arial.json
--rw-r--r--   0        0        0     1450 2023-05-15 16:37:09.601570 mocodo-3.2.0/mocodo/resources/shapes/copperplate.json
--rw-r--r--   0        0        0     1441 2023-05-15 14:48:07.012008 mocodo-3.2.0/mocodo/resources/shapes/georgia.json
--rw-r--r--   0        0        0     1599 2023-05-15 14:50:47.803027 mocodo-3.2.0/mocodo/resources/shapes/mondrian.json
--rw-r--r--   0        0        0     1506 2023-05-15 14:41:58.295545 mocodo-3.2.0/mocodo/resources/shapes/sans.json
--rw-r--r--   0        0        0     1514 2023-05-15 14:41:58.296140 mocodo-3.2.0/mocodo/resources/shapes/serif.json
--rw-r--r--   0        0        0     1481 2023-05-15 14:51:53.188174 mocodo-3.2.0/mocodo/resources/shapes/times.json
--rw-r--r--   0        0        0     1466 2023-05-15 14:52:43.367466 mocodo-3.2.0/mocodo/resources/shapes/trebuchet.json
--rw-r--r--   0        0        0     1591 2023-05-15 14:55:47.087364 mocodo-3.2.0/mocodo/resources/shapes/verdana.json
--rw-r--r--   0        0        0     1487 2023-05-15 14:56:47.062651 mocodo-3.2.0/mocodo/resources/shapes/xinnian.json
--rw-r--r--   0        0        0       18 2023-05-15 16:44:12.700272 mocodo-3.2.0/mocodo/version_number.py
--rw-r--r--   0        0        0     1216 2023-05-15 16:44:24.208663 mocodo-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     8543 1970-01-01 00:00:00.000000 mocodo-3.2.0/setup.py
--rw-r--r--   0        0        0     7939 1970-01-01 00:00:00.000000 mocodo-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2017-09-06 13:23:36.000000 mocodo-3.2.1/LICENSE
+-rw-r--r--   0        0        0     6731 2023-05-17 06:07:39.197058 mocodo-3.2.1/README.md
+-rw-r--r--   0        0        0       75 2022-09-05 13:09:15.074760 mocodo-3.2.1/mocodo/__init__.py
+-rwxr-xr-x   0        0        0     3798 2022-11-02 08:58:46.486058 mocodo-3.2.1/mocodo/__main__.py
+-rwxr-xr-x   0        0        0    16632 2023-01-28 11:18:09.584553 mocodo-3.2.1/mocodo/argument_parser.py
+-rwxr-xr-x   0        0        0     8988 2022-09-29 15:13:08.365059 mocodo-3.2.1/mocodo/arrange_bb.py
+-rwxr-xr-x   0        0        0     5511 2022-09-22 13:40:19.000000 mocodo-3.2.1/mocodo/arrange_ga.py
+-rwxr-xr-x   0        0        0    21404 2023-05-15 13:04:54.384907 mocodo-3.2.1/mocodo/association.py
+-rwxr-xr-x   0        0        0     3903 2022-09-05 13:09:15.079105 mocodo-3.2.1/mocodo/attribute.py
+-rwxr-xr-x   0        0        0     5886 2023-01-28 11:16:39.787010 mocodo-3.2.1/mocodo/common.py
+-rwxr-xr-x   0        0        0     4418 2023-05-15 17:43:30.305592 mocodo-3.2.1/mocodo/constraint.py
+-rwxr-xr-x   0        0        0     1437 2022-09-05 13:09:15.080189 mocodo-3.2.1/mocodo/cross.py
+-rw-r--r--   0        0        0     1991 2022-09-05 13:09:15.080684 mocodo-3.2.1/mocodo/damerau_levenshtein.py
+-rwxr-xr-x   0        0        0     4484 2022-09-05 13:09:15.081151 mocodo-3.2.1/mocodo/diagram_link.py
+-rwxr-xr-x   0        0        0     6558 2022-12-12 09:58:24.000000 mocodo-3.2.1/mocodo/entity.py
+-rwxr-xr-x   0        0        0      228 2022-09-05 13:09:15.082116 mocodo-3.2.1/mocodo/file_helpers.py
+-rwxr-xr-x   0        0        0     1280 2022-09-05 13:09:15.082712 mocodo-3.2.1/mocodo/fitness.py
+-rwxr-xr-x   0        0        0     1110 2023-01-28 11:16:39.787918 mocodo-3.2.1/mocodo/font_metrics.py
+-rwxr-xr-x   0        0        0     1957 2022-09-05 13:09:15.083736 mocodo-3.2.1/mocodo/grid.py
+-rwxr-xr-x   0        0        0    25987 2023-05-15 15:42:56.641165 mocodo-3.2.1/mocodo/leg.py
+-rw-r--r--   0        0        0     5334 2022-12-12 12:51:27.098572 mocodo-3.2.1/mocodo/magic_command.py
+-rwxr-xr-x   0        0        0    24808 2023-05-15 16:00:16.400968 mocodo-3.2.1/mocodo/mcd.py
+-rw-r--r--   0        0        0    11367 2023-05-15 14:17:26.992323 mocodo-3.2.1/mocodo/mcd_to_svg.py
+-rwxr-xr-x   0        0        0      630 2022-09-18 17:39:21.116186 mocodo-3.2.1/mocodo/mocodo_error.py
+-rwxr-xr-x   0        0        0     4807 2023-05-15 15:25:26.108679 mocodo-3.2.1/mocodo/obfuscate.py
+-rwxr-xr-x   0        0        0      542 2022-09-05 13:09:15.088019 mocodo-3.2.1/mocodo/phantom.py
+-rwxr-xr-x   0        0        0     1639 2022-09-12 10:44:29.393788 mocodo-3.2.1/mocodo/pluralize_fr.py
+-rwxr-xr-x   0        0        0     4535 2023-01-28 11:16:39.790562 mocodo-3.2.1/mocodo/read_template.py
+-rwxr-xr-x   0        0        0    35235 2023-01-28 11:16:39.791270 mocodo-3.2.1/mocodo/relations.py
+-rw-r--r--   0        0        0      650 2023-05-15 17:14:17.009755 mocodo-3.2.1/mocodo/resources/colors/blank.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.899518 mocodo-3.2.1/mocodo/resources/colors/brewer+1.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.907572 mocodo-3.2.1/mocodo/resources/colors/brewer+2.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.905622 mocodo-3.2.1/mocodo/resources/colors/brewer+3.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903628 mocodo-3.2.1/mocodo/resources/colors/brewer+4.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903285 mocodo-3.2.1/mocodo/resources/colors/brewer+5.json
+-rw-r--r--   0        0        0      693 2023-05-15 14:44:57.900653 mocodo-3.2.1/mocodo/resources/colors/brewer+6.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.900431 mocodo-3.2.1/mocodo/resources/colors/brewer+7.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.904370 mocodo-3.2.1/mocodo/resources/colors/brewer+8.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.902137 mocodo-3.2.1/mocodo/resources/colors/brewer+9.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.899761 mocodo-3.2.1/mocodo/resources/colors/brewer-1.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.905982 mocodo-3.2.1/mocodo/resources/colors/brewer-2.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.907245 mocodo-3.2.1/mocodo/resources/colors/brewer-3.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.901837 mocodo-3.2.1/mocodo/resources/colors/brewer-4.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.904980 mocodo-3.2.1/mocodo/resources/colors/brewer-5.json
+-rw-r--r--   0        0        0      693 2023-05-15 14:44:57.900217 mocodo-3.2.1/mocodo/resources/colors/brewer-6.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.901531 mocodo-3.2.1/mocodo/resources/colors/brewer-7.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.902965 mocodo-3.2.1/mocodo/resources/colors/brewer-8.json
+-rw-r--r--   0        0        0      702 2023-05-15 14:44:57.903848 mocodo-3.2.1/mocodo/resources/colors/brewer-9.json
+-rw-r--r--   0        0        0      656 2023-05-15 17:13:10.230401 mocodo-3.2.1/mocodo/resources/colors/bw-alpha.json
+-rw-r--r--   0        0        0      660 2023-05-15 14:44:57.899228 mocodo-3.2.1/mocodo/resources/colors/bw.json
+-rw-r--r--   0        0        0      706 2023-05-15 17:13:10.207409 mocodo-3.2.1/mocodo/resources/colors/desert.json
+-rw-r--r--   0        0        0      658 2023-05-15 17:13:10.207350 mocodo-3.2.1/mocodo/resources/colors/gray.json
+-rw-r--r--   0        0        0      686 2023-05-15 17:13:10.206133 mocodo-3.2.1/mocodo/resources/colors/keepsake.json
+-rw-r--r--   0        0        0      715 2023-05-15 14:44:57.901018 mocodo-3.2.1/mocodo/resources/colors/mondrian.json
+-rw-r--r--   0        0        0      706 2023-05-15 17:13:44.139095 mocodo-3.2.1/mocodo/resources/colors/ocean.json
+-rw-r--r--   0        0        0      706 2023-05-15 17:13:07.899644 mocodo-3.2.1/mocodo/resources/colors/pond.json
+-rw-r--r--   0        0        0      663 2023-05-15 14:44:57.906877 mocodo-3.2.1/mocodo/resources/colors/wb.json
+-rw-r--r--   0        0        0      714 2023-05-15 14:44:57.907841 mocodo-3.2.1/mocodo/resources/colors/xinnian.json
+-rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.100146 mocodo-3.2.1/mocodo/resources/font_metrics.json
+-rw-r--r--   0        0        0    64345 2022-09-05 13:09:15.100633 mocodo-3.2.1/mocodo/resources/lorem/disparition.txt
+-rw-r--r--   0        0        0     3200 2022-09-05 13:09:15.100777 mocodo-3.2.1/mocodo/resources/lorem/four_letter_words.txt
+-rw-r--r--   0        0        0     2051 2022-09-05 13:09:15.100888 mocodo-3.2.1/mocodo/resources/lorem/lorem_ipsum.txt
+-rw-r--r--   0        0        0      743 2023-05-17 06:05:12.196694 mocodo-3.2.1/mocodo/resources/pristine_sandbox.mcd
+-rw-r--r--   0        0        0     3237 2022-12-11 18:28:56.187987 mocodo-3.2.1/mocodo/resources/relation_templates/debug.json
+-rw-r--r--   0        0        0     1137 2023-01-28 11:16:39.791612 mocodo-3.2.1/mocodo/resources/relation_templates/dependencies.json
+-rw-r--r--   0        0        0      973 2022-12-12 15:29:58.319997 mocodo-3.2.1/mocodo/resources/relation_templates/diagram.json
+-rw-r--r--   0        0        0     1362 2022-12-13 17:17:49.267440 mocodo-3.2.1/mocodo/resources/relation_templates/html.json
+-rw-r--r--   0        0        0    18311 2022-12-12 15:29:58.320955 mocodo-3.2.1/mocodo/resources/relation_templates/html_verbose.json
+-rw-r--r--   0        0        0     7363 2022-12-12 15:29:58.321361 mocodo-3.2.1/mocodo/resources/relation_templates/json.json
+-rw-r--r--   0        0        0     1253 2022-12-12 15:29:58.321750 mocodo-3.2.1/mocodo/resources/relation_templates/latex.json
+-rw-r--r--   0        0        0      104 2023-01-28 11:16:39.792002 mocodo-3.2.1/mocodo/resources/relation_templates/latex_without_def.json
+-rw-r--r--   0        0        0      421 2022-12-12 15:29:58.322622 mocodo-3.2.1/mocodo/resources/relation_templates/markdown.json
+-rw-r--r--   0        0        0     1441 2022-12-12 15:29:58.323069 mocodo-3.2.1/mocodo/resources/relation_templates/markdown_data_dict.json
+-rw-r--r--   0        0        0    14169 2022-12-12 15:29:58.323618 mocodo-3.2.1/mocodo/resources/relation_templates/markdown_verbose.json
+-rw-r--r--   0        0        0     5065 2022-12-12 15:29:58.323968 mocodo-3.2.1/mocodo/resources/relation_templates/mysql.json
+-rw-r--r--   0        0        0     5104 2022-12-12 15:29:58.324305 mocodo-3.2.1/mocodo/resources/relation_templates/oracle.json
+-rw-r--r--   0        0        0     4918 2022-12-12 15:29:58.324644 mocodo-3.2.1/mocodo/resources/relation_templates/postgresql.json
+-rw-r--r--   0        0        0     5311 2022-12-12 15:29:58.325008 mocodo-3.2.1/mocodo/resources/relation_templates/sqlite.json
+-rw-r--r--   0        0        0       25 2023-01-28 11:16:39.792840 mocodo-3.2.1/mocodo/resources/relation_templates/text.json
+-rw-r--r--   0        0        0      347 2022-12-12 09:58:24.000000 mocodo-3.2.1/mocodo/resources/relation_templates/txt2tags.json
+-rw-r--r--   0        0        0     4777 2022-09-05 13:09:15.107446 mocodo-3.2.1/mocodo/resources/res/messages_de.mo
+-rw-r--r--   0        0        0     9078 2023-05-15 17:26:46.559028 mocodo-3.2.1/mocodo/resources/res/messages_fr.mo
+-rw-r--r--   0        0        0    10357 2023-01-28 11:16:39.793653 mocodo-3.2.1/mocodo/resources/res/messages_fr.po
+-rw-r--r--   0        0        0     4048 2022-09-05 13:09:15.109006 mocodo-3.2.1/mocodo/resources/res/messages_zh.mo
+-rw-r--r--   0        0        0     1451 2023-05-15 14:49:17.550663 mocodo-3.2.1/mocodo/resources/shapes/arial.json
+-rw-r--r--   0        0        0     1450 2023-05-15 16:37:09.601570 mocodo-3.2.1/mocodo/resources/shapes/copperplate.json
+-rw-r--r--   0        0        0     1441 2023-05-15 14:48:07.012008 mocodo-3.2.1/mocodo/resources/shapes/georgia.json
+-rw-r--r--   0        0        0     1599 2023-05-15 14:50:47.803027 mocodo-3.2.1/mocodo/resources/shapes/mondrian.json
+-rw-r--r--   0        0        0     1506 2023-05-15 14:41:58.295545 mocodo-3.2.1/mocodo/resources/shapes/sans.json
+-rw-r--r--   0        0        0     1514 2023-05-15 14:41:58.296140 mocodo-3.2.1/mocodo/resources/shapes/serif.json
+-rw-r--r--   0        0        0     1481 2023-05-15 14:51:53.188174 mocodo-3.2.1/mocodo/resources/shapes/times.json
+-rw-r--r--   0        0        0     1466 2023-05-15 14:52:43.367466 mocodo-3.2.1/mocodo/resources/shapes/trebuchet.json
+-rw-r--r--   0        0        0     1591 2023-05-15 14:55:47.087364 mocodo-3.2.1/mocodo/resources/shapes/verdana.json
+-rw-r--r--   0        0        0     1487 2023-05-15 14:56:47.062651 mocodo-3.2.1/mocodo/resources/shapes/xinnian.json
+-rw-r--r--   0        0        0       18 2023-05-15 16:44:12.700272 mocodo-3.2.1/mocodo/version_number.py
+-rw-r--r--   0        0        0     1216 2023-05-17 06:51:00.904653 mocodo-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8545 1970-01-01 00:00:00.000000 mocodo-3.2.1/setup.py
+-rw-r--r--   0        0        0     7941 1970-01-01 00:00:00.000000 mocodo-3.2.1/PKG-INFO
```

### Comparing `mocodo-3.2.0/LICENSE` & `mocodo-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/README.md` & `mocodo-3.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-associations).
+**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-les-associations).
 
 **11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.
 
 **24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).
 
 **14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel : prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).
 
@@ -79,15 +79,15 @@
 - qté requise
 - num. société
 - raison sociale
 
 Ainsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:
 
 ```
-%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1
+%mocodo --input mocodo_notebook/sandbox.mld --colors desert
 ```
 
 ![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_2.png)
 
 La devise de Mocodo, « nickel, ni souris », en résume les principaux points forts:
 
 - description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement ;
```

### Comparing `mocodo-3.2.0/mocodo/__main__.py` & `mocodo-3.2.1/mocodo/__main__.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/argument_parser.py` & `mocodo-3.2.1/mocodo/argument_parser.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/arrange_bb.py` & `mocodo-3.2.1/mocodo/arrange_bb.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/arrange_ga.py` & `mocodo-3.2.1/mocodo/arrange_ga.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/association.py` & `mocodo-3.2.1/mocodo/association.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/attribute.py` & `mocodo-3.2.1/mocodo/attribute.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/common.py` & `mocodo-3.2.1/mocodo/common.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/constraint.py` & `mocodo-3.2.1/mocodo/constraint.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/cross.py` & `mocodo-3.2.1/mocodo/cross.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/damerau_levenshtein.py` & `mocodo-3.2.1/mocodo/damerau_levenshtein.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/diagram_link.py` & `mocodo-3.2.1/mocodo/diagram_link.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/entity.py` & `mocodo-3.2.1/mocodo/entity.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/fitness.py` & `mocodo-3.2.1/mocodo/fitness.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/font_metrics.py` & `mocodo-3.2.1/mocodo/font_metrics.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/grid.py` & `mocodo-3.2.1/mocodo/grid.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/leg.py` & `mocodo-3.2.1/mocodo/leg.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/magic_command.py` & `mocodo-3.2.1/mocodo/magic_command.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/mcd.py` & `mocodo-3.2.1/mocodo/mcd.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/mcd_to_svg.py` & `mocodo-3.2.1/mocodo/mcd_to_svg.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/mocodo_error.py` & `mocodo-3.2.1/mocodo/mocodo_error.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/obfuscate.py` & `mocodo-3.2.1/mocodo/obfuscate.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/phantom.py` & `mocodo-3.2.1/mocodo/phantom.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/pluralize_fr.py` & `mocodo-3.2.1/mocodo/pluralize_fr.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/read_template.py` & `mocodo-3.2.1/mocodo/read_template.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/relations.py` & `mocodo-3.2.1/mocodo/relations.py`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/blank.json` & `mocodo-3.2.1/mocodo/resources/colors/blank.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+1.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+1.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+2.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+2.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+3.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+3.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+4.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+4.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+5.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+5.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+6.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+6.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+7.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+7.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+8.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+8.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer+9.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer+9.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-1.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-1.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-2.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-2.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-3.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-3.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-4.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-4.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-5.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-5.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-6.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-6.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-7.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-7.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-8.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-8.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/brewer-9.json` & `mocodo-3.2.1/mocodo/resources/colors/brewer-9.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/bw-alpha.json` & `mocodo-3.2.1/mocodo/resources/colors/bw-alpha.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/bw.json` & `mocodo-3.2.1/mocodo/resources/colors/bw.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/desert.json` & `mocodo-3.2.1/mocodo/resources/colors/desert.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/gray.json` & `mocodo-3.2.1/mocodo/resources/colors/gray.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/keepsake.json` & `mocodo-3.2.1/mocodo/resources/colors/keepsake.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/mondrian.json` & `mocodo-3.2.1/mocodo/resources/colors/mondrian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/ocean.json` & `mocodo-3.2.1/mocodo/resources/colors/ocean.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/pond.json` & `mocodo-3.2.1/mocodo/resources/colors/pond.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/wb.json` & `mocodo-3.2.1/mocodo/resources/colors/wb.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/colors/xinnian.json` & `mocodo-3.2.1/mocodo/resources/colors/xinnian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/font_metrics.json` & `mocodo-3.2.1/mocodo/resources/font_metrics.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/lorem/disparition.txt` & `mocodo-3.2.1/mocodo/resources/lorem/disparition.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/lorem/four_letter_words.txt` & `mocodo-3.2.1/mocodo/resources/lorem/four_letter_words.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/lorem/lorem_ipsum.txt` & `mocodo-3.2.1/mocodo/resources/lorem/lorem_ipsum.txt`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/pristine_sandbox.mcd` & `mocodo-3.2.1/mocodo/resources/pristine_sandbox.mcd`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 AYANT-DROIT: nom ayant-droit, lien
 DIRIGER, 0N EMPLOYÉ, 01 PROJET
 REQUÉRIR, 1N PROJET, 0N PIÈCE: qté requise
 PIÈCE: réf. pièce, libellé pièce
-Composer, 0N [composée] PIÈCE, 0N [composante] PIÈCE: quantité
+COMPOSER, 0N [composée] PIÈCE, 0N [composante] PIÈCE: quantité
 
 DF1, _11 AYANT-DROIT, 0N EMPLOYÉ
 EMPLOYÉ: matricule, nom employé
 PROJET: num. projet, nom projet
 FOURNIR, 1N PROJET, 1N PIÈCE, 1N SOCIÉTÉ: qté fournie
 
 DÉPARTEMENT: num. département, nom département
 EMPLOYER, 11 EMPLOYÉ, 1N DÉPARTEMENT
 TRAVAILLER, 0N EMPLOYÉ, 1N PROJET
 SOCIÉTÉ: num. société, raison sociale
 CONTRÔLER, 0N< [filiale] SOCIÉTÉ, 01 [mère] SOCIÉTÉ
 
-(I) [Les pièces fournies par une société pour un projet font partie de celles qu'il requiert.] ..PIÈCE, ->REQUÉRIR, --FOURNIR, PROJET
+  (I) [Les pièces fournies par une société pour un projet font partie de celles qu'il requiert.] ..PIÈCE, ->REQUÉRIR, --FOURNIR, PROJET
```

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/debug.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/debug.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/dependencies.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/dependencies.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/diagram.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/diagram.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/html.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/html.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/html_verbose.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/html_verbose.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/json.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/json.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/latex.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/latex.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/markdown_data_dict.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/markdown_data_dict.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/markdown_verbose.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/markdown_verbose.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/mysql.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/mysql.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/oracle.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/oracle.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/postgresql.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/postgresql.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/relation_templates/sqlite.json` & `mocodo-3.2.1/mocodo/resources/relation_templates/sqlite.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/res/messages_de.mo` & `mocodo-3.2.1/mocodo/resources/res/messages_de.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/res/messages_fr.mo` & `mocodo-3.2.1/mocodo/resources/res/messages_fr.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/res/messages_fr.po` & `mocodo-3.2.1/mocodo/resources/res/messages_fr.po`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/res/messages_zh.mo` & `mocodo-3.2.1/mocodo/resources/res/messages_zh.mo`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/arial.json` & `mocodo-3.2.1/mocodo/resources/shapes/arial.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/copperplate.json` & `mocodo-3.2.1/mocodo/resources/shapes/copperplate.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/georgia.json` & `mocodo-3.2.1/mocodo/resources/shapes/georgia.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/mondrian.json` & `mocodo-3.2.1/mocodo/resources/shapes/mondrian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/sans.json` & `mocodo-3.2.1/mocodo/resources/shapes/sans.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/serif.json` & `mocodo-3.2.1/mocodo/resources/shapes/serif.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/times.json` & `mocodo-3.2.1/mocodo/resources/shapes/times.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/trebuchet.json` & `mocodo-3.2.1/mocodo/resources/shapes/trebuchet.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/verdana.json` & `mocodo-3.2.1/mocodo/resources/shapes/verdana.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/mocodo/resources/shapes/xinnian.json` & `mocodo-3.2.1/mocodo/resources/shapes/xinnian.json`

 * *Files identical despite different names*

### Comparing `mocodo-3.2.0/pyproject.toml` & `mocodo-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mocodo"
-version = "3.2.0"
+version = "3.2.1"
 description = "Modélisation Conceptuelle de Données. Nickel. Ni souris."
 authors = ["Aristide Grange"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.mocodo.net"
 repository = "https://github.com/laowantong/mocodo/"
 keywords = ["education",
```

### Comparing `mocodo-3.2.0/setup.py` & `mocodo-3.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             'resources/shapes/*']}
 
 entry_points = \
 {'console_scripts': ['mocodo = mocodo.__main__:main']}
 
 setup_kwargs = {
     'name': 'mocodo',
-    'version': '3.2.0',
+    'version': '3.2.1',
     'description': 'Modélisation Conceptuelle de Données. Nickel. Ni souris.',
-    'long_description': "**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-associations).\n\n**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.\n\n**24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).\n\n**14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel\xa0: prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).\n\n**11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).\n\n------\n\nDocumentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou sous forme de [notebook](doc/fr_refman.ipynb) Jupyter.\n\n----\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)\n\nMocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).\n\n- En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).\n- En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](\nhttps://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.\n\nCi-dessous, un exemple d'utilisation sous [Jupyter Notebook](https://jupyter.org). L'appel du programme est en première ligne, sur un texte d'entrée donné lignes suivantes. Le cas est adapté de l'article fondateur de Peter Chen, [_The entity-relationship model—toward a unified view of data_](https://doi.org/10.1145/320434.320440) (ACM Trans. Database Syst. 1, 1, March 1976, pp. 9–36), avec en bonus une association de type hiérarchique et une contrainte d'inclusion.\n\n```\n%%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict\n\nAyant-droit: nom ayant-droit, lien\nDiriger, 0N Employé, 01 Projet\nRequérir, 1N Projet, 0N Pièce: qté requise\nPièce: réf. pièce, libellé pièce\nComposer, 0N [composée] Pièce, 0N [composante] Pièce: quantité\n\nDF1, _11 Ayant-droit, 0N Employé\nEmployé: matricule, nom employé\nProjet: num. projet, nom projet\nFournir, 1N Projet, 1N Pièce, 1N Société: qté fournie\n\nDépartement: num. département, nom département\nEmployer, 11 Employé, 1N Département\nTravailler, 0N Employé, 1N Projet\nSociété: num. société, raison sociale\nContrôler, 0N< [filiale] Société, 01 [mère] Société\n\n(I) --Fournir, ->Requérir, ..Pièce, Projet\n```\n\nEn sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.png)\n\n**Ayant-droit** (<ins>_#matricule_</ins>, <ins>nom ayant-droit</ins>, lien)<br>\n**Composer** (<ins>_#réf. pièce composée_</ins>, <ins>_#réf. pièce composante_</ins>, quantité)<br>\n**Département** (<ins>num. département</ins>, nom département)<br>\n**Employé** (<ins>matricule</ins>, nom employé, _#num. département_)<br>\n**Fournir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, <ins>_#num. société_</ins>, qté fournie)<br>\n**Pièce** (<ins>réf. pièce</ins>, libellé pièce)<br>\n**Projet** (<ins>num. projet</ins>, nom projet, _#matricule_)<br>\n**Requérir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, qté requise)<br>\n**Société** (<ins>num. société</ins>, raison sociale, _#num. société mère_)<br>\n**Travailler** (<ins>_#matricule_</ins>, <ins>_#num. projet_</ins>)\n\nL'appel précédent a également créé un fichier `mocodo_notebook/sandbox_data_dict.md` contenant le dictionnaire des données :\n\n- nom ayant-droit\n- lien\n- quantité\n- num. département\n- nom département\n- matricule\n- nom employé\n- qté fournie\n- réf. pièce\n- libellé pièce\n- num. projet\n- nom projet\n- qté requise\n- num. société\n- raison sociale\n\nAinsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:\n\n```\n%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1\n```\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_2.png)\n\nLa devise de Mocodo, «\xa0nickel, ni souris\xa0», en résume les principaux points forts:\n\n- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement\xa0;\n- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité\xa0;\n- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs\xa0: là encore, il travaille sur une description textuelle, et non directement sur le dessin.\n\nMocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support\xa0: cela augmentera ses chances d'attirer des contributeurs qui le feront évoluer.\n\nPour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).\n",
+    'long_description': "**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-les-associations).\n\n**11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.\n\n**24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).\n\n**14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel\xa0: prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).\n\n**11 septembre 2022.** Mocodo 3.0 introduit l'[héritage](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), l'[agrégation](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Agrégation-(ou-pseudo-entité)), les [calques](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), les [sorties PDF et PNG](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Héritage-(ou-spécialisation)), [etc](https://github.com/laowantong/mocodo/releases/tag/3.0).\n\n------\n\nDocumentation [au format HTML](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html) ou sous forme de [notebook](doc/fr_refman.ipynb) Jupyter.\n\n----\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/logos/banner.svg)\n\nMocodo est un logiciel d'aide à l'enseignement et à la conception des [bases de données relationnelles](https://fr.wikipedia.org/wiki/Base_de_données_relationnelle).\n\n- En entrée, il prend une description textuelle des entités et associations du modèle conceptuel de données ([MCD](https://fr.wikipedia.org/wiki/Modèle_entité-association)).\n- En sortie, il produit son diagramme entité-association en [SVG](https://fr.wikipedia.org/wiki/Scalable_Vector_Graphics) et son schéma relationnel ([MLD](\nhttps://fr.wikipedia.org/wiki/Merise_%28informatique%29#MLD_:_mod.C3.A8le_logique_des_donn.C3.A9es)) en [SQL](https://fr.wikipedia.org/wiki/Structured_Query_Language), [LaTeX](https://fr.wikipedia.org/wiki/LaTeX), [Markdown](https://fr.wikipedia.org/wiki/Markdown), etc.\n\nCi-dessous, un exemple d'utilisation sous [Jupyter Notebook](https://jupyter.org). L'appel du programme est en première ligne, sur un texte d'entrée donné lignes suivantes. Le cas est adapté de l'article fondateur de Peter Chen, [_The entity-relationship model—toward a unified view of data_](https://doi.org/10.1145/320434.320440) (ACM Trans. Database Syst. 1, 1, March 1976, pp. 9–36), avec en bonus une association de type hiérarchique et une contrainte d'inclusion.\n\n```\n%%mocodo --mld --colors brewer+1 --shapes copperplate --relations diagram markdown_data_dict\n\nAyant-droit: nom ayant-droit, lien\nDiriger, 0N Employé, 01 Projet\nRequérir, 1N Projet, 0N Pièce: qté requise\nPièce: réf. pièce, libellé pièce\nComposer, 0N [composée] Pièce, 0N [composante] Pièce: quantité\n\nDF1, _11 Ayant-droit, 0N Employé\nEmployé: matricule, nom employé\nProjet: num. projet, nom projet\nFournir, 1N Projet, 1N Pièce, 1N Société: qté fournie\n\nDépartement: num. département, nom département\nEmployer, 11 Employé, 1N Département\nTravailler, 0N Employé, 1N Projet\nSociété: num. société, raison sociale\nContrôler, 0N< [filiale] Société, 01 [mère] Société\n\n(I) --Fournir, ->Requérir, ..Pièce, Projet\n```\n\nEn sortie, le MCD (diagramme conceptuel) et le MLD (schéma relationnel) correspondants:\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_1.png)\n\n**Ayant-droit** (<ins>_#matricule_</ins>, <ins>nom ayant-droit</ins>, lien)<br>\n**Composer** (<ins>_#réf. pièce composée_</ins>, <ins>_#réf. pièce composante_</ins>, quantité)<br>\n**Département** (<ins>num. département</ins>, nom département)<br>\n**Employé** (<ins>matricule</ins>, nom employé, _#num. département_)<br>\n**Fournir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, <ins>_#num. société_</ins>, qté fournie)<br>\n**Pièce** (<ins>réf. pièce</ins>, libellé pièce)<br>\n**Projet** (<ins>num. projet</ins>, nom projet, _#matricule_)<br>\n**Requérir** (<ins>_#num. projet_</ins>, <ins>_#réf. pièce_</ins>, qté requise)<br>\n**Société** (<ins>num. société</ins>, raison sociale, _#num. société mère_)<br>\n**Travailler** (<ins>_#matricule_</ins>, <ins>_#num. projet_</ins>)\n\nL'appel précédent a également créé un fichier `mocodo_notebook/sandbox_data_dict.md` contenant le dictionnaire des données :\n\n- nom ayant-droit\n- lien\n- quantité\n- num. département\n- nom département\n- matricule\n- nom employé\n- qté fournie\n- réf. pièce\n- libellé pièce\n- num. projet\n- nom projet\n- qté requise\n- num. société\n- raison sociale\n\nAinsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:\n\n```\n%mocodo --input mocodo_notebook/sandbox.mld --colors desert\n```\n\n![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_2.png)\n\nLa devise de Mocodo, «\xa0nickel, ni souris\xa0», en résume les principaux points forts:\n\n- description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement\xa0;\n- propreté du rendu. La sortie se fait en vectoriel, prête à être affichée, imprimée, agrandie, exportée dans une multitude de formats sans perte de qualité\xa0;\n- rapidité des retouches. L'utilisateur rectifie les alignements en insérant des éléments invisibles, en dupliquant des coordonnées ou en ajustant des facteurs mutiplicatifs\xa0: là encore, il travaille sur une description textuelle, et non directement sur le dessin.\n\nMocodo est libre, gratuit et multiplateforme. Si vous l'aimez, répandez la bonne nouvelle en incluant l'un de ses logos dans votre support\xa0: cela augmentera ses chances d'attirer des contributeurs qui le feront évoluer.\n\nPour vous familiariser avec Mocodo, le mieux est d'utiliser [sa version en ligne](https://www.mocodo.net).\n",
     'author': 'Aristide Grange',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.mocodo.net',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mocodo-3.2.0/PKG-INFO` & `mocodo-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocodo
-Version: 3.2.0
+Version: 3.2.1
 Summary: Modélisation Conceptuelle de Données. Nickel. Ni souris.
 Home-page: https://www.mocodo.net
 License: MIT
 Keywords: education,relational,database,drawing,ERD,SVG,Merise
 Author: Aristide Grange
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
 Classifier: Topic :: Education
 Project-URL: Repository, https://github.com/laowantong/mocodo/
 Project-URL: issues, https://github.com/laowantong/mocodo/issues
 Description-Content-Type: text/markdown
 
-**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-associations).
+**15 mai 2023.** Mocodo 3.2.0 prend en charge la [visualisation des contraintes sur associations](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Visualisation-des-contraintes-sur-les-associations).
 
 **11 mai 2023.** Ajout d'un tutoriel / galerie d'exemples dans la [version en ligne](https://www.mocodo.net) de Mocodo 3.1.2.
 
 **24 décembre 2022.** Mocodo 3.1.1 corrige la [gestion des collisions des SVG interactifs](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Éviter-qu'une-interaction-sur-un-SVG-ne-s'applique-à-un-autre).
 
 **14 décembre 2022.** Mocodo 3.1 améliore le passage au relationnel : prise en charge de [gabarits personnels dérivés des gabarits existants](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Dérivation-de-gabarits), traitement des [tables indépendantes réduites à leur clé primaire](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Suppression-des-tables-indépendantes-réduites-à-leur-clé-primaire), génération d'un [graphe des dépendances](https://rawgit.com/laowantong/mocodo/master/doc/fr_refman.html#Graphe-des-dépendances) pour le tri topologique des tables, [etc](https://github.com/laowantong/mocodo/releases/tag/3.1.0).
 
@@ -109,15 +109,15 @@
 - qté requise
 - num. société
 - raison sociale
 
 Ainsi que le diagramme relationnel, qui peut être visualisé par un nouvel appel:
 
 ```
-%mocodo --input mocodo_notebook/sandbox.mld --colors brewer+1
+%mocodo --input mocodo_notebook/sandbox.mld --colors desert
 ```
 
 ![](https://cdn.rawgit.com/laowantong/mocodo/master/doc/readme_2.png)
 
 La devise de Mocodo, « nickel, ni souris », en résume les principaux points forts:
 
 - description textuelle des données. L'utilisateur n'a pas à renseigner, placer et déplacer des éléments comme avec une lessive ordinaire. Il ne fournit rien de plus que les informations définissant son MCD. L'outil s'occupe tout seul du plongement ;
```

