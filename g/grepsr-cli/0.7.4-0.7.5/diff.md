# Comparing `tmp/grepsr-cli-0.7.4.tar.gz` & `tmp/grepsr-cli-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grepsr-cli-0.7.4.tar", last modified: Wed May 17 10:45:57 2023, max compression
+gzip compressed data, was "grepsr-cli-0.7.5.tar", last modified: Wed May 17 10:48:52 2023, max compression
```

## Comparing `grepsr-cli-0.7.4.tar` & `grepsr-cli-0.7.5.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.395314 grepsr-cli-0.7.4/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2023-04-21 07:31:39.000000 grepsr-cli-0.7.4/.version
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1219 2023-04-21 07:31:11.000000 grepsr-cli-0.7.4/CHANGELOG.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/LICENSE.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/MANIFEST.in
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2729 2023-05-17 10:45:57.395314 grepsr-cli-0.7.4/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2450 2023-05-17 09:49:27.000000 grepsr-cli-0.7.4/README.md
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.391314 grepsr-cli-0.7.4/grepsr_cli.egg-info/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2729 2023-05-17 10:45:57.000000 grepsr-cli-0.7.4/grepsr_cli.egg-info/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1280 2023-05-17 10:45:57.000000 grepsr-cli-0.7.4/grepsr_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2023-05-17 10:45:57.000000 grepsr-cli-0.7.4/grepsr_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2023-05-17 10:45:57.000000 grepsr-cli-0.7.4/grepsr_cli.egg-info/entry_points.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2023-05-17 10:45:57.000000 grepsr-cli-0.7.4/grepsr_cli.egg-info/requires.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2023-05-17 10:45:57.000000 grepsr-cli-0.7.4/grepsr_cli.egg-info/top_level.txt
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.391314 grepsr-cli-0.7.4/grepsrcli/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.391314 grepsr-cli-0.7.4/grepsrcli/controllers/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/controllers/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/controllers/base.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    18101 2023-05-17 09:49:27.000000 grepsr-cli-0.7.4/grepsrcli/controllers/crawler.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/controllers/generate.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/controllers/report.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.391314 grepsr-cli-0.7.4/grepsrcli/core/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/core/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr-cli-0.7.4/grepsrcli/core/aws_s3.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-03-02 07:11:29.000000 grepsr-cli-0.7.4/grepsrcli/core/config.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/core/exc.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/core/input_prompts.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr-cli-0.7.4/grepsrcli/core/message_log.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     5244 2023-05-17 09:49:27.000000 grepsr-cli-0.7.4/grepsrcli/core/multiproc_server.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/core/report_api.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-03-02 07:11:29.000000 grepsr-cli-0.7.4/grepsrcli/core/sdk_setup.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     6178 2023-05-17 09:49:27.000000 grepsr-cli-0.7.4/grepsrcli/core/test_local.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    11117 2023-04-21 07:32:16.000000 grepsr-cli-0.7.4/grepsrcli/core/utils.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.391314 grepsr-cli-0.7.4/grepsrcli/ext/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/ext/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2023-05-17 09:49:27.000000 grepsr-cli-0.7.4/grepsrcli/main.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.391314 grepsr-cli-0.7.4/grepsrcli/plugins/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/plugins/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.395314 grepsr-cli-0.7.4/grepsrcli/templates/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/templates/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/templates/autocomplete.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/templates/autocomplete_zsh.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/templates/composer.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/templates/node_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1846 2023-03-07 07:03:13.000000 grepsr-cli-0.7.4/grepsrcli/templates/php_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3087 2023-03-07 07:03:13.000000 grepsr-cli-0.7.4/grepsrcli/templates/php_brp_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1904 2023-04-21 07:31:11.000000 grepsr-cli-0.7.4/grepsrcli/templates/php_vc_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/grepsrcli/templates/py_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/requirements-dev.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2023-04-21 07:31:11.000000 grepsr-cli-0.7.4/requirements.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2023-05-17 10:45:57.395314 grepsr-cli-0.7.4/setup.cfg
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr-cli-0.7.4/setup.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:45:57.395314 grepsr-cli-0.7.4/tests/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      949 2023-01-07 17:34:33.000000 grepsr-cli-0.7.4/tests/test_grepsrcli.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2023-05-17 10:48:13.000000 grepsr-cli-0.7.5/.version
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1219 2023-04-21 07:31:11.000000 grepsr-cli-0.7.5/CHANGELOG.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/LICENSE.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/MANIFEST.in
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3178 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2899 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/README.md
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.852318 grepsr-cli-0.7.5/grepsr_cli.egg-info/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3178 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1245 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/requires.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/top_level.txt
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.852318 grepsr-cli-0.7.5/grepsrcli/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.852318 grepsr-cli-0.7.5/grepsrcli/controllers/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/base.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    16858 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/grepsrcli/controllers/crawler.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/generate.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/report.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/core/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr-cli-0.7.5/grepsrcli/core/aws_s3.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-03-02 07:11:29.000000 grepsr-cli-0.7.5/grepsrcli/core/config.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/exc.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/input_prompts.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr-cli-0.7.5/grepsrcli/core/message_log.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/report_api.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-03-02 07:11:29.000000 grepsr-cli-0.7.5/grepsrcli/core/sdk_setup.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     5716 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/grepsrcli/core/test_local.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    11117 2023-04-21 07:32:16.000000 grepsr-cli-0.7.5/grepsrcli/core/utils.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/ext/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/ext/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2157 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/grepsrcli/main.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/plugins/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/plugins/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/templates/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/autocomplete.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/autocomplete_zsh.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/composer.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/node_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1846 2023-03-07 07:03:13.000000 grepsr-cli-0.7.5/grepsrcli/templates/php_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3087 2023-03-07 07:03:13.000000 grepsr-cli-0.7.5/grepsrcli/templates/php_brp_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1904 2023-04-21 07:31:11.000000 grepsr-cli-0.7.5/grepsrcli/templates/php_vc_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/py_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/requirements-dev.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2023-04-21 07:31:11.000000 grepsr-cli-0.7.5/requirements.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/setup.cfg
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/setup.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/tests/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      949 2023-01-07 17:34:33.000000 grepsr-cli-0.7.5/tests/test_grepsrcli.py
```

### Comparing `grepsr-cli-0.7.4/CHANGELOG.md` & `grepsr-cli-0.7.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/PKG-INFO` & `grepsr-cli-0.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -78,7 +78,13 @@
 `pip uninstall grepsr-cli`
 
 ```bash
 git clone git@bitbucket.org:zznixt07/gcli.git grepsrcli
 cd grepsrcli
 pip install -e .
 ```
