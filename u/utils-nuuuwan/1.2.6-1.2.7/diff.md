# Comparing `tmp/utils-nuuuwan-1.2.6.tar.gz` & `tmp/utils-nuuuwan-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-nuuuwan-1.2.6.tar", last modified: Mon Apr 17 11:59:48 2023, max compression
+gzip compressed data, was "utils-nuuuwan-1.2.7.tar", last modified: Wed May 17 09:30:36 2023, max compression
```

## Comparing `utils-nuuuwan-1.2.6.tar` & `utils-nuuuwan-1.2.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.717640 utils-nuuuwan-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 11:59:48.717640 utils-nuuuwan-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:59:48.717640 utils-nuuuwan-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.709640 utils-nuuuwan-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.709640 utils-nuuuwan-1.2.6/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/GitReadOnly.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/GitWrite.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/List.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/String.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.713640 utils-nuuuwan-1.2.6/src/utils/file/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/CSVFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/Directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/File.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/FileOrDirectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/FiledVariable.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/JSONFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/PDFFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/TSVFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/XSVFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/Zip.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/hashx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/mr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.713640 utils-nuuuwan-1.2.6/src/utils/time/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/TIMEZONE_OFFSET.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/Time.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/TimeDelta.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/TimeFormat.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/TimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/TimeUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.713640 utils-nuuuwan-1.2.6/src/utils/twitter/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/Tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/Twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/TwitterActionerMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/TwitterActionerMixinHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/TwitterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/TwitterLoaderMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/www.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/src/utils/xmlx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.713640 utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 11:59:48.000000 utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-17 11:59:48.000000 utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:59:48.000000 utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 11:59:48.000000 utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 11:59:48.000000 utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:59:48.717640 utils-nuuuwan-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_file_pdf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_filed_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_hashx.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_mr.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_random_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_twitter_actioner_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_twitter_actioner_mixin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_www.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-17 11:58:20.000000 utils-nuuuwan-1.2.6/tests/test_xmlx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.958643 utils-nuuuwan-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-17 09:30:36.958643 utils-nuuuwan-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:30:36.958643 utils-nuuuwan-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.942642 utils-nuuuwan-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.946642 utils-nuuuwan-1.2.7/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/GitReadOnly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/GitWrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/List.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/String.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.950642 utils-nuuuwan-1.2.7/src/utils/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/CSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/Directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/FileOrDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/FiledVariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/JSONFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/PDFFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/TSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/XSVFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/Zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/hashx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/mr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.950642 utils-nuuuwan-1.2.7/src/utils/time/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/TIMEZONE_OFFSET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/Time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/TimeDelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/TimeFormat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/TimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/TimeUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.954642 utils-nuuuwan-1.2.7/src/utils/twitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/Tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/Twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/TwitterActionerMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/TwitterActionerMixinHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/TwitterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/TwitterLoaderMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/twitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/www.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/src/utils/xmlx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.954642 utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-17 09:30:36.000000 utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 09:30:36.000000 utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:30:36.000000 utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 09:30:36.000000 utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 09:30:36.000000 utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:36.958643 utils-nuuuwan-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_file_pdf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_filed_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_hashx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_random_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_twitter_actioner_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_twitter_actioner_mixin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_www.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-17 09:29:02.000000 utils-nuuuwan-1.2.7/tests/test_xmlx.py
```

### Comparing `utils-nuuuwan-1.2.6/LICENSE` & `utils-nuuuwan-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/PKG-INFO` & `utils-nuuuwan-1.2.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-nuuuwan
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simple extensions to the core python libraries.
 Home-page: https://github.com/nuuuwan/utils
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils-nuuuwan-1.2.6/README.md` & `utils-nuuuwan-1.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 ```
 pip install utils-nuuuwan
 ```
 
 ## Version History (1.2.x)
 
-### 1.2.6  (CURRENT RELEASE)
+
+### 1.2.7  (CURRENT RELEASE)
+* fix TSVFile encoding BUG
+
+### 1.2.6 
 * WWW: Updated local_path for download
 
 ### 1.2.5
 * Fix windows-specific BUGS
 
 ### 1.2.4 
 * Removed Dependency on WGET from WWW. Updated local file logic.
