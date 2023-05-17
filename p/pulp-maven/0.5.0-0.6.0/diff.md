# Comparing `tmp/pulp-maven-0.5.0.tar.gz` & `tmp/pulp-maven-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-maven-0.5.0.tar", last modified: Fri Mar 17 10:15:18 2023, max compression
+gzip compressed data, was "pulp-maven-0.6.0.tar", last modified: Wed May 17 14:23:51 2023, max compression
```

## Comparing `pulp-maven-0.5.0.tar` & `pulp-maven-0.6.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-17 10:15:16.000000 pulp-maven-0.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.221429 pulp-maven-0.5.0/pulp_maven/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.221429 pulp-maven-0.5.0/pulp_maven/app/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-17 10:15:17.000000 pulp-maven-0.5.0/pulp_maven/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/maven_deploy_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.221429 pulp-maven-0.5.0/pulp_maven/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/migrations/0002_maven_related_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/migrations/0003_mavenrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/migrations/0004_swap_distribution_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/migrations/0005_mavenmetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.221429 pulp-maven-0.5.0/pulp_maven/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/pom.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/examples/App.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.217429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/AppTest.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/api/test_mvn_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/pulp_maven/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pulp_maven/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:15:18.221429 pulp-maven-0.5.0/pulp_maven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-17 10:15:18.000000 pulp-maven-0.5.0/pulp_maven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-17 10:15:18.000000 pulp-maven-0.5.0/pulp_maven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:15:18.000000 pulp-maven-0.5.0/pulp_maven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-17 10:15:18.000000 pulp-maven-0.5.0/pulp_maven.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-17 10:15:18.000000 pulp-maven-0.5.0/pulp_maven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-17 10:15:18.000000 pulp-maven-0.5.0/pulp_maven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 10:15:18.225429 pulp-maven-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-03-17 10:15:17.000000 pulp-maven-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 10:15:02.000000 pulp-maven-0.5.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.675844 pulp-maven-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-17 14:23:49.000000 pulp-maven-0.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 14:23:51.675844 pulp-maven-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 14:23:50.000000 pulp-maven-0.6.0/pulp_maven/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/maven_deploy_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/0002_maven_related_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/0003_mavenrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/0004_swap_distribution_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/0005_mavenmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/0006_alter_mavenartifact_content_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/pom.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/examples/App.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.667844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/AppTest.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/api/test_mvn_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pulp_maven/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:51.671844 pulp-maven-0.6.0/pulp_maven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 14:23:51.000000 pulp-maven-0.6.0/pulp_maven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 14:23:51.000000 pulp-maven-0.6.0/pulp_maven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:23:51.000000 pulp-maven-0.6.0/pulp_maven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 14:23:51.000000 pulp-maven-0.6.0/pulp_maven.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 14:23:51.000000 pulp-maven-0.6.0/pulp_maven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 14:23:51.000000 pulp-maven-0.6.0/pulp_maven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:23:51.675844 pulp-maven-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-05-17 14:23:50.000000 pulp-maven-0.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 14:23:39.000000 pulp-maven-0.6.0/unittest_requirements.txt
```

### Comparing `pulp-maven-0.5.0/CHANGES.rst` & `pulp-maven-0.6.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,29 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+0.6.0 (2023-05-17)
+==================
+
+Features
+--------
+
+- Added ability to add cached content to a repository.
+  `#136 <https://pulp.plan.io/issues/136>`_
+- Updated pulpcore compatibility to >=3.25.0,<3.40.
+  `#153 <https://pulp.plan.io/issues/153>`_
+
+
+----
+
+
 0.5.0 (2023-03-17)
 ==================
 
 Features
 --------
 
 - Added ability to add cached content to a repository.
