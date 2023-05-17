# Comparing `tmp/barectf-3.1.1.tar.gz` & `tmp/barectf-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barectf-3.1.1.tar", max compression
+gzip compressed data, was "barectf-3.1.2.tar", max compression
```

## Comparing `barectf-3.1.1.tar` & `barectf-3.1.2.tar`

### file list

```diff
@@ -1,97 +1,96 @@
--rw-r--r--   0        0        0     1118 2020-09-25 13:31:14.688037 barectf-3.1.1/LICENSE
--rw-r--r--   0        0        0     4731 2020-09-25 13:31:14.688037 barectf-3.1.1/barectf/__init__.py
--rw-r--r--   0        0        0    13645 2020-09-25 13:31:14.688037 barectf-3.1.1/barectf/argpar.py
--rw-r--r--   0        0        0    33067 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/cgen.py
--rw-r--r--   0        0        0    21913 2020-09-25 13:31:14.688037 barectf-3.1.1/barectf/cli.py
--rw-r--r--   0        0        0     3680 2020-09-25 13:31:14.688037 barectf-3.1.1/barectf/codegen.py
--rw-r--r--   0        0        0    31310 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/config.py
--rw-r--r--   0        0        0     2732 2020-09-25 13:31:14.688037 barectf-3.1.1/barectf/config_file.py
--rw-r--r--   0        0        0     5223 2020-09-25 13:31:14.688037 barectf-3.1.1/barectf/config_parse.py
--rw-r--r--   0        0        0    31311 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/config_parse_common.py
--rw-r--r--   0        0        0    36669 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/config_parse_v2.py
--rw-r--r--   0        0        0    60747 2022-11-21 20:57:21.207223 barectf-3.1.1/barectf/config_parse_v3.py
--rw-r--r--   0        0        0      469 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/2/lttng-ust-log-levels.yaml
--rw-r--r--   0        0        0      371 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/2/stdfloat.yaml
--rw-r--r--   0        0        0     2327 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/2/stdint.yaml
--rw-r--r--   0        0        0      349 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/2/stdmisc.yaml
--rw-r--r--   0        0        0      657 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/2/trace-basic.yaml
--rw-r--r--   0        0        0      478 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/3/lttng-ust-log-levels.yaml
--rw-r--r--   0        0        0     3153 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/3/stdint.yaml
--rw-r--r--   0        0        0      185 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/3/stdmisc.yaml
--rw-r--r--   0        0        0      785 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/include/3/stdreal.yaml
--rw-r--r--   0        0        0     1410 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/clock-type-pre-include.yaml
--rw-r--r--   0        0        0     1416 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/config-min.yaml
--rw-r--r--   0        0        0     3784 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/config-pre-field-type-expansion.yaml
--rw-r--r--   0        0        0     1440 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/config-pre-include.yaml
--rw-r--r--   0        0        0     9509 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/config.yaml
--rw-r--r--   0        0        0     1598 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/dst-pre-include.yaml
--rw-r--r--   0        0        0     1410 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/ert-pre-include.yaml
--rw-r--r--   0        0        0     8456 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/field-type.yaml
--rw-r--r--   0        0        0     1372 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/include-prop.yaml
--rw-r--r--   0        0        0     1868 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/metadata-pre-include.yaml
--rw-r--r--   0        0        0     1410 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/2/trace-type-pre-include.yaml
--rw-r--r--   0        0        0     1410 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/3/clock-type-pre-include.yaml
--rw-r--r--   0        0        0     6731 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/schemas/config/3/config-pre-field-type-expansion.yaml
--rw-r--r--   0        0        0     1431 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/3/config-pre-include.yaml
--rw-r--r--   0        0        0     2782 2020-09-25 13:31:14.691371 barectf-3.1.1/barectf/schemas/config/3/config-pre-log-level-alias-sub.yaml
--rw-r--r--   0        0        0    10360 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/schemas/config/3/config.yaml
--rw-r--r--   0        0        0     1610 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/3/dst-pre-include.yaml
--rw-r--r--   0        0        0     1410 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/3/ert-pre-include.yaml
--rw-r--r--   0        0        0    10085 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/3/field-type.yaml
--rw-r--r--   0        0        0     1372 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/3/include-prop.yaml
--rw-r--r--   0        0        0     1483 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/3/trace-pre-include.yaml
--rw-r--r--   0        0        0     1803 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/3/trace-type-pre-include.yaml
--rw-r--r--   0        0        0     4257 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/schemas/config/common/common.yaml
--rw-r--r--   0        0        0     3080 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/template.py
--rw-r--r--   0        0        0     1372 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/align-statements-comment.j2
--rw-r--r--   0        0        0     2497 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/barectf.c-macros.j2
--rw-r--r--   0        0        0    16204 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/templates/c/barectf.c.j2
--rw-r--r--   0        0        0     5692 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/templates/c/barectf.h.j2
--rw-r--r--   0        0        0     8306 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/bitfield.h.j2
--rw-r--r--   0        0        0     1451 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/close-func-proto.j2
--rw-r--r--   0        0        0     2281 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/common.j2
--rw-r--r--   0        0        0     1539 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/ctx-init-func-proto.j2
--rw-r--r--   0        0        0     1359 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/func-proto-params.j2
--rw-r--r--   0        0        0     1497 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/open-func-proto.j2
--rw-r--r--   0        0        0     1254 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-align-statements.j2
--rw-r--r--   0        0        0     1591 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-array-statements.j2
--rw-r--r--   0        0        0     2004 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-bit-array-statements.j2
--rw-r--r--   0        0        0     1330 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-dst-id-statements.j2
--rw-r--r--   0        0        0     1332 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-dynamic-array-statements.j2
--rw-r--r--   0        0        0     1333 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-ert-id-statements.j2
--rw-r--r--   0        0        0     1402 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-int-statements.j2
--rw-r--r--   0        0        0     1331 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-magic-statements.j2
--rw-r--r--   0        0        0     1340 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-packet-size-statements.j2
--rw-r--r--   0        0        0     1658 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-real-statements.j2
--rw-r--r--   0        0        0     1365 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-saved-int-statements.j2
--rw-r--r--   0        0        0     1328 2022-11-21 20:53:07.954558 barectf-3.1.1/barectf/templates/c/serialize-write-seq-num-statements.j2
--rw-r--r--   0        0        0     1352 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-skip-save-statements.j2
--rw-r--r--   0        0        0     1212 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-statements-comment.j2
--rw-r--r--   0        0        0     1280 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-static-array-statements.j2
--rw-r--r--   0        0        0     1317 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-string-statements.j2
--rw-r--r--   0        0        0     1511 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-struct-statements.j2
--rw-r--r--   0        0        0     1372 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-timestamp-statements.j2
--rw-r--r--   0        0        0     1434 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/serialize-write-uuid-statements.j2
--rw-r--r--   0        0        0     1249 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-align-statements.j2
--rw-r--r--   0        0        0     1586 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-write-array-statements.j2
--rw-r--r--   0        0        0     1251 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-write-bit-array-statements.j2
--rw-r--r--   0        0        0     1327 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-write-dynamic-array-statements.j2
--rw-r--r--   0        0        0     1275 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-write-static-array-statements.j2
--rw-r--r--   0        0        0     1325 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-write-string-statements.j2
--rw-r--r--   0        0        0     1522 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/size-write-struct-statements.j2
--rw-r--r--   0        0        0     1540 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/c/trace-func-proto.j2
--rw-r--r--   0        0        0     1482 2020-09-25 13:31:14.694704 barectf-3.1.1/barectf/templates/common.j2
--rw-r--r--   0        0        0     1452 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/license-header-footer.j2
--rw-r--r--   0        0        0     2396 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/license-header.j2
--rw-r--r--   0        0        0     1512 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/metadata/enum-ft.j2
--rw-r--r--   0        0        0     1464 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/metadata/int-ft.j2
--rw-r--r--   0        0        0     3607 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/metadata/metadata.j2
--rw-r--r--   0        0        0     1336 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/metadata/real-ft.j2
--rw-r--r--   0        0        0     1203 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/metadata/str-ft.j2
--rw-r--r--   0        0        0     1422 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/templates/metadata/struct-ft.j2
--rw-r--r--   0        0        0     4446 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/tsdl182gen.py
--rw-r--r--   0        0        0     1395 2020-09-25 13:31:14.698037 barectf-3.1.1/barectf/typing.py
--rw-r--r--   0        0        0     1332 2022-11-21 20:58:04.554343 barectf-3.1.1/barectf/version.py
--rw-r--r--   0        0        0     2549 2022-11-21 20:58:06.241027 barectf-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 barectf-3.1.1/setup.py
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 barectf-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1118 2023-03-31 15:15:21.903167 barectf-3.1.2/LICENSE
+-rw-r--r--   0        0        0     4820 2023-05-17 18:39:58.179981 barectf-3.1.2/barectf/__init__.py
+-rw-r--r--   0        0        0    13645 2023-03-31 15:15:21.903167 barectf-3.1.2/barectf/argpar.py
+-rw-r--r--   0        0        0    33068 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/cgen.py
+-rw-r--r--   0        0        0    21913 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/cli.py
+-rw-r--r--   0        0        0     3680 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/codegen.py
+-rw-r--r--   0        0        0    32602 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/config.py
+-rw-r--r--   0        0        0     2732 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/config_file.py
+-rw-r--r--   0        0        0     5223 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/config_parse.py
+-rw-r--r--   0        0        0    31311 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/config_parse_common.py
+-rw-r--r--   0        0        0    36730 2023-05-17 18:39:58.179981 barectf-3.1.2/barectf/config_parse_v2.py
+-rw-r--r--   0        0        0    61260 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/config_parse_v3.py
+-rw-r--r--   0        0        0      469 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/2/lttng-ust-log-levels.yaml
+-rw-r--r--   0        0        0      371 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/2/stdfloat.yaml
+-rw-r--r--   0        0        0     2327 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/2/stdint.yaml
+-rw-r--r--   0        0        0      349 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/2/stdmisc.yaml
+-rw-r--r--   0        0        0      657 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/2/trace-basic.yaml
+-rw-r--r--   0        0        0      478 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/3/lttng-ust-log-levels.yaml
+-rw-r--r--   0        0        0     3153 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/3/stdint.yaml
+-rw-r--r--   0        0        0      185 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/3/stdmisc.yaml
+-rw-r--r--   0        0        0      785 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/include/3/stdreal.yaml
+-rw-r--r--   0        0        0     1410 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/schemas/config/2/clock-type-pre-include.yaml
+-rw-r--r--   0        0        0     1416 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/schemas/config/2/config-min.yaml
+-rw-r--r--   0        0        0     3784 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/schemas/config/2/config-pre-field-type-expansion.yaml
+-rw-r--r--   0        0        0     1440 2023-03-31 15:15:21.906500 barectf-3.1.2/barectf/schemas/config/2/config-pre-include.yaml
+-rw-r--r--   0        0        0     9509 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/config.yaml
+-rw-r--r--   0        0        0     1598 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/dst-pre-include.yaml
+-rw-r--r--   0        0        0     1410 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/ert-pre-include.yaml
+-rw-r--r--   0        0        0     8456 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/field-type.yaml
+-rw-r--r--   0        0        0     1372 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/include-prop.yaml
+-rw-r--r--   0        0        0     1868 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/metadata-pre-include.yaml
+-rw-r--r--   0        0        0     1410 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/2/trace-type-pre-include.yaml
+-rw-r--r--   0        0        0     1410 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/clock-type-pre-include.yaml
+-rw-r--r--   0        0        0     6731 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/schemas/config/3/config-pre-field-type-expansion.yaml
+-rw-r--r--   0        0        0     1431 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/config-pre-include.yaml
+-rw-r--r--   0        0        0     2782 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/config-pre-log-level-alias-sub.yaml
+-rw-r--r--   0        0        0    10557 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/schemas/config/3/config.yaml
+-rw-r--r--   0        0        0     1610 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/dst-pre-include.yaml
+-rw-r--r--   0        0        0     1410 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/ert-pre-include.yaml
+-rw-r--r--   0        0        0    10085 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/field-type.yaml
+-rw-r--r--   0        0        0     1372 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/include-prop.yaml
+-rw-r--r--   0        0        0     1483 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/trace-pre-include.yaml
+-rw-r--r--   0        0        0     1803 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/3/trace-type-pre-include.yaml
+-rw-r--r--   0        0        0     4257 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/schemas/config/common/common.yaml
+-rw-r--r--   0        0        0     3080 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/template.py
+-rw-r--r--   0        0        0     1372 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/templates/c/align-statements-comment.j2
+-rw-r--r--   0        0        0     2497 2023-03-31 15:15:21.909834 barectf-3.1.2/barectf/templates/c/barectf.c-macros.j2
+-rw-r--r--   0        0        0    16204 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/templates/c/barectf.c.j2
+-rw-r--r--   0        0        0     5692 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/templates/c/barectf.h.j2
+-rw-r--r--   0        0        0     8303 2023-05-17 18:39:58.183315 barectf-3.1.2/barectf/templates/c/bitfield.h.j2
+-rw-r--r--   0        0        0     1451 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/close-func-proto.j2
+-rw-r--r--   0        0        0     2281 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/common.j2
+-rw-r--r--   0        0        0     1539 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/ctx-init-func-proto.j2
+-rw-r--r--   0        0        0     1359 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/func-proto-params.j2
+-rw-r--r--   0        0        0     1497 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/open-func-proto.j2
+-rw-r--r--   0        0        0     1254 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-align-statements.j2
+-rw-r--r--   0        0        0     1591 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-array-statements.j2
+-rw-r--r--   0        0        0     2088 2023-05-17 18:39:58.183315 barectf-3.1.2/barectf/templates/c/serialize-write-bit-array-statements.j2
+-rw-r--r--   0        0        0     1330 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-dst-id-statements.j2
+-rw-r--r--   0        0        0     1332 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-dynamic-array-statements.j2
+-rw-r--r--   0        0        0     1333 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-ert-id-statements.j2
+-rw-r--r--   0        0        0     1402 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-int-statements.j2
+-rw-r--r--   0        0        0     1331 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-magic-statements.j2
+-rw-r--r--   0        0        0     1340 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-packet-size-statements.j2
+-rw-r--r--   0        0        0     1658 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-real-statements.j2
+-rw-r--r--   0        0        0     1365 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-saved-int-statements.j2
+-rw-r--r--   0        0        0     1328 2023-05-17 18:40:26.843314 barectf-3.1.2/barectf/templates/c/serialize-write-seq-num-statements.j2
+-rw-r--r--   0        0        0     1352 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-skip-save-statements.j2
+-rw-r--r--   0        0        0     1212 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-statements-comment.j2
+-rw-r--r--   0        0        0     1280 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-static-array-statements.j2
+-rw-r--r--   0        0        0     1317 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-string-statements.j2
+-rw-r--r--   0        0        0     1511 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-struct-statements.j2
+-rw-r--r--   0        0        0     1372 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-timestamp-statements.j2
+-rw-r--r--   0        0        0     1434 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/serialize-write-uuid-statements.j2
+-rw-r--r--   0        0        0     1249 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-align-statements.j2
+-rw-r--r--   0        0        0     1586 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-write-array-statements.j2
+-rw-r--r--   0        0        0     1251 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-write-bit-array-statements.j2
+-rw-r--r--   0        0        0     1327 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-write-dynamic-array-statements.j2
+-rw-r--r--   0        0        0     1275 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-write-static-array-statements.j2
+-rw-r--r--   0        0        0     1325 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-write-string-statements.j2
+-rw-r--r--   0        0        0     1522 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/size-write-struct-statements.j2
+-rw-r--r--   0        0        0     1540 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/c/trace-func-proto.j2
+-rw-r--r--   0        0        0     1482 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/common.j2
+-rw-r--r--   0        0        0     1452 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/license-header-footer.j2
+-rw-r--r--   0        0        0     2396 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/license-header.j2
+-rw-r--r--   0        0        0     1512 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/metadata/enum-ft.j2
+-rw-r--r--   0        0        0     1464 2023-03-31 15:15:21.913167 barectf-3.1.2/barectf/templates/metadata/int-ft.j2
+-rw-r--r--   0        0        0     3762 2023-05-17 18:39:58.183315 barectf-3.1.2/barectf/templates/metadata/metadata.j2
+-rw-r--r--   0        0        0     1336 2023-03-31 15:15:21.916500 barectf-3.1.2/barectf/templates/metadata/real-ft.j2
+-rw-r--r--   0        0        0     1203 2023-03-31 15:15:21.916500 barectf-3.1.2/barectf/templates/metadata/str-ft.j2
+-rw-r--r--   0        0        0     1422 2023-03-31 15:15:21.916500 barectf-3.1.2/barectf/templates/metadata/struct-ft.j2
+-rw-r--r--   0        0        0     4446 2023-03-31 15:15:21.916500 barectf-3.1.2/barectf/tsdl182gen.py
+-rw-r--r--   0        0        0     1395 2023-03-31 15:15:21.916500 barectf-3.1.2/barectf/typing.py
+-rw-r--r--   0        0        0     1332 2023-05-17 18:40:39.426647 barectf-3.1.2/barectf/version.py
+-rw-r--r--   0        0        0     2560 2023-05-17 18:40:39.426647 barectf-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 barectf-3.1.2/PKG-INFO
```

### Comparing `barectf-3.1.1/LICENSE` & `barectf-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/__init__.py` & `barectf-3.1.2/barectf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 StringFieldType = barectf_config.StringFieldType
 StructureFieldType = barectf_config.StructureFieldType
 StructureFieldTypeMember = barectf_config.StructureFieldTypeMember
 StructureFieldTypeMembers = barectf_config.StructureFieldTypeMembers
 Trace = barectf_config.Trace
 TraceEnvironment = barectf_config.TraceEnvironment
 TraceType = barectf_config.TraceType
