# Comparing `tmp/sarus_data_spec_public-3.2.1.dev5.tar.gz` & `tmp/sarus_data_spec_public-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.2.1.dev5.tar", last modified: Fri May 12 12:50:50 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.2.2.tar", last modified: Mon May 15 10:12:58 2023, max compression
```

## Comparing `sarus_data_spec_public-3.2.1.dev5.tar` & `sarus_data_spec_public-3.2.2.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.291256 sarus_data_spec_public-3.2.1.dev5/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-12 12:50:50.291256 sarus_data_spec_public-3.2.1.dev5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.237252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.239252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5679 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.240252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3712 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.241252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.242252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.245252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11237 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)    20331 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.246252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    29039 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.247252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8793 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.248252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.249252 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.250253 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.250253 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.253253 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11451 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.255253 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    74578 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.260253 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38717 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     7004 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    18437 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.264253 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10332 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.266254 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.287255 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     6521 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    74241 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29134 2023-05-12 12:50:39.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.288255 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35688 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:50:50.291256 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-12 12:50:50.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7837 2023-05-12 12:50:50.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 12:50:50.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 12:50:50.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-12 12:50:50.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-12 12:50:50.000000 sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-12 12:50:50.292255 sarus_data_spec_public-3.2.1.dev5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-12 12:50:27.000000 sarus_data_spec_public-3.2.1.dev5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.204516 sarus_data_spec_public-3.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-15 10:12:58.204516 sarus_data_spec_public-3.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.151515 sarus_data_spec_public-3.2.2/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      825 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.154515 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.154515 sarus_data_spec_public-3.2.2/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3712 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.155515 sarus_data_spec_public-3.2.2/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.157515 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.159515 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11237 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    20331 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.160515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    29039 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.161515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8793 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.162515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.163515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.163515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.164515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.168515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11451 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.169515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    74578 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.174515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38717 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     7004 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    18437 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.178515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10337 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.180515 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.200515 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    74241 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29134 2023-05-15 10:12:47.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.202515 sarus_data_spec_public-3.2.2/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35688 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:12:58.204516 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-15 10:12:58.000000 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7837 2023-05-15 10:12:58.000000 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 10:12:58.000000 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 10:12:58.000000 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-15 10:12:58.000000 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 10:12:58.000000 sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-15 10:12:58.205515 sarus_data_spec_public-3.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-05-15 10:12:35.000000 sarus_data_spec_public-3.2.2/setup.py
```

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.2.1.dev5'
+VERSION: Final[str] = '3.2.2'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/admin_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -66,18 +66,28 @@
             field_names = list(batch.schema.names)
             index_cols = pandas_index_columns(batch.schema)
             index_arrays = [
                 batch.columns[field_names.index(col)]
                 for col in pandas_index_columns(batch.schema)
             ]
             data_arrays = batch.columns[field_names.index(DATA)].flatten()
+            arrays = index_arrays + data_arrays
+            names = index_cols + data_cols
 
-            new_struct_array = pa.StructArray.from_arrays(
-                index_arrays + data_arrays, index_cols + data_cols
-            )
+            if len(arrays) != len(names):
+                raise ValueError(
+                    f"Incompatible number of arrays {len(arrays)} and"
+                    f" names {len(names)}.\n"
+                    f"Names are index cols {index_cols} and data "
+                    f"cols {data_cols}.\n"
+                    f"There are {len(index_arrays)} index arrays "
+                    f"and {len(data_arrays)} data arrays.\n"
+                    f"Arrow batch schema is {batch.schema}."
+                )
+            new_struct_array = pa.StructArray.from_arrays(arrays, names)
             data_batch = pa.RecordBatch.from_struct_array(new_struct_array)
             data_batch = data_batch.replace_schema_metadata(
                 batch.schema.metadata
             )
             yield data_batch
 
     return extract_data(batches_async_it)
```

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.2.2/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 table_map = table_mapping(
                     tables=current_schema.tables(),
                     sarus_schema_name=current_schema.name(),
                 )
 
                 parent_query = rename_tables.rename_tables(
                     t.cast(str, query),
-                    t.cast(t.Dict[st.Path, t.Tuple[str]], table_map),
+                    t.cast(t.Dict[st.Path, t.Tuple[str, ...]], table_map),
                 )
         else:
             transfo_renamed = {
                 name_encoder(
                     names=tuple(tab_name.to_strings_list()[0]),
                     length=10,
                 ): query_str
```

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/path.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/size.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/status.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/type.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.2.2/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.2.2/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/setup.cfg` & `sarus_data_spec_public-3.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev5/setup.py` & `sarus_data_spec_public-3.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.2.1.dev5')
+    setup(version='3.2.2')
```
