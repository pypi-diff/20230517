# Comparing `tmp/prism-dev-0.1.0.tar.gz` & `tmp/prism-dev-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prism-dev-0.1.0.tar", last modified: Fri May  5 11:34:30 2023, max compression
+gzip compressed data, was "prism-dev-0.1.1.tar", last modified: Wed May 17 12:13:42 2023, max compression
```

## Comparing `prism-dev-0.1.0.tar` & `prism-dev-0.1.1.tar`

### file list

```diff
@@ -1,402 +1,409 @@
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.705806 prism-dev-0.1.0/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-dev-0.1.0/LICENSE
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-dev-0.1.0/MANIFEST.in
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5557 2023-05-05 11:34:30.705967 prism-dev-0.1.0/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4595 2023-04-04 01:59:51.000000 prism-dev-0.1.0/README.md
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.628875 prism-dev-0.1.0/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-dev-0.1.0/prism/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/admin.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.630185 prism-dev-0.1.0/prism/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4689 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/agents/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19578 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/agents/docker_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/agents/meta.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.633477 prism-dev-0.1.0/prism/cli/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/cli/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9495 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/cli/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6974 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/cli/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6235 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/cli/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4391 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/cli/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4186 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/cli/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4548 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/cli/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4408 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/cli/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5415 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/cli/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5452 2023-05-04 13:05:27.000000 prism-dev-0.1.0/prism/cli/init.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9372 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/cli/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/cli/spark_submit.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.633795 prism-dev-0.1.0/prism/client/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12158 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/client/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1724 2023-05-04 13:24:57.000000 prism-dev-0.1.0/prism/constants.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6480 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/decorators.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.634038 prism-dev-0.1.0/prism/docs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/docs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.637624 prism-dev-0.1.0/prism/docs/build/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-dev-0.1.0/prism/docs/build/311ea03002abadcdcaba.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-dev-0.1.0/prism/docs/build/54968a39190c43d592b9.svg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-dev-0.1.0/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/docs/build/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-dev-0.1.0/prism/docs/build/ce188596011a8fa32931.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/docs/build/index.html
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/docs/build/main.js.LICENSE.txt
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.637974 prism-dev-0.1.0/prism/event_managers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/event_managers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5985 2023-05-04 14:38:23.000000 prism-dev-0.1.0/prism/event_managers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5955 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/exceptions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.640284 prism-dev-0.1.0/prism/infra/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/infra/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13452 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/infra/compiler.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12699 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/infra/executor.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2395 2023-05-04 13:05:27.000000 prism-dev-0.1.0/prism/infra/hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/infra/manifest.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6433 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/infra/module.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3629 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/infra/pipeline.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17123 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/infra/project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/infra/sys_path.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      719 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/infra/task_manager.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21159 2023-05-04 22:11:22.000000 prism-dev-0.1.0/prism/logging.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21156 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/main.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.642720 prism-dev-0.1.0/prism/mixins/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.0/prism/mixins/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/mixins/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/mixins/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8170 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/mixins/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7262 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/mixins/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2306 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/mixins/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4713 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/mixins/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5422 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/mixins/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/mixins/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-dev-0.1.0/prism/mixins/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/mixins/sys_handler.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.643680 prism-dev-0.1.0/prism/parsers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/parsers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15219 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/parsers/ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/parsers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/parsers/yml_parser.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.646073 prism-dev-0.1.0/prism/profiles/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/profiles/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/profiles/adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/profiles/bigquery.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15559 2023-05-04 13:05:27.000000 prism-dev-0.1.0/prism/profiles/dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/profiles/meta.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/profiles/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9047 2023-05-04 13:05:27.000000 prism-dev-0.1.0/prism/profiles/profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/profiles/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/profiles/redshift.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/profiles/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/profiles/trino.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.646543 prism-dev-0.1.0/prism/spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/spark/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/spark/script.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/spark/wrapper.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1180 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4676 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.646718 prism-dev-0.1.0/prism/templates/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-dev-0.1.0/prism/templates/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.646983 prism-dev-0.1.0/prism/templates/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/agents/docker.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.647449 prism-dev-0.1.0/prism/templates/minimal_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-dev-0.1.0/prism/templates/minimal_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/minimal_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.647613 prism-dev-0.1.0/prism/templates/minimal_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/minimal_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1323 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/minimal_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.647858 prism-dev-0.1.0/prism/templates/profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.648088 prism-dev-0.1.0/prism/templates/profile/bigquery/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      153 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/bigquery/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.648256 prism-dev-0.1.0/prism/templates/profile/dbt/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/dbt/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.648450 prism-dev-0.1.0/prism/templates/profile/postgres/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/postgres/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.648621 prism-dev-0.1.0/prism/templates/profile/pyspark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      483 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/pyspark/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.648783 prism-dev-0.1.0/prism/templates/profile/redshift/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/redshift/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.648968 prism-dev-0.1.0/prism/templates/profile/snowflake/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/snowflake/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.649271 prism-dev-0.1.0/prism/templates/profile/trino/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      194 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/profile/trino/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.650031 prism-dev-0.1.0/prism/templates/starter_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/templates/starter_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/starter_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.650406 prism-dev-0.1.0/prism/templates/starter_project/data/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.0/prism/templates/starter_project/data/.exists
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.650588 prism-dev-0.1.0/prism/templates/starter_project/dev/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/templates/starter_project/dev/dev.ipynb
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.650971 prism-dev-0.1.0/prism/templates/starter_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/starter_project/modules/module01.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.651172 prism-dev-0.1.0/prism/templates/starter_project/output/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.0/prism/templates/starter_project/output/.exists
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1109 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/starter_project/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/starter_project/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.651828 prism-dev-0.1.0/prism/templates/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/tasks/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/tasks/python.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/tasks/sql.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.652483 prism-dev-0.1.0/prism/templates/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/templates/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/triggers/function.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/templates/triggers/prism_project.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.652711 prism-dev-0.1.0/prism/tests/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.655254 prism-dev-0.1.0/prism/tests/integration/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/integration/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7910 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/integration_test_class.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14137 2023-05-04 13:05:27.000000 prism-dev-0.1.0/prism/tests/integration/test_client.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10275 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4524 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_create.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4010 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5729 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4601 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_init.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.622639 prism-dev-0.1.0/prism/tests/integration/test_projects/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.656054 prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.656231 prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1117 2023-05-04 22:22:43.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.656563 prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.656991 prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1340 2023-05-04 22:22:43.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.657426 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.658349 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.658871 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.659496 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.659861 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.660624 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.661399 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.662326 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.662742 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.663849 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1264 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.664106 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.664939 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.665336 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.666302 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/csv.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/parquet.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/txt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.666468 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.666586 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.667004 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.667373 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.667754 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.668189 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.668422 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.668846 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.669112 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.669640 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.669830 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.670109 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.670876 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.671181 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.672079 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1080 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.672373 prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.672896 prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.673254 prism-dev-0.1.0/prism/tests/integration/test_projects/015_test_triggers_no_dir/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.673421 prism-dev-0.1.0/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.673875 prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.674063 prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.674532 prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.674749 prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.675194 prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.675353 prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.675817 prism-dev-0.1.0/prism/tests/integration/test_projects/common/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/common/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_projects/common/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31080 2023-05-04 22:20:29.000000 prism-dev-0.1.0/prism/tests/integration/test_run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11844 2023-03-26 19:43:45.000000 prism-dev-0.1.0/prism/tests/integration/test_spark_submit.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5358 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/integration/test_targets.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.682875 prism-dev-0.1.0/prism/tests/unit/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/unit/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.683195 prism-dev-0.1.0/prism/tests/unit/dummy_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/dummy_modules/dummy_module1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13709 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_adapter_profile.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.683307 prism-dev-0.1.0/prism/tests/unit/test_agent/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_agent/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_agents.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_dag_fns.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.684160 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.685901 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.692523 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.693187 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.694870 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.696318 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.698237 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/unit/test_import.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5017 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_jinja.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10636 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_module_parser.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.701988 prism-dev-0.1.0/prism/tests/unit/test_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/bad_run_no_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/diff_import_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/if_name_main.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/no_run_func.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/other_classes.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_modules/tasks_refs.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.703854 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/multiple_profiles.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/no_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/non_null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/triggers_normal.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_trigger.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.704222 prism-dev-0.1.0/prism/tests/unit/test_trigger_yml/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_trigger_yml/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-dev-0.1.0/prism/tests/unit/test_trigger_yml/test_fn.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.704438 prism-dev-0.1.0/prism/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19434 2023-05-04 14:37:27.000000 prism-dev-0.1.0/prism/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-dev-0.1.0/prism/ui.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-05 11:34:30.705612 prism-dev-0.1.0/prism_dev.egg-info/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5557 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15808 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/SOURCES.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/dependency_links.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       42 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/entry_points.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/not-zip-safe
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      553 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/requires.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       15 2023-05-05 11:34:30.000000 prism-dev-0.1.0/prism_dev.egg-info/top_level.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-dev-0.1.0/pyproject.toml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1727 2023-05-05 11:34:30.706462 prism-dev-0.1.0/setup.cfg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-dev-0.1.0/setup.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.550318 prism-dev-0.1.1/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-dev-0.1.1/LICENSE
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-dev-0.1.1/MANIFEST.in
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5534 2023-05-17 12:13:42.550425 prism-dev-0.1.1/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4572 2023-05-16 12:50:41.000000 prism-dev-0.1.1/README.md
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.439597 prism-dev-0.1.1/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-dev-0.1.1/prism/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/admin.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.444039 prism-dev-0.1.1/prism/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7778 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18475 2023-05-15 14:21:16.000000 prism-dev-0.1.1/prism/agents/docker_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    37139 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/ec2.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/agents/meta.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.446648 prism-dev-0.1.1/prism/agents/scripts/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-dev-0.1.1/prism/agents/scripts/__init__.py
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3276 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/scripts/apply.sh
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      680 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/scripts/run.sh
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.449398 prism-dev-0.1.1/prism/cli/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/cli/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9886 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/cli/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6974 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/cli/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6235 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/cli/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4391 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4186 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4548 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4408 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5415 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/cli/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5452 2023-05-04 13:05:27.000000 prism-dev-0.1.1/prism/cli/init.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9372 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/cli/spark_submit.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.449660 prism-dev-0.1.1/prism/client/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12158 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/client/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4973 2023-05-16 03:01:00.000000 prism-dev-0.1.1/prism/constants.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6480 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/decorators.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.449843 prism-dev-0.1.1/prism/docs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/docs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.455189 prism-dev-0.1.1/prism/docs/build/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/311ea03002abadcdcaba.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/54968a39190c43d592b9.svg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/docs/build/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/ce188596011a8fa32931.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/docs/build/index.html
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/docs/build/main.js.LICENSE.txt
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.455567 prism-dev-0.1.1/prism/event_managers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/event_managers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5985 2023-05-04 14:38:23.000000 prism-dev-0.1.1/prism/event_managers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6544 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/exceptions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.460701 prism-dev-0.1.1/prism/infra/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/infra/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13452 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/infra/compiler.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12699 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/infra/executor.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2395 2023-05-04 13:05:27.000000 prism-dev-0.1.1/prism/infra/hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/infra/manifest.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6433 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/infra/module.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3629 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/infra/pipeline.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17123 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/infra/project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/infra/sys_path.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      719 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/infra/task_manager.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21250 2023-05-15 14:21:16.000000 prism-dev-0.1.1/prism/logging.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22073 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/main.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.463633 prism-dev-0.1.1/prism/mixins/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/mixins/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2823 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/mixins/aws.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/mixins/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8170 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/mixins/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7300 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/mixins/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2306 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4713 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5422 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/mixins/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/mixins/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/mixins/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/sys_handler.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.464283 prism-dev-0.1.1/prism/parsers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/parsers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15219 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/parsers/ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/parsers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/parsers/yml_parser.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.468775 prism-dev-0.1.1/prism/profiles/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/profiles/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/bigquery.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15601 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/profiles/dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/profiles/meta.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9047 2023-05-04 13:05:27.000000 prism-dev-0.1.1/prism/profiles/profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/profiles/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/redshift.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/trino.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.469581 prism-dev-0.1.1/prism/spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/spark/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/spark/script.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/spark/wrapper.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1180 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4676 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.469788 prism-dev-0.1.1/prism/templates/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-dev-0.1.1/prism/templates/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.470267 prism-dev-0.1.1/prism/templates/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/agents/docker.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-16 03:00:05.000000 prism-dev-0.1.1/prism/templates/agents/ec2.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471219 prism-dev-0.1.1/prism/templates/minimal_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/templates/minimal_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/minimal_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471419 prism-dev-0.1.1/prism/templates/minimal_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/minimal_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1323 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/minimal_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471612 prism-dev-0.1.1/prism/templates/profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471858 prism-dev-0.1.1/prism/templates/profile/bigquery/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      153 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/bigquery/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.473508 prism-dev-0.1.1/prism/templates/profile/dbt/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/dbt/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.473803 prism-dev-0.1.1/prism/templates/profile/postgres/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/postgres/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.473996 prism-dev-0.1.1/prism/templates/profile/pyspark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      483 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/pyspark/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.474183 prism-dev-0.1.1/prism/templates/profile/redshift/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/redshift/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.474388 prism-dev-0.1.1/prism/templates/profile/snowflake/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/snowflake/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.474558 prism-dev-0.1.1/prism/templates/profile/trino/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      194 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/trino/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.476260 prism-dev-0.1.1/prism/templates/starter_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/templates/starter_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/starter_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.477202 prism-dev-0.1.1/prism/templates/starter_project/data/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/templates/starter_project/data/.exists
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.477364 prism-dev-0.1.1/prism/templates/starter_project/dev/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/templates/starter_project/dev/dev.ipynb
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.477793 prism-dev-0.1.1/prism/templates/starter_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/starter_project/modules/module01.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.478036 prism-dev-0.1.1/prism/templates/starter_project/output/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/templates/starter_project/output/.exists
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1109 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/starter_project/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/starter_project/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.478577 prism-dev-0.1.1/prism/templates/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/tasks/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/tasks/python.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/tasks/sql.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.480730 prism-dev-0.1.1/prism/templates/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/triggers/function.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/triggers/prism_project.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.480899 prism-dev-0.1.1/prism/tests/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.487213 prism-dev-0.1.1/prism/tests/integration/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/integration/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7910 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/integration_test_class.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14197 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/tests/integration/test_client.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10275 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4524 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_create.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4010 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5729 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4601 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_init.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.429699 prism-dev-0.1.1/prism/tests/integration/test_projects/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.494853 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.495306 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1117 2023-05-15 12:58:47.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.495883 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.496119 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1340 2023-05-15 12:58:47.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.499058 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.501910 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.504024 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.504573 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.504854 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.505342 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.506511 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.507160 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.508678 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.509702 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1264 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.510049 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.510957 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.511444 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.512697 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/parquet.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/txt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.512984 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.513125 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.513527 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.513843 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.514127 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.514528 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.514734 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515036 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515237 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515629 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515819 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.516087 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.517173 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.521927 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.524749 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1080 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.525119 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.526009 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.526450 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.526621 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.527099 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.527614 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.529180 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.529645 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.530148 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.530322 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.530613 prism-dev-0.1.1/prism/tests/integration/test_projects/common/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/common/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/common/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31080 2023-05-04 22:20:29.000000 prism-dev-0.1.1/prism/tests/integration/test_run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11844 2023-03-26 19:43:45.000000 prism-dev-0.1.1/prism/tests/integration/test_spark_submit.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5358 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_targets.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534336 prism-dev-0.1.1/prism/tests/unit/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534625 prism-dev-0.1.1/prism/tests/unit/dummy_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/dummy_modules/dummy_module1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13709 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_adapter_profile.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534741 prism-dev-0.1.1/prism/tests/unit/test_agent/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_agent/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_agents.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_dag_fns.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534930 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.536177 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.539908 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.540691 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.541930 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.542968 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.544196 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_import.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5017 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_jinja.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10636 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_module_parser.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.546809 prism-dev-0.1.1/prism/tests/unit/test_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/bad_run_no_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/diff_import_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/if_name_main.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/no_run_func.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/other_classes.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/tasks_refs.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.548379 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/no_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/non_null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/triggers_normal.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_trigger.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.548728 prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/test_fn.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.548895 prism-dev-0.1.1/prism/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19434 2023-05-04 14:37:27.000000 prism-dev-0.1.1/prism/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-dev-0.1.1/prism/ui.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.550204 prism-dev-0.1.1/prism_dev.egg-info/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5534 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15970 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       42 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/entry_points.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-05 11:34:30.000000 prism-dev-0.1.1/prism_dev.egg-info/not-zip-safe
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      553 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/requires.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       15 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/top_level.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-dev-0.1.1/pyproject.toml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1753 2023-05-17 12:13:42.550827 prism-dev-0.1.1/setup.cfg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-dev-0.1.1/setup.py
```

### Comparing `prism-dev-0.1.0/LICENSE` & `prism-dev-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/PKG-INFO` & `prism-dev-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-dev
-Version: 0.1.0
+Version: 0.1.1
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -98,18 +98,19 @@
 | **Trino** | ```pip install "prism-ds[trino]"``` |
 
 ### Agents
 Agents allow users to run their projects on external computing environments, e.g., Docker containers, EC2 instances, EMR clusters, and more. Prism currently supports the following agents:
 | Agent      | Command |
 | ------------ | ----------- |
 | **docker** | ```pip install "prism-ds[docker]"``` |