+TraceTypeWithUnknownNativeByteOrder = barectf_config.TraceTypeWithUnknownNativeByteOrder
 TraceTypeFeatures = barectf_config.TraceTypeFeatures
 UnsignedEnumerationFieldType = barectf_config.UnsignedEnumerationFieldType
 UnsignedIntegerFieldType = barectf_config.UnsignedIntegerFieldType
 
 
 # configuration file API
 configuration_file_major_version = barectf_config_file.configuration_file_major_version
```

### Comparing `barectf-3.1.1/barectf/argpar.py` & `barectf-3.1.2/barectf/argpar.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/cgen.py` & `barectf-3.1.2/barectf/cgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,15 +542,15 @@
     #
     # See _create_template_base() for `name`.
     def _create_file_template(self, name: str) -> barectf_template._Template:
         return self._create_template_base(name, True)
 
     # Trace type of this code generator's barectf configuration.
     @property
-    def _trace_type(self) -> barectf_config.TraceType:
+    def _trace_type(self) -> barectf_config._TraceType:
         return self._cfg.trace.type
 
     # Returns the name of a source variable for the operation `op`.
     def _op_src_var_name(self, op: _LeafOp) -> str:
         s = ''
 
         for index, name in enumerate(op.names):
```

### Comparing `barectf-3.1.1/barectf/cli.py` & `barectf-3.1.2/barectf/cli.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/codegen.py` & `barectf-3.1.2/barectf/codegen.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/config.py` & `barectf-3.1.2/barectf/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,18 +699,18 @@
         return self._uuid_field_type
 
     @property
     def data_stream_type_id_field_type(self) -> _OptUIntFt:
         return self._data_stream_type_id_field_type
 
 