```

### Comparing `utils-nuuuwan-1.2.6/setup.py` & `utils-nuuuwan-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils'
-VERSION = "1.2.6"
+VERSION = "1.2.7"
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
     description="Simple extensions to the core python libraries.",
```

### Comparing `utils-nuuuwan-1.2.6/src/utils/Browser.py` & `utils-nuuuwan-1.2.7/src/utils/Browser.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/Color.py` & `utils-nuuuwan-1.2.7/src/utils/Color.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/Dict.py` & `utils-nuuuwan-1.2.7/src/utils/Dict.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/GitReadOnly.py` & `utils-nuuuwan-1.2.7/src/utils/GitReadOnly.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/List.py` & `utils-nuuuwan-1.2.7/src/utils/List.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/Log.py` & `utils-nuuuwan-1.2.7/src/utils/Log.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/String.py` & `utils-nuuuwan-1.2.7/src/utils/String.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/Table.py` & `utils-nuuuwan-1.2.7/src/utils/Table.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/__init__.py` & `utils-nuuuwan-1.2.7/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/file/Directory.py` & `utils-nuuuwan-1.2.7/src/utils/file/Directory.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/file/File.py` & `utils-nuuuwan-1.2.7/src/utils/file/File.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 
 from utils.file.FileOrDirectory import FileOrDirectory
 
 DIALECT = 'excel'
 DELIMITER_CSV = ','
 DELIMITER_TSV = '\t'
 DELIM_LINE = '\n'
+ENCODING = 'utf-8'
 
 
 class File(FileOrDirectory):
     def delete(self):
         if self.exists:
             os.remove(self.path)
 
     @property
     def ext(self):
         return self.name.split('.')[-1]
 
     def read(self):
-        with open(self.path, 'r') as fin:
+        with open(self.path, 'r', encoding=ENCODING) as fin:
             content = fin.read()
             fin.close()
         return content
 
     def readBinary(self):
         with open(self.path, 'rb') as fin:
             content = fin.read()
             fin.close()
         return content
 
     def write(self, content):
-        with open(self.path, 'w', encoding="utf-8") as fout:
+        with open(self.path, 'w', encoding=ENCODING) as fout:
             fout.write(content)
             fout.close()
 
     def writeBinary(self, content):
         with open(self.path, 'wb') as fout:
             fout.write(content)
             fout.close()
```

### Comparing `utils-nuuuwan-1.2.6/src/utils/file/FiledVariable.py` & `utils-nuuuwan-1.2.7/src/utils/file/FiledVariable.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/file/PDFFile.py` & `utils-nuuuwan-1.2.7/src/utils/file/PDFFile.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/file/XSVFile.py` & `utils-nuuuwan-1.2.7/src/utils/file/XSVFile.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                     )
                 ),
                 data_list,
             )
         )
 
     def write(self, data_list):
-        with open(self.path, 'w') as fout:
+        with open(self.path, 'w', encoding="utf8") as fout:
             writer = csv.writer(
                 fout,
                 dialect=DIALECT,
                 delimiter=self.delimiter,
             )
 
             field_names = XSVFile.get_field_names(data_list)