+| **ec2** | N/A - comes with base Prism |
 
 
 ## Product Roadmap
 
 We're always looking to improve our product. Here's what we're working on at the moment:
 
-- **Agents**: Agents allow users to run their projects on containers (e.g., Docker) or virtual machines (e.g., Amazon EMR, Amazon EC2)
+- **Additional Agents**: EMR clusters, Databricks clusters, and more!
 - **Additional adapters**: Celery, Dask, MySQL, Presto, and more!
 - **Cloud deployment**: Managed orchestration platform to deploy Prism projects in the cloud
 
 Let us know if you'd like to see another feature!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prism-dev Version: 0.1.0 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-dev Version: 0.1.1 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -56,13 +56,13 @@
 "prism-ds[postgres]"``` | | **PySpark** | ```pip install "prism-ds[pyspark]"```
 | | **Redshift** | ```pip install "prism-ds[redshift]"``` | | **Snowflake** |
 ```pip install "prism-ds[snowflake]"``` | | **Trino** | ```pip install "prism-
 ds[trino]"``` | ### Agents Agents allow users to run their projects on external
 computing environments, e.g., Docker containers, EC2 instances, EMR clusters,
 and more. Prism currently supports the following agents: | Agent | Command | |
 ------------ | ----------- | | **docker** | ```pip install "prism-ds
-[docker]"``` | ## Product Roadmap We're always looking to improve our product.
-Here's what we're working on at the moment: - **Agents**: Agents allow users to
-run their projects on containers (e.g., Docker) or virtual machines (e.g.,
-Amazon EMR, Amazon EC2) - **Additional adapters**: Celery, Dask, MySQL, Presto,
-and more! - **Cloud deployment**: Managed orchestration platform to deploy
-Prism projects in the cloud Let us know if you'd like to see another feature!
+[docker]"``` | | **ec2** | N/A - comes with base Prism | ## Product Roadmap
+We're always looking to improve our product. Here's what we're working on at
+the moment: - **Additional Agents**: EMR clusters, Databricks clusters, and
+more! - **Additional adapters**: Celery, Dask, MySQL, Presto, and more! -
+**Cloud deployment**: Managed orchestration platform to deploy Prism projects
+in the cloud Let us know if you'd like to see another feature!
```

### Comparing `prism-dev-0.1.0/README.md` & `prism-dev-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -66,18 +66,19 @@
 | **Trino** | ```pip install "prism-ds[trino]"``` |
 
 ### Agents
 Agents allow users to run their projects on external computing environments, e.g., Docker containers, EC2 instances, EMR clusters, and more. Prism currently supports the following agents:
 | Agent      | Command |
 | ------------ | ----------- |
 | **docker** | ```pip install "prism-ds[docker]"``` |