-class TraceType:
-    def __init__(self, native_byte_order: ByteOrder, data_stream_types: Set[DataStreamType],
-                 uuid: _OptUuid = None, features: Optional[TraceTypeFeatures] = None):
-        self._native_byte_order = native_byte_order
+class _TraceType:
+    def __init__(self, trace_byte_order: ByteOrder, data_stream_types: Set[DataStreamType],
+                 uuid: _OptUuid, features: Optional[TraceTypeFeatures]):
+        self._trace_byte_order = trace_byte_order
         self._data_stream_types = frozenset(data_stream_types)
 
         # assign unique IDs
         for index, dst in enumerate(sorted(self._data_stream_types, key=lambda st: st.name)):
             assert dst._id is None
             dst._id = Id(index)
 
@@ -738,16 +738,16 @@
 
         add_member_if_exists('magic', self._features.magic_field_type)
         add_member_if_exists('uuid', self._features.uuid_field_type)
         add_member_if_exists('stream_id', self._features.data_stream_type_id_field_type)
         self._pkt_header_ft = StructureFieldType(8, members)
 
     @property
-    def native_byte_order(self) -> ByteOrder:
-        return self._native_byte_order
+    def trace_byte_order(self) -> ByteOrder:
+        return self._trace_byte_order
 
     @property
     def uuid(self) -> _OptUuid:
         return self._uuid
 
     @property
     def data_stream_types(self) -> FrozenSet[DataStreamType]:
@@ -771,14 +771,43 @@
         for dst in self._data_stream_types:
             if dst.default_clock_type is not None:
                 clk_types.add(dst.default_clock_type)
 
         return clk_types
 
 
+# Standard trace type class for a barectf 3 configuration.
+#
+# The trace byte order property of an instance is the same as the
+# expected native byte order of the target system.
+class TraceType(_TraceType):
+    def __init__(self, trace_byte_order: ByteOrder, data_stream_types: Set[DataStreamType],
+                 uuid: _OptUuid = None, features: Optional[TraceTypeFeatures] = None):
+        super().__init__(trace_byte_order, data_stream_types, uuid, features)
+
+    @property
+    def native_byte_order(self) -> ByteOrder:
+        return self._trace_byte_order
+
+
+# This trace type class specifically exists to support barectf 2
+# configurations. Such configurations define the actual trace byte order
+# instead of the expected native byte order of the target system.
+#
+# The user provides the trace byte order property of an instance.
+#
+# IMPORTANT: When possible, prefer the `TraceType` class instead, as
+# enforcing the trace byte order could result in a less efficient
+# generated tracer.
+class TraceTypeWithUnknownNativeByteOrder(_TraceType):
+    def __init__(self, trace_byte_order: ByteOrder, data_stream_types: Set[DataStreamType],
+                 uuid: _OptUuid = None, features: Optional[TraceTypeFeatures] = None):
+        super().__init__(trace_byte_order, data_stream_types, uuid, features)
+
+
 _EnvEntry = Union[str, int]
 _EnvEntries = Mapping[str, _EnvEntry]
 
 
 class TraceEnvironment(collections.abc.Mapping):
     def __init__(self, environment: _EnvEntries):
         self._env = {name: value for name, value in environment.items()}
