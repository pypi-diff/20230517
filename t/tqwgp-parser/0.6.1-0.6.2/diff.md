# Comparing `tmp/tqwgp-parser-0.6.1.tar.gz` & `tmp/tqwgp-parser-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tqwgp-parser-0.6.1.tar", last modified: Fri Mar 24 17:10:26 2023, max compression
+gzip compressed data, was "tqwgp-parser-0.6.2.tar", last modified: Wed May 17 14:48:07 2023, max compression
```

## Comparing `tqwgp-parser-0.6.1.tar` & `tqwgp-parser-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/
--rw-r--r--   0 yoan      (1000) yoan      (1000)    34523 2021-01-14 19:27:47.000000 tqwgp-parser-0.6.1/LICENSE
--rw-r--r--   0 yoan      (1000) yoan      (1000)     5281 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/PKG-INFO
--rw-r--r--   0 yoan      (1000) yoan      (1000)     4887 2021-01-15 13:24:29.000000 tqwgp-parser-0.6.1/README.md
-drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/scripts/
--rw-r--r--   0 yoan      (1000) yoan      (1000)      117 2022-05-09 15:51:00.000000 tqwgp-parser-0.6.1/scripts/tqwgp
--rw-r--r--   0 yoan      (1000) yoan      (1000)       38 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/setup.cfg
--rw-r--r--   0 yoan      (1000) yoan      (1000)     1424 2023-03-24 16:59:24.000000 tqwgp-parser-0.6.1/setup.py
-drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/tqwgp_parser/
--rw-r--r--   0 yoan      (1000) yoan      (1000)      236 2022-05-09 13:44:53.000000 tqwgp-parser-0.6.1/tqwgp_parser/__init__.py
--rw-r--r--   0 yoan      (1000) yoan      (1000)    14385 2023-03-24 17:08:22.000000 tqwgp-parser-0.6.1/tqwgp_parser/__main__.py
--rw-r--r--   0 yoan      (1000) yoan      (1000)       64 2022-05-09 13:10:55.000000 tqwgp-parser-0.6.1/tqwgp_parser/constants.py
-drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/tqwgp_parser/files/
--rw-r--r--   0 yoan      (1000) yoan      (1000)     3984 2022-05-11 18:58:55.000000 tqwgp-parser-0.6.1/tqwgp_parser/files/loaders.py
--rw-r--r--   0 yoan      (1000) yoan      (1000)    12621 2023-02-10 23:03:12.000000 tqwgp-parser-0.6.1/tqwgp_parser/parser.hy
--rw-r--r--   0 yoan      (1000) yoan      (1000)     2781 2023-02-10 22:47:49.000000 tqwgp-parser-0.6.1/tqwgp_parser/utils.hy
-drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-03-24 17:10:26.839476 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/
--rw-r--r--   0 yoan      (1000) yoan      (1000)     5281 2023-03-24 17:10:26.000000 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/PKG-INFO
--rw-r--r--   0 yoan      (1000) yoan      (1000)      405 2023-03-24 17:10:26.000000 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/SOURCES.txt
--rw-r--r--   0 yoan      (1000) yoan      (1000)        1 2023-03-24 17:10:26.000000 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/dependency_links.txt
--rw-r--r--   0 yoan      (1000) yoan      (1000)        1 2021-01-15 12:17:06.000000 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/not-zip-safe
--rw-r--r--   0 yoan      (1000) yoan      (1000)       56 2023-03-24 17:10:26.000000 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/requires.txt
--rw-r--r--   0 yoan      (1000) yoan      (1000)       13 2023-03-24 17:10:26.000000 tqwgp-parser-0.6.1/tqwgp_parser.egg-info/top_level.txt
+drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-05-17 14:48:07.368676 tqwgp-parser-0.6.2/
+-rw-r--r--   0 yoan      (1000) yoan      (1000)    34523 2021-01-14 19:27:47.000000 tqwgp-parser-0.6.2/LICENSE
+-rw-r--r--   0 yoan      (1000) yoan      (1000)     5279 2023-05-17 14:48:07.368676 tqwgp-parser-0.6.2/PKG-INFO
+-rw-r--r--   0 yoan      (1000) yoan      (1000)     4887 2021-01-15 13:24:29.000000 tqwgp-parser-0.6.2/README.md
+drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-05-17 14:48:07.365342 tqwgp-parser-0.6.2/scripts/
+-rw-r--r--   0 yoan      (1000) yoan      (1000)      117 2022-05-09 15:51:00.000000 tqwgp-parser-0.6.2/scripts/tqwgp
+-rw-r--r--   0 yoan      (1000) yoan      (1000)       38 2023-05-17 14:48:07.368676 tqwgp-parser-0.6.2/setup.cfg
+-rw-r--r--   0 yoan      (1000) yoan      (1000)     1425 2023-05-17 14:34:32.000000 tqwgp-parser-0.6.2/setup.py
+drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-05-17 14:48:07.365342 tqwgp-parser-0.6.2/tests/
+-rw-r--r--   0 yoan      (1000) yoan      (1000)    21994 2023-03-24 17:08:22.000000 tqwgp-parser-0.6.2/tests/test_definitions_parsing.py
+drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-05-17 14:48:07.368676 tqwgp-parser-0.6.2/tqwgp_parser/
+-rw-r--r--   0 yoan      (1000) yoan      (1000)      236 2022-05-09 13:44:53.000000 tqwgp-parser-0.6.2/tqwgp_parser/__init__.py
+-rw-r--r--   0 yoan      (1000) yoan      (1000)    14385 2023-03-24 17:08:22.000000 tqwgp-parser-0.6.2/tqwgp_parser/__main__.py
+-rw-r--r--   0 yoan      (1000) yoan      (1000)       64 2022-05-09 13:10:55.000000 tqwgp-parser-0.6.2/tqwgp_parser/constants.py
+drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-05-17 14:48:07.368676 tqwgp-parser-0.6.2/tqwgp_parser/files/
+-rw-r--r--   0 yoan      (1000) yoan      (1000)     3984 2022-05-11 18:58:55.000000 tqwgp-parser-0.6.2/tqwgp_parser/files/loaders.py
+-rw-r--r--   0 yoan      (1000) yoan      (1000)    12630 2023-05-17 14:46:25.000000 tqwgp-parser-0.6.2/tqwgp_parser/parser.hy
+-rw-r--r--   0 yoan      (1000) yoan      (1000)     2774 2023-05-17 14:45:09.000000 tqwgp-parser-0.6.2/tqwgp_parser/utils.hy
+drwxr-xr-x   0 yoan      (1000) yoan      (1000)        0 2023-05-17 14:48:07.368676 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/
+-rw-r--r--   0 yoan      (1000) yoan      (1000)     5279 2023-05-17 14:48:07.000000 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/PKG-INFO
+-rw-r--r--   0 yoan      (1000) yoan      (1000)      439 2023-05-17 14:48:07.000000 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 yoan      (1000) yoan      (1000)        1 2023-05-17 14:48:07.000000 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 yoan      (1000) yoan      (1000)        1 2021-01-15 12:17:06.000000 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/not-zip-safe
+-rw-r--r--   0 yoan      (1000) yoan      (1000)       57 2023-05-17 14:48:07.000000 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/requires.txt
+-rw-r--r--   0 yoan      (1000) yoan      (1000)       13 2023-05-17 14:48:07.000000 tqwgp-parser-0.6.2/tqwgp_parser.egg-info/top_level.txt
```

### Comparing `tqwgp-parser-0.6.1/LICENSE` & `tqwgp-parser-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tqwgp-parser-0.6.1/PKG-INFO` & `tqwgp-parser-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqwgp-parser
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library for parsing Talk Quote Work Get-Paid (TQWGP) text-based compliant sales and accounting documents.
 Home-page: https://github.com/YtoTech/talk-quote-work-getpaid-parser
 Author: Yoan Tournade
 Author-email: y@yoantournade.com
 License: AGPL-3.0
 Platform: any
 Description-Content-Type: text/markdown