+| **ec2** | N/A - comes with base Prism |
 
 
 ## Product Roadmap
 
 We're always looking to improve our product. Here's what we're working on at the moment:
 
-- **Agents**: Agents allow users to run their projects on containers (e.g., Docker) or virtual machines (e.g., Amazon EMR, Amazon EC2)
+- **Additional Agents**: EMR clusters, Databricks clusters, and more!
 - **Additional adapters**: Celery, Dask, MySQL, Presto, and more!
 - **Cloud deployment**: Managed orchestration platform to deploy Prism projects in the cloud
 
 Let us know if you'd like to see another feature!
```

#### html2text {}

```diff
@@ -43,13 +43,13 @@
 "prism-ds[postgres]"``` | | **PySpark** | ```pip install "prism-ds[pyspark]"```
 | | **Redshift** | ```pip install "prism-ds[redshift]"``` | | **Snowflake** |
 ```pip install "prism-ds[snowflake]"``` | | **Trino** | ```pip install "prism-
 ds[trino]"``` | ### Agents Agents allow users to run their projects on external
 computing environments, e.g., Docker containers, EC2 instances, EMR clusters,
 and more. Prism currently supports the following agents: | Agent | Command | |
 ------------ | ----------- | | **docker** | ```pip install "prism-ds
-[docker]"``` | ## Product Roadmap We're always looking to improve our product.
-Here's what we're working on at the moment: - **Agents**: Agents allow users to
-run their projects on containers (e.g., Docker) or virtual machines (e.g.,
-Amazon EMR, Amazon EC2) - **Additional adapters**: Celery, Dask, MySQL, Presto,
-and more! - **Cloud deployment**: Managed orchestration platform to deploy
-Prism projects in the cloud Let us know if you'd like to see another feature!
+[docker]"``` | | **ec2** | N/A - comes with base Prism | ## Product Roadmap
+We're always looking to improve our product. Here's what we're working on at
+the moment: - **Additional Agents**: EMR clusters, Databricks clusters, and
+more! - **Additional adapters**: Celery, Dask, MySQL, Presto, and more! -
+**Cloud deployment**: Managed orchestration platform to deploy Prism projects
+in the cloud Let us know if you'd like to see another feature!
```

### Comparing `prism-dev-0.1.0/prism/admin.py` & `prism-dev-0.1.1/prism/admin.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/agents/docker_agent.py` & `prism-dev-0.1.1/prism/agents/docker_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,39 +165,19 @@
         }
         optional_keys = {
             "image": str,
             "server_url": str,
             "env": dict
         }
 
