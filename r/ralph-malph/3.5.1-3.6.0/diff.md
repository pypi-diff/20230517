# Comparing `tmp/ralph-malph-3.5.1.tar.gz` & `tmp/ralph-malph-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-3.5.1.tar", last modified: Wed Apr 19 07:45:08 2023, max compression
+gzip compressed data, was "ralph-malph-3.6.0.tar", last modified: Wed May 17 11:54:32 2023, max compression
```

## Comparing `ralph-malph-3.5.1.tar` & `ralph-malph-3.6.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6299 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5147 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2726 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.099809 ralph-malph-3.5.1/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.099809 ralph-malph-3.5.1/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.099809 ralph-malph-3.5.1/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      840 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5321 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/auth.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13641 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3688 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    12909 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/database/mongo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/mixins.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/storage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5171 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/storage/swift.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.111809 ralph-malph-3.5.1/src/ralph/backends/stream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/stream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/stream/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/backends/stream/ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19679 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10266 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.115809 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.119809 ralph-malph-3.5.1/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      356 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1820 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3802 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/actors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2380 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1941 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3941 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1554 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/fields/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.123809 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.127809 ralph-malph-3.5.1/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.127809 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5335 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/verbs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7490 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/models/xapi/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.127809 ralph-malph-3.5.1/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6299 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4104 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-19 07:45:08.000000 ralph-malph-3.5.1/src/ralph_malph.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-19 07:45:08.131809 ralph-malph-3.5.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3521 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_auth.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_cli_usage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_dependencies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-04-19 07:45:07.000000 ralph-malph-3.5.1/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6443 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2655 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.560460 ralph-malph-3.6.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.560460 ralph-malph-3.6.0/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.560460 ralph-malph-3.6.0/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1406 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5321 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/auth.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15226 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3688 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    12909 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/database/mongo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/mixins.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/storage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5171 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/storage/swift.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/backends/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/stream/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/backends/stream/ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19679 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10326 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.564460 ralph-malph-3.6.0/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.568460 ralph-malph-3.6.0/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      356 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1820 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3802 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/actors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2380 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1941 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3941 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1554 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/fields/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5335 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/verbs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7490 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/models/xapi/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.572461 ralph-malph-3.6.0/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6443 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4104 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 11:54:32.000000 ralph-malph-3.6.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 11:54:32.576460 ralph-malph-3.6.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3521 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_auth.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-05-17 11:54:31.000000 ralph-malph-3.6.0/tests/test_utils.py
```

### Comparing `ralph-malph-3.5.1/LICENSE.md` & `ralph-malph-3.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/PKG-INFO` & `ralph-malph-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.5.1
+Version: 3.6.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,16 @@
 Provides-Extra: dev
 Provides-Extra: ci
 Provides-Extra: lrs
 License-File: LICENSE.md
 
 # Ralph
 