@@ -178,9 +178,7 @@
 To contribute to the parser and specification, please wrote test samples for your modifications.
 
 The tests are written for being runned with `pytest`:
 
 ```sh
 pipenv run pytest -vv
 ```
-
-
```

### Comparing `tqwgp-parser-0.6.1/README.md` & `tqwgp-parser-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tqwgp-parser-0.6.1/setup.py` & `tqwgp-parser-0.6.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 readme_markdown = None
 with open("README.md") as f:
     readme_markdown = f.read()
 
 setup(
     name="tqwgp-parser",
-    version="0.6.1",
+    version="0.6.2",
     url="https://github.com/YtoTech/talk-quote-work-getpaid-parser",
     license="AGPL-3.0",
     author="Yoan Tournade",
     author_email="y@yoantournade.com",
     description="A library for parsing Talk Quote Work Get-Paid (TQWGP) text-based compliant sales and accounting documents.",
     long_description=readme_markdown,
     long_description_content_type="text/markdown",
@@ -36,15 +36,15 @@
     package_data={
         "tqwgp_parser": ["*.hy"],
         "tqwgp_parser": package_files("tqwgp_parser"),
     },
     zip_safe=False,
     platforms="any",
     install_requires=[
-        "hy>=1.0a4",
+        "hy>=0.26.0",
         "toolz",
         "hyrule",
         "pendulum",
         "toml",
         "pyyaml",
         "click",
         "babel",
```

### Comparing `tqwgp-parser-0.6.1/tqwgp_parser/__main__.py` & `tqwgp-parser-0.6.2/tqwgp_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `tqwgp-parser-0.6.1/tqwgp_parser/files/loaders.py` & `tqwgp-parser-0.6.2/tqwgp_parser/files/loaders.py`

 * *Files identical despite different names*

### Comparing `tqwgp-parser-0.6.1/tqwgp_parser/parser.hy` & `tqwgp-parser-0.6.2/tqwgp_parser/parser.hy`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! /usr/bin/env hy
 """
     tqwgp-parser.parser
     ~~~~~~~~~~~~~~~~~~~~~
     Parse the definitions of TWWGP quotes and invoices.
-    :copyright: (c) 2017-2021 Yoan Tournade.
+    :copyright: (c) 2017-2023 Yoan Tournade <yoan@ytotech.com>.
 """
 (import os)
 (import .utils *)
 (import hyrule [reduce])
 
 ;; Data parsing and normalization.
 
@@ -25,15 +25,15 @@
       (do
         (setv section-prestations
           (get (parse-all-prestations (get prestation "prestations") vat-rate options prestation) 0))
         (.append sections (parse-section prestation section-prestations vat-rate options))
         (.extend all-prestations section-prestations))
       (.append all-prestations (parse-prestation prestation section options))
     )) prestation))