-        # Check required keys
-        for _key, _type in required_keys.items():
-            if _key not in list(agent_conf.keys()):
-                raise prism.exceptions.InvalidAgentsConfException(
-                    message=f"`{_key}` not in agent `{self.agent_name}` configuration"
-                )
-
-            if not isinstance(agent_conf[_key], _type):
-                raise prism.exceptions.InvalidAgentsConfException(
-                    message=f"`{_key}` is not the correct type"
-                )
-
-        # Check optional keys, if they exist
-        for _key, _type in optional_keys.items():  # type: ignore
-            if _key in list(agent_conf.keys()):
-                if (
-                    agent_conf[_key] is not None
-                    and not isinstance(agent_conf[_key], _type)  # noqa: W503
-                ):
-                    raise prism.exceptions.InvalidAgentsConfException(
-                        message=f"`{_key}` is not the correct type"
-                    )
-
-        # If no exception has been raised, return True
-        return True
+        return self.check_conf_keys(
+            agent_conf,
+            required_keys,
+            optional_keys
+        )
 
     def _copy_file_dir(self,
         src: Optional[Union[str, Path]],
         target: Path,
     ):
         """
         Copy directory from source to target
@@ -206,28 +186,30 @@
             src: source directory to copy
             target: target location of directory
         returns:
             None
         """
         if src is None:
             return