@@ -790,15 +819,15 @@
         return iter(self._env)
 
     def __len__(self) -> int:
         return len(self._env)
 
 
 class Trace:
-    def __init__(self, type: TraceType, environment: Optional[_EnvEntries] = None):
+    def __init__(self, type: _TraceType, environment: Optional[_EnvEntries] = None):
         self._type = type
         self._set_env(environment)
 
     def _set_env(self, environment: Optional[_EnvEntries]):
         init_env = collections.OrderedDict([
             ('domain', 'bare'),
             ('tracer_name', 'barectf'),
@@ -812,15 +841,15 @@
         if environment is None:
             environment = {}
 
         init_env.update(environment)
         self._env = TraceEnvironment(typing.cast(_EnvEntries, init_env))
 
     @property
-    def type(self) -> TraceType:
+    def type(self) -> _TraceType:
         return self._type
 
     @property
     def environment(self) -> TraceEnvironment:
         return self._env
```

### Comparing `barectf-3.1.1/barectf/config_file.py` & `barectf-3.1.2/barectf/config_file.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/config_parse.py` & `barectf-3.1.2/barectf/config_parse.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/config_parse_common.py` & `barectf-3.1.2/barectf/config_parse_common.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/config_parse_v2.py` & `barectf-3.1.2/barectf/config_parse_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,16 @@
 
         # rename `base` property to `preferred-display-base`
         _rename_prop(v3_ft_node, 'base', 'preferred-display-base')
 
         # remove `encoding` property
         _del_prop_if_exists(v3_ft_node, 'encoding')
 
-        # remove `byte-order` property (always native BO in v3)
+        # remove `byte-order` property (the equivalent barectf 3
+        # configuration property is named `trace-byte-order`)
         _del_prop_if_exists(v3_ft_node, 'byte-order')
 
         # remove `property-mappings` property
         _del_prop_if_exists(v3_ft_node, 'property-mappings')
 
         return v3_ft_node
 
@@ -485,16 +486,16 @@
             set_if_exists('data-stream-type-id-field-type', v3_dst_id_ft_node)
             return v3_features_node
 
         v3_trace_node: _MapNode = collections.OrderedDict()
         v3_trace_type_node: _MapNode = collections.OrderedDict()
         v2_trace_node = v2_meta_node['trace']
 
-        # copy `byte-order` property as `native-byte-order` property
-        _copy_prop_if_exists(v3_trace_type_node, v2_trace_node, 'byte-order', 'native-byte-order')
+        # copy `byte-order` property as `trace-byte-order` property
+        _copy_prop_if_exists(v3_trace_type_node, v2_trace_node, 'byte-order', 'trace-byte-order')
 
         # copy `uuid` property
         _copy_prop_if_exists(v3_trace_type_node, v2_trace_node, 'uuid')
 
         # copy `$log-levels`/`log-levels` property
         new_prop_name = '$log-level-aliases'
         _copy_prop_if_exists(v3_trace_type_node, v2_meta_node, 'log-levels', new_prop_name)
```

### Comparing `barectf-3.1.1/barectf/config_parse_v3.py` & `barectf-3.1.2/barectf/config_parse_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,15 +588,15 @@
             offset_seconds = offset_node.get('seconds', 0)
             offset_cycles = offset_node.get('cycles', Count(0))
 
         return barectf_config.ClockType(name, clk_type_node.get('frequency', int(1e9)),
                                         clk_type_uuid, clk_type_node.get('description'),
                                         clk_type_node.get('precision', 0),
                                         barectf_config.ClockTypeOffset(offset_seconds, offset_cycles),
-                                        clk_type_node.get('origin-is-unix-epoch', False))
+                                        clk_type_node.get('origin-is-unix-epoch', True))
 
     def _create_clk_types(self):
         self._clk_types = {}
 
         for clk_type_name, clk_type_node in self._trace_type_node.get('clock-types', {}).items():
             self._clk_types[clk_type_name] = self._create_clk_type(clk_type_name, clk_type_node)
 
@@ -653,16 +653,20 @@
             # create data stream types
             dsts = set()
 
             for dst_name, dst_node in self._trace_type_node[dsts_prop_name].items():
                 dsts.add(self._create_dst(dst_name, dst_node))
 
             # create trace type
-            return barectf_config.TraceType(self._native_byte_order, dsts, trace_type_uuid,
-                                            features)
+            if self._trace_byte_order_prop_key == 'native-byte-order':
+                trace_type_cls = barectf_config.TraceType
+            else:
+                trace_type_cls = barectf_config.TraceTypeWithUnknownNativeByteOrder
+
+            return trace_type_cls(self._trace_byte_order, dsts, trace_type_uuid, features)
         except _ConfigurationParseError as exc:
             _append_error_ctx(exc, 'Trace type')
 
     def _create_trace(self):
         try:
             trace_type = self._create_trace_type()
             trace_node = self.config_node['trace']
@@ -1087,24 +1091,29 @@
         elif type(node) is list:
             for item_node in node:
                 yield from _Parser._props(item_node)
 
     def _trace_type_props(self) -> Iterable[Tuple[Any, str]]:
         yield from _Parser._props(self.config_node['trace']['type'])
 
+    def _set_trace_byte_order_prop_key(self):
+        if 'native-byte-order' in self._trace_type_node:
+            self._trace_byte_order_prop_key = 'native-byte-order'
+        else:
+            self._trace_byte_order_prop_key = 'trace-byte-order'
+
     # Normalize the properties of the configuration node.
     #
     # This method, for each property of the trace type node:
     #
     # 1. Removes it if it's `None` (means default).
     #
     # 2. Chooses a specific `class` property value.
     #
-    # 3. Chooses a specific `byte-order`/`native-byte-order` property
-    #    value.
+    # 3. Chooses a specific trace byte order property value.
     #
     # 4. Chooses a specific `preferred-display-base` property value.
     #
     # This method also applies 1. to the trace node's `environment`
     # property.
     def _normalize_props(self):
         def normalize_byte_order_prop(parent_node: _MapNode, key: str):
@@ -1112,15 +1121,15 @@
 
             if node in ['be', 'big']:
                 parent_node[key] = 'big-endian'
             elif node in ['le', 'little']:
                 parent_node[key] = 'little-endian'
 
         trace_node = self.config_node['trace']
-        normalize_byte_order_prop(self._trace_type_node, 'native-byte-order')
+        normalize_byte_order_prop(self._trace_type_node, self._trace_byte_order_prop_key)
 
         for parent_node, key in self._trace_type_props():
             node = parent_node[key]
 
             if node is None:
                 # a `None` property is equivalent to not having it
                 del parent_node[key]
@@ -1155,18 +1164,18 @@
 
         if prop_name in trace_node:
             node = trace_node[prop_name]
 
             if node is None:
                 del trace_node[prop_name]
 
-    # Sets the parser's native byte order.
-    def _set_native_byte_order(self):
-        self._native_byte_order_node = self._trace_type_node['native-byte-order']
-        self._native_byte_order = self._byte_order_from_node(self._native_byte_order_node)
+    # Sets the parser's trace byte order.
+    def _set_trace_byte_order(self):
+        self._trace_byte_order_node = self._trace_type_node[self._trace_byte_order_prop_key]
+        self._trace_byte_order = self._byte_order_from_node(self._trace_byte_order_node)
 
     # Processes the inclusions of the event record type node
     # `ert_node`, returning the effective node.
     def _process_ert_node_include(self, ert_node: _MapNode) -> _MapNode:
         # Make sure the event record type node is valid for the
         # inclusion processing stage.
         self._schema_validator.validate(ert_node, 'config/3/ert-pre-include')
@@ -1318,30 +1327,33 @@
         #    type node.
         self._sub_log_level_aliases()
 
         # At this point, the configuration node must be valid as an
         # effective configuration node.
         self._schema_validator.validate(self.config_node, 'config/3/config')
 
+        # Set the trace byte order property key.
+        self._set_trace_byte_order_prop_key()
+
         # Normalize properties.
         #
         # This process removes `None` properties and chooses specific
         # enumerators when aliases exist (for example, `big-endian`
         # instead of `be`).
         #
         # The goal of this is that, if the user then gets this parser's
         # `config_node` property, it has a normal and very readable
         # form.
         #
         # It also makes _create_config() easier to implement because it
         # doesn't need to check for `None` nodes or enumerator aliases.
         self._normalize_props()
 
-        # Set the native byte order.
-        self._set_native_byte_order()
+        # Set the trace byte order.
+        self._set_trace_byte_order()
 
         # Create a barectf configuration object from the configuration
         # node.
         self._create_config()
 
     @property
     def config(self) -> barectf_config.Configuration:
```

### Comparing `barectf-3.1.1/barectf/include/2/stdint.yaml` & `barectf-3.1.2/barectf/include/2/stdint.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/include/2/trace-basic.yaml` & `barectf-3.1.2/barectf/include/2/trace-basic.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/include/3/stdint.yaml` & `barectf-3.1.2/barectf/include/3/stdint.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/include/3/stdreal.yaml` & `barectf-3.1.2/barectf/include/3/stdreal.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/clock-type-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/2/clock-type-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/config-min.yaml` & `barectf-3.1.2/barectf/schemas/config/2/config-min.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/config-pre-field-type-expansion.yaml` & `barectf-3.1.2/barectf/schemas/config/2/config-pre-field-type-expansion.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/config-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/2/config-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/config.yaml` & `barectf-3.1.2/barectf/schemas/config/2/config.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/dst-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/2/dst-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/ert-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/2/ert-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/field-type.yaml` & `barectf-3.1.2/barectf/schemas/config/2/field-type.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/include-prop.yaml` & `barectf-3.1.2/barectf/schemas/config/2/include-prop.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/metadata-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/2/metadata-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/2/trace-type-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/2/trace-type-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/clock-type-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/3/clock-type-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/config-pre-field-type-expansion.yaml` & `barectf-3.1.2/barectf/schemas/config/3/config-pre-field-type-expansion.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/config-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/3/config-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/config-pre-log-level-alias-sub.yaml` & `barectf-3.1.2/barectf/schemas/config/3/config-pre-log-level-alias-sub.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/config.yaml` & `barectf-3.1.2/barectf/schemas/config/3/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
       - type
   trace-type:
     title: Trace type object
     type: object
     properties:
       native-byte-order:
         $ref: https://barectf.org/schemas/config/common/common.json#/definitions/byte-order-prop
+      trace-byte-order:
+        $ref: https://barectf.org/schemas/config/common/common.json#/definitions/byte-order-prop
       uuid:
         $ref: https://barectf.org/schemas/config/common/common.json#/definitions/opt-trace-type-uuid-prop
       $features:
         if:
           type: object
         then:
           properties:
@@ -150,16 +152,20 @@
         type: object
         patternProperties:
           '^[A-Za-z_][A-Za-z0-9_]*$':
             $ref: '#/definitions/dst'
         additionalProperties: false
         minProperties: 1
     required:
-      - native-byte-order
       - data-stream-types
+    oneOf:
+      - required:
+        - trace-byte-order
+      - required:
+        - native-byte-order
     additionalProperties: false
   clock-type:
     title: Clock type object
     type: object
     properties:
       uuid:
         $ref: https://barectf.org/schemas/config/common/common.json#/definitions/opt-uuid-prop
```

### Comparing `barectf-3.1.1/barectf/schemas/config/3/dst-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/3/dst-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/ert-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/3/ert-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/field-type.yaml` & `barectf-3.1.2/barectf/schemas/config/3/field-type.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/include-prop.yaml` & `barectf-3.1.2/barectf/schemas/config/3/include-prop.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/trace-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/3/trace-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/3/trace-type-pre-include.yaml` & `barectf-3.1.2/barectf/schemas/config/3/trace-type-pre-include.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/schemas/config/common/common.yaml` & `barectf-3.1.2/barectf/schemas/config/common/common.yaml`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/template.py` & `barectf-3.1.2/barectf/template.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/align-statements-comment.j2` & `barectf-3.1.2/barectf/templates/c/align-statements-comment.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/barectf.c-macros.j2` & `barectf-3.1.2/barectf/templates/c/barectf.c-macros.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/barectf.c.j2` & `barectf-3.1.2/barectf/templates/c/barectf.c.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/barectf.h.j2` & `barectf-3.1.2/barectf/templates/c/barectf.h.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/bitfield.h.j2` & `barectf-3.1.2/barectf/templates/c/bitfield.h.j2`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
  * significant. Also, consecutive bitfields are placed from lower bits to higher
  * bits.
  *
  * On big endian, bytes are places from most significant to less significant.
  * Also, consecutive bitfields are placed from higher to lower bits.
  */
 
-{% if cfg.trace.type.native_byte_order == barectf_config.ByteOrder.LITTLE_ENDIAN %}
-/* Native byte order: little-endian */
+{% if cfg.trace.type.trace_byte_order == barectf_config.ByteOrder.LITTLE_ENDIAN %}
+/* Trace byte order: little-endian */
 
 #define _bt_bitfield_write_le(_ptr, type, _start, _length, _vtype, _v)	\
 do {									\
 	_vtype __v = (_v);						\
 	type *__ptr = _CAST_PTR(type *, _ptr);				\
 	unsigned long __start = (_start), __length = (_length);		\
 	type mask, cmask;						\
@@ -159,15 +159,15 @@
 	} else								\
 		__ptr[this_unit] = (type) __v;				\
 } while (0)
 
 #define bt_bitfield_write_le(ptr, _start, _length, _vtype, _v) \
 	_bt_bitfield_write_le(ptr, uint8_t, _start, _length, _vtype, _v)
 {% else %}