+[![Discord](https://img.shields.io/discord/1082704478463082496?label=discord&logo=discord&style=for-the-badge)](https://discord.gg/vYx6YWxJCS)
+
 Ralph is a toolbox for your learning analytics, it can be used as a:
 
 - **library**, to fetch learning events from various backends, (de)serialize or
     convert them from various standard formats such as
     [xAPI](https://adlnet.gov/projects/xapi/), or
     [openedx](https://docs.openedx.org/en/latest/developers/references/internal_data_formats/tracking_logs/index.html)
 - **command-line interface** (CLI), to build data pipelines the UNIX-way™️,
```

### Comparing `ralph-malph-3.5.1/README.md` & `ralph-malph-3.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Ralph
 
+[![Discord](https://img.shields.io/discord/1082704478463082496?label=discord&logo=discord&style=for-the-badge)](https://discord.gg/vYx6YWxJCS)
+
 Ralph is a toolbox for your learning analytics, it can be used as a:
 
 - **library**, to fetch learning events from various backends, (de)serialize or
     convert them from various standard formats such as
     [xAPI](https://adlnet.gov/projects/xapi/), or
     [openedx](https://docs.openedx.org/en/latest/developers/references/internal_data_formats/tracking_logs/index.html)
 - **command-line interface** (CLI), to build data pipelines the UNIX-way™️,
```

### Comparing `ralph-malph-3.5.1/setup.cfg` & `ralph-malph-3.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ralph-malph
-version = 3.5.1
+version = 3.6.0
 description = The ultimate toolbox for your learning analytics
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://openfun.github.io/ralph/
 license = MIT
@@ -58,42 +58,38 @@
 	click>=8.1.0
 	click-option-group>=0.5.0
 	sentry-sdk[fastapi]>=1.9.0
 dev = 
 	bandit==1.7.5
 	black==23.3.0
 	factory-boy==3.2.1
-	Faker==18.4.0
 	flake8==6.0.0
-	hypothesis==6.72.0
-	ipdb==0.13.13
-	ipython==8.12.0
+	hypothesis==6.75.3
 	isort==5.12.0
 	logging-gelf==0.0.26
-	memory-profiler==0.61.0
-	mkdocs==1.4.2
+	mkdocs==1.4.3
 	mkdocs-click==0.8.0
-	mkdocs-material==9.1.6
+	mkdocs-material==9.1.12
 	mkdocstrings[python-legacy]==0.21.2
-	moto==4.1.7
+	moto==4.1.9
 	pydocstyle==6.3.0
 	pyfakefs==5.2.2
-	pylint==2.17.2
+	pylint==2.17.4
 	pytest==7.3.1
 	pytest-asyncio==0.21.0
 	pytest-cov==4.0.0
 ci = 
 	twine==4.0.2
 lrs = 
 	bcrypt==4.0.1
 	fastapi==0.95.1
 	h11>=0.11.0
 	httpx==0.24.0
-	sentry_sdk==1.19.1
-	uvicorn[standard]==0.21.1
+	sentry_sdk==1.22.2
+	uvicorn[standard]==0.22.0
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	ralph = ralph.__main__:cli.cli
```

### Comparing `ralph-malph-3.5.1/src/ralph/__main__.py` & `ralph-malph-3.6.0/src/ralph/__main__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/api/__init__.py` & `ralph-malph-3.6.0/src/ralph/api/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,45 @@
 """Main module for Ralph's LRS API."""
+from functools import lru_cache
+from urllib.parse import urlparse
+
 import sentry_sdk
 from fastapi import Depends, FastAPI
 
 from ralph.conf import settings
 
 from .. import __version__
 from .auth import AuthenticatedUser, authenticated_user
 from .routers import health, statements
 
+
+@lru_cache(maxsize=None)
+def get_health_check_routes():
+    """Return the health check routes."""
+    return [route.path for route in health.router.routes]
+
+
+def filter_transactions(event, hint):  # pylint: disable=unused-argument
+    """Filter transactions for Sentry."""
+    url = urlparse(event["request"]["url"])
+
+    if settings.SENTRY_IGNORE_HEALTH_CHECKS and url.path in get_health_check_routes():
+        return None
+
+    return event
+
+
 if settings.SENTRY_DSN is not None:
     sentry_sdk.init(
         dsn=settings.SENTRY_DSN,
         traces_sample_rate=settings.SENTRY_LRS_TRACES_SAMPLE_RATE,
         release=__version__,
         environment=settings.EXECUTION_ENVIRONMENT,
         max_breadcrumbs=50,
+        before_send_transaction=filter_transactions,
     )
 
 app = FastAPI()
 app.include_router(statements.router)
 app.include_router(health.router)
```

### Comparing `ralph-malph-3.5.1/src/ralph/api/auth.py` & `ralph-malph-3.6.0/src/ralph/api/auth.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/api/forwarding.py` & `ralph-malph-3.6.0/src/ralph/api/forwarding.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/api/models.py` & `ralph-malph-3.6.0/src/ralph/api/models.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/api/routers/health.py` & `ralph-malph-3.6.0/src/ralph/api/routers/health.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/api/routers/statements.py` & `ralph-malph-3.6.0/src/ralph/api/routers/statements.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API routes related to statements."""
 
 import logging
 from datetime import datetime
 from typing import List, Literal, Optional, Union
+from urllib.parse import ParseResult, urlencode
 from uuid import UUID, uuid4
 
 from fastapi import (
     APIRouter,
     BackgroundTasks,
     Depends,
     HTTPException,
@@ -187,14 +188,51 @@
 
     LRS Specification:
     https://github.com/adlnet/xAPI-Spec/blob/1.0.3/xAPI-Communication.md#213-get-statements
     """
     # Make sure the limit does not go above max from settings
     limit = min(limit, settings.RUNSERVER_MAX_SEARCH_HITS_COUNT)
 
+    # 400 Bad Request for requests using both `statementId` and `voidedStatementId`
+    if (statementId is not None) and (voidedStatementId is not None):
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail=(
+                "Query parameters cannot include both `statementId`"
+                "and `voidedStatementId`"
+            ),
+        )
+
+    # 400 Bad Request for any request containing `statementId` or
+    # `voidedStatementId` and any other parameter besides `attachments` or `format`.
+    # NB: `limit` and `ascending` are not handled to simplify implementation, and as it
+    # has no incidence on UX, when fetching a single statement
+    excluded_params = [
+        agent,
+        verb,
+        activity,
+        registration,
+        related_activities,
+        related_agents,
+        since,
+        until,
+    ]
+    # NB: bool(param) relies on all defaults being None, 0, or False
+    if (statementId or voidedStatementId) and any(
+        bool(param) for param in excluded_params
+    ):
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail=(
+                "Querying by id only accepts `attachments` and `format` as extra"
+                "parameters"
+            ),
+        )
+
+    # Query Database
     try:
         query_result = DATABASE_CLIENT.query_statements(
             StatementParameters(**{**request.query_params, "limit": limit})
         )
     except BackendException as error:
         raise HTTPException(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
@@ -205,22 +243,34 @@
     # consistency of search results.
     # NB: There is an unhandled edge case where the total number of results is
     # exactly a multiple of the "limit", in which case we'll offer an extra page
     # with 0 results.
     response = {}
     if len(query_result.statements) == limit:
         # Search after relies on sorting info located in the last hit
-        path = request.url.components.path
-        query = request.url.components.query
+        path = request.url.path
+        query = dict(request.query_params)
+
+        query.update(
+            {
+                "pit_id": query_result.pit_id,
+                "search_after": query_result.search_after,
+            }
+        )
+
         response.update(
             {
-                "more": (
-                    f"{path}{query + '&' if query else '?'}pit_id={query_result.pit_id}"
-                    f"&search_after={query_result.search_after}"
-                )
+                "more": ParseResult(
+                    scheme="",
+                    netloc="",
+                    path=path,
+                    params="",
+                    query=urlencode(query),
+                    fragment="",
+                ).geturl(),
             }
         )
 
     return {**response, "statements": query_result.statements}
 
 
 @router.put("/", responses=POST_PUT_RESPONSES, status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `ralph-malph-3.5.1/src/ralph/backends/database/base.py` & `ralph-malph-3.6.0/src/ralph/backends/database/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/database/clickhouse.py` & `ralph-malph-3.6.0/src/ralph/backends/database/clickhouse.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/database/es.py` & `ralph-malph-3.6.0/src/ralph/backends/database/es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/database/mongo.py` & `ralph-malph-3.6.0/src/ralph/backends/database/mongo.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/mixins.py` & `ralph-malph-3.6.0/src/ralph/backends/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/storage/base.py` & `ralph-malph-3.6.0/src/ralph/backends/storage/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/storage/fs.py` & `ralph-malph-3.6.0/src/ralph/backends/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/storage/ldp.py` & `ralph-malph-3.6.0/src/ralph/backends/storage/ldp.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/storage/s3.py` & `ralph-malph-3.6.0/src/ralph/backends/storage/s3.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/storage/swift.py` & `ralph-malph-3.6.0/src/ralph/backends/storage/swift.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/backends/stream/ws.py` & `ralph-malph-3.6.0/src/ralph/backends/stream/ws.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/cli.py` & `ralph-malph-3.6.0/src/ralph/cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/conf.py` & `ralph-malph-3.6.0/src/ralph/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,17 +320,18 @@
     }
     PARSERS: ParserSettings = ParserSettings()
     RUNSERVER_BACKEND: Literal["clickhouse", "es", "mongo"] = "es"
     RUNSERVER_HOST: str = "0.0.0.0"  # nosec
     RUNSERVER_MAX_SEARCH_HITS_COUNT: int = 100
     RUNSERVER_POINT_IN_TIME_KEEP_ALIVE: str = "1m"
     RUNSERVER_PORT: int = 8100
+    SENTRY_CLI_TRACES_SAMPLE_RATE: float = 1.0
     SENTRY_DSN: str = None
-    SENTRY_CLI_TRACES_SAMPLE_RATE = 1.0
-    SENTRY_LRS_TRACES_SAMPLE_RATE = 0.1
+    SENTRY_IGNORE_HEALTH_CHECKS: bool = False
+    SENTRY_LRS_TRACES_SAMPLE_RATE: float = 1.0
     XAPI_FORWARDINGS: List[XapiForwardingConfigurationSettings] = []
 
     @property
     def APP_DIR(self) -> Path:  # pylint: disable=invalid-name
         """Returns the path to Ralph's configuration directory."""
         return self._CORE.APP_DIR
```

### Comparing `ralph-malph-3.5.1/src/ralph/exceptions.py` & `ralph-malph-3.6.0/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/filters.py` & `ralph-malph-3.6.0/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/converter.py` & `ralph-malph-3.6.0/src/ralph/models/converter.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/__init__.py` & `ralph-malph-3.6.0/src/ralph/models/edx/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/base.py` & `ralph-malph-3.6.0/src/ralph/models/edx/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/browser.py` & `ralph-malph-3.6.0/src/ralph/models/edx/browser.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-3.6.0/src/ralph/models/edx/converters/xapi/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-3.6.0/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-3.6.0/src/ralph/models/edx/enrollment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-3.6.0/src/ralph/models/edx/navigational/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-3.6.0/src/ralph/models/edx/navigational/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-3.6.0/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/server.py` & `ralph-malph-3.6.0/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-3.6.0/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-3.6.0/src/ralph/models/edx/video/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/edx/video/statements.py` & `ralph-malph-3.6.0/src/ralph/models/edx/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/selector.py` & `ralph-malph-3.6.0/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/validator.py` & `ralph-malph-3.6.0/src/ralph/models/validator.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/base.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/config.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/config.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/constants.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/actors.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/actors.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/attachments.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/attachments.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/common.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/common.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/contexts.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/objects.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/results.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/unnested_objects.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/unnested_objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/fields/verbs.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/fields/verbs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/navigation/fields/objects.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/navigation/fields/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/navigation/statements.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/navigation/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/video/constants.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/video/constants.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/contexts.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/objects.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/results.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/video/fields/verbs.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/video/fields/verbs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/models/xapi/video/statements.py` & `ralph-malph-3.6.0/src/ralph/models/xapi/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/parsers.py` & `ralph-malph-3.6.0/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph/utils.py` & `ralph-malph-3.6.0/src/ralph/utils.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-3.6.0/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.5.1
+Version: 3.6.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,16 @@
 Provides-Extra: dev
 Provides-Extra: ci
 Provides-Extra: lrs
 License-File: LICENSE.md
 
 # Ralph
 
+[![Discord](https://img.shields.io/discord/1082704478463082496?label=discord&logo=discord&style=for-the-badge)](https://discord.gg/vYx6YWxJCS)
+
 Ralph is a toolbox for your learning analytics, it can be used as a:
 
 - **library**, to fetch learning events from various backends, (de)serialize or
     convert them from various standard formats such as
     [xAPI](https://adlnet.gov/projects/xapi/), or
     [openedx](https://docs.openedx.org/en/latest/developers/references/internal_data_formats/tracking_logs/index.html)
 - **command-line interface** (CLI), to build data pipelines the UNIX-way™️,
```

### Comparing `ralph-malph-3.5.1/src/ralph_malph.egg-info/SOURCES.txt` & `ralph-malph-3.6.0/src/ralph_malph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-3.6.0/src/ralph_malph.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -37,34 +37,30 @@
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
 bandit==1.7.5
 black==23.3.0
 factory-boy==3.2.1
-Faker==18.4.0
 flake8==6.0.0
-hypothesis==6.72.0
-ipdb==0.13.13
-ipython==8.12.0
+hypothesis==6.75.3
 isort==5.12.0
 logging-gelf==0.0.26
-memory-profiler==0.61.0
-mkdocs==1.4.2
+mkdocs==1.4.3
 mkdocs-click==0.8.0
-mkdocs-material==9.1.6
+mkdocs-material==9.1.12
 mkdocstrings[python-legacy]==0.21.2
-moto==4.1.7
+moto==4.1.9
 pydocstyle==6.3.0
 pyfakefs==5.2.2
-pylint==2.17.2
+pylint==2.17.4
 pytest==7.3.1
 pytest-asyncio==0.21.0
 pytest-cov==4.0.0
 
 [lrs]
 bcrypt==4.0.1
 fastapi==0.95.1
 h11>=0.11.0
 httpx==0.24.0
-sentry_sdk==1.19.1
-uvicorn[standard]==0.21.1
+sentry_sdk==1.22.2
+uvicorn[standard]==0.22.0
```

### Comparing `ralph-malph-3.5.1/tests/test_auth.py` & `ralph-malph-3.6.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_cli.py` & `ralph-malph-3.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_cli_usage.py` & `ralph-malph-3.6.0/tests/test_cli_usage.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_conf.py` & `ralph-malph-3.6.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_dependencies.py` & `ralph-malph-3.6.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_filters.py` & `ralph-malph-3.6.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_logger.py` & `ralph-malph-3.6.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_parsers.py` & `ralph-malph-3.6.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.5.1/tests/test_utils.py` & `ralph-malph-3.6.0/tests/test_utils.py`

 * *Files identical despite different names*