-        if Path(src).is_dir() and not target.is_dir():
-            shutil.copytree(
+        if Path(src).is_dir():
+            # Mypy doesn't think the `dirs_exist_ok` argument exists, but it does...
+            shutil.copytree(  # type: ignore
                 src,
-                target
+                target,
+                dirs_exist_ok=True
             )
         elif Path(src).is_file() and not target.is_file():
             # Make the parent directory first
             if not os.path.exists(Path(target).parent):
                 os.makedirs(Path(target.parent), exist_ok=True)
 
             # Copy file
             shutil.copyfile(
                 src,
-                target
+                target,
             )
         return
 
     def parse_profile_paths(self,
         project: PrismProject
     ):
         """
@@ -492,38 +474,16 @@
             )
         self.image_version = new_img_version
 
     def run(self):
         """
         Run the project using the Docker agent
         """
-        # Construct command
-        full_tb = self.args.full_tb
-        log_level = self.args.log_level
-        vars = self.args.vars
-        context = self.args.context
-        modules = self.args.modules
-        all_upstream = self.args.all_upstream
-        all_downstream = self.args.all_downstream
-
-        # Namespace to string conversion
-        full_tb_cmd = "" if not full_tb else "--full-tb"
-        log_level_cmd = "" if log_level == "info" else f"--log-level {log_level}"
-        vars_cmd = "" if vars is None else " ".join([
-            f"{k}={v}" for k, v in vars.items()
-        ])
-        context_cmd = "" if context == '{}' else f"--context '{context}'"
-        modules_cmd = "" if modules is None else "--modules " + " ".join([
-            m for m in modules
-        ])
-        all_upstream_cmd = "" if not all_upstream else "--all-upstream"
-        all_downstream_cmd = "" if not all_downstream else "--all-downstream"
-
         # Full command
-        full_cmd = f"prism run {full_tb_cmd} {log_level_cmd} {vars_cmd} {context_cmd} {modules_cmd} {all_upstream_cmd} {all_downstream_cmd}"  # noqa: E501
+        full_cmd = self.construct_command()
 
         # Run container
         container = client.containers.run(
             f"{self.image_name}:{self.image_version}",
             command=full_cmd,
             detach=True,
             stdout=True,
@@ -536,7 +496,27 @@
             log_str = log.decode('utf-8')
             no_newline = log_str.replace("\n", "")
             if not re.findall(r"^[\-]+$", no_newline):
                 prism.logging.DEFAULT_LOGGER.agent(  # type: ignore
                     f"{prism.ui.AGENT_EVENT}{self.image_name}:{self.image_version}{prism.ui.AGENT_WHICH_RUN}[run]{prism.ui.RESET} | {no_newline}"  # noqa: E501
                 )
         return
+
+    def delete(self):
+        """
+        Delete the Docker agent
+        """
+        # Fire an empty line event... it just looks nicer
+        prism.logging.fire_empty_line_event()
+        log_prefix = f"{prism.ui.AGENT_EVENT}{self.image_name}:{self.image_version}{prism.ui.RED}[delete]{prism.ui.RESET}"  # noqa: E501
+
+        # Remove all images with the label "stage=intermediate"
+        images = client.images.list(
+            filters={"label": "stage=intermediate"}
+        )
+        for img in images:
+            prism.logging.DEFAULT_LOGGER.agent(  # type: ignore
+                f"{log_prefix} | Deleting image {prism.ui.MAGENTA}{img.tags[0]}{prism.ui.RESET}"  # noqa: E501
+            )
+            client.images.remove(
+                image=img.tags[0]
+            )
```

### Comparing `prism-dev-0.1.0/prism/agents/meta.py` & `prism-dev-0.1.1/prism/agents/meta.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/agent.py` & `prism-dev-0.1.1/prism/cli/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
             prism_project,
         )
 
         # If we just want to run the agent, we do that in a separate function call.
         if args.which == "agent-run":
             return agent
 
+        elif args.which == "agent-delete":
+            agent.delete()
+
         # Otherwise, we either want to build the agent (`prism agent apply`) or build &
         # run the agent (`prism agent build`). We run the agent in a separate function,
         # so focus on just building it for now.
         else:
             agent.apply()
             return agent
 
@@ -180,19 +183,30 @@
                 event_list,
                 log_level='error'
             )
             event_list = self.fire_tail_event(event_list)
             return prism.cli.base.TaskRunReturnResult(event_list, True)
 
         # ------------------------------------------------------------------------------
+        # Delete the agent
+
+        # If the user wants to delete the agent, then execute the delete function and
+        # return
+        if self.args.which == "agent-delete":
+            event_list = fire_console_event(
+                prism.logging.DeletingAgentEvent(),
+                event_list
+            )
+
+        # ------------------------------------------------------------------------------
         # Create the agent
 
         # Fire a log event indicating that we're creating the agent (we only do this for
         # `agent-apply` and `agent-build`).
-        if self.args.which in ["agent-apply", "agent-build"]:
+        elif self.args.which in ["agent-apply", "agent-build"]:
             event_list = fire_console_event(
                 prism.logging.CreatingAgentEvent(),
                 event_list
             )
 
         # The build_agent function will only actually *build* the agent if `agent-apply`
         # or `agent-build` is called. Otherwise, it will just instantiate the Agent
@@ -226,15 +240,14 @@
             )
             event_list = self.fire_tail_event(event_list)
             return prism.cli.base.TaskRunReturnResult(event_list, True)
 
         # ------------------------------------------------------------------------------
         # Execute the agent
 
-        # If we built the agents and streamed the logs, then fire an empty line event.
         if self.args.which in ["agent-apply", "agent-build"]:
             event_list = fire_empty_line_event(event_list)
 
         # Only execute the agent with `agent-run` or `agent-build`
         if self.args.which in ["agent-run", "agent-build"]:
             event_list = fire_console_event(
                 prism.logging.StreamingLogsStartEvent(),
```

### Comparing `prism-dev-0.1.0/prism/cli/base.py` & `prism-dev-0.1.1/prism/cli/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/compile.py` & `prism-dev-0.1.1/prism/cli/compile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/connect.py` & `prism-dev-0.1.1/prism/cli/connect.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/create_agent.py` & `prism-dev-0.1.1/prism/cli/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/create_task.py` & `prism-dev-0.1.1/prism/cli/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/create_trigger.py` & `prism-dev-0.1.1/prism/cli/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/graph.py` & `prism-dev-0.1.1/prism/cli/graph.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/init.py` & `prism-dev-0.1.1/prism/cli/init.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/run.py` & `prism-dev-0.1.1/prism/cli/run.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/cli/spark_submit.py` & `prism-dev-0.1.1/prism/cli/spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/client/__init__.py` & `prism-dev-0.1.1/prism/client/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/decorators.py` & `prism-dev-0.1.1/prism/decorators.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/docs/build/311ea03002abadcdcaba.png` & `prism-dev-0.1.1/prism/docs/build/311ea03002abadcdcaba.png`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/docs/build/54968a39190c43d592b9.svg` & `prism-dev-0.1.1/prism/docs/build/54968a39190c43d592b9.svg`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/docs/build/737ad70b3f2d3a9b5f6e.ico` & `prism-dev-0.1.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/docs/build/ce188596011a8fa32931.png` & `prism-dev-0.1.1/prism/docs/build/ce188596011a8fa32931.png`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/docs/build/index.html` & `prism-dev-0.1.1/prism/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/docs/build/main.js.LICENSE.txt` & `prism-dev-0.1.1/prism/docs/build/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/event_managers/base.py` & `prism-dev-0.1.1/prism/event_managers/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/exceptions.py` & `prism-dev-0.1.1/prism/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,7 +276,33 @@
 
     def __init__(self, environment_var):
         self.message = f"environment variable `{environment_var}` not found"
         super().__init__(self.message)
 
     def __str__(self):
         return self.message
+
+
+class ClusterNotFoundException(PrismException):
+    """
+    Exception raise if the EMR agent (cluster) is not found
+    """
+
+    def __init__(self, cluster_id: str):
+        self.message = f"cluster `{cluster_id}` not found!"
+        super().__init__(self.message)
+
+    def __str__(self):
+        return self.message
+
+
+class AwsException(PrismException):
+    """
+    Exception raise if the EMR agent (cluster) is not found
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+    def __str__(self):
+        return self.message
```

### Comparing `prism-dev-0.1.0/prism/infra/compiler.py` & `prism-dev-0.1.1/prism/infra/compiler.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/executor.py` & `prism-dev-0.1.1/prism/infra/executor.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/hooks.py` & `prism-dev-0.1.1/prism/infra/hooks.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/manifest.py` & `prism-dev-0.1.1/prism/infra/manifest.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/module.py` & `prism-dev-0.1.1/prism/infra/module.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/pipeline.py` & `prism-dev-0.1.1/prism/infra/pipeline.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/project.py` & `prism-dev-0.1.1/prism/infra/project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/sys_path.py` & `prism-dev-0.1.1/prism/infra/sys_path.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/infra/task_manager.py` & `prism-dev-0.1.1/prism/infra/task_manager.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/logging.py` & `prism-dev-0.1.1/prism/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,18 +154,18 @@
         raise AttributeError('{} already defined in logger class'.format(method_name))
 
     # This method was inspired by the answers to Stack Overflow post
     # http://stackoverflow.com/q/2183233/2988730, especially
     # http://stackoverflow.com/a/13638084/2988730
     def logForLevel(self, message, *args, **kwargs):
         if self.isEnabledFor(level_num):
-            self._log(level_num, message.format(**kwargs), args)
+            self._log(level_num, message, args, **kwargs)
 
     def logToRoot(message, *args, **kwargs):
-        logging.log(level_num, message.format(**kwargs), *args)
+        logging.log(level_num, message, *args, **kwargs)
 
     # Add level
     logging.addLevelName(level_num, level_name)
     setattr(logging, level_name, level_num)
     setattr(logging.getLoggerClass(), method_name, logForLevel)
     setattr(logging, method_name, logToRoot)
 
@@ -674,14 +674,21 @@
 class CreatingAgentEvent(Event):
 
     def message(self):
         return 'Creating agent...'
 
 
 @dataclass
+class DeletingAgentEvent(Event):
+
+    def message(self):
+        return 'Deleting agent...'
+
+
+@dataclass
 class DefaultServerURLEvent(Event):
 
     def message(self):
         return f"Did not find `server_url` in configuration...defaulting to {BRIGHT_YELLOW}{prism.constants.DEFAULT_SERVER_URL}{RESET}"  # noqa: E501
 
 
 @dataclass
```

### Comparing `prism-dev-0.1.0/prism/main.py` & `prism-dev-0.1.1/prism/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -729,14 +729,47 @@
     # General options
     general_options = agent_build_sub.add_argument_group("General Options")
     general_options = add_other_option_arguments(general_options)
 
     # Set defaults
     agent_build_sub.set_defaults(cls=agent.AgentTask, which='agent-build')
 
+    # ----------------------------------------------------------------------------------
+    # Add a subparser for the "run" command. This command runs the project on the agent.
+
+    desc = """
+    Delete your agent
+    """
+    agent_delete_sub = agent_sub.add_parser(
+        'delete',
+        help=desc,
+        description=desc,
+        formatter_class=RichHelpFormatter
+    )
+
+    subcommand_options = agent_delete_sub.add_argument_group('Subcommand Options')
+    subcommand_options.add_argument(
+        "-f",
+        "--file",
+        required=True,
+        help="""
+        Path to agent configuration YML
+        """
+    )
+
+    # General options
+    general_options = agent_delete_sub.add_argument_group("General Options")
+    general_options = add_other_option_arguments(general_options)
+
+    # Set defaults
+    agent_delete_sub.set_defaults(
+        cls=agent.AgentTask,
+        which='agent-delete'
+    )
+
 
 def build_full_arg_parser() -> argparse.ArgumentParser:
     """
     Build full argument parser
     """
     # Base parser
     base_parser = argparse.ArgumentParser(formatter_class=RichHelpFormatter)
```

### Comparing `prism-dev-0.1.0/prism/mixins/agent.py` & `prism-dev-0.1.1/prism/mixins/agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/base.py` & `prism-dev-0.1.1/prism/mixins/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/compile.py` & `prism-dev-0.1.1/prism/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/connect.py` & `prism-dev-0.1.1/prism/mixins/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,21 +120,21 @@
             )
         profile_type = new_profile_values_dict['type']
         if profile_type not in prism.constants.VALID_ADAPTERS:
             raise prism.exceptions.InvalidProfileException(
                 message=f"invalid type `{profile_type}`"
             )
 