+
+## Features Added
+- stash untracked files to avoid failure when applying stash.
+- drop stash after pushed successully. Before this, all stashes were always kept.
+- run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
+- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
```

### Comparing `grepsr-cli-0.7.4/README.md` & `grepsr-cli-0.7.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -66,8 +66,14 @@
 > Be sure to uninstall gcli first, with
 `pip uninstall grepsr-cli`
 
 ```bash
 git clone git@bitbucket.org:zznixt07/gcli.git grepsrcli
 cd grepsrcli
 pip install -e .
-```
+```
+
+## Features Added
+- stash untracked files to avoid failure when applying stash.
+- drop stash after pushed successully. Before this, all stashes were always kept.
+- run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
+- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
```

### Comparing `grepsr-cli-0.7.4/grepsr_cli.egg-info/PKG-INFO` & `grepsr-cli-0.7.5/grepsr_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -78,7 +78,13 @@
 `pip uninstall grepsr-cli`
 
 ```bash
 git clone git@bitbucket.org:zznixt07/gcli.git grepsrcli
 cd grepsrcli
 pip install -e .
 ```
+
+## Features Added
+- stash untracked files to avoid failure when applying stash.
+- drop stash after pushed successully. Before this, all stashes were always kept.
+- run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
+- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
```

### Comparing `grepsr-cli-0.7.4/grepsr_cli.egg-info/SOURCES.txt` & `grepsr-cli-0.7.5/grepsr_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 grepsrcli/controllers/report.py
 grepsrcli/core/__init__.py
 grepsrcli/core/aws_s3.py
 grepsrcli/core/config.py
 grepsrcli/core/exc.py
 grepsrcli/core/input_prompts.py
 grepsrcli/core/message_log.py
-grepsrcli/core/multiproc_server.py
 grepsrcli/core/report_api.py
 grepsrcli/core/sdk_setup.py
 grepsrcli/core/test_local.py
 grepsrcli/core/utils.py
 grepsrcli/ext/__init__.py
 grepsrcli/plugins/__init__.py
 grepsrcli/templates/__init__.py
```

### Comparing `grepsr-cli-0.7.4/grepsrcli/controllers/base.py` & `grepsr-cli-0.7.5/grepsrcli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/controllers/crawler.py` & `grepsr-cli-0.7.5/grepsrcli/controllers/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from os import system, path
-import os
 import sys
+import time
 import subprocess
-import multiprocessing
-import signal
 import json
 import pathlib
 from semver import VersionInfo
 from cement import Controller, ex
 from ..core.config import load_config
 from ..core.utils import (
     create_boilerplate,
@@ -18,14 +16,15 @@
     user_input,
     insert_all_chained_dependencies
 )
 from ..core.test_local import TestLocal
 from ..core.message_log import Log
 from ..core.aws_s3 import S3
 