```

### Comparing `pulp-maven-0.5.0/COMMITMENT` & `pulp-maven-0.6.0/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/COPYRIGHT` & `pulp-maven-0.6.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/LICENSE` & `pulp-maven-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/PKG-INFO` & `pulp-maven-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-maven
-Version: 0.5.0
+Version: 0.6.0
 Summary: pulp-maven plugin for the Pulp Project
 Home-page: http://www.pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pulp-maven-0.5.0/README.rst` & `pulp-maven-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/maven_deploy_api.py` & `pulp-maven-0.6.0/pulp_maven/app/maven_deploy_api.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/migrations/0001_initial.py` & `pulp-maven-0.6.0/pulp_maven/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/migrations/0002_maven_related_names.py` & `pulp-maven-0.6.0/pulp_maven/app/migrations/0002_maven_related_names.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/migrations/0003_mavenrepository.py` & `pulp-maven-0.6.0/pulp_maven/app/migrations/0003_mavenrepository.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/migrations/0004_swap_distribution_models.py` & `pulp-maven-0.6.0/pulp_maven/app/migrations/0004_swap_distribution_models.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/migrations/0005_mavenmetadata.py` & `pulp-maven-0.6.0/pulp_maven/app/migrations/0005_mavenmetadata.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/models.py` & `pulp-maven-0.6.0/pulp_maven/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/serializers.py` & `pulp-maven-0.6.0/pulp_maven/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/tasks/__init__.py` & `pulp-maven-0.6.0/pulp_maven/app/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/app/viewsets.py` & `pulp-maven-0.6.0/pulp_maven/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/pom.xml` & `pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/pom.xml`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/AppTest.java` & `pulp-maven-0.6.0/pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/AppTest.java`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/functional/api/test_crud_remotes.py` & `pulp-maven-0.6.0/pulp_maven/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/functional/api/test_download_content.py` & `pulp-maven-0.6.0/pulp_maven/tests/functional/api/test_download_content.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/functional/api/test_mvn_deploy.py` & `pulp-maven-0.6.0/pulp_maven/tests/functional/api/test_mvn_deploy.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/functional/conftest.py` & `pulp-maven-0.6.0/pulp_maven/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven/tests/functional/utils.py` & `pulp-maven-0.6.0/pulp_maven/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/pulp_maven.egg-info/PKG-INFO` & `pulp-maven-0.6.0/pulp_maven.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-maven
-Version: 0.5.0
+Version: 0.6.0
 Summary: pulp-maven plugin for the Pulp Project
 Home-page: http://www.pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pulp-maven-0.5.0/pulp_maven.egg-info/SOURCES.txt` & `pulp-maven-0.6.0/pulp_maven.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pulp_maven/app/urls.py
 pulp_maven/app/viewsets.py
 pulp_maven/app/migrations/0001_initial.py
 pulp_maven/app/migrations/0002_maven_related_names.py
 pulp_maven/app/migrations/0003_mavenrepository.py
 pulp_maven/app/migrations/0004_swap_distribution_models.py
 pulp_maven/app/migrations/0005_mavenmetadata.py
+pulp_maven/app/migrations/0006_alter_mavenartifact_content_ptr_and_more.py
 pulp_maven/app/migrations/__init__.py
 pulp_maven/app/tasks/__init__.py
 pulp_maven/tests/__init__.py
 pulp_maven/tests/assets/simple-project/pom.xml
 pulp_maven/tests/assets/simple-project/src/main/java/org/sonatype/nexus/examples/App.java
 pulp_maven/tests/assets/simple-project/src/test/java/org/sonatype/nexus/examples/AppTest.java
 pulp_maven/tests/functional/__init__.py
```

### Comparing `pulp-maven-0.5.0/pyproject.toml` & `pulp-maven-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-maven-0.5.0/setup.py` & `pulp-maven-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("requirements.txt") as requirements:
     requirements = requirements.readlines()
 
 setup(
     name="pulp-maven",
-    version="0.5.0",
+    version="0.6.0",
     description="pulp-maven plugin for the Pulp Project",
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-dev@redhat.com",
     url="http://www.pulpproject.org/",
     python_requires=">=3.8",
     install_requires=requirements,
```