-        # Check if profile already exists in adapters or clusters
+        # Check if the adapters key is defined at all
         if profile_type in prism.constants.VALID_ADAPTERS:
             try:
-                for adapter_name, adapter_body in profile_body['adapters'].items():
-                    if profile_type == adapter_body['type']:
+                for adapter_name, _ in profile_body['adapters'].items():
+                    if adapter_name == f"{profile_type}_adapter_name_here":
                         raise prism.exceptions.InvalidProfileException(
-                            message=f"profile of type `{profile_type}` already found in profile YML"  # noqa: E501
+                            message=f"adapter with name `{profile_type}_adapter_name_here` already exists! Change this adapter name and try again"  # noqa: E501
                         )
 
             # THe 'adapters' section isn't defined as of yet
             except KeyError:
                 profile_body['adapters'] = {}
 
         # If new_profile is an adapter, add the profile to the `adapters` section of
@@ -171,15 +171,15 @@
         """
         Create a connection for the inputted `profile_type`
 
         args:
             profile_type: profile type
             profile_yml_path: path to profile YML
         returns:
-            profile YML with added profile of type `profile_type`
+            profile YML with added adapter of type `profile_type`
         """
         # If the profile doesn't exist, then create it
         if not profile_yml_path.is_file():
             self.create_profile_from_template(profile_type, profile_yml_path)
             return
 
         # If the profile does exist, then update the profile based on the profile type