-  (, all-prestations sections))
+  #(all-prestations sections))
 
 (defn apply-any-price-formula [price price-formula]
   (if (and
         (get-in price-formula ["enabled"] False)
         (string? price)
         (= (get price 0) "="))
     (eval (cut price 1 None))
@@ -93,22 +93,22 @@
   ;; Must accept (but ignore for total) None and string values.
   ;; Set to None if no price defined at all.
   (rounded-number
     (reduce
       (fn [total prestation]
         (setv price (apply-any-price-formula (get prestation "price") price-formula))
         (setv add-price (and (numeric? price) (or count-optional (not (get-default prestation "optional" False)))))
-        (setv prestation-total (if (numeric? price) (* price (get-default prestation "quantity" 1))))
+        (setv prestation-total (when (numeric? price) (* price (get-default prestation "quantity" 1))))
         (cond
-          [(and add-price (numeric? total))
-            (+ total prestation-total)]
-          [add-price
-            prestation-total]
-          [True
-            total]))
+          (and add-price (numeric? total))
+            (+ total prestation-total)
+          add-price
+            prestation-total
+          True
+            total))
       prestations
       None)
     rounding-decimals))
 
 (defn compute-vat [price vat-rate [rounding-decimals None]]
   """
   Compute VAT part on a numerical price.
@@ -180,15 +180,15 @@
 
 (defn recompose-batches [all-prestations]
   "Recompose batches"
   ;; Get all batch names.
   (defn unique-batch-names [prestation]
     (reduce (fn [batches prestation]
     (setv batch (get prestation "batch"))
-    (if (and (not (none? batch)) (not (in batch batches)))
+    (when (and (not (none? batch)) (not (in batch batches)))
       (.append batches batch))
       batches) all-prestations []))
   ;; Get all prestations that match the name.
   (defn batch-prestations [batch-name all-prestations]
     (list (filter (fn [prestation]
       (= (get prestation "batch") batch-name)) all-prestations)))
   ;; map-batch: get batch prestations and derive price.
@@ -199,16 +199,15 @@
       "prestations" prestations
       "price" (compute-price prestations)
     })
   (list (map map-batch (unique-batch-names all-prestations))))
 
 (defn recompose-optional-prestations [sections all-prestations]
   "Recompose optional prestations: is equal to all optional sections and all optional non-section prestations."
-  (,
-    (list (filter (fn [prestation]
+  #((list (filter (fn [prestation]
                     (and (is-optional? prestation) (not (has-optional-section? prestation))))
           all-prestations))
     (list (filter is-optional? sections))))
 
 (defn get-file-extension [filename]
   (get (.splitext os.path filename) 1))
 
@@ -245,17 +244,17 @@
     {
       "rounding-decimals" 2
     }
     kwargs
     (parse-parser-options definition)
   ]))
   (setv vat-rate (get-default definition "vat_rate" None))
-  (setv (, all-prestations sections)
+  (setv #(all-prestations sections)
     (parse-all-prestations (get definition "prestations") vat-rate options))
-  (setv (, all-optional-prestations optional-sections)
+  (setv #(all-optional-prestations optional-sections)
     (recompose-optional-prestations sections all-prestations))
   (setv has-quantities (any (map (fn [prestation] (> (get prestation "quantity") 1)) all-prestations)))
   (merge-dicts [
     ;; TODO Make the validation of the input dict recursive.
     (parse-dict-values definition
       ["title" "date" "author" "place" "sect" "client" "legal" "object" "prestations"]
       ["context" "version" "definitions" "conditions" "documents" "display_project_reference" "vat_rate"])
```

### Comparing `tqwgp-parser-0.6.1/tqwgp_parser/utils.hy` & `tqwgp-parser-0.6.2/tqwgp_parser/utils.hy`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 (import copy)
 (import toolz.itertoolz [drop])
 (require hyrule [assoc])
 
 ; Predicates.
 
 (defn numeric? [v]
-  (isinstance v (, int float)))
+  (isinstance v #(int float)))
 
 (defn string? [v]
-  (isinstance v (, str bytes)))
+  (isinstance v #(str bytes)))
 
 (defn none? [v]
   (= v None))
 
 (defn none-or-true? [value]
   (or (none? value) (bool value)))
 
@@ -26,19 +26,19 @@
   (setv parsed-dict {})
   (for [key (.keys value)] ((fn [key]
     (if (or (in key mandatories) (in key optionals))
       (assoc parsed-dict key (get value key))
       (print (.format "Ignoring key {}" key)))) key))
   ;; Check all mandatories are here.
   (for [mandatory mandatories] ((fn [mandatory]
-    (if (not (in mandatory parsed-dict))
+    (when (not (in mandatory parsed-dict))
       (raise (ValueError (.format "Missing key {}" mandatory))))) mandatory))
   ;; Affect None to non-set optionals.
   (for [optional optionals] ((fn [optional]
-    (if (not (in optional parsed-dict))
+    (when (not (in optional parsed-dict))
       (assoc parsed-dict optional None))) optional))
   parsed-dict)
 
 (defn merge-dicts [dicts]
   (setv merged (.deepcopy copy (get dicts 0)))
   (for [one-dict (drop 1 dicts)] ((fn [one-dict]
     (.update merged one-dict)) one-dict))
@@ -50,23 +50,23 @@
 ;     (if (pred (get a-dict it) it)
 ;       (assoc new-dict it (get a-dict it))))
 ;   new-dict)
 (defn filter-dict [a-dict pred]
   (setv new-dict {})
   (for [key (.keys a-dict)]
     ((fn [key]
-      (if (pred (get a-dict key) key)
+      (when (pred (get a-dict key) key)
         (assoc new-dict key (get a-dict key))))
       key))
   new-dict)
 
 (defn pick-by [pred value]
   (setv new-value {})
   (for [key (.keys value)] ((fn [key]
-    (if (pred key)
+    (when (pred key)
       (assoc new-value key (get value key)))) key))
   new-value)
 
 (defn get-default [value key default]
   (if (in key value)
     (get value key)
     default))
@@ -85,18 +85,17 @@
       default)))
 
 ; Lists.
 
 (defn find-in-list [l pred]
   (setv element None)
   (for [item l] ((fn [item])
-    (if (pred item)
-      (do
-        (setv element item)
-        (break))) l))
+    (when (pred item)
+      (setv element item)
+      (break)) l))
   element)
 
 
 ; Numbers.
 
 (defn simplest-numerical-format [price]
   (if (.is_integer (float price))
```

### Comparing `tqwgp-parser-0.6.1/tqwgp_parser.egg-info/PKG-INFO` & `tqwgp-parser-0.6.2/tqwgp_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqwgp-parser
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library for parsing Talk Quote Work Get-Paid (TQWGP) text-based compliant sales and accounting documents.
 Home-page: https://github.com/YtoTech/talk-quote-work-getpaid-parser
 Author: Yoan Tournade
 Author-email: y@yoantournade.com
 License: AGPL-3.0
 Platform: any
 Description-Content-Type: text/markdown
@@ -178,9 +178,7 @@
 To contribute to the parser and specification, please wrote test samples for your modifications.
 
 The tests are written for being runned with `pytest`:
 
 ```sh
 pipenv run pytest -vv
 ```
-
-
```