+
 class CrawlerBase(Controller):
     class Meta:
         label = 'crawler_base'
 
 
 class Crawler(Controller):
     config = load_config('config.yml')
@@ -65,55 +64,31 @@
     def test(self):
         plugin_name = self.app.pargs.plugin_name
         main_fn_params = self.app.pargs.params
         main_fn_params_file = self.app.pargs.params_file
         is_multi_proc = self.app.pargs.multi_proc_mode
 
         platforms = ['php', 'php_next']
-        proc = None
         for platform in platforms:
             if platform in self.config:
                 plugin_path = get_plugin_path(plugin_name, type=platform)
                 if plugin_path:
                     base_path = pathlib.Path(get_plugin_path(plugin_name, type=platform)).parent
-                    if is_multi_proc == '1':
-                        from ..core import multiproc_server
-                        proc = multiprocessing.Process(target=multiproc_server.start, args=[])
-                        proc.start()
                     try:
                         TestLocal(type=platform, base_path=base_path, plugin_name=plugin_name, params=main_fn_params, params_file=main_fn_params_file, is_multi_proc=is_multi_proc)
                     except json.JSONDecodeError as e:
                         self.app.log.error(f"Error decoding params as JSON. {e}")
                         self.app.exit_code = 10
                     except FileNotFoundError as e:
                         self.app.log.error(f"Params file: `{main_fn_params_file}` not found. {e}")
                         self.app.exit_code = 20
                     break
         else:
             self.app.log.error(f"path: {plugin_name} not found!")
             self.app.exit_code = 127
