# Comparing `tmp/schema_jobs-0.1.0.tar.gz` & `tmp/schema_jobs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_jobs-0.1.0.tar", max compression
+gzip compressed data, was "schema_jobs-0.1.1.tar", max compression
```

## Comparing `schema_jobs-0.1.0.tar` & `schema_jobs-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,19 @@
--rw-r--r--   0        0        0      440 2023-05-10 15:42:19.451156 schema_jobs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.0/schema_jobs/__init__.py
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 schema_jobs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      460 2023-05-17 19:14:50.314884 schema_jobs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:59.929513 schema_jobs-0.1.1/schema_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.1/schema_jobs/jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358473 schema_jobs-0.1.1/schema_jobs/jobs/configuration/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-16 17:55:05.825154 schema_jobs-0.1.1/schema_jobs/jobs/configuration/database_configuration.py
+-rw-r--r--   0        0        0      917 2023-05-16 18:03:06.305152 schema_jobs-0.1.1/schema_jobs/jobs/configuration/table_configs.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.1/schema_jobs/jobs/deploy/__init__.py
+-rw-r--r--   0        0        0      492 2023-05-17 18:49:09.092458 schema_jobs-0.1.1/schema_jobs/jobs/deploy/deploy_database_tables.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.1/schema_jobs/jobs/migration/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-16 18:15:04.261246 schema_jobs-0.1.1/schema_jobs/jobs/migration/deploy_migration.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.1/schema_jobs/jobs/utility/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:07:02.358000 schema_jobs-0.1.1/schema_jobs/jobs/utility/schema/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-17 18:44:53.925791 schema_jobs-0.1.1/schema_jobs/jobs/utility/schema/database.py
+-rw-r--r--   0        0        0       62 2023-05-16 18:12:06.405926 schema_jobs-0.1.1/schema_jobs/jobs/utility/schema/migration.py
+-rw-r--r--   0        0        0     1769 2023-05-17 18:22:00.078921 schema_jobs-0.1.1/schema_jobs/jobs/utility/schema/schemas.py
+-rw-r--r--   0        0        0      112 2023-05-17 18:46:35.559107 schema_jobs-0.1.1/schema_jobs/jobs/utility/schema/sql.py
+-rw-r--r--   0        0        0      433 2023-05-17 18:48:28.770890 schema_jobs-0.1.1/schema_jobs/jobs/utility/schema/table.py
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 schema_jobs-0.1.1/PKG-INFO
```

