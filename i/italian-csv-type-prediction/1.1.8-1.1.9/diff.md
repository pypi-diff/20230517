# Comparing `tmp/italian_csv_type_prediction-1.1.8.tar.gz` & `tmp/italian_csv_type_prediction-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\italian_csv_type_prediction-1.1.8.tar", last modified: Wed Apr  1 18:00:30 2020, max compression
+gzip compressed data, was "dist\italian_csv_type_prediction-1.1.9.tar", last modified: Wed Apr  1 18:44:50 2020, max compression
```

## Comparing `italian_csv_type_prediction-1.1.8.tar` & `italian_csv_type_prediction-1.1.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/
--rw-rw-rw-   0        0        0      109 2020-03-21 21:38:52.000000 italian_csv_type_prediction-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5116 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3806 2020-03-26 16:59:56.000000 italian_csv_type_prediction-1.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/
--rw-rw-rw-   0        0        0       64 2020-04-01 09:58:57.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/__init__.py
--rw-rw-rw-   0        0        0       82 2020-04-01 17:59:54.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/__version__.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/column_types/
--rw-rw-rw-   0        0        0        0 2020-04-01 09:18:48.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/column_types/__init__.py
--rw-rw-rw-   0        0        0      976 2020-04-01 09:26:40.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/column_types/column_type_predictor.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/dataframe_generators/
--rw-rw-rw-   0        0        0      100 2020-04-01 11:52:14.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/dataframe_generators/__init__.py
--rw-rw-rw-   0        0        0     3350 2020-04-01 16:13:15.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/dataframe_generators/simple_dataset_generator.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/
--rw-rw-rw-   0        0        0    56974 2020-03-22 17:58:44.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Address.json.gz
--rw-rw-rw-   0        0        0       83 2020-04-01 09:15:52.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/BiologicalSex.json.gz
--rw-rw-rw-   0        0        0    10281 2020-03-22 23:24:05.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/CAP.json.gz
--rw-rw-rw-   0        0        0   103603 2020-03-22 14:35:22.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/CodiceFiscale.json.gz
--rw-rw-rw-   0        0        0     1012 2020-03-22 14:19:18.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Country.json.gz
--rw-rw-rw-   0        0        0      446 2020-03-22 14:18:57.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/CountryCode.json.gz
--rw-rw-rw-   0        0        0    14930 2020-03-22 20:29:13.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/IVA.json.gz
--rw-rw-rw-   0        0        0    36886 2020-03-22 14:16:33.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Municipality.json.gz
--rw-rw-rw-   0        0        0   700882 2020-03-22 19:25:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Name.json.gz
--rw-rw-rw-   0        0        0      287 2020-03-22 14:15:44.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/ProvinceCode.json.gz
--rw-rw-rw-   0        0        0      187 2020-03-22 14:16:05.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Region.json.gz
--rw-rw-rw-   0        0        0     8709 2020-03-22 14:34:15.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/String.json.gz
--rw-rw-rw-   0        0        0   424018 2020-03-22 19:26:25.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Surname.json.gz
--rw-rw-rw-   0        0        0      815 2020-04-01 16:13:20.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/__init__.py
--rw-rw-rw-   0        0        0      395 2020-03-30 13:30:25.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/address_starters.json.gz
--rw-rw-rw-   0        0        0    31190 2020-03-22 12:38:33.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/date.json.gz
--rw-rw-rw-   0        0        0     4449 2020-03-22 10:54:57.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/email.json.gz
--rw-rw-rw-   0        0        0    34594 2020-03-22 12:39:13.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/euro.json.gz
--rw-rw-rw-   0        0        0     1464 2020-04-01 16:17:24.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/load_json.py
--rw-rw-rw-   0        0        0       89 2020-04-01 13:48:12.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/nan.json.gz
--rw-rw-rw-   0        0        0     2479 2020-03-22 11:33:28.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/phone.json.gz
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/embedding/
--rw-rw-rw-   0        0        0       95 2020-04-01 11:49:15.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/embedding/__init__.py
--rw-rw-rw-   0        0        0     1358 2020-04-01 12:05:48.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/embedding/dataframe_embedding.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/
--rw-rw-rw-   0        0        0       72 2020-04-01 09:58:36.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/__init__.py
--rw-rw-rw-   0        0        0     2253 2020-04-01 16:13:47.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/test.pkl.gz
--rw-rw-rw-   0        0        0     3826 2020-04-01 17:59:39.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/type_predictor.pkl.gz
--rw-rw-rw-   0        0        0     1333 2020-04-01 15:21:17.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/type_predictor.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/
--rw-rw-rw-   0        0        0      542 2020-04-01 17:53:09.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/CAP_type.py
--rw-rw-rw-   0        0        0      535 2020-04-01 17:41:00.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/IVA_type.py
--rw-rw-rw-   0        0        0       91 2020-04-01 09:48:33.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/__init__.py
--rw-rw-rw-   0        0        0      484 2020-03-30 13:33:07.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/address_type.py
--rw-rw-rw-   0        0        0     1831 2020-04-01 16:13:05.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/any_simple_type.py
--rw-rw-rw-   0        0        0      571 2020-04-01 09:16:19.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/biological_sex_type.py
--rw-rw-rw-   0        0        0      371 2020-03-30 11:54:01.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/codice_fiscale_type.py
--rw-rw-rw-   0        0        0      565 2020-03-30 12:40:01.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/country_code_type.py
--rw-rw-rw-   0        0        0      548 2020-03-30 12:39:19.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/country_type.py
--rw-rw-rw-   0        0        0      444 2020-03-30 13:20:07.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/currency_type.py
--rw-rw-rw-   0        0        0     1244 2020-04-01 17:42:29.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/date_type.py
--rw-rw-rw-   0        0        0      342 2020-03-30 12:23:03.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/email_type.py
--rw-rw-rw-   0        0        0      500 2020-03-30 11:38:53.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/float_type.py
--rw-rw-rw-   0        0        0      326 2020-03-30 11:42:54.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/integer_type.py
--rw-rw-rw-   0        0        0      568 2020-03-30 12:49:01.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/municipality_type.py
--rw-rw-rw-   0        0        0     1029 2020-03-30 13:08:11.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/name_type.py
--rw-rw-rw-   0        0        0      627 2020-04-01 13:49:55.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/nan_type.py
--rw-rw-rw-   0        0        0      773 2020-03-30 13:03:16.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/partial_set_type_predictor.py
--rw-rw-rw-   0        0        0      515 2020-03-30 13:44:09.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/phone_number_type.py
--rw-rw-rw-   0        0        0      571 2020-03-30 12:48:14.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/province_code_type.py
--rw-rw-rw-   0        0        0      566 2020-03-30 11:38:29.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/regex_type_predictor.py
--rw-rw-rw-   0        0        0      542 2020-03-30 12:47:00.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/region_type.py
--rw-rw-rw-   0        0        0     1129 2020-03-30 12:38:46.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/set_type_predictor.py
--rw-rw-rw-   0        0        0      763 2020-03-30 11:37:45.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/simple_type.py
--rw-rw-rw-   0        0        0      263 2020-03-30 11:52:59.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/string_type.py
--rw-rw-rw-   0        0        0     1036 2020-03-30 13:07:22.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/surname_type.py
--rw-rw-rw-   0        0        0      506 2020-04-01 15:32:37.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/year_type.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/
--rw-rw-rw-   0        0        0     5116 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4307 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      227 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/old_test_suite/
--rw-rw-rw-   0        0        0        0 2020-03-02 14:47:56.000000 italian_csv_type_prediction-1.1.8/old_test_suite/__init__.py
--rw-rw-rw-   0        0        0      159 2020-03-22 20:38:19.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_generate_training_set.py
--rw-rw-rw-   0        0        0      169 2020-03-22 16:56:41.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_address.py
--rw-rw-rw-   0        0        0      207 2020-03-22 22:31:36.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_cap.py
--rw-rw-rw-   0        0        0      160 2020-03-22 14:03:52.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_cf.py
--rw-rw-rw-   0        0        0      227 2020-03-22 14:36:37.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_country.py
--rw-rw-rw-   0        0        0      288 2020-03-22 14:39:49.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_country_code.py
--rw-rw-rw-   0        0        0      229 2020-03-22 19:31:26.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_date.py
--rw-rw-rw-   0        0        0      244 2020-03-22 19:32:54.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_euro.py
--rw-rw-rw-   0        0        0      245 2020-03-22 19:27:52.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_house_number.py
--rw-rw-rw-   0        0        0      207 2020-03-22 19:34:10.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_iva.py
--rw-rw-rw-   0        0        0      302 2020-03-22 14:36:53.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_municipality.py
--rw-rw-rw-   0        0        0      315 2020-03-22 14:36:15.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_name.py
--rw-rw-rw-   0        0        0      253 2020-03-22 14:18:46.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_nan.py
--rw-rw-rw-   0        0        0      265 2020-03-22 14:35:34.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_province_codes.py
--rw-rw-rw-   0        0        0      213 2020-03-22 14:12:31.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_region.py
--rw-rw-rw-   0        0        0      294 2020-03-22 14:24:01.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_surname.py
--rw-rw-rw-   0        0        0      203 2020-03-22 19:30:25.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_is_year.py
--rw-rw-rw-   0        0        0      988 2020-03-14 17:38:27.000000 italian_csv_type_prediction-1.1.8/old_test_suite/test_set_prediction.py
-drwxrwxrwx   0        0        0        0 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/old_test_suite/utils/
--rw-rw-rw-   0        0        0     2382 2020-03-22 23:02:52.000000 italian_csv_type_prediction-1.1.8/old_test_suite/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2020-04-01 18:00:30.000000 italian_csv_type_prediction-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2096 2020-04-01 11:25:30.000000 italian_csv_type_prediction-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/
+-rw-rw-rw-   0        0        0      109 2020-03-21 21:38:52.000000 italian_csv_type_prediction-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5116 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3806 2020-03-26 16:59:56.000000 italian_csv_type_prediction-1.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/
+-rw-rw-rw-   0        0        0       64 2020-04-01 09:58:57.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/__init__.py
+-rw-rw-rw-   0        0        0       82 2020-04-01 18:44:30.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/__version__.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/column_types/
+-rw-rw-rw-   0        0        0        0 2020-04-01 09:18:48.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/column_types/__init__.py
+-rw-rw-rw-   0        0        0      976 2020-04-01 09:26:40.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/column_types/column_type_predictor.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/dataframe_generators/
+-rw-rw-rw-   0        0        0      100 2020-04-01 11:52:14.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/dataframe_generators/__init__.py
+-rw-rw-rw-   0        0        0     3350 2020-04-01 16:13:15.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/dataframe_generators/simple_dataset_generator.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/
+-rw-rw-rw-   0        0        0    56974 2020-03-22 17:58:44.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Address.json.gz
+-rw-rw-rw-   0        0        0       83 2020-04-01 09:15:52.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/BiologicalSex.json.gz
+-rw-rw-rw-   0        0        0    10281 2020-03-22 23:24:05.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/CAP.json.gz
+-rw-rw-rw-   0        0        0   103603 2020-03-22 14:35:22.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/CodiceFiscale.json.gz
+-rw-rw-rw-   0        0        0     1012 2020-03-22 14:19:18.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Country.json.gz
+-rw-rw-rw-   0        0        0      446 2020-03-22 14:18:57.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/CountryCode.json.gz
+-rw-rw-rw-   0        0        0    14930 2020-03-22 20:29:13.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/IVA.json.gz
+-rw-rw-rw-   0        0        0    36886 2020-03-22 14:16:33.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Municipality.json.gz
+-rw-rw-rw-   0        0        0   700882 2020-03-22 19:25:30.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Name.json.gz
+-rw-rw-rw-   0        0        0      287 2020-03-22 14:15:44.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/ProvinceCode.json.gz
+-rw-rw-rw-   0        0        0      187 2020-03-22 14:16:05.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Region.json.gz
+-rw-rw-rw-   0        0        0     8709 2020-03-22 14:34:15.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/String.json.gz
+-rw-rw-rw-   0        0        0   424018 2020-03-22 19:26:25.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Surname.json.gz
+-rw-rw-rw-   0        0        0      815 2020-04-01 16:13:20.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/__init__.py
+-rw-rw-rw-   0        0        0      395 2020-03-30 13:30:25.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/address_starters.json.gz
+-rw-rw-rw-   0        0        0    31190 2020-03-22 12:38:33.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/date.json.gz
+-rw-rw-rw-   0        0        0     4449 2020-03-22 10:54:57.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/email.json.gz
+-rw-rw-rw-   0        0        0    34594 2020-03-22 12:39:13.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/euro.json.gz
+-rw-rw-rw-   0        0        0     1464 2020-04-01 16:17:24.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/load_json.py
+-rw-rw-rw-   0        0        0       89 2020-04-01 13:48:12.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/nan.json.gz
+-rw-rw-rw-   0        0        0     2479 2020-03-22 11:33:28.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/phone.json.gz
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/embedding/
+-rw-rw-rw-   0        0        0       95 2020-04-01 11:49:15.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/embedding/__init__.py
+-rw-rw-rw-   0        0        0     1358 2020-04-01 12:05:48.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/embedding/dataframe_embedding.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/
+-rw-rw-rw-   0        0        0       72 2020-04-01 09:58:36.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/__init__.py
+-rw-rw-rw-   0        0        0     2253 2020-04-01 16:13:47.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/test.pkl.gz
+-rw-rw-rw-   0        0        0     7345 2020-04-01 18:44:29.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/type_predictor.pkl.gz
+-rw-rw-rw-   0        0        0     1333 2020-04-01 15:21:17.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/type_predictor.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/
+-rw-rw-rw-   0        0        0      542 2020-04-01 17:53:09.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/CAP_type.py
+-rw-rw-rw-   0        0        0      535 2020-04-01 17:41:00.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/IVA_type.py
+-rw-rw-rw-   0        0        0       91 2020-04-01 09:48:33.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/__init__.py
+-rw-rw-rw-   0        0        0      484 2020-03-30 13:33:07.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/address_type.py
+-rw-rw-rw-   0        0        0     1831 2020-04-01 16:13:05.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/any_simple_type.py
+-rw-rw-rw-   0        0        0      571 2020-04-01 09:16:19.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/biological_sex_type.py
+-rw-rw-rw-   0        0        0      371 2020-03-30 11:54:01.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/codice_fiscale_type.py
+-rw-rw-rw-   0        0        0      565 2020-03-30 12:40:01.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/country_code_type.py
+-rw-rw-rw-   0        0        0      548 2020-03-30 12:39:19.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/country_type.py
+-rw-rw-rw-   0        0        0      444 2020-03-30 13:20:07.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/currency_type.py
+-rw-rw-rw-   0        0        0     1244 2020-04-01 17:42:29.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/date_type.py
+-rw-rw-rw-   0        0        0      342 2020-03-30 12:23:03.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/email_type.py
+-rw-rw-rw-   0        0        0      500 2020-03-30 11:38:53.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/float_type.py
+-rw-rw-rw-   0        0        0      326 2020-03-30 11:42:54.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/integer_type.py
+-rw-rw-rw-   0        0        0      568 2020-03-30 12:49:01.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/municipality_type.py
+-rw-rw-rw-   0        0        0     1029 2020-03-30 13:08:11.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/name_type.py
+-rw-rw-rw-   0        0        0      627 2020-04-01 13:49:55.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/nan_type.py
+-rw-rw-rw-   0        0        0      773 2020-03-30 13:03:16.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/partial_set_type_predictor.py
+-rw-rw-rw-   0        0        0      515 2020-03-30 13:44:09.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/phone_number_type.py
+-rw-rw-rw-   0        0        0      571 2020-03-30 12:48:14.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/province_code_type.py
+-rw-rw-rw-   0        0        0      566 2020-03-30 11:38:29.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/regex_type_predictor.py
+-rw-rw-rw-   0        0        0      542 2020-03-30 12:47:00.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/region_type.py
+-rw-rw-rw-   0        0        0     1129 2020-03-30 12:38:46.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/set_type_predictor.py
+-rw-rw-rw-   0        0        0      763 2020-03-30 11:37:45.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/simple_type.py
+-rw-rw-rw-   0        0        0      263 2020-03-30 11:52:59.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/string_type.py
+-rw-rw-rw-   0        0        0     1036 2020-03-30 13:07:22.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/surname_type.py
+-rw-rw-rw-   0        0        0      506 2020-04-01 15:32:37.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/year_type.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/
+-rw-rw-rw-   0        0        0     5116 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4307 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      227 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/old_test_suite/
+-rw-rw-rw-   0        0        0        0 2020-03-02 14:47:56.000000 italian_csv_type_prediction-1.1.9/old_test_suite/__init__.py
+-rw-rw-rw-   0        0        0      159 2020-03-22 20:38:19.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_generate_training_set.py
+-rw-rw-rw-   0        0        0      169 2020-03-22 16:56:41.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_address.py
+-rw-rw-rw-   0        0        0      207 2020-03-22 22:31:36.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_cap.py
+-rw-rw-rw-   0        0        0      160 2020-03-22 14:03:52.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_cf.py
+-rw-rw-rw-   0        0        0      227 2020-03-22 14:36:37.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_country.py
+-rw-rw-rw-   0        0        0      288 2020-03-22 14:39:49.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_country_code.py
+-rw-rw-rw-   0        0        0      229 2020-03-22 19:31:26.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_date.py
+-rw-rw-rw-   0        0        0      244 2020-03-22 19:32:54.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_euro.py
+-rw-rw-rw-   0        0        0      245 2020-03-22 19:27:52.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_house_number.py
+-rw-rw-rw-   0        0        0      207 2020-03-22 19:34:10.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_iva.py
+-rw-rw-rw-   0        0        0      302 2020-03-22 14:36:53.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_municipality.py
+-rw-rw-rw-   0        0        0      315 2020-03-22 14:36:15.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_name.py
+-rw-rw-rw-   0        0        0      253 2020-03-22 14:18:46.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_nan.py
+-rw-rw-rw-   0        0        0      265 2020-03-22 14:35:34.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_province_codes.py
+-rw-rw-rw-   0        0        0      213 2020-03-22 14:12:31.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_region.py
+-rw-rw-rw-   0        0        0      294 2020-03-22 14:24:01.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_surname.py
+-rw-rw-rw-   0        0        0      203 2020-03-22 19:30:25.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_is_year.py
+-rw-rw-rw-   0        0        0      988 2020-03-14 17:38:27.000000 italian_csv_type_prediction-1.1.9/old_test_suite/test_set_prediction.py
+drwxrwxrwx   0        0        0        0 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/old_test_suite/utils/
+-rw-rw-rw-   0        0        0     2382 2020-03-22 23:02:52.000000 italian_csv_type_prediction-1.1.9/old_test_suite/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2020-04-01 18:44:50.000000 italian_csv_type_prediction-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2096 2020-04-01 11:25:30.000000 italian_csv_type_prediction-1.1.9/setup.py
```

### Comparing `italian_csv_type_prediction-1.1.8/PKG-INFO` & `italian_csv_type_prediction-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian_csv_type_prediction
-Version: 1.1.8
+Version: 1.1.9
 Summary: Attempt at predicting common types in CSVs about Italian people and places using Spacy NLP tool.
 Home-page: https://github.com/LucaCappelletti94/italian_csv_type_prediction
 Author: LucaCappelletti94
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: italian_csv_type_prediction
         =========================================================================================