```

### Comparing `prism-dev-0.1.0/prism/mixins/create_agent.py` & `prism-dev-0.1.1/prism/mixins/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/create_task.py` & `prism-dev-0.1.1/prism/mixins/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/create_trigger.py` & `prism-dev-0.1.1/prism/mixins/create_trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         """
         Create a trigger for the inputted `trigger_type`
 
         args:
             trigger_type: trigger type (either `function` or `prism_project`)
             triggers_filepath: path to triggers.yml
         returns:
-            profile YML with added profile of type `trigger_type`
+            trigger YML with added trigger of type `trigger_type`
         """
         # If the profile doesn't exist, then create it
         if not triggers_filepath.is_file():
             self.create_trigger_from_template(trigger_type, triggers_filepath)
             return
 
         # If the profile does exist, then update the profile based on the profile type
```

### Comparing `prism-dev-0.1.0/prism/mixins/graph.py` & `prism-dev-0.1.1/prism/mixins/graph.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/run.py` & `prism-dev-0.1.1/prism/mixins/run.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/mixins/sys_handler.py` & `prism-dev-0.1.1/prism/mixins/sys_handler.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/parsers/ast_parser.py` & `prism-dev-0.1.1/prism/parsers/ast_parser.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/parsers/base.py` & `prism-dev-0.1.1/prism/parsers/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/parsers/yml_parser.py` & `prism-dev-0.1.1/prism/parsers/yml_parser.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/adapter.py` & `prism-dev-0.1.1/prism/profiles/adapter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/bigquery.py` & `prism-dev-0.1.1/prism/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/dbt.py` & `prism-dev-0.1.1/prism/profiles/dbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
+from argparse import Namespace
 from dataclasses import dataclass
 from datetime import datetime
 import os
 import pandas as pd
 from pathlib import Path
 from typing import List, Optional, Tuple
 from uuid import uuid4
@@ -57,15 +58,15 @@
     threads: Optional[int]
     single_threaded: bool
     profile: Optional[str]
     target: Optional[str]
 
 
 @dataclass
-class InitializeFlagsArgs:
+class InitializeFlagsArgs(Namespace):
     profiles_dir: str
     use_colors: Optional[bool]
 
 
 @dataclass
 class InitializeDbtCompileTaskArgs:
     selector_name: Optional[str]
```

### Comparing `prism-dev-0.1.0/prism/profiles/meta.py` & `prism-dev-0.1.1/prism/profiles/meta.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/postgres.py` & `prism-dev-0.1.1/prism/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/profile.py` & `prism-dev-0.1.1/prism/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/pyspark.py` & `prism-dev-0.1.1/prism/profiles/pyspark.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/redshift.py` & `prism-dev-0.1.1/prism/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/snowflake.py` & `prism-dev-0.1.1/prism/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/profiles/trino.py` & `prism-dev-0.1.1/prism/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/spark/wrapper.py` & `prism-dev-0.1.1/prism/spark/wrapper.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/target.py` & `prism-dev-0.1.1/prism/target.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/task.py` & `prism-dev-0.1.1/prism/task.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/templates/minimal_project/modules/module01.py` & `prism-dev-0.1.1/prism/templates/minimal_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/templates/minimal_project/prism_project.py` & `prism-dev-0.1.1/prism/templates/minimal_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/templates/starter_project/dev/dev.ipynb` & `prism-dev-0.1.1/prism/templates/starter_project/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/templates/starter_project/modules/module01.py` & `prism-dev-0.1.1/prism/templates/starter_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/templates/starter_project/prism_project.py` & `prism-dev-0.1.1/prism/templates/starter_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/integration_test_class.py` & `prism-dev-0.1.1/prism/tests/integration/integration_test_class.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_client.py` & `prism-dev-0.1.1/prism/tests/integration/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         dag.connect(connection_type='snowflake')
         profile_yml = self._profile_yml_as_dict(P006_SIMPLE_PROJECT_WITH_PROFILE)
         self.assertEqual(expected_snowflake_dict, profile_yml)
 
         # Try connecting to Snowflake again, this should produce an error
         with self.assertRaises(prism.exceptions.InvalidProfileException) as cm:
             dag.connect(connection_type='snowflake')
-        expected_msg = 'profile of type `snowflake` already found in profile YML'
+        expected_msg = "adapter with name `snowflake_adapter_name_here` already exists! Change this adapter name and try again"  # noqa: E501
         self.assertEqual(expected_msg, str(cm.exception))
 
         # Connect to PySpark
         dag.connect(connection_type='pyspark')
         profile_yml = self._profile_yml_as_dict(P006_SIMPLE_PROJECT_WITH_PROFILE)
         self.assertEqual(expected_snowflake_pyspark_dict, profile_yml)