-/* Native byte order: big-endian */
+/* Trace byte order: big-endian */
 
 #define _bt_bitfield_write_be(_ptr, type, _start, _length, _vtype, _v)	\
 do {									\
 	_vtype __v = (_v);						\
 	type *__ptr = _CAST_PTR(type *, _ptr);				\
 	unsigned long __start = (_start), __length = (_length);		\
 	type mask, cmask;						\
```

### Comparing `barectf-3.1.1/barectf/templates/c/close-func-proto.j2` & `barectf-3.1.2/barectf/templates/c/close-func-proto.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/common.j2` & `barectf-3.1.2/barectf/templates/c/common.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/ctx-init-func-proto.j2` & `barectf-3.1.2/barectf/templates/c/ctx-init-func-proto.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/func-proto-params.j2` & `barectf-3.1.2/barectf/templates/c/func-proto-params.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/open-func-proto.j2` & `barectf-3.1.2/barectf/templates/c/open-func-proto.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-align-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-align-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-bit-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-bit-array-statements.j2`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,25 @@
  # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
  # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
  # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
  # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  #}
 {% import 'common.j2' as common %}
 {% set incr_at %}ctx->at += {{ op.ft.size }}{% endset %}
-{% if op.ft.alignment % 8 == 0 and op.ft.size in [8, 16, 32, 64] %}
+{% if op.ft.alignment % 8 == 0 and
+	op.ft.size in [8, 16, 32, 64] and
+	cfg.trace.type.__class__ != barectf_config.TraceTypeWithUnknownNativeByteOrder %}
 	{% set c_type %}uint{{ op.ft.size }}_t{% endset %}
 {
 	const {{ c_type }} tmp_val = ({{ c_type }}) {{ src }};
 
 	memcpy(&ctx->buf[_BITS_TO_BYTES(ctx->at)], &tmp_val, sizeof(tmp_val));
 	{{ incr_at }};
 }
 {%- else %}
-	{% set bo = 'le' if cfg.trace.type.native_byte_order == barectf_config.ByteOrder.LITTLE_ENDIAN else 'be' %}
+	{% set bo = 'le' if cfg.trace.type.trace_byte_order == barectf_config.ByteOrder.LITTLE_ENDIAN else 'be' %}
 	{% set c_type_non_const = c_type | replace('const ', '') %}
 	{% set offset_in_byte = 'ctx->at % 8' if op.offset_in_byte == none else op.offset_in_byte %}
 bt_bitfield_write_{{ bo }}(&ctx->buf[_BITS_TO_BYTES(ctx->at)], {{ offset_in_byte }}, {{ op.ft.size }},
 	{{ c_type_non_const }}, ({{ c_type_non_const }}) {{ src }});
 {{ incr_at }};
 {%- endif %}
```

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-dst-id-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-dst-id-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-dynamic-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-dynamic-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-ert-id-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-ert-id-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-int-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-int-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-magic-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-magic-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-packet-size-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-packet-size-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-real-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-real-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-saved-int-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-saved-int-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-seq-num-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-seq-num-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-skip-save-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-skip-save-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-statements-comment.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-statements-comment.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-static-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-static-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-string-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-string-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-struct-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-struct-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-timestamp-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-timestamp-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/serialize-write-uuid-statements.j2` & `barectf-3.1.2/barectf/templates/c/serialize-write-uuid-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-align-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-align-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-write-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-write-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-write-bit-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-write-bit-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-write-dynamic-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-write-dynamic-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-write-static-array-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-write-static-array-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-write-string-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-write-string-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/size-write-struct-statements.j2` & `barectf-3.1.2/barectf/templates/c/size-write-struct-statements.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/c/trace-func-proto.j2` & `barectf-3.1.2/barectf/templates/c/trace-func-proto.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/common.j2` & `barectf-3.1.2/barectf/templates/common.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/license-header-footer.j2` & `barectf-3.1.2/barectf/templates/license-header-footer.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/license-header.j2` & `barectf-3.1.2/barectf/templates/license-header.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/metadata/enum-ft.j2` & `barectf-3.1.2/barectf/templates/metadata/enum-ft.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/metadata/int-ft.j2` & `barectf-3.1.2/barectf/templates/metadata/int-ft.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/metadata/metadata.j2` & `barectf-3.1.2/barectf/templates/metadata/metadata.j2`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  #}
 {% macro root_ft(name, rft) %}
 {{ name }} := {{ rft | ft_str }};
 {%- endmacro %}
 trace {
 	major = 1;
 	minor = 8;
-	byte_order = {{ 'le' if cfg.trace.type.native_byte_order == barectf_config.ByteOrder.LITTLE_ENDIAN else 'be' }};
+	byte_order = {{ 'le' if cfg.trace.type.trace_byte_order == barectf_config.ByteOrder.LITTLE_ENDIAN else 'be' }};
 {% if cfg.trace.type.uuid %}
 	uuid = "{{ cfg.trace.type.uuid }}";
 {% endif %}
 {% if cfg.trace.type._pkt_header_ft %}
 	{{ root_ft('packet.header', cfg.trace.type._pkt_header_ft) | indent_tab }}
 {% endif %}
 };
@@ -72,28 +72,32 @@
 };
 
 {% endfor %}
 {# data stream types and their event record types #}
 {% for dst in cfg.trace.type.data_stream_types | sort %}
 /* Data stream type `{{ dst.name }}` */
 stream {
+	{% if cfg.trace.type.features.data_stream_type_id_field_type %}
 	id = {{ dst.id }};
+	{% endif %}
 	{{ root_ft('packet.context', dst._pkt_ctx_ft) | indent_tab }}
 	{% if dst._er_header_ft %}
 	{{ root_ft('event.header', dst._er_header_ft) | indent_tab }}
 	{% endif %}
 	{% if dst.event_record_common_context_field_type %}
 	{{ root_ft('event.context', dst.event_record_common_context_field_type) | indent_tab }}
 	{% endif %}
 };
 
 	{# data stream type's event record types #}
 	{% for ert in dst.event_record_types | sort %}
 event {
+	{% if cfg.trace.type.features.data_stream_type_id_field_type %}
 	stream_id = {{ dst.id }};
+	{% endif %}
 	id = {{ ert.id }};
 	name = "{{ ert.name }}";
 		{% if ert.log_level %}
 	loglevel = {{ ert.log_level }};
 		{% endif %}
 		{% if ert.specific_context_field_type %}
 	{{ root_ft('context', ert.specific_context_field_type) | indent_tab }}
```

### Comparing `barectf-3.1.1/barectf/templates/metadata/real-ft.j2` & `barectf-3.1.2/barectf/templates/metadata/real-ft.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/metadata/str-ft.j2` & `barectf-3.1.2/barectf/templates/metadata/str-ft.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/templates/metadata/struct-ft.j2` & `barectf-3.1.2/barectf/templates/metadata/struct-ft.j2`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/tsdl182gen.py` & `barectf-3.1.2/barectf/tsdl182gen.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/typing.py` & `barectf-3.1.2/barectf/typing.py`

 * *Files identical despite different names*

### Comparing `barectf-3.1.1/barectf/version.py` & `barectf-3.1.2/barectf/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 __major_version__ = 3
 __minor_version__ = 1
-__patch_version__ = 1
+__patch_version__ = 2
 __pre_version__ = ''
 __version__ = f'{__major_version__}.{__minor_version__}.{__patch_version__}{__pre_version__}'
```

### Comparing `barectf-3.1.1/pyproject.toml` & `barectf-3.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'barectf'
-version = '3.1.1'
+version = '3.1.2'
 description = 'Generator of ANSI C tracers which output CTF data streams'
 license = 'MIT'
 authors = ['Philippe Proulx <eeppeliteloop@gmail.com>']
 homepage = 'https://barectf.org/'
 repository = 'https://github.com/efficios/barectf/'
 keywords = [
     'ctf',
@@ -49,24 +49,24 @@
     'Operating System :: OS Independent',
     'Programming Language :: C',
     'Topic :: Software Development :: Code Generators',
 ]
 packages = [{include = 'barectf'}]
 
 [tool.poetry.dependencies]
-python = '^3.6'
+python = '>=3.6.2, <4'
 termcolor = '^1.1'
 pyyaml = '^5.3'
 jsonschema = '^3.2'
 setuptools = '*'
 jinja2 = '^3.0'
 
 [tool.poetry.dev-dependencies]
 flake8 = '*'
-pylint = '*'
+pylint = '^2.13'
 mypy = '*'
 pytest = '^6'
 pytest-xdist = '^2'
 
 [tool.poetry.scripts]
 barectf = 'barectf.cli:_run'
```

### Comparing `barectf-3.1.1/PKG-INFO` & `barectf-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: barectf
-Version: 3.1.1
+Version: 3.1.2
 Summary: Generator of ANSI C tracers which output CTF data streams
 Home-page: https://barectf.org/
 License: MIT
 Keywords: ctf,generator,tracing,bare-metal,bare-machine
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.6.2,<4
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: jinja2 (>=3.0,<4.0)
 Requires-Dist: jsonschema (>=3.2,<4.0)
 Requires-Dist: pyyaml (>=5.3,<6.0)
 Requires-Dist: setuptools
 Requires-Dist: termcolor (>=1.1,<2.0)
 Project-URL: Bug tracker, https://github.com/efficios/barectf/issues/
```