```

### Comparing `utils-nuuuwan-1.2.6/src/utils/file/Zip.py` & `utils-nuuuwan-1.2.7/src/utils/file/Zip.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/mr.py` & `utils-nuuuwan-1.2.7/src/utils/mr.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/time/Time.py` & `utils-nuuuwan-1.2.7/src/utils/time/Time.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/time/TimeDelta.py` & `utils-nuuuwan-1.2.7/src/utils/time/TimeDelta.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/time/TimeFormat.py` & `utils-nuuuwan-1.2.7/src/utils/time/TimeFormat.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/time/TimeUnit.py` & `utils-nuuuwan-1.2.7/src/utils/time/TimeUnit.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/twitter/TwitterActionerMixin.py` & `utils-nuuuwan-1.2.7/src/utils/twitter/TwitterActionerMixin.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/twitter/TwitterActionerMixinHelpers.py` & `utils-nuuuwan-1.2.7/src/utils/twitter/TwitterActionerMixinHelpers.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/twitter/TwitterBase.py` & `utils-nuuuwan-1.2.7/src/utils/twitter/TwitterBase.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/twitter/TwitterLoaderMixin.py` & `utils-nuuuwan-1.2.7/src/utils/twitter/TwitterLoaderMixin.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/www.py` & `utils-nuuuwan-1.2.7/src/utils/www.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils/xmlx.py` & `utils-nuuuwan-1.2.7/src/utils/xmlx.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/PKG-INFO` & `utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-nuuuwan
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simple extensions to the core python libraries.
 Home-page: https://github.com/nuuuwan/utils
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils-nuuuwan-1.2.6/src/utils_nuuuwan.egg-info/SOURCES.txt` & `utils-nuuuwan-1.2.7/src/utils_nuuuwan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_browser.py` & `utils-nuuuwan-1.2.7/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_color.py` & `utils-nuuuwan-1.2.7/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_dict.py` & `utils-nuuuwan-1.2.7/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_directory.py` & `utils-nuuuwan-1.2.7/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_file.py` & `utils-nuuuwan-1.2.7/tests/test_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import tempfile
 import unittest
+from urllib.parse import urljoin
 
 from utils import CSVFile, File, JSONFile, TSVFile, XSVFile
+from utils.www import WWW
 
 TEST_DATA_LIST = [
     {'name': 'Alpha', 'age': '1'},
     {'name': 'Bravo', 'age': '2'},
 ]
 
 TEST_DATA_ITEM_LIST = [
@@ -93,14 +95,30 @@
                 prefix="utils_test_file.", suffix=".tsv"
             ).name
         )
         tsv_file.write(TEST_DATA_LIST)
         data_list = tsv_file.read()
         self.assertEqual(TEST_DATA_LIST, data_list)
 
+    def test_tsv_read_and_write_custom(self):
+        URL_SUMMARY = urljoin(
+            'https://raw.githubusercontent.com',
+            'nuuuwan/news_lk3_data/main/reports/summary.tsv',
+        )
+        tmp_file = WWW(URL_SUMMARY).download()
+        d_list = TSVFile(tmp_file).read()
+        tsv_file = TSVFile(
+            tempfile.NamedTemporaryFile(
+                prefix="utils_test_file.", suffix=".tsv"
+            ).name
+        )
+        tsv_file.write(d_list)
+        data_list2 = tsv_file.read()
+        self.assertEqual(d_list, data_list2)
+
     def write_test_json_file(self):
         json_file_name = tempfile.NamedTemporaryFile(
             prefix="utils.test_zip_read_and_write.", suffix=".json"
         ).name
         data = [i for i in range(0, 1_000)]
         json_file = JSONFile(json_file_name)
         json_file.write(data)
```

### Comparing `utils-nuuuwan-1.2.6/tests/test_filed_variable.py` & `utils-nuuuwan-1.2.7/tests/test_filed_variable.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_git.py` & `utils-nuuuwan-1.2.7/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_iter.py` & `utils-nuuuwan-1.2.7/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_list.py` & `utils-nuuuwan-1.2.7/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_mr.py` & `utils-nuuuwan-1.2.7/tests/test_mr.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_random_color.py` & `utils-nuuuwan-1.2.7/tests/test_random_color.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_string.py` & `utils-nuuuwan-1.2.7/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_table.py` & `utils-nuuuwan-1.2.7/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_time.py` & `utils-nuuuwan-1.2.7/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_twitter_actioner_mixin.py` & `utils-nuuuwan-1.2.7/tests/test_twitter_actioner_mixin.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_twitter_actioner_mixin_helpers.py` & `utils-nuuuwan-1.2.7/tests/test_twitter_actioner_mixin_helpers.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_www.py` & `utils-nuuuwan-1.2.7/tests/test_www.py`

 * *Files identical despite different names*

### Comparing `utils-nuuuwan-1.2.6/tests/test_xmlx.py` & `utils-nuuuwan-1.2.7/tests/test_xmlx.py`

 * *Files identical despite different names*