```

### Comparing `italian_csv_type_prediction-1.1.8/README.rst` & `italian_csv_type_prediction-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/column_types/column_type_predictor.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/column_types/column_type_predictor.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/dataframe_generators/simple_dataset_generator.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/dataframe_generators/simple_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Address.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Address.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/CAP.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/CAP.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/CodiceFiscale.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/CodiceFiscale.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Country.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Country.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/IVA.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/IVA.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Municipality.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Municipality.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Name.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Name.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/String.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/String.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/Surname.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/Surname.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/__init__.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/date.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/date.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/email.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/email.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/euro.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/euro.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/load_json.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/load_json.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/datasets/phone.json.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/datasets/phone.json.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/embedding/dataframe_embedding.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/embedding/dataframe_embedding.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/test.pkl.gz` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/test.pkl.gz`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/models/type_predictor.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/models/type_predictor.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/CAP_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/CAP_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/IVA_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/IVA_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/any_simple_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/any_simple_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/biological_sex_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/biological_sex_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/country_code_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/country_code_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/country_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/country_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/date_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/date_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/municipality_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/municipality_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/name_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/name_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/nan_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/nan_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/partial_set_type_predictor.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/partial_set_type_predictor.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/phone_number_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/province_code_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/province_code_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/regex_type_predictor.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/regex_type_predictor.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/region_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/region_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/set_type_predictor.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/set_type_predictor.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/simple_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/simple_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction/simple_types/surname_type.py` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction/simple_types/surname_type.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/PKG-INFO` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-csv-type-prediction
-Version: 1.1.8
+Version: 1.1.9
 Summary: Attempt at predicting common types in CSVs about Italian people and places using Spacy NLP tool.
 Home-page: https://github.com/LucaCappelletti94/italian_csv_type_prediction
 Author: LucaCappelletti94
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: italian_csv_type_prediction
         =========================================================================================
```

### Comparing `italian_csv_type_prediction-1.1.8/italian_csv_type_prediction.egg-info/SOURCES.txt` & `italian_csv_type_prediction-1.1.9/italian_csv_type_prediction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/old_test_suite/test_set_prediction.py` & `italian_csv_type_prediction-1.1.9/old_test_suite/test_set_prediction.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/old_test_suite/utils/__init__.py` & `italian_csv_type_prediction-1.1.9/old_test_suite/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `italian_csv_type_prediction-1.1.8/setup.py` & `italian_csv_type_prediction-1.1.9/setup.py`

 * *Files identical despite different names*