```

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_compile.py` & `prism-dev-0.1.1/prism/tests/integration/test_compile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_connect.py` & `prism-dev-0.1.1/prism/tests/integration/test_connect.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_create.py` & `prism-dev-0.1.1/prism/tests/integration/test_create.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_dbt.py` & `prism-dev-0.1.1/prism/tests/integration/test_dbt.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_hooks.py` & `prism-dev-0.1.1/prism/tests/integration/test_hooks.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_init.py` & `prism-dev-0.1.1/prism/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/001_init/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/functions.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/functions.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/004_simple_project/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/modules/module04.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/007_spark_project/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/csv.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/modules/parquet.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/parquet.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/008_targets/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module02.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module03.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/modules/module04.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/012_concurrency/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py` & `prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_run.py` & `prism-dev-0.1.1/prism/tests/integration/test_run.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_spark_submit.py` & `prism-dev-0.1.1/prism/tests/integration/test_spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/integration/test_targets.py` & `prism-dev-0.1.1/prism/tests/integration/test_targets.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_adapter_profile.py` & `prism-dev-0.1.1/prism/tests/unit/test_adapter_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_agent/prism_project.py` & `prism-dev-0.1.1/prism/tests/unit/test_agent/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_agents.py` & `prism-dev-0.1.1/prism/tests/unit/test_agents.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_all_dag_fns.py` & `prism-dev-0.1.1/prism/tests/unit/test_all_dag_fns.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_jinja.py` & `prism-dev-0.1.1/prism/tests/unit/test_jinja.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_module_parser.py` & `prism-dev-0.1.1/prism/tests/unit/test_module_parser.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/bad_trigger_key.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/multiple_profiles.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/no_profile.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/no_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/non_null_profile.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/non_null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/null_profile.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_prism_project_py/triggers_normal.py` & `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/triggers_normal.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_project.py` & `prism-dev-0.1.1/prism/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_trigger.py` & `prism-dev-0.1.1/prism/tests/unit/test_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/tests/unit/test_trigger_yml/prism_project.py` & `prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/triggers/__init__.py` & `prism-dev-0.1.1/prism/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism/ui.py` & `prism-dev-0.1.1/prism/ui.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/prism_dev.egg-info/PKG-INFO` & `prism-dev-0.1.1/prism_dev.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-dev
-Version: 0.1.0
+Version: 0.1.1
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -98,18 +98,19 @@
 | **Trino** | ```pip install "prism-ds[trino]"``` |
 
 ### Agents
 Agents allow users to run their projects on external computing environments, e.g., Docker containers, EC2 instances, EMR clusters, and more. Prism currently supports the following agents:
 | Agent      | Command |
 | ------------ | ----------- |
 | **docker** | ```pip install "prism-ds[docker]"``` |
+| **ec2** | N/A - comes with base Prism |
 
 
 ## Product Roadmap
 
 We're always looking to improve our product. Here's what we're working on at the moment:
 
-- **Agents**: Agents allow users to run their projects on containers (e.g., Docker) or virtual machines (e.g., Amazon EMR, Amazon EC2)
+- **Additional Agents**: EMR clusters, Databricks clusters, and more!
 - **Additional adapters**: Celery, Dask, MySQL, Presto, and more!
 - **Cloud deployment**: Managed orchestration platform to deploy Prism projects in the cloud
 
 Let us know if you'd like to see another feature!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prism-dev Version: 0.1.0 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-dev Version: 0.1.1 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -56,13 +56,13 @@
 "prism-ds[postgres]"``` | | **PySpark** | ```pip install "prism-ds[pyspark]"```
 | | **Redshift** | ```pip install "prism-ds[redshift]"``` | | **Snowflake** |
 ```pip install "prism-ds[snowflake]"``` | | **Trino** | ```pip install "prism-
 ds[trino]"``` | ### Agents Agents allow users to run their projects on external
 computing environments, e.g., Docker containers, EC2 instances, EMR clusters,
 and more. Prism currently supports the following agents: | Agent | Command | |
 ------------ | ----------- | | **docker** | ```pip install "prism-ds
-[docker]"``` | ## Product Roadmap We're always looking to improve our product.
-Here's what we're working on at the moment: - **Agents**: Agents allow users to
-run their projects on containers (e.g., Docker) or virtual machines (e.g.,
-Amazon EMR, Amazon EC2) - **Additional adapters**: Celery, Dask, MySQL, Presto,
-and more! - **Cloud deployment**: Managed orchestration platform to deploy
-Prism projects in the cloud Let us know if you'd like to see another feature!
+[docker]"``` | | **ec2** | N/A - comes with base Prism | ## Product Roadmap
+We're always looking to improve our product. Here's what we're working on at
+the moment: - **Additional Agents**: EMR clusters, Databricks clusters, and
+more! - **Additional adapters**: Celery, Dask, MySQL, Presto, and more! -
+**Cloud deployment**: Managed orchestration platform to deploy Prism projects
+in the cloud Let us know if you'd like to see another feature!
```

### Comparing `prism-dev-0.1.0/prism_dev.egg-info/SOURCES.txt` & `prism-dev-0.1.1/prism_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 prism/main.py
 prism/target.py
 prism/task.py
 prism/ui.py
 prism/agents/__init__.py
 prism/agents/base.py
 prism/agents/docker_agent.py
+prism/agents/ec2.py
 prism/agents/meta.py
+prism/agents/scripts/__init__.py
+prism/agents/scripts/apply.sh
+prism/agents/scripts/run.sh
 prism/cli/__init__.py
 prism/cli/agent.py
 prism/cli/base.py
 prism/cli/compile.py
 prism/cli/connect.py
 prism/cli/create_agent.py
 prism/cli/create_task.py
@@ -49,14 +53,15 @@
 prism/infra/module.py
 prism/infra/pipeline.py
 prism/infra/project.py
 prism/infra/sys_path.py
 prism/infra/task_manager.py
 prism/mixins/__init__.py
 prism/mixins/agent.py
+prism/mixins/aws.py
 prism/mixins/base.py
 prism/mixins/compile.py
 prism/mixins/connect.py
 prism/mixins/create_agent.py
 prism/mixins/create_task.py
 prism/mixins/create_trigger.py
 prism/mixins/graph.py
@@ -79,14 +84,15 @@
 prism/profiles/trino.py
 prism/spark/__init__.py
 prism/spark/script.py
 prism/spark/wrapper.py
 prism/templates/__init__.py
 prism/templates/agents/__init__.py
 prism/templates/agents/docker.yml
+prism/templates/agents/ec2.yml
 prism/templates/minimal_project/.gitignore
 prism/templates/minimal_project/__init__.py
 prism/templates/minimal_project/prism_project.py
 prism/templates/minimal_project/modules/module01.py
 prism/templates/profile/__init__.py
 prism/templates/profile/bigquery/profile.yml
 prism/templates/profile/dbt/profile.yml
```

### Comparing `prism-dev-0.1.0/prism_dev.egg-info/requires.txt` & `prism-dev-0.1.1/prism_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/pyproject.toml` & `prism-dev-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.0/setup.cfg` & `prism-dev-0.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = prism-dev
 description = The easiest way to create data pipelines in Python.
 long_description_content_type = text/markdown
 long_description = file: README.md
-version = 0.1.0
+version = 0.1.1
 author = prism founders
 author_email = hello@runprism.com
 license = Apache-2.0
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
@@ -75,14 +75,15 @@
 [flake8]
 ignore = E124, E128
 per-file-ignores = 
 	prism/cli/init.py: W605
 	prism/spark/script.py: F401, E201, E202, F821
 	prism/logging.py: F821
 	prism/templates/*: E501
+	prism/constants.py: E501
 max-line-length = 88
 count = true
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