-        if proc:
-            print('terminating server proc', flush=True)
-
-            '''these 2 methods cannot kill the currently running process on linux.
-            Although they will raise an Exception on the target server process,
-            the child process of that script cannot be terminated from it.
-            '''
-            # proc.terminate()
-            # proc.kill()
-            
-            '''instead killing whole process group works on linux.
-            The OS handles this, killing all the processes at once.
-            '''
-            pgid = os.getpgid(os.getpid())
-            if pgid == 1:
-                os.kill(os.getpid(), signal.SIGINT)
-            else:
-                os.killpg(os.getpgid(os.getpid()), signal.SIGINT)
-
 
     @ex(
         help="performs git pull to update the codebase",
         arguments=[
             (['-t', '--type'], {
                 'action': 'store',
                 'dest': 'type',
@@ -284,19 +259,19 @@
             plugin_info = get_plugin_info(plugin_dir_path)
             if plugin_info:
                 base_class = plugin_info['base_class']
                 if base_class != 'Vtx_Service_Plugin':
                     if base_class not in plugin_info['dependencies']:
                         msg = f'Plugin extends {base_class} but does not declare it as a dependency.'
                         self.app.log.warning(msg)
-                        if user_input(f'[Experimental] Do you want to automatically add dependencies?') == 'Y':
-                            insert_all_chained_dependencies(plugin_name)
-                        go_fwd = user_input(f'Do you want to continue?')
-                        if go_fwd == 'N':
-                            continue
+                        # if user_input(f'[Experimental] Do you want to automatically add dependencies?') == 'Y':
+                        #     insert_all_chained_dependencies(plugin_name)
+                        # go_fwd = user_input(f'Do you want to continue?')
+                        # if go_fwd == 'N':
+                        #     continue
             # add .version or update .version
             version_path = '{}/.version'.format(plugin_dir_path)
             if path.exists(version_path):
                 with open(version_path, 'r') as f:
                     version_info = VersionInfo.parse(f.read())
                     if(major_flag):
                         version_info = version_info.next_version(
@@ -464,17 +439,7 @@
 
             render_boilerplate(boilerplate='composer.jinja2', data=data,
                                destination_path=target_plugin_path + '/composer.json')
             system(
                 f""" cd {target_plugin_path} &&  composer install""")
         else:
             Log.error(f"Target plugin: {target_plugin_name} not found")
-
-
-    @ex(
-        help="start multiprocess facilitation server",
-        arguments=[]
-    )
-    def multiprocess(self):
-        from ..core import multiproc_server
-        multiproc_server.start()
-
```

### Comparing `grepsr-cli-0.7.4/grepsrcli/controllers/generate.py` & `grepsr-cli-0.7.5/grepsrcli/controllers/generate.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/controllers/report.py` & `grepsr-cli-0.7.5/grepsrcli/controllers/report.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/aws_s3.py` & `grepsr-cli-0.7.5/grepsrcli/core/aws_s3.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/config.py` & `grepsr-cli-0.7.5/grepsrcli/core/config.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/message_log.py` & `grepsr-cli-0.7.5/grepsrcli/core/message_log.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/report_api.py` & `grepsr-cli-0.7.5/grepsrcli/core/report_api.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/sdk_setup.py` & `grepsr-cli-0.7.5/grepsrcli/core/sdk_setup.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/test_local.py` & `grepsr-cli-0.7.5/grepsrcli/core/test_local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from os import path, system
-import os
 import json
 import subprocess
-import platform
 from .message_log import Log
 from .config import load_config, config_path as CONFIG_PATH
 from .utils import get_docker_entrypoints, write_text, read_text
 
 class TestLocal:
     def __init__(self, type, base_path, plugin_name, params=None, params_file=None, is_multi_proc=False):
         self.type = type
@@ -33,27 +31,22 @@
         elif self.type == "php_next":
             self.test_script_php_next()
 
     def test_script_php(self, env=False):
         if self.is_multi_proc is None:
             # only use the value of multiprocess if it is not passed explicitly from cmd line
             try:
-                self.is_multi_proc = '1' if self.type_config['multiprocess'] == True else '0'
+                self.is_multi_proc = 1 if self.type_config['multiprocess'] == True else 0
             except KeyError:
                 pass
         env_vars = []
         if env:
             env_vars = [
                 f'-e {env_var}={self.type_config["env"][env_var]}' for env_var in self.type_config["env"].keys()
             ]
-        if os.environ.get('GCLI_CHILD_PROC_NUM'):
-            print('\n', flush=True)
-            print('This is Child Process Number:', os.environ.get('GCLI_CHILD_PROC_NUM'), flush=True)
-            print('\n', flush=True)
-            env_vars.append(f'-e GCLI_CHILD_PROC_NUM={os.environ.get("GCLI_CHILD_PROC_NUM")}')
         sdk_args_list = [
             f'-s {self.plugin_name}',
         ]
         if self.is_multi_proc is not None:
             sdk_args_list.append(f'-m {self.is_multi_proc}')
         docker_image_name = self.type_config["sdk_image"]
         json_content = self.params
@@ -103,17 +96,16 @@
             sdk_args = ' '.join(sdk_args_list)
             original_entrypoints = get_docker_entrypoints(image_name=docker_image_name)
             sh_contents.append(f'source {original_entrypoints[0]} {sdk_args} {pipe_params}')
             write_text(custom_shell_file_local, '\n'.join(sh_contents))
 
             bash_cmd = f'source /tmp/{custom_shell_file}'
 
-        win_single = (platform.system() == 'Windows') and (self.is_multi_proc == '1')
         commands = [
-                f'docker run {"-i" if win_single else ""} -t --network="host" --rm',
+                'docker run -t -i --network="host" --rm',
                 f'-v {self.base_path}:/home/grepsr/vortex-plugins/{path.basename(self.base_path)}',
                 f'-v {self.tmp_path}:/tmp',
                 f'-e APP_ENV={self.config["app_env"]}',
                 " ".join(env_vars),
                 f'--entrypoint=""' if not only_service else '',
                 docker_image_name,
                 f'bash -ci "{bash_cmd}"' if not only_service else sdk_args,
```

### Comparing `grepsr-cli-0.7.4/grepsrcli/core/utils.py` & `grepsr-cli-0.7.5/grepsrcli/core/utils.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/main.py` & `grepsr-cli-0.7.5/grepsrcli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
             if app.debug is True:
                 import traceback
                 traceback.print_exc()
 
         except CaughtSignal as e:
             # Default Cement signals are SIGINT and SIGTERM, exit 0 (non-error)
-            print('\n%s' % e, flush=True)
+            print('\n%s' % e)
             app.exit_code = 0
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `grepsr-cli-0.7.4/grepsrcli/templates/autocomplete_zsh.jinja2` & `grepsr-cli-0.7.5/grepsrcli/templates/autocomplete_zsh.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/templates/node_boilerplate.jinja2` & `grepsr-cli-0.7.5/grepsrcli/templates/node_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/templates/php_boilerplate.jinja2` & `grepsr-cli-0.7.5/grepsrcli/templates/php_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/templates/php_brp_boilerplate.jinja2` & `grepsr-cli-0.7.5/grepsrcli/templates/php_brp_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/templates/php_vc_boilerplate.jinja2` & `grepsr-cli-0.7.5/grepsrcli/templates/php_vc_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/grepsrcli/templates/py_boilerplate.jinja2` & `grepsr-cli-0.7.5/grepsrcli/templates/py_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/setup.py` & `grepsr-cli-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.4/tests/test_grepsrcli.py` & `grepsr-cli-0.7.5/tests/test_grepsrcli.py`

 * *Files identical despite different names*

