# Comparing `tmp/mautrix-signal-0.4.2.tar.gz` & `tmp/mautrix-signal-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mautrix-signal-0.4.2.tar", last modified: Sat Dec  3 12:53:28 2022, max compression
+gzip compressed data, was "mautrix-signal-0.4.3.tar", last modified: Wed May 17 13:52:56 2023, max compression
```

## Comparing `mautrix-signal-0.4.2.tar` & `mautrix-signal-0.4.3.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.445054 mautrix-signal-0.4.2/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12981 2022-12-03 12:19:53.000000 mautrix-signal-0.4.2/CHANGELOG.md
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/LICENSE
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      114 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/MANIFEST.in
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2382 2022-12-03 12:53:28.445054 mautrix-signal-0.4.2/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1351 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/README.md
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.437054 mautrix-signal-0.4.2/mausignald/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       35 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mausignald/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4327 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mausignald/errors.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9335 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mausignald/rpc.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    20074 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mausignald/signald.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    20255 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mausignald/types.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.437054 mautrix-signal-0.4.2/mautrix_signal/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2022-12-03 12:20:04.000000 mautrix-signal-0.4.2/mautrix_signal/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5442 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/__main__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.441054 mautrix-signal-0.4.2/mautrix_signal/commands/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      103 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/commands/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10491 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/commands/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3490 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/commands/conn.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    20713 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/commands/signal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      329 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/commands/typehint.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4630 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/config.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.441054 mautrix-signal-0.4.2/mautrix_signal/db/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      584 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3118 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/disappearing_message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5035 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4433 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4792 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4542 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/reaction.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.445054 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      399 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4509 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v00_latest_revision.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1084 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v02_portal_avatar_info.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1023 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v03_puppet_base_url.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1895 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v04_phone_sender_identifier.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1351 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v05_puppet_avatar_info.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1377 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v06_portal_revision.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1019 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v07_portal_relay_user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1311 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v08_disappearing_messages.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1009 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v09_group_topic.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1042 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v10_puppet_name_quality.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5193 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v11_drop_number_support.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2677 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      358 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/db/util.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17059 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/example-config.yaml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5989 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/formatter.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1436 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/get_version.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9934 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/matrix.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)   104188 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17800 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    15914 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/signal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    16613 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.445054 mautrix-signal-0.4.2/mautrix_signal/util/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      140 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/util/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1114 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/util/color_log.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1066 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/util/normalize_number.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1440 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/util/user_has_power_level.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      173 2022-12-03 12:53:28.000000 mautrix-signal-0.4.2/mautrix_signal/version.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.445054 mautrix-signal-0.4.2/mautrix_signal/web/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       46 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/web/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    18562 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/web/provisioning_api.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      946 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/mautrix_signal/web/segment_analytics.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-12-03 12:53:28.437054 mautrix-signal-0.4.2/mautrix_signal.egg-info/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2382 2022-12-03 12:53:28.000000 mautrix-signal-0.4.2/mautrix_signal.egg-info/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2004 2022-12-03 12:53:28.000000 mautrix-signal-0.4.2/mautrix_signal.egg-info/SOURCES.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2022-12-03 12:53:28.000000 mautrix-signal-0.4.2/mautrix_signal.egg-info/dependency_links.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      593 2022-12-03 12:53:28.000000 mautrix-signal-0.4.2/mautrix_signal.egg-info/requires.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       26 2022-12-03 12:53:28.000000 mautrix-signal-0.4.2/mautrix_signal.egg-info/top_level.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      395 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/optional-requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/pyproject.toml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      151 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       93 2022-12-03 12:53:28.445054 mautrix-signal-0.4.2/setup.cfg
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2163 2022-11-07 15:03:09.000000 mautrix-signal-0.4.2/setup.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.166938 mautrix-signal-0.4.3/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    14767 2023-05-17 13:52:04.000000 mautrix-signal-0.4.3/CHANGELOG.md
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/LICENSE
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      114 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/MANIFEST.in
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2345 2023-05-17 13:52:56.166938 mautrix-signal-0.4.3/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1351 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/README.md
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.154938 mautrix-signal-0.4.3/mausignald/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       35 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mausignald/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5253 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mausignald/errors.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9382 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mausignald/rpc.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    22028 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mausignald/signald.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    20214 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mausignald/types.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.158938 mautrix-signal-0.4.3/mautrix_signal/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2023-05-17 12:03:08.000000 mautrix-signal-0.4.3/mautrix_signal/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5819 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/__main__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.158938 mautrix-signal-0.4.3/mautrix_signal/commands/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      103 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/commands/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    11088 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/commands/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3490 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/commands/conn.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    21782 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/commands/signal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      329 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/commands/typehint.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2310 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/commands/util.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5240 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/config.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.162938 mautrix-signal-0.4.3/mautrix_signal/db/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      584 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3118 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/disappearing_message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5035 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4433 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4913 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4542 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/reaction.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.162938 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      435 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4602 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v00_latest_revision.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1084 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v02_portal_avatar_info.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1023 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v03_puppet_base_url.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1895 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v04_phone_sender_identifier.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1351 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v05_puppet_avatar_info.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1377 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v06_portal_revision.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1019 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v07_portal_relay_user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1311 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v08_disappearing_messages.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1009 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v09_group_topic.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1042 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v10_puppet_name_quality.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5193 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v11_drop_number_support.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1062 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v12_add_contact_info_to_puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2677 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      358 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/db/util.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    18804 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/example-config.yaml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5989 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/formatter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1436 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/get_version.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13406 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/matrix.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)   109269 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19072 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    18409 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/signal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19677 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.166938 mautrix-signal-0.4.3/mautrix_signal/util/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      140 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/util/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1114 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/util/color_log.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1066 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/util/normalize_number.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1440 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/util/user_has_power_level.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      173 2023-05-17 13:52:56.000000 mautrix-signal-0.4.3/mautrix_signal/version.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.166938 mautrix-signal-0.4.3/mautrix_signal/web/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       46 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/web/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19122 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/web/provisioning_api.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1105 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/mautrix_signal/web/segment_analytics.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-05-17 13:52:56.158938 mautrix-signal-0.4.3/mautrix_signal.egg-info/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2345 2023-05-17 13:52:56.000000 mautrix-signal-0.4.3/mautrix_signal.egg-info/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2096 2023-05-17 13:52:56.000000 mautrix-signal-0.4.3/mautrix_signal.egg-info/SOURCES.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2023-05-17 13:52:56.000000 mautrix-signal-0.4.3/mautrix_signal.egg-info/dependency_links.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      594 2023-05-17 13:52:56.000000 mautrix-signal-0.4.3/mautrix_signal.egg-info/requires.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       26 2023-05-17 13:52:56.000000 mautrix-signal-0.4.3/mautrix_signal.egg-info/top_level.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      395 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/optional-requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      203 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/pyproject.toml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      152 2023-05-17 12:03:36.000000 mautrix-signal-0.4.3/requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       93 2023-05-17 13:52:56.166938 mautrix-signal-0.4.3/setup.cfg
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2163 2023-05-14 10:31:52.000000 mautrix-signal-0.4.3/setup.py
```

### Comparing `mautrix-signal-0.4.2/CHANGELOG.md` & `mautrix-signal-0.4.3/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+# v0.4.3 (2023-05-17)
+
+Target signald version: [v0.23.2](https://gitlab.com/signald/signald/-/releases/0.23.2)
+
+* Added option to not set name/avatar for DM rooms even if the room is encrypted.
+* Added options to automatically ratchet/delete megolm sessions to minimize
+  access to old messages.
+* Added command to request group/contact sync from primary device.
+* Added error notices if incoming attachments are dropped.
+* Fixed bugs with creating groups.
+* Fixed handling changes to disappearing message timer in groups.
+
+## Changes by [@maltee1]
+
+* Added bridging of group join requests on Signal to knocks on Matrix ([#275]).
+* Added bridging of banned users from Signal to Matrix ([#275]).
+* Added admin command to force logout other Matrix users from the bridge ([#359]).
+* Added `submit-challenge` command to submit captcha codes when encountering
+  ratelimits on sending messages ([#320]).
+* Added invite command for inviting Signal users to a group by phone number ([#285]).
+* Added support for bridging Matrix invites to Signal via relay user ([#285]).
+* Added automatic group creation when inviting multiple Signal ghosts to a
+  non-DM room ([#294]).
+* Fixed ghost user getting kicked from Matrix room when trying to invite a user
+  who's already in the group on Signal ([#345]).
+* Fixed bridging power levels from Signal for users who are logged into the
+  bridge, but don't have double puppeting enabled ([#333]).
+
+[#275]: https://github.com/mautrix/signal/pull/275
+[#285]: https://github.com/mautrix/signal/pull/285
+[#294]: https://github.com/mautrix/signal/pull/294
+[#320]: https://github.com/mautrix/signal/pull/320
+[#333]: https://github.com/mautrix/signal/pull/333
+[#345]: https://github.com/mautrix/signal/pull/345
+[#359]: https://github.com/mautrix/signal/pull/359
+
 # v0.4.2 (2022-12-03)
 
 Target signald version: [v0.23.0](https://gitlab.com/signald/signald/-/releases/0.23.0)
 
 * Fixed database schema upgrade for users who used SQLite before it was
   stabilized in v0.4.1.
 * Fixed error in commands that use phone numbers (like `!signal pm`).
```

### Comparing `mautrix-signal-0.4.2/LICENSE` & `mautrix-signal-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/PKG-INFO` & `mautrix-signal-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mautrix-signal
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Matrix-Signal puppeting bridge.
 Home-page: https://github.com/mautrix/signal
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/mautrix/signal/blob/master/CHANGELOG.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -49,9 +47,7 @@
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/signal/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#signal:maunium.net`](https://matrix.to/#/#signal:maunium.net)
-
-
```

### Comparing `mautrix-signal-0.4.2/README.md` & `mautrix-signal-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mausignald/errors.py` & `mautrix-signal-0.4.3/mausignald/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Any
 
+from mautrix.util.format_duration import format_duration
+
 
 class RPCError(Exception):
     pass
 
 
 class UnexpectedError(RPCError):
     pass
@@ -106,28 +108,53 @@
     pass
 
 
 class ProfileUnavailableError(ResponseError):
     pass
 
 
+class NoSuchAccountError(ResponseError):
+    pass
+
+
+class GroupPatchNotAcceptedError(ResponseError):
+    pass
+
+
+class ProofRequiredError(ResponseError):
+    def __init__(self, data: dict[str, Any]) -> None:
+        self.options = data.get("options")
+        self.retry_after = data.get("retry_after")
+        self.token = data.get("token")
+        message = "You have been rate limited by Signal."
+        if isinstance(self.retry_after, (int, float)):
+            message += (
+                f" Try again in {format_duration(int(self.retry_after))} "
+                "or complete a captcha challenge using the `submit-challenge` command."
+            )
+        super().__init__(data, message_override=message)
+
+
 response_error_types = {
     "invalid_request": RequestValidationFailure,
     "TimeoutException": TimeoutException,
     "UserAlreadyExists": UserAlreadyExistsError,
     "RequestValidationFailure": RequestValidationFailure,
     "UnknownIdentityKey": UnknownIdentityKey,
     "CaptchaRequiredError": CaptchaRequiredError,
     "InternalError": InternalError,
     "AttachmentTooLargeError": AttachmentTooLargeError,
     "AuthorizationFailedError": AuthorizationFailedError,
     "ScanTimeoutError": ScanTimeoutError,
     "OwnProfileKeyDoesNotExistError": OwnProfileKeyDoesNotExistError,
     "UnregisteredUserError": UnregisteredUserError,
     "ProfileUnavailableError": ProfileUnavailableError,
+    "NoSuchAccountError": NoSuchAccountError,
+    "GroupPatchNotAcceptedError": GroupPatchNotAcceptedError,
+    "ProofRequiredError": ProofRequiredError,
     # TODO add rest from https://gitlab.com/signald/signald/-/tree/main/src/main/java/io/finn/signald/clientprotocol/v1/exceptions
 }
 
 
 def make_response_error(data: dict[str, Any]) -> ResponseError:
     error_data = data["error"]
     if isinstance(error_data, str):
```

### Comparing `mautrix-signal-0.4.2/mausignald/rpc.py` & `mautrix-signal-0.4.3/mausignald/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from typing import Any, Awaitable, Callable, Dict
 from uuid import UUID, uuid4
 import asyncio
 import json
 import logging
 
+from mautrix.util import background_task
 from mautrix.util.logging import TraceLogger
 
 from .errors import NotConnected, UnexpectedError, UnexpectedResponse, make_response_error
 
 EventHandler = Callable[[Dict[str, Any]], Awaitable[None]]
 
 # These are synthetic RPC events for registering callbacks on socket
@@ -86,15 +87,15 @@
         except OSError as e:
             self.log.error(f"Connection to {self.socket_path} failed: {e}")
             await asyncio.sleep(5)
             return
 
         read_loop = asyncio.create_task(self._try_read_loop())
         self.is_connected = True
-        asyncio.create_task(self._run_rpc_handler(CONNECT_EVENT, {}))
+        background_task.create(self._run_rpc_handler(CONNECT_EVENT, {}))
         self._connect_future.set_result(True)
 
         await read_loop
         self.is_connected = False
         self._connect_future = self.loop.create_future()
         await self._run_rpc_handler(DISCONNECT_EVENT, {})
 
@@ -160,15 +161,15 @@
             self.log.debug(f"Got invalid request from server: {line}")
             return
 
         self.log.trace("Got data from server: %s", req)
 
         req_id = req.get("id")
         if req_id is None:
-            asyncio.create_task(self._run_rpc_handler(req_type, req))
+            background_task.create(self._run_rpc_handler(req_type, req))
         else:
             self._run_response_handlers(UUID(req_id), req_type, req)
 
     async def _try_read_loop(self) -> None:
         try:
             await self._read_loop()
         except Exception:
```

### Comparing `mautrix-signal-0.4.2/mausignald/signald.py` & `mautrix-signal-0.4.3/mausignald/signald.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from typing import Any, Awaitable, Callable, Type, TypeVar
 from uuid import UUID
 import asyncio
 
 from mautrix.util.logging import TraceLogger
 
-from .errors import AuthorizationFailedError, RPCError, UnexpectedResponse
+from .errors import AuthorizationFailedError, NoSuchAccountError, RPCError, UnexpectedResponse
 from .rpc import CONNECT_EVENT, DISCONNECT_EVENT, SignaldRPCClient
 from .types import (
     Account,
     Address,
     Attachment,
     DeviceInfo,
     ErrorMessage,
@@ -25,14 +25,15 @@
     GroupMember,
     GroupV2,
     IncomingMessage,
     JoinGroupResponse,
     LinkPreview,
     LinkSession,
     Mention,
+    MessageResendSuccessEvent,
     Profile,
     ProofRequiredType,
     Quote,
     Reaction,
     SendMessageResponse,
     StorageChange,
     TrustLevel,
@@ -58,14 +59,15 @@
         self._event_handlers = {}
         self._subscriptions = set()
         self.add_rpc_handler("IncomingMessage", self._parse_message)
         self.add_rpc_handler("ProtocolInvalidMessageError", self._parse_error)
         self.add_rpc_handler("WebSocketConnectionState", self._websocket_connection_state_change)
         self.add_rpc_handler("version", self._log_version)
         self.add_rpc_handler("StorageChange", self._parse_storage_change)
+        self.add_rpc_handler("MessageResendSuccess", self._parse_message_resend_request)
         self.add_rpc_handler(CONNECT_EVENT, self._resubscribe)
         self.add_rpc_handler(DISCONNECT_EVENT, self._on_disconnect)
 
     def add_event_handler(self, event_class: Type[T], handler: EventHandler) -> None:
         self._event_handlers.setdefault(event_class, []).append(handler)
 
     def remove_event_handler(self, event_class: Type[T], handler: EventHandler) -> None:
@@ -89,14 +91,19 @@
         await self._run_event_handler(ErrorMessage.deserialize(data))
 
     async def _parse_storage_change(self, data: dict[str, Any]) -> None:
         if data["type"] != "StorageChange":
             return
         await self._run_event_handler(StorageChange.deserialize(data))
 
+    async def _parse_message_resend_request(self, data: dict[str, Any]) -> None:
+        if data["type"] != "MesaageResendSuccess":
+            return
+        await self._run_event_handler(MessageResendSuccessEvent.deserialize(data))
+
     async def _parse_message(self, data: dict[str, Any]) -> None:
         event_type = data["type"]
         event_data = data["data"]
         event_class = {
             "IncomingMessage": IncomingMessage,
         }[event_type]
         event = event_class.deserialize(event_data)
@@ -120,15 +127,15 @@
         try:
             await self.request_v1("subscribe", account=username)
             self._subscriptions.add(username)
             return True
         except RPCError as e:
             self.log.debug("Failed to subscribe to %s: %s", username, e)
             state = WebsocketConnectionState.DISCONNECTED
-            if isinstance(e, AuthorizationFailedError):
+            if isinstance(e, (AuthorizationFailedError, NoSuchAccountError)):
                 state = WebsocketConnectionState.AUTHENTICATION_FAILED
             evt = WebsocketConnectionStateChangeEvent(state=state, account=username)
             await self._run_event_handler(evt)
             return False
 
     async def unsubscribe(self, username: str) -> bool:
         try:
@@ -335,14 +342,31 @@
 
     async def add_linked_device(self, username: str, uri: str) -> None:
         await self.request_v1("add_device", account=username, uri=uri)
 
     async def remove_linked_device(self, username: str, device_id: int) -> None:
         await self.request_v1("remove_linked_device", account=username, deviceId=device_id)
 
+    async def request_sync(
+        self,
+        username: str,
+        blocked: bool = True,
+        configuration: bool = True,
+        contacts: bool = True,
+        groups: bool = True,
+    ) -> None:
+        await self.request_v1(
+            "request_sync",
+            account=username,
+            blocked=blocked,
+            configuration=configuration,
+            contacts=contacts,
+            groups=groups,
+        )
+
     async def list_contacts(self, username: str, use_cache: bool = False) -> list[Profile]:
         kwargs = {"async": use_cache}
         resp = await self.request_v1("list_contacts", account=username, **kwargs)
         return [Profile.deserialize(contact) for contact in resp["profiles"]]
 
     async def list_groups(self, username: str) -> list[GroupV2]:
         resp = await self.request_v1("list_groups", account=username)
@@ -365,14 +389,36 @@
     async def unban_user(self, username: str, group_id: GroupID, users: list[Address]) -> GroupV2:
         serialized_users = [user.serialize() for user in (users or [])]
         resp = await self.request_v1(
             "unban_user", account=username, group_id=group_id, users=serialized_users
         )
         return GroupV2.deserialize(resp)
 
+    async def approve_membership(
+        self, username: str, group_id: GroupID, members: list[Address]
+    ) -> GroupV2:
+        serialized_members = [member.serialize() for member in (members or [])]
+        resp = await self.request_v1(
+            "approve_membership", account=username, groupID=group_id, members=serialized_members
+        )
+        return GroupV2.deserialize(resp)
+
+    async def refuse_membership(
+        self, username: str, group_id: GroupID, members: list[Address], also_ban: bool = False
+    ) -> GroupV2:
+        serialized_members = [member.serialize() for member in (members or [])]
+        resp = await self.request_v1(
+            "refuse_membership",
+            account=username,
+            group_id=group_id,
+            members=serialized_members,
+            also_ban=also_ban,
+        )
+        return GroupV2.deserialize(resp)
+
     async def update_group(
         self,
         username: str,
         group_id: GroupID,
         title: str | None = None,
         description: str | None = None,
         avatar_path: str | None = None,
@@ -420,18 +466,18 @@
         if "id" not in resp:
             return None
         return GroupV2.deserialize(resp)
 
     async def create_group(
         self,
         username: str,
+        title: str,
         avatar_path: str | None = None,
         member_role_administrator: bool = False,
         members: list[Address] | None = None,
-        title: str | None = None,
     ) -> GroupV2 | None:
         create_params = {
             "avatar": avatar_path,
             "member_role": "ADMINISTRATOR" if member_role_administrator else "DEFAULT",
             "title": title,
             "members": [addr.serialize() for addr in members],
         }
@@ -498,7 +544,14 @@
         )
 
     async def find_uuid(self, username: str, number: str) -> UUID | None:
         resp = await self.request_v1(
             "resolve_address", partial=Address(number=number).serialize(), account=username
         )
         return Address.deserialize(resp).uuid
+
+    async def submit_challenge(
+        self, username: str, captcha_token: str | None, challenge: str | None
+    ) -> None:
+        await self.request_v1(
+            "submit_challenge", account=username, captcha_token=captcha_token, challenge=challenge
+        )
```

### Comparing `mautrix-signal-0.4.2/mausignald/types.py` & `mautrix-signal-0.4.3/mausignald/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,27 +156,14 @@
     inbox_position: Optional[int] = None
     mobilecoin_address: Optional[str] = None
     expiration_time: Optional[int] = None
     capabilities: Optional[Capabilities] = None
     # visible_badge_ids: List[str]
 
 
-@dataclass
-class Group(SerializableAttrs):
-    group_id: GroupID = field(json="groupId")
-    name: str = "Unknown group"
-
-    # Sometimes "UPDATE"
-    type: Optional[str] = None
-
-    # Not always present
-    members: List[Address] = field(factory=lambda: [])
-    avatar_id: int = field(default=0, json="avatarId")
-
-
 class AccessControlMode(SerializableEnum):
     UNKNOWN = "UNKNOWN"
     ANY = "ANY"
     MEMBER = "MEMBER"
     ADMINISTRATOR = "ADMINISTRATOR"
     UNSATISFIABLE = "UNSATISFIABLE"
     UNRECOGNIZED = "UNRECOGNIZED"
@@ -422,15 +409,14 @@
     quote: Optional[Quote] = None
     reaction: Optional[Reaction] = None
     attachments: List[Attachment] = field(factory=lambda: [])
     sticker: Optional[Sticker] = None
     mentions: List[Mention] = field(factory=lambda: [])
     contacts: List[SharedContact] = field(factory=lambda: [])
 
-    group: Optional[Group] = None
     group_v2: Optional[GroupV2ID] = field(default=None, json="groupV2")
 
     end_session: bool = field(default=False, json="endSession")
     expires_in_seconds: int = field(default=0, json="expiresInSeconds")
     is_expiration_update: bool = field(default=False)
     profile_key_update: bool = field(default=False, json="profileKeyUpdate")
     view_once: bool = field(default=False, json="viewOnce")
@@ -486,14 +472,21 @@
 class ReceiptMessage(SerializableAttrs):
     type: ReceiptType
     timestamps: List[int]
     when: int
 
 
 @dataclass
+class DecryptionErrorMessage(SerializableAttrs):
+    timestamp: int
+    device_id: int
+    ratchet_key: Optional[str] = None
+
+
+@dataclass
 class ContactSyncMeta(SerializableAttrs):
     id: Optional[str] = None
 
 
 @dataclass
 class ConfigItem(SerializableAttrs):
     present: bool = False
@@ -622,14 +615,15 @@
     has_legacy_message: bool
 
     call_message: Optional[CallMessage] = field(default=None)
     data_message: Optional[MessageData] = field(default=None)
     sync_message: Optional[SyncMessage] = field(default=None)
     typing_message: Optional[TypingMessage] = None
     receipt_message: Optional[ReceiptMessage] = None
+    decryption_error_message: Optional[DecryptionErrorMessage] = None
 
 
 @dataclass(kw_only=True)
 class ErrorMessageData(SerializableAttrs):
     sender: str
     timestamp: int
     message: str
@@ -675,14 +669,20 @@
 
 class WebsocketType(SerializableEnum):
     IDENTIFIED = "IDENTIFIED"
     UNIDENTIFIED = "UNIDENTIFIED"
 
 
 @dataclass
+class MessageResendSuccessEvent(SerializableAttrs):
+    account: str
+    timestamp: int
+
+
+@dataclass
 class WebsocketConnectionStateChangeEvent(SerializableAttrs):
     state: WebsocketConnectionState
     account: str
     socket: Optional[WebsocketType] = None
     exception: Optional[str] = None
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/__main__.py` & `mautrix-signal-0.4.3/mautrix_signal/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 SYNC_JITTER = 10
 
 
 class SignalBridge(Bridge):
     module = "mautrix_signal"
     name = "mautrix-signal"
+    beeper_service_name = "signal"
+    beeper_network_name = "signal"
     command = "python -m mautrix-signal"
     description = "A Matrix-Signal puppeting bridge."
     repo_url = "https://github.com/mautrix/signal"
     version = version
     markdown_version = linkified_version
     config_class = Config
     matrix_class = MatrixHandler
@@ -57,54 +59,61 @@
         super().prepare_db()
         init_db(self.db)
 
     def prepare_bridge(self) -> None:
         self.signal = SignalHandler(self)
         super().prepare_bridge()
         cfg = self.config["bridge.provisioning"]
-        self.provisioning_api = ProvisioningAPI(self, cfg["shared_secret"], cfg["segment_key"])
+        self.provisioning_api = ProvisioningAPI(
+            self, cfg["shared_secret"], cfg["segment_key"], cfg["segment_user_id"]
+        )
         self.az.app.add_subapp(cfg["prefix"], self.provisioning_api.app)
 
     async def start(self) -> None:
         User.init_cls(self)
         self.add_startup_actions(Puppet.init_cls(self))
         Portal.init_cls(self)
         self.add_startup_actions(Portal.restart_scheduled_disappearing())
         if self.config["bridge.resend_bridge_info"]:
             self.add_startup_actions(self.resend_bridge_info())
         self.add_startup_actions(self.signal.start())
         await super().start()
         self.periodic_sync_task = asyncio.create_task(self._periodic_sync_loop())
 
-    @staticmethod
-    async def _actual_periodic_sync_loop(log: logging.Logger, interval: int) -> None:
+    async def _actual_periodic_sync_loop(self, log: logging.Logger, interval: int) -> None:
+        n = 0
+        hacky_daily_resync = self.config["bridge.hacky_contact_name_mixup_detection"]
         while True:
+            n += 1
             try:
                 await asyncio.sleep(interval)
             except asyncio.CancelledError:
                 return
             log.info("Executing periodic syncs")
             for user in User.by_username.values():
                 # Add some randomness to the sync to avoid a thundering herd
                 await asyncio.sleep(uniform(0, SYNC_JITTER))
                 try:
-                    await user.sync()
+                    await user.sync(is_startup=hacky_daily_resync and n % 24 == 23)
                 except asyncio.CancelledError:
                     return
                 except Exception:
                     log.exception("Error while syncing %s", user.mxid)
 
     async def _periodic_sync_loop(self) -> None:
         log = logging.getLogger("mau.periodic_sync")
         interval = self.config["bridge.periodic_sync"]
         if interval <= 0:
             log.debug("Periodic sync is not enabled")
             return
         log.debug("Starting periodic sync loop")
-        await self._actual_periodic_sync_loop(log, interval)
+        try:
+            await self._actual_periodic_sync_loop(log, interval)
+        except Exception:
+            log.fatal("Error in periodic resync", exc_info=True)
         log.debug("Periodic sync stopped")
 
     def prepare_stop(self) -> None:
         self.add_shutdown_actions(self.signal.stop())
         for puppet in Puppet.by_custom_mxid.values():
             puppet.stop()
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/commands/auth.py` & `mautrix-signal-0.4.3/mautrix_signal/commands/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,14 +242,33 @@
         await evt.reply("You're not logged in")
         return
     await evt.sender.logout()
     await evt.reply("Successfully logged out")
 
 
 @command_handler(
+    needs_auth=False,
+    management_only=True,
+    needs_admin=True,
+    help_section=SECTION_AUTH,
+    help_text="Remove all local data about a user's Signal link",
+    help_args="<mxid>",
+)
+async def logout_user(evt: CommandEvent) -> None:
+    if len(evt.args) == 0:
+        await evt.reply("**Usage**: $cmdprefix+sp logout-user <mxid>")
+    user = await evt.bridge.get_user(UserID(evt.args[0]))
+    if not await user.is_logged_in():
+        await evt.reply("This user is not logged in")
+        return
+    await user.logout()
+    await evt.reply("Successfully logged out")
+
+
+@command_handler(
     needs_auth=True,
     management_only=True,
     help_section=SECTION_AUTH,
     help_text="List devices linked to your Signal account",
 )
 async def list_devices(evt: CommandEvent) -> None:
     devices = await evt.bridge.signal.get_linked_devices(evt.sender.username)
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/commands/conn.py` & `mautrix-signal-0.4.3/mautrix_signal/commands/conn.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/commands/signal.py` & `mautrix-signal-0.4.3/mautrix_signal/commands/signal.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import Awaitable
-import asyncio
 import base64
 import json
 
 from mausignald.errors import UnknownIdentityKey, UnregisteredUserError
 from mausignald.types import Address, GroupID, TrustLevel
-from mautrix.appservice import IntentAPI
+from mautrix.bridge import RejectMatrixInvite
 from mautrix.bridge.commands import SECTION_ADMIN, HelpSection, command_handler
 from mautrix.types import (
     ContentURI,
     EventID,
     EventType,
     JoinRule,
     PowerLevelStateEventContent,
     RoomID,
 )
+from mautrix.util import background_task
 
 from .. import portal as po, puppet as pu
 from ..util import normalize_number, user_has_power_level
 from .auth import make_qr
 from .typehint import CommandEvent
+from .util import get_initial_state
 
 try:
     import PIL as _
     import qrcode
 except ImportError:
     qrcode = None
 
@@ -252,22 +253,32 @@
     return await evt.reply(f"Successfully marked {number} as {trust_level.human_str}")
 
 
 @command_handler(
     needs_admin=False,
     needs_auth=True,
     help_section=SECTION_SIGNAL,
-    help_text="Sync data from Signal",
+    help_text="Sync data from signald",
 )
 async def sync(evt: CommandEvent) -> None:
     await evt.sender.sync()
     await evt.reply("Sync complete")
 
 
 @command_handler(
+    needs_admin=False,
+    needs_auth=True,
+    help_section=SECTION_SIGNAL,
+    help_text="Request your phone to re-send data like contacts and group info",
+)
+async def request_sync(evt: CommandEvent) -> None:
+    await evt.bridge.signal.request_sync(evt.sender.username)
+
+
+@command_handler(
     needs_admin=True,
     needs_auth=False,
     help_section=SECTION_ADMIN,
     help_text="Send raw requests to signald",
     help_args="[--user] <type> <_json_>",
 )
 async def raw(evt: CommandEvent) -> None:
@@ -338,27 +349,29 @@
     if evt.portal:
         return await evt.reply("This is already a portal room.")
 
     title, about, levels, encrypted, avatar_url, join_rule = await get_initial_state(
         evt.az.intent, evt.room_id
     )
 
+    if not title:
+        return await evt.reply("Please set a room name before creating a Signal group.")
+
     portal = po.Portal(
         chat_id=GroupID(""),
         mxid=evt.room_id,
         name=title,
         topic=about or "",
         encrypted=encrypted,
         receiver="",
         avatar_url=avatar_url,
     )
     await warn_missing_power(levels, evt)
 
     await portal.create_signal_group(evt.sender, levels, join_rule)
-    await evt.reply(f"Signal chat created. ID: {portal.chat_id}")
 
 
 @command_handler(
     name="id",
     needs_auth=True,
     management_only=False,
     help_section=SECTION_SIGNAL,
@@ -493,14 +506,42 @@
     evt.sender.command_status = None
     async with portal._create_room_lock:
         await _locked_confirm_bridge(
             evt, portal=portal, room_id=bridge_to_mxid, is_logged_in=is_logged_in
         )
 
 
+@command_handler(
+    needs_auth=True,
+    management_only=False,
+    help_section=SECTION_SIGNAL,
+    help_text="Submit a captcha challenge for the last occuring token",
+    help_args="<captcha token>",
+)
+async def submit_challenge(evt: CommandEvent) -> None:
+    if len(evt.args) == 0:
+        await evt.reply("**Usage:** `$cmdprefix+sp submit-challenge <captcha token>`")
+        return
+    challenge_token = evt.sender.challenge_token
+    captcha_token = evt.args[0]
+    if not challenge_token:
+        return await evt.reply(
+            "No open challenge found. If the bridge was restarted, try"
+            "triggering another ProofRequiredError"
+        )
+    evt.log.debug(f"Submitting challenge for token {challenge_token}")
+    try:
+        await evt.bridge.signal.submit_challenge(
+            evt.sender.username, captcha_token=evt.args[0], challenge=challenge_token
+        )
+    except Exception as e:
+        return await evt.reply(f"Failed to submit captcha challenge: {e}")
+    return await evt.reply("Captcha challenge submitted successfully")
+
+
 async def _locked_confirm_bridge(
     evt: CommandEvent, portal: po.Portal, room_id: RoomID, is_logged_in: bool
 ) -> EventID | None:
     try:
         group = await evt.bridge.signal.get_group(
             evt.sender.username, portal.chat_id, portal.revision
         )
@@ -520,69 +561,57 @@
     portal.by_mxid[portal.mxid] = portal
     (
         portal.title,
         portal.about,
         levels,
         portal.encrypted,
         portal.photo_id,
+        join_rule,
     ) = await get_initial_state(evt.az.intent, evt.room_id)
     await portal.save()
     await portal.update_bridge_info()
 
-    asyncio.create_task(portal.update_matrix_room(evt.sender, group))
+    background_task.create(portal.update_matrix_room(evt.sender, group))
 
     await warn_missing_power(levels, evt)
 
     return await evt.reply("Bridging complete. Portal synchronization should begin momentarily.")
 
 
-async def get_initial_state(
-    intent: IntentAPI, room_id: RoomID
-) -> tuple[
-    str | None,
-    str | None,
-    PowerLevelStateEventContent | None,
-    bool,
-    ContentURI | None,
-    JoinRule | None,
-]:
-    state = await intent.get_state(room_id)
-    title: str | None = None
-    about: str | None = None
-    levels: PowerLevelStateEventContent | None = None
-    encrypted: bool = False
-    avatar_url: ContentURI | None = None
-    join_rule: JoinRule | None = None
-    for event in state:
-        try:
-            if event.type == EventType.ROOM_NAME:
-                title = event.content.name
-            elif event.type == EventType.ROOM_TOPIC:
-                about = event.content.topic
-            elif event.type == EventType.ROOM_POWER_LEVELS:
-                levels = event.content
-            elif event.type == EventType.ROOM_CANONICAL_ALIAS:
-                title = title or event.content.canonical_alias
-            elif event.type == EventType.ROOM_ENCRYPTION:
-                encrypted = True
-            elif event.type == EventType.ROOM_AVATAR:
-                avatar_url = event.content.url
-            elif event.type == EventType.ROOM_JOIN_RULES:
-                join_rule = event.content.join_rule
-        except KeyError:
-            # Some state event probably has empty content
-            pass
-    return title, about, levels, encrypted, avatar_url, join_rule
-
-
 async def warn_missing_power(levels: PowerLevelStateEventContent, evt: CommandEvent) -> None:
     bot_pl = levels.get_user_level(evt.az.bot_mxid)
     if bot_pl < levels.get_event_level(EventType.ROOM_POWER_LEVELS):
         await evt.reply(missing_power_warning.format(bot_mxid=evt.az.bot_mxid))
     elif bot_pl <= 50:
         await evt.reply(low_power_warning.format(bot_mxid=evt.az.bot_mxid))
     if levels.state_default < 50 and (
         levels.events[EventType.ROOM_NAME] >= 50
         or levels.events[EventType.ROOM_AVATAR] >= 50
         or levels.events[EventType.ROOM_TOPIC] >= 50
     ):
         await evt.reply(meta_power_warning)
+
+
+@command_handler(
+    needs_auth=False,
+    management_only=False,
+    help_section=SECTION_SIGNAL,
+    help_text="Invite a Signal user by phone number",
+    help_args="<_phone_>",
+)
+async def invite(evt: CommandEvent) -> EventID | None:
+    if not evt.is_portal:
+        return await evt.reply("This is not a portal room.")
+    portal = evt.portal
+    puppet = await _get_puppet_from_cmd(evt)
+    if not puppet:
+        return None
+    levels = await portal.main_intent.get_power_levels(portal.mxid)
+    if levels.get_user_level(puppet.mxid) < levels.invite:
+        return await evt.reply("You do not have permissions to invite users to this room")
+
+    try:
+        info = await portal.handle_matrix_invite(evt.sender, puppet)
+        sender, is_relay = await portal.get_relay_sender(evt.sender, "updating info")
+        await portal.update_info(sender, info)
+    except RejectMatrixInvite as e:
+        return await evt.reply(f"Failed to invite {puppet.name}: {e}")
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/config.py` & `mautrix-signal-0.4.3/mautrix_signal/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,44 +60,55 @@
         copy("bridge.autocreate_group_portal")
         copy("bridge.autocreate_contact_portal")
         copy("bridge.sync_with_custom_puppets")
         copy("bridge.public_portals")
         copy("bridge.sync_direct_chat_list")
         copy("bridge.double_puppet_server_map")
         copy("bridge.double_puppet_allow_discovery")
+        copy("bridge.create_group_on_invite")
+        copy("bridge.hacky_contact_name_mixup_detection")
         if self["bridge.login_shared_secret"]:
             base["bridge.login_shared_secret_map"] = {
                 base["homeserver.domain"]: self["bridge.login_shared_secret"]
             }
         else:
             copy("bridge.login_shared_secret_map")
         copy("bridge.federate_rooms")
-        copy("bridge.private_chat_portal_meta")
+        if isinstance(self.get("bridge.private_chat_portal_meta", "default"), bool):
+            base["bridge.private_chat_portal_meta"] = (
+                "always" if self["bridge.private_chat_portal_meta"] else "default"
+            )
+        else:
+            copy("bridge.private_chat_portal_meta")
+            if base["bridge.private_chat_portal_meta"] not in ("default", "always", "never"):
+                base["bridge.private_chat_portal_meta"] = "default"
         copy("bridge.delivery_receipts")
         copy("bridge.delivery_error_reports")
         copy("bridge.message_status_events")
         copy("bridge.resend_bridge_info")
         copy("bridge.periodic_sync")
 
         copy("bridge.provisioning.enabled")
         copy("bridge.provisioning.prefix")
         if base["bridge.provisioning.prefix"].endswith("/v1"):
             base["bridge.provisioning.prefix"] = base["bridge.provisioning.prefix"][: -len("/v1")]
         copy("bridge.provisioning.shared_secret")
         if base["bridge.provisioning.shared_secret"] == "generate":
             base["bridge.provisioning.shared_secret"] = self._new_token()
         copy("bridge.provisioning.segment_key")
+        copy("bridge.provisioning.segment_user_id")
 
         copy("bridge.command_prefix")
 
         copy_dict("bridge.permissions")
 
         copy("bridge.relay.enabled")
         copy_dict("bridge.relay.message_formats")
         copy("bridge.relay.relaybot")
+        copy("bridge.relay.invite")
         copy("bridge.bridge_matrix_leave")
         copy("bridge.location_format")
 
     def _get_permissions(self, key: str) -> Permissions:
         level = self["bridge.permissions"].get(key, "")
         admin = level == "admin"
         user = level == "user" or admin
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/__init__.py` & `mautrix-signal-0.4.3/mautrix_signal/db/__init__.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/disappearing_message.py` & `mautrix-signal-0.4.3/mautrix_signal/db/disappearing_message.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/message.py` & `mautrix-signal-0.4.3/mautrix_signal/db/message.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/portal.py` & `mautrix-signal-0.4.3/mautrix_signal/db/portal.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/puppet.py` & `mautrix-signal-0.4.3/mautrix_signal/db/puppet.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     number: str | None
     name: str | None
     name_quality: int
     avatar_hash: str | None
     avatar_url: ContentURI | None
     name_set: bool
     avatar_set: bool
+    contact_info_set: bool
     is_registered: bool
 
     custom_mxid: UserID | None
     access_token: str | None
     next_batch: SyncToken | None
     base_url: URL | None
 
@@ -58,14 +59,15 @@
             self.number,
             self.name,
             self.name_quality,
             self.avatar_hash,
             self.avatar_url,
             self.name_set,
             self.avatar_set,
+            self.contact_info_set,
             self.is_registered,
             self.custom_mxid,
             self.access_token,
             self.next_batch,
             self._base_url_str,
         )
 
@@ -75,51 +77,51 @@
         await conn.execute(
             "UPDATE puppet SET number=null WHERE number=$1 AND uuid<>$2", self.number, self.uuid
         )
 
     async def insert(self) -> None:
         q = """
         INSERT INTO puppet (uuid, number, name, name_quality, avatar_hash, avatar_url,
-                            name_set, avatar_set, is_registered,
+                            name_set, avatar_set, contact_info_set, is_registered,
                             custom_mxid, access_token, next_batch, base_url)
-        VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13)
+        VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13, $14)
         """
         async with self.db.acquire() as conn, conn.transaction():
             await self._delete_existing_number(conn)
             await conn.execute(q, *self._values)
 
     async def _update_number(self) -> None:
         async with self.db.acquire() as conn, conn.transaction():
             await self._delete_existing_number(conn)
             await conn.execute("UPDATE puppet SET number=$1 WHERE uuid=$2", self.number, self.uuid)
 
     async def update(self) -> None:
         q = """
         UPDATE puppet
         SET number=$2, name=$3, name_quality=$4, avatar_hash=$5, avatar_url=$6,
-            name_set=$7, avatar_set=$8, is_registered=$9,
-            custom_mxid=$10, access_token=$11, next_batch=$12, base_url=$13
+            name_set=$7, avatar_set=$8, contact_info_set=$9, is_registered=$10,
+            custom_mxid=$11, access_token=$12, next_batch=$13, base_url=$14
         WHERE uuid=$1
         """
         await self.db.execute(q, *self._values)
 
     @classmethod
     def _from_row(cls, row: asyncpg.Record | None) -> Puppet | None:
         if not row:
             return None
         data = {**row}
         base_url_str = data.pop("base_url")
         base_url = URL(base_url_str) if base_url_str is not None else None
         return cls(base_url=base_url, **data)
 
-    _select_base = (
-        "SELECT uuid, number, name, name_quality, avatar_hash, avatar_url, name_set, avatar_set, "
-        "       is_registered, custom_mxid, access_token, next_batch, base_url "
-        "FROM puppet"
-    )
+    _select_base = """
+        SELECT uuid, number, name, name_quality, avatar_hash, avatar_url, name_set, avatar_set,
+               contact_info_set, is_registered, custom_mxid, access_token, next_batch, base_url
+        FROM puppet
+    """
 
     @classmethod
     async def get_by_uuid(cls, uuid: UUID) -> Puppet | None:
         return cls._from_row(await cls.db.fetchrow(f"{cls._select_base} WHERE uuid=$1", uuid))
 
     @classmethod
     async def get_by_number(cls, number: str) -> Puppet | None:
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/reaction.py` & `mautrix-signal-0.4.3/mautrix_signal/db/reaction.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v00_latest_revision.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v00_latest_revision.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from mautrix.util.async_db import Connection
 
 from . import upgrade_table
 
 
-@upgrade_table.register(description="Initial revision", upgrades_to=11)
+@upgrade_table.register(description="Initial revision", upgrades_to=12)
 async def upgrade_latest(conn: Connection) -> None:
     await conn.execute(
         """CREATE TABLE portal (
             chat_id     TEXT,
             receiver    TEXT,
             mxid        TEXT,
             name        TEXT,
@@ -45,22 +45,23 @@
             username    TEXT,
             uuid        UUID,
             notice_room TEXT
         )"""
     )
     await conn.execute(
         """CREATE TABLE puppet (
-            uuid         UUID PRIMARY KEY,
-            number       TEXT UNIQUE,
-            name         TEXT,
-            name_quality INTEGER NOT NULL DEFAULT 0,
-            avatar_hash  TEXT,
-            avatar_url   TEXT,
-            name_set     BOOLEAN NOT NULL DEFAULT false,
-            avatar_set   BOOLEAN NOT NULL DEFAULT false,
+            uuid             UUID PRIMARY KEY,
+            number           TEXT UNIQUE,
+            name             TEXT,
+            name_quality     INTEGER NOT NULL DEFAULT 0,
+            avatar_hash      TEXT,
+            avatar_url       TEXT,
+            name_set         BOOLEAN NOT NULL DEFAULT false,
+            avatar_set       BOOLEAN NOT NULL DEFAULT false,
+            contact_info_set BOOLEAN NOT NULL DEFAULT false,
 
             is_registered BOOLEAN NOT NULL DEFAULT false,
 
             custom_mxid  TEXT,
             access_token TEXT,
             next_batch   TEXT,
             base_url     TEXT
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v02_portal_avatar_info.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v02_portal_avatar_info.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v03_puppet_base_url.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v03_puppet_base_url.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v04_phone_sender_identifier.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v04_phone_sender_identifier.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v05_puppet_avatar_info.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v05_puppet_avatar_info.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v06_portal_revision.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v06_portal_revision.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v07_portal_relay_user.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v07_portal_relay_user.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v08_disappearing_messages.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v08_disappearing_messages.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v09_group_topic.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v09_group_topic.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v10_puppet_name_quality.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v10_puppet_name_quality.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/upgrade/v11_drop_number_support.py` & `mautrix-signal-0.4.3/mautrix_signal/db/upgrade/v11_drop_number_support.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/db/user.py` & `mautrix-signal-0.4.3/mautrix_signal/db/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/example-config.yaml` & `mautrix-signal-0.4.3/mautrix_signal/example-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Homeserver details
 homeserver:
     # The address that this appservice can use to connect to the homeserver.
-    address: https://example.com
-    # The domain of the homeserver (for MXIDs, etc).
+    address: https://matrix.example.com
+    # The domain of the homeserver (also known as server_name, used for MXIDs, etc).
     domain: example.com
     # Whether or not to verify the SSL certificate of the homeserver.
     # Only applies if address starts with https://
     verify_ssl: true
     # What software is the homeserver running?
     # Standard Matrix homeservers like Synapse, Dendrite and Conduit should just use "standard" here.
     software: standard
@@ -175,14 +175,31 @@
         # Whether to use MSC2409/MSC3202 instead of /sync long polling for receiving encryption-related data.
         appservice: false
         # Require encryption, drop any unencrypted messages.
         require: false
         # Enable key sharing? If enabled, key requests for rooms where users are in will be fulfilled.
         # You must use a client that supports requesting keys from other users to use this feature.
         allow_key_sharing: false
+        # Options for deleting megolm sessions from the bridge.
+        delete_keys:
+            # Beeper-specific: delete outbound sessions when hungryserv confirms
+            # that the user has uploaded the key to key backup.
+            delete_outbound_on_ack: false
+            # Don't store outbound sessions in the inbound table.
+            dont_store_outbound: false
+            # Ratchet megolm sessions forward after decrypting messages.
+            ratchet_on_decrypt: false
+            # Delete fully used keys (index >= max_messages) after decrypting messages.
+            delete_fully_used_on_decrypt: false
+            # Delete previous megolm sessions from same device when receiving a new one.
+            delete_prev_on_new_session: false
+            # Delete megolm sessions received from a device when the device is deleted.
+            delete_on_device_delete: false
+            # Periodically delete megolm sessions when 2x max_age has passed since receiving the session.
+            periodically_delete_expired: false
         # What level of device verification should be required from users?
         #
         # Valid levels:
         #   unverified - Send keys to all device in the room.
         #   cross-signed-untrusted - Require valid cross-signing, but trust all cross-signing keys.
         #   cross-signed-tofu - Require valid cross-signing, trust cross-signing keys on first use (and reject changes).
         #   cross-signed-verified - Require valid cross-signing, plus a valid user signature from the bridge bot.
@@ -210,17 +227,19 @@
             # as the default.
             milliseconds: 604800000
             # The maximum number of messages that should be sent with a given a
             # session before changing it. The Matrix spec recommends 100 as the
             # default.
             messages: 100
 
-    # Whether or not to explicitly set the avatar and room name for private
-    # chat portal rooms. This will be implicitly enabled if encryption.default is true.
-    private_chat_portal_meta: false
+    # Whether to explicitly set the avatar and room name for private chat portal rooms.
+    # If set to `default`, this will be enabled in encrypted rooms and disabled in unencrypted rooms.
+    # If set to `always`, all DM rooms will have explicit names and avatars set.
+    # If set to `never`, DM rooms will never have names and avatars set.
+    private_chat_portal_meta: default
     # Whether or not the bridge should send a read receipt from the bridge bot when a message has
     # been sent to Signal. This let's you check manually whether the bridge is receiving your
     # messages.
     # Note that this is not related to Signal delivery receipts.
     delivery_receipts: false
     # Whether or not delivery errors should be reported as messages in the Matrix room.
     delivery_error_reports: true
@@ -230,14 +249,18 @@
     # This field will automatically be changed back to false after it,
     # except if the config file is not writable.
     resend_bridge_info: false
     # Interval at which to resync contacts (in seconds).
     periodic_sync: 0
     # Should leaving the room on Matrix make the user leave on Signal?
     bridge_matrix_leave: true
+    # Should the bridge auto-create a group chat on Signal when a ghost is invited to a room?
+    # Requires the user to have sufficient power level and double puppeting enabled.
+    create_group_on_invite: true
+    hacky_contact_name_mixup_detection: false
 
     # Provisioning API part of the web server for automated portal creation and fetching information.
     # Used by things like mautrix-manager (https://github.com/tulir/mautrix-manager).
     provisioning:
         # Whether or not the provisioning API should be enabled.
         enabled: true
         # The prefix to use in the provisioning API endpoints.
@@ -246,14 +269,16 @@
         # Set to "generate" to generate and save a new token.
         shared_secret: generate
         # Segment API key to enable analytics tracking for web server
         # endpoints. Set to null to disable.
         # Currently the only events are login start, QR code scan, and login
         # success/failure.
         segment_key: null
+        # Optional user_id to use when sending Segment events. If null, defaults to using mxID.
+        segment_user_id: null
 
     # The prefix for commands. Only required in non-management rooms.
     command_prefix: "!signal"
 
     # Messages sent upon joining a management room.
     # Markdown is supported. The defaults are listed below.
     management_room_text:
@@ -303,14 +328,16 @@
             m.audio: '$sender_displayname sent an audio file'
             m.video: '$sender_displayname sent a video'
             m.location: '$sender_displayname sent a location'
         # Specify a dedicated relay account. Must be a regular matrix account logged into this bridge
         # and double puppeting working to auto-accept invites. When this user is invited to a room
         # it will automatically be set as the relay user. May be overridden with `set-relay` or `unset-relay`
         relaybot: '@relaybot:example.com'
+        # Whether or not invites from non-logged-in users should be relayed
+        invite: true
 
     # Format for generating URLs from location messages for sending to Signal
     # Google Maps: 'https://www.google.com/maps/place/{lat},{long}'
     # OpenStreetMap: 'https://www.openstreetmap.org/?mlat={lat}&mlon={long}'
     location_format: 'https://www.google.com/maps/place/{lat},{long}'
 
 # Python logging configuration.
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/formatter.py` & `mautrix-signal-0.4.3/mautrix_signal/formatter.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/get_version.py` & `mautrix-signal-0.4.3/mautrix_signal/get_version.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/matrix.py` & `mautrix-signal-0.4.3/mautrix_signal/matrix.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from mausignald.types import Address
+from mausignald.types import Address, GroupID
 from mautrix.bridge import BaseMatrixHandler, RejectMatrixInvite
 from mautrix.types import (
     Event,
     EventID,
     EventType,
     PresenceEvent,
     ReactionEvent,
@@ -33,14 +33,15 @@
     SingleReceiptEventContent,
     StateEvent,
     TypingEvent,
     UserID,
 )
 
 from . import portal as po, puppet as pu, signal as s, user as u
+from .commands.util import get_initial_state
 from .db import Message as DBMessage
 
 if TYPE_CHECKING:
     from .__main__ import SignalBridge
 
 
 class MatrixHandler(BaseMatrixHandler):
@@ -51,14 +52,64 @@
         homeserver = bridge.config["homeserver.domain"]
         self.user_id_prefix = f"@{prefix}"
         self.user_id_suffix = f"{suffix}:{homeserver}"
         self.signal = bridge.signal
 
         super().__init__(bridge=bridge)
 
+    async def handle_puppet_group_invite(
+        self,
+        room_id: RoomID,
+        puppet: pu.Puppet,
+        invited_by: u.User,
+        evt: StateEvent,
+        members: list[UserID],
+    ) -> None:
+        double_puppet = await pu.Puppet.get_by_custom_mxid(invited_by.mxid)
+        if (
+            not double_puppet
+            or self.az.bot_mxid in members
+            or not self.config["bridge.create_group_on_invite"]
+        ):
+            if self.az.bot_mxid not in members:
+                await puppet.default_mxid_intent.leave_room(
+                    room_id,
+                    reason="This ghost does not join multi-user rooms without the bridge bot.",
+                )
+            else:
+                await puppet.default_mxid_intent.send_notice(
+                    room_id,
+                    "This ghost will remain inactive "
+                    "until a Signal Group is created for this room.",
+                )
+            return
+
+        await double_puppet.intent.invite_user(room_id, self.az.bot_mxid)
+
+        title, about, levels, encrypted, avatar_url, join_rule = await get_initial_state(
+            double_puppet.intent, room_id
+        )
+
+        portal = po.Portal(
+            chat_id=GroupID(""),
+            mxid=evt.room_id,
+            name=title,
+            topic=about or "",
+            encrypted=encrypted,
+            receiver="",
+            avatar_url=avatar_url,
+        )
+        await portal.az.intent.ensure_joined(room_id)
+        invited_by_level = levels.get_user_level(invited_by.mxid)
+        if invited_by_level > levels.get_user_level(self.az.bot_mxid):
+            levels.users[self.az.bot_mxid] = 100 if invited_by_level >= 100 else invited_by_level
+            await double_puppet.intent.set_power_levels(room_id, levels)
+
+        await portal.create_signal_group(invited_by, levels, join_rule)
+
     async def handle_invite(
         self, room_id: RoomID, user_id: UserID, inviter: u.User, event_id: EventID
     ) -> None:
         user = await u.User.get_by_mxid(user_id, create=False)
         if not user or not await user.is_logged_in():
             return
         portal = await po.Portal.get_by_mxid(room_id)
@@ -148,14 +199,52 @@
         await self.handle_kick_ban("unbanned", room_id, user_id, unbanned_by, reason, event_id)
 
     async def handle_ban(
         self, room_id: RoomID, user_id: UserID, banned_by: UserID, reason: str, event_id: EventID
     ) -> None:
         await self.handle_kick_ban("banned", room_id, user_id, banned_by, reason, event_id)
 
+    async def handle_accept_knock(
+        self, room_id: RoomID, user_id: UserID, sender: UserID, reason: str, event_id: EventID
+    ) -> None:
+        self.log.debug(f"Knock {user_id} to {room_id} was accepted: {reason}")
+        portal = await po.Portal.get_by_mxid(room_id)
+        if not portal:
+            return
+        sender = await u.User.get_by_mxid(sender)
+        sender, is_relay = await portal.get_relay_sender(sender, "knock accept")
+        if not sender:
+            return
+
+        user = await pu.Puppet.get_by_mxid(user_id)
+        if not user:
+            user = await u.User.get_by_mxid(user_id, create=False)
+            if not user or not await user.is_logged_in():
+                return
+        await portal.matrix_accept_knock(sender, user)
+
+    async def handle_reject_knock(
+        self, room_id: RoomID, user_id: UserID, sender: UserID, reason: str, event_id: EventID
+    ) -> None:
+        self.log.debug(f"Knock from {user_id} to {room_id} was rejected: {reason}")
+        portal = await po.Portal.get_by_mxid(room_id)
+        if not portal:
+            return
+        sender = await u.User.get_by_mxid(sender)
+        sender, is_relay = await portal.get_relay_sender(sender, "knock reject")
+        if not sender:
+            return
+
+        user = await pu.Puppet.get_by_mxid(user_id)
+        if not user:
+            user = await u.User.get_by_mxid(user_id, create=False)
+            if not user or not await user.is_logged_in():
+                return
+        await portal.matrix_reject_knock(sender, user)
+
     @classmethod
     async def handle_reaction(
         cls, room_id: RoomID, user_id: UserID, event_id: EventID, content: ReactionEventContent
     ) -> None:
         if content.relates_to.rel_type != RelationType.ANNOTATION:
             cls.log.debug(
                 f"Ignoring m.reaction event in {room_id} from {user_id} with unexpected "
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/portal.py` & `mautrix-signal-0.4.3/mautrix_signal/portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,37 +11,38 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Union, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Literal, Union, cast
 from collections import deque
 from uuid import UUID, uuid4
 import asyncio
 import hashlib
 import mimetypes
 import os
 import os.path
 import pathlib
 import time
 
 from mausignald.errors import (
     AttachmentTooLargeError,
+    GroupPatchNotAcceptedError,
     NotConnected,
     ProfileUnavailableError,
+    ProofRequiredError,
     RPCError,
 )
 from mausignald.types import (
     AccessControlMode,
     Address,
     AnnouncementsMode,
     Attachment,
-    Group,
     GroupAccessControl,
     GroupChange,
     GroupID,
     GroupMember,
     GroupMemberRole,
     GroupV2,
     GroupV2ID,
@@ -80,15 +81,15 @@
     RelatesTo,
     RelationType,
     RoomID,
     TextMessageEventContent,
     UserID,
     VideoInfo,
 )
-from mautrix.util import ffmpeg, variation_selector
+from mautrix.util import background_task, ffmpeg, variation_selector
 from mautrix.util.format_duration import format_duration
 from mautrix.util.message_send_checkpoint import MessageSendCheckpointStatus
 
 from . import matrix as m, puppet as p, signal as s, user as u
 from .config import Config
 from .db import (
     DisappearingMessage,
@@ -115,15 +116,15 @@
 try:
     from mautrix.util import magic
 except ImportError:
     magic = None
 
 StateBridge = EventType.find("m.bridge", EventType.Class.STATE)
 StateHalfShotBridge = EventType.find("uk.half-shot.bridge", EventType.Class.STATE)
-ChatInfo = Union[Group, GroupV2, GroupV2ID, Profile, Address]
+ChatInfo = Union[GroupV2, Profile, Address]
 MAX_MATRIX_MESSAGE_SIZE = 30000
 BEEPER_LINK_PREVIEWS_KEY = "com.beeper.linkpreviews"
 BEEPER_IMAGE_ENCRYPTION_KEY = "beeper:image:encryption"
 
 
 class UnknownReactionTarget(Exception):
     pass
@@ -134,15 +135,15 @@
     by_chat_id: dict[tuple[str, str], Portal] = {}
     _sticker_meta_cache: dict[str, StickerPack] = {}
     disappearing_msg_class = DisappearingMessage
     config: Config
     matrix: m.MatrixHandler
     signal: s.SignalHandler
     az: AppService
-    private_chat_portal_meta: bool
+    private_chat_portal_meta: Literal["default", "always", "never"]
     expiration_time: int | None
 
     _main_intent: IntentAPI | None
     _create_room_lock: asyncio.Lock
     _msgts_dedup: deque[tuple[UUID, int]]
     _reaction_dedup: deque[tuple[UUID, int, str, UUID, bool]]
     _reaction_lock: asyncio.Lock
@@ -199,14 +200,22 @@
         return self._main_intent
 
     @property
     def is_direct(self) -> bool:
         return isinstance(self.chat_id, UUID)
 
     @property
+    def set_dm_room_metadata(self) -> bool:
+        return (
+            not self.is_direct
+            or self.private_chat_portal_meta == "always"
+            or (self.encrypted and self.private_chat_portal_meta != "never")
+        )
+
+    @property
     def disappearing_enabled(self) -> bool:
         return self.is_direct or self.config["signal.enable_disappearing_messages_in_groups"]
 
     @classmethod
     def init_cls(cls, bridge: "SignalBridge") -> None:
         cls.config = bridge.config
         cls.matrix = bridge.matrix
@@ -316,16 +325,18 @@
                 if isinstance(e, AttachmentTooLargeError)
                 else MessageSendCheckpointStatus.PERM_FAILURE
             )
             sender.send_remote_checkpoint(
                 status, event_id, self.mxid, EventType.ROOM_MESSAGE, message.msgtype, error=e
             )
             await sender.handle_auth_failure(e)
+            if isinstance(e, ProofRequiredError):
+                sender.challenge_token = e.token
             await self._send_error_notice("message", e)
-            asyncio.create_task(self._send_message_status(event_id, e))
+            background_task.create(self._send_message_status(event_id, e))
 
     async def _send_error_notice(self, type_name: str, err: Exception) -> None:
         if not self.config["bridge.delivery_error_reports"]:
             return
         message = f"{type(err).__name__}: {err}"
         if isinstance(err, NotConnected):
             message = "There was an error connecting to signald."
@@ -359,15 +370,15 @@
                 status.message = "too large file (maximum is 100MB)"
             elif isinstance(err, UnknownReactionTarget):
                 status.status = MessageStatus.FAIL
             else:
                 status.status = MessageStatus.RETRIABLE
         else:
             status.status = MessageStatus.SUCCESS
-        status.fill_legacy_booleans()
+
         await intent.send_message_event(
             room_id=self.mxid,
             event_type=EventType.BEEPER_MESSAGE_STATUS,
             content=status,
         )
 
     async def _beeper_link_preview_to_signal(
@@ -510,26 +521,26 @@
                 pass
 
         # Handle disappearing messages
         if self.expiration_time and self.disappearing_enabled:
             dm = DisappearingMessage(self.mxid, event_id, self.expiration_time)
             dm.start_timer()
             await dm.insert()
-            asyncio.create_task(self._disappear_event(dm))
+            background_task.create(self._disappear_event(dm))
 
         sender.send_remote_checkpoint(
             MessageSendCheckpointStatus.SUCCESS,
             event_id,
             self.mxid,
             EventType.ROOM_MESSAGE,
             message.msgtype,
             retry_num=retry_count,
         )
         await self._send_delivery_receipt(event_id)
-        asyncio.create_task(self._send_message_status(event_id, err=None))
+        background_task.create(self._send_message_status(event_id, err=None))
 
     async def _signal_send_with_retries(
         self,
         sender: u.User,
         event_id: EventID,
         send_fn: Callable,
         event_type: EventType,
@@ -604,25 +615,25 @@
                 event_id,
                 self.mxid,
                 EventType.REACTION,
                 error=e,
             )
             await self._send_error_notice("reaction", e)
             await sender.handle_auth_failure(e)
-            asyncio.create_task(self._send_message_status(event_id, e))
+            background_task.create(self._send_message_status(event_id, e))
         else:
             sender.send_remote_checkpoint(
                 MessageSendCheckpointStatus.SUCCESS,
                 event_id,
                 self.mxid,
                 EventType.REACTION,
                 retry_num=retry_count,
             )
             await self._send_delivery_receipt(event_id)
-            asyncio.create_task(self._send_message_status(event_id, err=None))
+            background_task.create(self._send_message_status(event_id, err=None))
 
     async def _handle_matrix_reaction(
         self,
         sender: u.User,
         event_id: EventID,
         reacting_to: EventID,
         emoji: str,
@@ -680,26 +691,26 @@
                     MessageSendCheckpointStatus.PERM_FAILURE,
                     redaction_event_id,
                     self.mxid,
                     EventType.ROOM_REDACTION,
                     error=e,
                 )
                 await sender.handle_auth_failure(e)
-                asyncio.create_task(self._send_error_notice("message deletion", e))
-                asyncio.create_task(self._send_message_status(event_id, e))
+                background_task.create(self._send_error_notice("message deletion", e))
+                background_task.create(self._send_message_status(event_id, e))
             else:
                 self.log.trace(f"Removed {message} after Matrix redaction")
                 sender.send_remote_checkpoint(
                     MessageSendCheckpointStatus.SUCCESS,
                     redaction_event_id,
                     self.mxid,
                     EventType.ROOM_REDACTION,
                 )
                 await self._send_delivery_receipt(redaction_event_id)
-                asyncio.create_task(self._send_message_status(redaction_event_id, err=None))
+                background_task.create(self._send_message_status(redaction_event_id, err=None))
             return
 
         reaction = await DBReaction.get_by_mxid(event_id, self.mxid)
         if reaction:
             try:
                 await reaction.delete()
                 remove_reaction = Reaction(
@@ -720,37 +731,37 @@
                     MessageSendCheckpointStatus.PERM_FAILURE,
                     redaction_event_id,
                     self.mxid,
                     EventType.ROOM_REDACTION,
                     error=e,
                 )
                 await sender.handle_auth_failure(e)
-                asyncio.create_task(self._send_error_notice("reaction deletion", e))
-                asyncio.create_task(self._send_message_status(event_id, e))
+                background_task.create(self._send_error_notice("reaction deletion", e))
+                background_task.create(self._send_message_status(event_id, e))
             else:
                 self.log.trace(f"Removed {reaction} after Matrix redaction")
                 sender.send_remote_checkpoint(
                     MessageSendCheckpointStatus.SUCCESS,
                     redaction_event_id,
                     self.mxid,
                     EventType.ROOM_REDACTION,
                 )
                 await self._send_delivery_receipt(redaction_event_id)
-                asyncio.create_task(self._send_message_status(redaction_event_id, err=None))
+                background_task.create(self._send_message_status(redaction_event_id, err=None))
             return
 
         sender.send_remote_checkpoint(
             MessageSendCheckpointStatus.PERM_FAILURE,
             redaction_event_id,
             self.mxid,
             EventType.ROOM_REDACTION,
             error="No message or reaction found for redaction",
         )
         status_err = UnknownReactionTarget("No message or reaction found for redaction")
-        asyncio.create_task(self._send_message_status(redaction_event_id, err=status_err))
+        background_task.create(self._send_message_status(redaction_event_id, err=status_err))
 
     async def handle_matrix_join(self, user: u.User) -> None:
         if self.is_direct or not await user.is_logged_in():
             return
         if self._pending_members is None:
             self.log.debug(
                 f"{user.mxid} ({user.uuid}) joined room, but pending_members is None,"
@@ -840,22 +851,38 @@
                 for member in info.banned_members:
                     if member.uuid == user.uuid:
                         await self.main_intent.ban_user(
                             self.mxid, user.mxid, reason=f"Failed to unban Signal user: {e}"
                         )
                         return
 
-    async def handle_matrix_invite(self, invited_by: u.User, user: u.User | p.Puppet) -> None:
+    async def handle_matrix_invite(
+        self, invited_by: u.User, user: u.User | p.Puppet
+    ) -> GroupV2 | None:
         if self.is_direct:
             raise RejectMatrixInvite("You can't invite additional users to private chats.")
-
+        invited_by, is_relay = await self.get_relay_sender(invited_by, "invite")
+        if is_relay:
+            if not self.config["bridge.relay.invite"]:
+                raise RejectMatrixInvite("Relaying invites is not enabled on this bridge")
+            if not invited_by:
+                raise RejectMatrixInvite("There is no relay in this room")
+        update_meta = None
         try:
-            await self.signal.update_group(
+            update_meta = await self.signal.update_group(
                 invited_by.username, self.chat_id, add_members=[user.address]
             )
+            self.revision = update_meta.revision
+        except GroupPatchNotAcceptedError as e:
+            update_meta = await self.signal.get_group(invited_by.username, self.chat_id)
+            if (
+                user.address not in update_meta.members
+                and user.address not in update_meta.pending_members
+            ):
+                raise RejectMatrixInvite(str(e)) from e
         except RPCError as e:
             raise RejectMatrixInvite(str(e)) from e
         if user.mxid == self.config["bridge.relay.relaybot"] != "@relaybot:example.com":
             await self._handle_relaybot_invited(user)
         power_levels = await self.main_intent.get_power_levels(self.mxid)
         invitee_pl = power_levels.get_user_level(user.mxid)
         if invitee_pl >= 50:
@@ -866,14 +893,15 @@
                 )
                 self.revision = update_meta.revision
             except Exception as e:
                 self.log.exception(f"Failed to update Signal member role: {e}")
                 await self._update_power_levels(
                     await self.signal.get_group(invited_by.username, self.chat_id)
                 )
+        return update_meta
 
     async def _handle_relaybot_invited(self, user: u.User) -> None:
         if not self.config["bridge.relay.enabled"]:
             await self.main_intent.send_notice(
                 self.mxid, "Relay mode is not enabled in this instance of the bridge."
             )
         else:
@@ -1065,14 +1093,54 @@
             self.revision = update_meta.revision
         except Exception as e:
             self.log.exception(f"Failed to update Signal link access control: {e}")
             await self._update_join_rules(
                 await self.signal.get_group(sender.username, self.chat_id)
             )
 
+    async def matrix_accept_knock(self, sender: u.User, user: p.Puppet | u.User) -> None:
+        try:
+            await self.signal.approve_membership(
+                sender.username, self.chat_id, members=[user.address]
+            )
+            if isinstance(user, p.Puppet):
+                await user.intent_for(self).ensure_joined(self.mxid)
+        except RPCError as e:
+            info = await self.signal.get_group(sender.username, self.chat_id)
+            if user.address in info.requesting_members:
+                raise RejectMatrixInvite(str(e)) from e
+        power_levels = await self.main_intent.get_power_levels(self.mxid)
+        invitee_pl = power_levels.get_user_level(user.mxid)
+        if invitee_pl >= 50:
+            group_member = GroupMember(uuid=user.uuid, role=GroupMemberRole.ADMINISTRATOR)
+            try:
+                update_meta = await self.signal.update_group(
+                    sender.username, self.chat_id, update_role=group_member
+                )
+                self.revision = update_meta.revision
+            except Exception as e:
+                self.log.exception(f"Failed to update Signal member role: {e}")
+                await self._update_power_levels(
+                    await self.signal.get_group(sender.username, self.chat_id)
+                )
+
+    async def matrix_reject_knock(self, sender: u.User, user: p.Puppet | u.User) -> None:
+        try:
+            await self.signal.refuse_membership(
+                sender.username, self.chat_id, members=[user.address]
+            )
+        except RPCError as e:
+            info = await self.signal.get_group(sender.username, self.chat_id)
+            if user.address in info.requesting_members:
+                await user.intent_for(self).knock(
+                    self.mxid,
+                    reason=f"refusing membership failed: {e}",
+                    servers=[self.config["homeserver.domain"]],
+                )
+
     # endregion
     # region Signal event handling
 
     async def _find_quote_event_id(self, quote: Quote | None) -> MessageEvent | EventID | None:
         if not quote:
             return None
 
@@ -1158,15 +1226,15 @@
             await self.signal.send_receipt(
                 source.username, sender.address, timestamps=[message.timestamp]
             )
             return
         self.log.debug(f"Started handling message {message.timestamp} by {sender.uuid}")
         self.log.trace(f"Message content: {message}")
         intent = sender.intent_for(self)
-        await intent.set_typing(self.mxid, False)
+        await intent.set_typing(self.mxid, timeout=0)
         event_id = None
         reply_to = await self._find_quote_event_id(message.quote)
 
         if message.sticker:
             if message.sticker.attachment.incoming_filename:
                 content = await self._handle_signal_attachment(
                     intent, message.sticker.attachment, sticker=True
@@ -1198,34 +1266,20 @@
             if reply_to and not message.body:
                 content.set_reply(reply_to)
                 reply_to = None
             event_id = await self._send_message(intent, content, timestamp=message.timestamp)
 
         is_first_text = True
         for attachment in message.attachments:
-            if not attachment.incoming_filename:
-                self.log.warning(
-                    "Failed to bridge attachment, no incoming filename: %s", attachment
-                )
-                continue
             as_text = (
                 is_first_text
                 and attachment.content_type == "text/x-signal-plain"
                 and attachment.size < MAX_MATRIX_MESSAGE_SIZE
             )
 
-            file_size = attachment.size or os.path.getsize(attachment.incoming_filename)
-            if file_size > self.matrix.media_config.upload_size:
-                self.log.warning(
-                    "Failed to bridge attachment %s in %s: file too large",
-                    attachment.id,
-                    message.timestamp,
-                )
-                continue
-
             content = await self._handle_signal_attachment(intent, attachment, text=as_text)
             if as_text:
                 is_first_text = False
                 message.body = ""
             if reply_to and not message.body:
                 # If there's no text, set the first image as the reply
                 content.set_reply(reply_to)
@@ -1261,15 +1315,15 @@
 
             if message.expires_in_seconds and self.disappearing_enabled:
                 dm = DisappearingMessage(self.mxid, event_id, message.expires_in_seconds)
                 # Start the timer immediately for own messages
                 if sender.uuid == source.uuid:
                     dm.start_timer()
                     await dm.insert()
-                    asyncio.create_task(self._disappear_event(dm))
+                    background_task.create(self._disappear_event(dm))
                     self.log.debug(
                         f"{event_id} set to be redacted in {message.expires_in_seconds} seconds"
                     )
                 else:
                     await dm.insert()
                     self.log.debug(
                         f"{event_id} set to be redacted {message.expires_in_seconds} seconds"
@@ -1320,20 +1374,18 @@
                 users = [
                     await p.Puppet.get_by_uuid(group_member.uuid),
                     await u.User.get_by_uuid(group_member.uuid),
                 ]
                 for user in users:
                     if not user:
                         continue
-                    if (
-                        group_member.role == GroupMemberRole.ADMINISTRATOR
-                        and levels.users.get(user.mxid, 0) < 50
-                    ):
-                        levels.users[user.mxid] = 50
-                        levels.users = {k: v for k, v in sorted(list(levels.users.items()))}
+                    if group_member.role == GroupMemberRole.ADMINISTRATOR:
+                        if levels.users.get(user.mxid, 0) < 50:
+                            levels.users[user.mxid] = 50
+                            levels.users = {k: v for k, v in sorted(list(levels.users.items()))}
                     elif levels.users.get(user.mxid, 0) >= 50:
                         levels.users.pop(user.mxid, 0)
             await self._try_with_puppet(
                 lambda i: i.set_power_levels(self.mxid, levels), puppet=editor
             )
 
         if group_change.new_banned_members:
@@ -1488,14 +1540,18 @@
                     await self.signal.get_group(
                         source.username, self.chat_id, group_change.revision
                     ),
                     editor,
                 )
                 or changed
             )
+        if group_change.new_timer:
+            changed = (
+                await self.update_expires_in_seconds(editor, group_change.new_timer) or changed
+            )
 
         if changed:
             await self.update_bridge_info()
             await self.update()
 
     @staticmethod
     async def _make_media_content(
@@ -1551,14 +1607,27 @@
             info.size = len(data)
 
         return content, data
 
     async def _handle_signal_attachment(
         self, intent: IntentAPI, attachment: Attachment, sticker: bool = False, text: bool = False
     ) -> MediaMessageEventContent | TextMessageEventContent:
+        if not attachment.incoming_filename:
+            self.log.warning("Failed to bridge attachment, no incoming filename: %s", attachment)
+            return TextMessageEventContent(
+                msgtype=MessageType.NOTICE, body="Missing attachment data"
+            )
+        file_size = attachment.size or os.path.getsize(attachment.incoming_filename)
+        if file_size > self.matrix.media_config.upload_size:
+            self.log.warning(
+                f"Dropping attachment {attachment.id}: file too large "
+                f"({file_size} > {self.matrix.media_config.upload_size})"
+            )
+            return TextMessageEventContent(msgtype=MessageType.NOTICE, body="Attachment too large")
+
         self.log.trace(f"Reuploading attachment {attachment}")
         if not attachment.content_type:
             attachment.content_type = (
                 magic.mimetype(attachment.incoming_filename)
                 if magic is not None
                 else "application/octet-stream"
             )
@@ -1801,28 +1870,29 @@
             await self.signal.update_group(source.username, self.chat_id, description=self.topic)
         await self.handle_matrix_power_level(source, levels)
         await self.handle_matrix_join_rules(source, join_rule)
         await self.update()
         await self.update_bridge_info()
         if relaybot:
             await self._handle_relaybot_invited(relaybot)
+        await self.main_intent.send_notice(self.mxid, f"Signal group created. ID: {self.chat_id}")
 
     async def bridge_signal_group(
         self, source: u.User, levels: PowerLevelStateEventContent
     ) -> None:
         await self._postinit()
         await self.insert()
         await self.handle_matrix_power_level(source, levels)
         await self.update()
         await self.update_bridge_info()
 
     # endregion
     # region Updating portal info
 
-    async def update_info(self, source: u.User, info: ChatInfo) -> None:
+    async def update_info(self, source: u.User, info: ChatInfo | GroupV2ID) -> None:
         if self.is_direct:
             if not isinstance(info, (Profile, Address)):
                 raise ValueError(f"Unexpected type for direct chat update_info: {type(info)}")
             if not self.name or not self.topic:
                 puppet = await self.get_dm_puppet()
                 if not puppet.name:
                     await puppet.update_info(info, source)
@@ -1844,60 +1914,55 @@
                 self.log.debug(
                     f"Failed to get full group v2 info through {source.username}, "
                     "cancelling update"
                 )
                 return
 
         changed = False
-        if isinstance(info, Group):
-            changed = await self._update_name(info.name) or changed
-        elif isinstance(info, GroupV2):
-            if self.revision < info.revision:
-                self.revision = info.revision
-                changed = True
-            elif self.revision > info.revision:
-                self.log.warning(
-                    f"Got outdated info when syncing through {source.username} "
-                    f"({info.revision} < {self.revision}), ignoring..."
-                )
-                return
-            changed = await self._update_name(info.title) or changed
-            changed = await self._update_topic(info.description) or changed
-        elif isinstance(info, GroupV2ID):
+        if self.revision < info.revision:
+            self.revision = info.revision
+            changed = True
+        elif self.revision > info.revision:
+            self.log.warning(
+                f"Got outdated info when syncing through {source.username} "
+                f"({info.revision} < {self.revision}), ignoring..."
+            )
             return
-        else:
-            raise ValueError(f"Unexpected type for group update_info: {type(info)}")
+        changed = await self._update_name(info.title) or changed
+        changed = await self._update_topic(info.description) or changed
         changed = await self._update_avatar(info) or changed
         await self._update_participants(source, info)
         try:
             await self._update_power_levels(info)
         except Exception:
             self.log.warning("Error updating power levels", exc_info=True)
         try:
             await self._update_join_rules(info)
         except:
             self.log.warning("Error updating join rules", exc_info=True)
         if changed:
             await self.update_bridge_info()
             await self.update()
 
-    async def update_expires_in_seconds(self, sender: p.Puppet, expires_in_seconds: int) -> None:
+    async def update_expires_in_seconds(self, sender: p.Puppet, expires_in_seconds: int) -> bool:
         if expires_in_seconds == 0:
             expires_in_seconds = None
         if self.expiration_time == expires_in_seconds:
-            return
+            return False
 
         assert self.mxid
+        self.log.debug(f"Setting portal expiration time to {expires_in_seconds}")
         self.expiration_time = expires_in_seconds
         await self.update()
 
         time_str = "Off" if expires_in_seconds is None else format_duration(expires_in_seconds)
         body = f"Set the disappearing message timer to {time_str}"
         content = TextMessageEventContent(msgtype=MessageType.NOTICE, body=body)
         await self._send_message(sender.intent_for(self), content)
+        return True
 
     async def get_dm_puppet(self) -> p.Puppet | None:
         if not self.is_direct:
             return None
         return await p.Puppet.get_by_uuid(self.chat_id)
 
     async def update_info_from_puppet(self, puppet: p.Puppet | None = None) -> None:
@@ -1907,64 +1972,55 @@
             puppet = await self.get_dm_puppet()
         await self.update_puppet_name(puppet.name, save=False)
         await self.update_puppet_avatar(puppet.avatar_hash, puppet.avatar_url, save=False)
         if puppet.number:
             await self.update_puppet_number(puppet.fmt_phone(puppet.number), save=False)
 
     async def update_puppet_number(self, number: str, save: bool = True) -> None:
-        if not self.encrypted and not self.private_chat_portal_meta:
-            return
-
         changed = await self._update_topic(number)
         if changed and save:
             await self.update_bridge_info()
             await self.update()
 
     async def update_puppet_avatar(
         self, new_hash: str, avatar_url: ContentURI, save: bool = True
     ) -> None:
-        if not self.encrypted and not self.private_chat_portal_meta:
-            return
-
-        if self.avatar_hash != new_hash or not self.avatar_set:
+        if self.avatar_hash != new_hash or (not self.avatar_set and self.set_dm_room_metadata):
             self.avatar_hash = new_hash
             self.avatar_url = avatar_url
-            if self.mxid:
+            self.avatar_set = False
+            if self.mxid and self.set_dm_room_metadata:
                 try:
                     await self.main_intent.set_room_avatar(self.mxid, avatar_url)
                     self.avatar_set = True
                 except Exception:
                     self.log.exception("Error setting avatar")
-                    self.avatar_set = False
                 if save:
                     await self.update_bridge_info()
                     await self.update()
 
     async def update_puppet_name(self, name: str, save: bool = True) -> None:
-        if not self.encrypted and not self.private_chat_portal_meta:
-            return
-
         changed = await self._update_name(name)
 
         if changed and save:
             await self.update_bridge_info()
             await self.update()
 
     async def _update_name(self, name: str, sender: p.Puppet | None = None) -> bool:
-        if self.name != name or not self.name_set:
+        if self.name != name or (not self.name_set and self.set_dm_room_metadata):
             self.name = name
-            if self.mxid:
+            self.name_set = False
+            if self.mxid and self.set_dm_room_metadata:
                 try:
                     await self._try_with_puppet(
                         lambda i: i.set_room_name(self.mxid, self.name), puppet=sender
                     )
                     self.name_set = True
                 except Exception:
                     self.log.exception("Error setting name")
-                    self.name_set = False
             return True
         return False
 
     async def _update_topic(self, topic: str, sender: p.Puppet | None = None) -> bool:
         if self.topic != topic:
             self.topic = topic
             if self.mxid:
@@ -1985,20 +2041,18 @@
             try:
                 await action(puppet.intent_for(self))
             except (MForbidden, IntentError):
                 await action(self.main_intent)
         else:
             await action(self.main_intent)
 
-    async def _update_avatar(self, info: ChatInfo, sender: p.Puppet | None = None) -> bool:
+    async def _update_avatar(self, info: GroupV2, sender: p.Puppet | None = None) -> bool:
         path = None
         if isinstance(info, GroupV2):
             path = info.avatar
-        elif isinstance(info, Group):
-            path = f"group-{self.chat_id}"
         res = await p.Puppet.upload_avatar(self, path, self.main_intent)
         if res is False:
             return False
         self.avatar_hash, self.avatar_url = res
         if not self.mxid:
             return True
 
@@ -2008,55 +2062,111 @@
             )
             self.avatar_set = True
         except Exception:
             self.log.exception("Error setting avatar")
             self.avatar_set = False
         return True
 
-    async def _update_participants(self, source: u.User, info: ChatInfo) -> None:
-        if not self.mxid or not isinstance(info, (Group, GroupV2)):
+    async def _update_participants(self, source: u.User, info: GroupV2) -> None:
+        if not self.mxid:
             return
 
         member_events = await self.main_intent.get_members(self.mxid)
         remove_users: set[UserID] = {
             UserID(evt.state_key)
             for evt in member_events
-            if evt.content.membership == Membership.JOIN and evt.state_key != self.az.bot_mxid
+            if (
+                evt.content.membership == Membership.JOIN
+                or evt.content.membership == Membership.INVITE
+                or evt.content.membership == Membership.KNOCK
+            )
+            and evt.state_key != self.az.bot_mxid
+        }
+        unban_users: set[UserID] = {
+            UserID(evt.state_key)
+            for evt in member_events
+            if evt.content.membership == Membership.BAN and evt.state_key != self.az.bot_mxid
         }
 
-        pending_members = info.pending_members if isinstance(info, GroupV2) else []
-        self._pending_members = {addr.uuid for addr in pending_members}
+        self._pending_members = {addr.uuid for addr in info.pending_members}
+
+        for member in info.banned_members:
+            user = await u.User.get_by_uuid(member.uuid)
+            if user:
+                unban_users.discard(user.mxid)
+                remove_users.discard(user.mxid)
+                try:
+                    await self.main_intent.ban_user(
+                        self.mxid, user.mxid, reason="Banned on Signal"
+                    )
+                except (MForbidden, MBadState) as e:
+                    self.log.debug(f"Could not ban {user.mxid}: {e}")
+            puppet = await p.Puppet.get_by_address(Address(uuid=member.uuid))
+            unban_users.discard(puppet.mxid)
+            remove_users.discard(puppet.mxid)
+            try:
+                await self.main_intent.ban_user(self.mxid, puppet.mxid, reason="Banned on Signal")
+            except (MForbidden, MBadState) as e:
+                self.log.debug(f"Could not ban {puppet.mxid}: {e}")
+
+        for mxid in unban_users:
+            user = await u.User.get_by_mxid(mxid, create=False)
+            if user and await user.is_logged_in():
+                try:
+                    await self.main_intent.unban_user(
+                        self.mxid, user.mxid, reason="Unbanned on Signal"
+                    )
+                except (MForbidden, MBadState) as e:
+                    self.log.debug(f"Could not unban {user.mxid}: {e}")
+            puppet = await p.Puppet.get_by_mxid(mxid, create=False)
+            if puppet:
+                try:
+                    await self.main_intent.unban_user(
+                        self.mxid, puppet.mxid, reason="Unbanned on Signal"
+                    )
+                except (MForbidden, MBadState) as e:
+                    self.log.debug(f"Could not unban {puppet.mxid}: {e}")
 
-        for address in info.members + pending_members:
+        for address in info.members + info.pending_members:
             user = await u.User.get_by_address(address)
             if user:
                 remove_users.discard(user.mxid)
                 try:
                     await self.main_intent.invite_user(self.mxid, user.mxid, check_cache=True)
                 except (MForbidden, IntentError, MBadState) as e:
                     self.log.debug(f"Failed to invite {user.mxid}: {e}")
 
             puppet = await p.Puppet.get_by_address(address)
             if not puppet:
                 self.log.warning(f"Didn't find puppet for member {address}")
                 continue
-            try:
-                await source.sync_contact(address)
-            except ProfileUnavailableError:
-                self.log.debug(f"Profile of puppet with {address} is unavailable")
+            await source.sync_contact(address)
             try:
                 await self.main_intent.invite_user(
                     self.mxid, puppet.intent_for(self).mxid, check_cache=True
                 )
             except (MForbidden, IntentError, MBadState) as e:
-                self.log.debug(f"could not invite {user.mxid}: {e}")
+                self.log.debug(f"Could not invite {user.mxid}: {e}")
             if address.uuid not in self._pending_members:
                 await puppet.intent_for(self).ensure_joined(self.mxid)
             remove_users.discard(puppet.default_mxid)
 
+        for address in info.requesting_members:
+            puppet = await p.Puppet.get_by_address(address)
+            if puppet:
+                remove_users.discard(puppet.mxid)
+                try:
+                    await puppet.intent_for(self).knock_room(
+                        self.mxid,
+                        reason="via invite link",
+                        servers=[self.config["homeserver.domain"]],
+                    )
+                except (MForbidden, IntentError) as e:
+                    self.log.debug(f"Failed to bridge knock: {e}")
+
         for mxid in remove_users:
             user = await u.User.get_by_mxid(mxid, create=False)
             if user and await user.is_logged_in():
                 try:
                     await self.main_intent.kick_user(
                         self.mxid, user.mxid, reason="not a member of this Signal group"
                     )
@@ -2067,15 +2177,15 @@
                 try:
                     await self.main_intent.kick_user(
                         self.mxid,
                         puppet.intent_for(self).mxid,
                         reason="not a member of this Signal group",
                     )
                 except (MForbidden, MBadState) as e:
-                    self.log.debug(f"could not kick {user.mxid}: {e}")
+                    self.log.debug(f"Could not kick {user.mxid}: {e}")
 
     async def _kick_with_puppet(self, user: p.Puppet | u.User, sender: p.Puppet) -> None:
         try:
             await sender.intent_for(self).kick_user(self.mxid, user.mxid)
         except MForbidden:
             try:
                 await self.main_intent.kick_user(
@@ -2083,15 +2193,15 @@
                 )
             except MForbidden as e:
                 self.log.debug(f"Could not remove {user.mxid}: {e}")
         except MBadState as e:
             self.log.debug(f"Could not remove {user.mxid}: {e}")
 
     async def _update_power_levels(self, info: ChatInfo) -> None:
-        if not self.mxid:
+        if not self.mxid or not info:
             return
 
         power_levels = await self.main_intent.get_power_levels(self.mxid)
         power_levels = await self._get_power_levels(power_levels, info=info, is_initial=False)
         await self.main_intent.set_power_levels(self.mxid, power_levels)
 
     async def _get_new_join_rule(self, link_access: AccessControlMode) -> JoinRule | None:
@@ -2114,15 +2224,15 @@
         else:
             join_rule = JoinRule.INVITE
             allowed_join_rules = (JoinRule.INVITE,)
         if old_join_rule in allowed_join_rules:
             return None
         return join_rule
 
-    async def _update_join_rules(self, info: ChatInfo) -> None:
+    async def _update_join_rules(self, info: GroupV2) -> None:
         if not self.mxid:
             return
         new_join_rule = await self._get_new_join_rule(info.access_control.link)
         if new_join_rule:
             await self.main_intent.set_join_rule(self.mxid, new_join_rule)
 
     async def _get_join_rule(self) -> JoinRule | None:
@@ -2169,38 +2279,31 @@
         except Exception:
             self.log.warning("Failed to update bridge info", exc_info=True)
 
     # endregion
     # region Creating Matrix rooms
 
     async def update_matrix_room(self, source: u.User, info: ChatInfo) -> None:
-        if not self.is_direct and not isinstance(info, (Group, GroupV2, GroupV2ID)):
+        if not self.is_direct and not isinstance(info, GroupV2):
             raise ValueError(f"Unexpected type for updating group portal: {type(info)}")
         elif self.is_direct and not isinstance(info, (Profile, Address)):
             raise ValueError(f"Unexpected type for updating direct chat portal: {type(info)}")
         try:
             await self._update_matrix_room(source, info)
         except Exception:
             self.log.exception("Failed to update portal")
 
-    async def create_matrix_room(self, source: u.User, info: ChatInfo) -> RoomID | None:
-        if not self.is_direct and not isinstance(info, (Group, GroupV2, GroupV2ID)):
+    async def create_matrix_room(
+        self, source: u.User, info: ChatInfo | GroupV2ID
+    ) -> RoomID | None:
+        if not self.is_direct and not isinstance(info, GroupV2ID):
             raise ValueError(f"Unexpected type for creating group portal: {type(info)}")
         elif self.is_direct and not isinstance(info, (Profile, Address)):
             raise ValueError(f"Unexpected type for creating direct chat portal: {type(info)}")
-        if isinstance(info, Group) and not info.members:
-            try:
-                groups = await self.signal.list_groups(source.username)
-            except Exception as e:
-                await source.handle_auth_failure(e)
-                raise
-            info = next(
-                (g for g in groups if isinstance(g, Group) and g.group_id == info.group_id), info
-            )
-        elif isinstance(info, GroupV2ID) and not isinstance(info, GroupV2):
+        if isinstance(info, GroupV2ID) and not isinstance(info, GroupV2):
             self.log.debug(
                 f"create_matrix_room() called with {info}, fetching full info from signald"
             )
             try:
                 info = await self.signal.get_group(source.username, info.id, info.revision or -1)
             except Exception as e:
                 await source.handle_auth_failure(e)
@@ -2238,52 +2341,51 @@
                 await source.update_direct_chats({self.main_intent.mxid: [self.mxid]})
 
         await self.update_info(source, info)
 
     async def _get_power_levels(
         self,
         levels: PowerLevelStateEventContent | None = None,
-        info: ChatInfo | None = None,
+        info: ChatInfo = None,
         is_initial: bool = False,
     ) -> PowerLevelStateEventContent:
         levels = levels or PowerLevelStateEventContent()
         bot_pl = levels.get_user_level(self.az.bot_mxid)
         levels.events_default = 0
         if self.is_direct:
             levels.ban = 99
             levels.kick = 99
             levels.invite = 99
             levels.state_default = 0
             meta_edit_level = 0
         else:
-            if isinstance(info, GroupV2):
-                ac = info.access_control
-                for detail in info.member_detail + info.pending_member_detail:
-                    puppet = await p.Puppet.get_by_uuid(detail.uuid)
-                    puppet_mxid = puppet.intent_for(self).mxid
-                    current_level = levels.get_user_level(puppet_mxid)
-                    if bot_pl > current_level and bot_pl >= 50:
-                        level = current_level
-                        if puppet.is_real_user:
-                            if current_level >= 50 and detail.role == GroupMemberRole.DEFAULT:
-                                level = 0
-                            elif (
-                                current_level < 50 and detail.role == GroupMemberRole.ADMINISTRATOR
-                            ):
-                                level = 50
-                        else:
-                            level = 50 if detail.role == GroupMemberRole.ADMINISTRATOR else 0
+            ac = info.access_control
+            for detail in info.member_detail + info.pending_member_detail:
+                puppet = await p.Puppet.get_by_uuid(detail.uuid)
+                puppet_mxid = puppet.intent_for(self).mxid
+                current_level = levels.get_user_level(puppet_mxid)
+                if bot_pl > current_level and bot_pl >= 50:
+                    level = current_level
+                    user = await u.User.get_by_uuid(detail.uuid)
+                    if user:
+                        if current_level >= 50 and detail.role == GroupMemberRole.DEFAULT:
+                            level = 0
+                        elif current_level < 50 and detail.role == GroupMemberRole.ADMINISTRATOR:
+                            level = 50
                         if level == 0:
-                            levels.users.pop(puppet_mxid, None)
+                            levels.users.pop(user.mxid, None)
                         else:
-                            levels.users[puppet_mxid] = level
-                announcements = info.announcements
-            else:
-                ac = GroupAccessControl()
-                announcements = AnnouncementsMode.UNKNOWN
+                            levels.users[user.mxid] = level
+                    else:
+                        level = 50 if detail.role == GroupMemberRole.ADMINISTRATOR else 0
+                    if level == 0:
+                        levels.users.pop(puppet_mxid, None)
+                    else:
+                        levels.users[puppet_mxid] = level
+            announcements = info.announcements
             levels.ban = 50
             levels.kick = 50
             levels.invite = 50 if ac.members == AccessControlMode.ADMINISTRATOR else 0
             levels.state_default = 50
             meta_edit_level = 50 if ac.attributes == AccessControlMode.ADMINISTRATOR else 0
             if announcements == AnnouncementsMode.ENABLED:
                 levels.events_default = 50
@@ -2335,17 +2437,17 @@
                     "content": self.get_encryption_state_event_json(),
                 }
             )
             if self.is_direct:
                 invites.append(self.az.bot_mxid)
         if self.is_direct and source.uuid == self.chat_id:
             name = self.name = "Signal Note to Self"
-        elif self.encrypted or self.private_chat_portal_meta or not self.is_direct:
+        elif self.set_dm_room_metadata:
             name = self.name
-        if self.avatar_url:
+        if self.avatar_url and self.set_dm_room_metadata:
             initial_state.append(
                 {
                     "type": str(EventType.ROOM_AVATAR),
                     "content": {"url": self.avatar_url},
                 }
             )
 
@@ -2364,15 +2466,15 @@
             # TODO remove this if the spec is changed to require servers to
             #      use the power level event in initial_state
             power_level_override={"users": {self.main_intent.mxid: 9001}},
         )
         if not self.mxid:
             raise Exception("Failed to create room: no mxid returned")
         self.name_set = bool(name)
-        self.avatar_set = bool(self.avatar_url)
+        self.avatar_set = bool(self.avatar_url) and self.set_dm_room_metadata
 
         if self.encrypted and self.matrix.e2ee and self.is_direct:
             try:
                 await self.az.intent.ensure_joined(self.mxid)
             except Exception:
                 self.log.warning("Failed to add bridge bot to new private chat {self.mxid}")
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/puppet.py` & `mautrix-signal-0.4.3/mautrix_signal/puppet.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ContentURI,
     EventType,
     PowerLevelStateEventContent,
     RoomID,
     SyncToken,
     UserID,
 )
+from mautrix.util import background_task
 from mautrix.util.simple_template import SimpleTemplate
 
 from . import portal as p, signal, user as u
 from .config import Config
 from .db import Puppet as DBPuppet
 
 if TYPE_CHECKING:
@@ -54,14 +55,15 @@
 class Puppet(DBPuppet, BasePuppet):
     by_uuid: dict[UUID, Puppet] = {}
     by_number: dict[str, Puppet] = {}
     by_custom_mxid: dict[UserID, Puppet] = {}
     hs_domain: str
     mxid_template: SimpleTemplate[str]
 
+    bridge: SignalBridge
     config: Config
     signal: signal.SignalHandler
 
     default_mxid_intent: IntentAPI
     default_mxid: UserID
 
     _uuid_lock: asyncio.Lock
@@ -73,14 +75,15 @@
         number: str | None,
         name: str | None = None,
         name_quality: int = 0,
         avatar_url: ContentURI | None = None,
         avatar_hash: str | None = None,
         name_set: bool = False,
         avatar_set: bool = False,
+        contact_info_set: bool = False,
         is_registered: bool = False,
         custom_mxid: UserID | None = None,
         access_token: str | None = None,
         next_batch: SyncToken | None = None,
         base_url: URL | None = None,
     ) -> None:
         assert uuid, "UUID must be set for ghosts"
@@ -90,14 +93,15 @@
             number=number,
             name=name,
             name_quality=name_quality,
             avatar_url=avatar_url,
             avatar_hash=avatar_hash,
             name_set=name_set,
             avatar_set=avatar_set,
+            contact_info_set=contact_info_set,
             is_registered=is_registered,
             custom_mxid=custom_mxid,
             access_token=access_token,
             next_batch=next_batch,
             base_url=base_url,
         )
         self.log = self.log.getChild(str(uuid) if uuid else number)
@@ -107,14 +111,15 @@
         self.intent = self._fresh_intent()
 
         self._uuid_lock = asyncio.Lock()
         self._update_info_lock = asyncio.Lock()
 
     @classmethod
     def init_cls(cls, bridge: "SignalBridge") -> AsyncIterable[Awaitable[None]]:
+        cls.bridge = bridge
         cls.config = bridge.config
         cls.loop = bridge.loop
         cls.signal = bridge.signal
         cls.mx = bridge.matrix
         cls.az = bridge.az
         cls.hs_domain = cls.config["homeserver.domain"]
         cls.mxid_template = SimpleTemplate(
@@ -186,29 +191,59 @@
                 await prev_intent.send_state_event(room_id, EventType.ROOM_POWER_LEVELS, powers)
         except Exception:
             self.log.warning("Failed to migrate power levels", exc_info=True)
 
     async def update_info(self, info: Profile | Address, source: u.User) -> None:
         update = False
         address = info.address if isinstance(info, Profile) else info
+        number_updated = False
         if address.number and address.number != self.number:
             await self.handle_number_receive(address.number)
             update = True
+            number_updated = True
+
         self.log.debug("Updating info with %s (source: %s)", info, source.mxid)
         async with self._update_info_lock:
+            update = await self._update_contact_info(force=number_updated) or update
+
             if isinstance(info, Profile) or self.name is None:
                 update = await self._update_name(info) or update
             if isinstance(info, Profile):
                 update = await self._update_avatar(info.avatar) or update
             elif self.config["bridge.contact_list_names"] != "disallow" and self.number:
                 # Try to use a contact list avatar
                 update = await self._update_avatar(f"contact-{self.number}") or update
             if update:
                 await self.update()
-                asyncio.create_task(self._try_update_portal_meta())
+                background_task.create(self._try_update_portal_meta())
+
+    async def _update_contact_info(self, force: bool = False) -> bool:
+        if not self.bridge.homeserver_software.is_hungry:
+            return False
+
+        if self.contact_info_set and not force:
+            return False
+
+        try:
+            identifiers = [f"signal:{self.uuid}"]
+            if self.number:
+                identifiers.append(f"tel:{self.number}")
+            await self.default_mxid_intent.beeper_update_profile(
+                {
+                    "com.beeper.bridge.identifiers": identifiers,
+                    "com.beeper.bridge.remote_id": str(self.uuid),
+                    "com.beeper.bridge.service": "signal",
+                    "com.beeper.bridge.network": "signal",
+                }
+            )
+            self.contact_info_set = True
+        except Exception:
+            self.log.exception("Error updating contact info")
+            self.contact_info_set = False
+        return True
 
     @staticmethod
     def fmt_phone(number: str) -> str:
         if phonenumbers is None:
             return number
         parsed = phonenumbers.parse(number)
         fmt = phonenumbers.PhoneNumberFormat.INTERNATIONAL
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/signal.py` & `mautrix-signal-0.4.3/mautrix_signal/signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,28 +22,32 @@
 
 from mausignald import SignaldClient
 from mausignald.types import (
     Address,
     ErrorMessage,
     IncomingMessage,
     MessageData,
+    MessageResendSuccessEvent,
     OfferMessageType,
     OwnReadReceipt,
     ReceiptMessage,
     ReceiptType,
     StorageChange,
     TypingAction,
     TypingMessage,
     WebsocketConnectionStateChangeEvent,
 )
-from mautrix.types import EventID, Format, MessageType, TextMessageEventContent
+from mautrix.types import EventID, EventType, Format, MessageType, TextMessageEventContent
+from mautrix.util import background_task
 from mautrix.util.logging import TraceLogger
+from mautrix.util.message_send_checkpoint import MessageSendCheckpointStatus
 
 from . import portal as po, puppet as pu, user as u
 from .db import Message as DBMessage
+from .web.segment_analytics import track
 
 if TYPE_CHECKING:
     from .__main__ import SignalBridge
 
 # Typing notifications seem to get resent every 10 seconds and the timeout is around 15 seconds
 SIGNAL_TYPING_TIMEOUT = 15000
 
@@ -62,14 +66,15 @@
         self.error_message_events = {}
         self.add_event_handler(IncomingMessage, self.on_message)
         self.add_event_handler(ErrorMessage, self.on_error_message)
         self.add_event_handler(StorageChange, self.on_storage_change)
         self.add_event_handler(
             WebsocketConnectionStateChangeEvent, self.on_websocket_connection_state_change
         )
+        self.add_event_handler(MessageResendSuccessEvent, self.on_message_resend_success)
 
     async def on_message(self, evt: IncomingMessage) -> None:
         sender = await pu.Puppet.get_by_address(evt.source, resolve_via=evt.account)
         if not sender:
             self.log.warning(f"Didn't find puppet for incoming message {evt.source}")
             return
         user = await u.User.get_by_username(evt.account)
@@ -79,14 +84,16 @@
             await self.handle_message(user, sender, evt.data_message)
         if evt.typing_message:
             await self.handle_typing(user, sender, evt.typing_message)
         if evt.receipt_message:
             await self.handle_receipt(sender, evt.receipt_message)
         if evt.call_message:
             await self.handle_call_message(user, sender, evt)
+        if evt.decryption_error_message:
+            await self.handle_decryption_error(user, sender, evt)
         if evt.sync_message:
             if evt.sync_message.read_messages:
                 await self.handle_own_receipts(sender, evt.sync_message.read_messages)
             if evt.sync_message.sent:
                 if (
                     evt.sync_message.sent.destination
                     and not evt.sync_message.sent.destination.uuid
@@ -117,14 +124,16 @@
         else:
             self.log.debug(f"Got previously errored message {evt.timestamp} from {sender.address}")
             event_id = await event_id_future if event_id_future is not None else None
             if event_id is not None:
                 portal = await po.Portal.get_by_chat_id(sender.uuid, receiver=user.username)
                 if portal and portal.mxid:
                     await sender.intent_for(portal).redact(portal.mxid, event_id)
+                    error = {"sender": str(sender.uuid), "timestamp": str(evt.timestamp)}
+                    track(user, "$signal_inbound_error_redacted", error)
 
     async def on_error_message(self, err: ErrorMessage) -> None:
         self.log.warning(
             f"Error reading message from {err.data.sender}/{err.data.sender_device} "
             f"(timestamp: {err.data.timestamp}, content hint: {err.data.content_hint}): "
             f"{err.data.message}"
         )
@@ -157,14 +166,20 @@
             fut = self.error_message_events[error_message_event_key] = self.loop.create_future()
             event_id = None
             try:
                 event_id = await portal._send_message(
                     intent=sender.intent_for(portal),
                     content=TextMessageEventContent(body=err_text, msgtype=MessageType.NOTICE),
                 )
+                error = {
+                    "message": err_text,
+                    "sender": str(sender.uuid),
+                    "timestamp": str(err.data.timestamp),
+                }
+                track(user, "$signal_inbound_error_displayed", error)
             finally:
                 fut.set_result(event_id)
 
     async def on_storage_change(self, storage_change: StorageChange) -> None:
         self.log.info("Handling StorageChange %s", str(storage_change))
         if user := await u.User.get_by_username(storage_change.account):
             await user.sync()
@@ -172,14 +187,19 @@
     @staticmethod
     async def on_websocket_connection_state_change(
         evt: WebsocketConnectionStateChangeEvent,
     ) -> None:
         user = await u.User.get_by_username(evt.account)
         user.on_websocket_connection_state_change(evt)
 
+    @staticmethod
+    async def on_message_resend_success(evt: MessageResendSuccessEvent):
+        user = await u.User.get_by_username(evt.account)
+        await user.on_message_resend_success(evt)
+
     async def handle_message(
         self,
         user: u.User,
         sender: pu.Puppet,
         msg: MessageData,
         addr_override: Address | None = None,
     ) -> None:
@@ -193,20 +213,18 @@
         self,
         user: u.User,
         sender: pu.Puppet,
         msg: MessageData,
         addr_override: Address | None = None,
     ) -> None:
         if msg.profile_key_update:
-            asyncio.create_task(user.sync_contact(sender.address, use_cache=False))
+            background_task.create(user.sync_contact(sender.address, use_cache=False))
             return
         if msg.group_v2:
             portal = await po.Portal.get_by_chat_id(msg.group_v2.id, create=True)
-        elif msg.group:
-            portal = await po.Portal.get_by_chat_id(msg.group.group_id, create=True)
         else:
             if addr_override and not addr_override.uuid:
                 target = await pu.Puppet.get_by_address(addr_override, resolve_via=user.username)
                 if not target:
                     self.log.warning(
                         f"Didn't find puppet for recipient of incoming message {addr_override}"
                     )
@@ -233,17 +251,15 @@
         if not portal.mxid:
             if not msg.is_message and not msg.group_v2:
                 user.log.debug(
                     f"Ignoring message {msg.timestamp},"
                     " probably not bridgeable as there's no portal yet"
                 )
                 return
-            await portal.create_matrix_room(
-                user, msg.group_v2 or msg.group or addr_override or sender.address
-            )
+            await portal.create_matrix_room(user, msg.group_v2 or addr_override or sender.address)
             if not portal.mxid:
                 user.log.warning(
                     f"Failed to create room for incoming message {msg.timestamp}, dropping message"
                 )
                 return
         elif (
             msg.group_v2
@@ -263,16 +279,14 @@
             await portal.update_info(user, msg.group_v2)
         if msg.expires_in_seconds is not None and (msg.is_message or msg.is_expiration_update):
             await portal.update_expires_in_seconds(sender, msg.expires_in_seconds)
         if msg.reaction:
             await portal.handle_signal_reaction(sender, msg.reaction, msg.timestamp)
         if msg.is_message:
             await portal.handle_signal_message(user, sender, msg)
-        if msg.group and msg.group.type == "UPDATE":
-            await portal.update_info(user, msg.group)
         if msg.remote_delete:
             await portal.handle_signal_delete(sender, msg.remote_delete.target_sent_timestamp)
 
     @staticmethod
     async def handle_call_message(user: u.User, sender: pu.Puppet, msg: IncomingMessage) -> None:
         assert msg.call_message
         portal = await po.Portal.get_by_chat_id(sender.uuid, receiver=user.username, create=True)
@@ -337,37 +351,76 @@
             portal = await po.Portal.get_by_chat_id(typing.group_id)
         else:
             portal = await po.Portal.get_by_chat_id(sender.uuid, receiver=user.username)
         if not portal or not portal.mxid:
             return
         is_typing = typing.action == TypingAction.STARTED
         await sender.intent_for(portal).set_typing(
-            portal.mxid, is_typing, ignore_cache=True, timeout=SIGNAL_TYPING_TIMEOUT
+            portal.mxid, timeout=SIGNAL_TYPING_TIMEOUT if is_typing else 0
         )
 
     @staticmethod
     async def handle_receipt(sender: pu.Puppet, receipt: ReceiptMessage) -> None:
         if receipt.type != ReceiptType.READ:
             return
         messages = await DBMessage.find_by_timestamps(receipt.timestamps)
         for message in messages:
             portal = await po.Portal.get_by_mxid(message.mx_room)
             await sender.intent_for(portal).mark_read(portal.mxid, message.mxid)
 
+    async def handle_decryption_error(
+        self, user: u.User, sender: pu.Puppet, msg: IncomingMessage
+    ) -> None:
+        # These messages mean that a message resend was requested. Signald will handle it, but we
+        # need to update the checkpoints.
+        assert msg.decryption_error_message
+        my_uuid = user.address.uuid
+        timestamp = msg.decryption_error_message.timestamp
+        self.log.debug(f"Got decryption error message for {my_uuid}/{timestamp}")
+        message = await DBMessage.find_by_sender_timestamp(my_uuid, timestamp)
+        if not message:
+            self.log.warning("Couldn't find message to referenced in decryption error")
+            return
+        self.log.debug(
+            f"Got decryption error message for {message.mxid} from {sender.uuid} "
+            f"in {message.mx_room}"
+        )
+        portal = await po.Portal.get_by_mxid(message.mx_room)
+        if not portal or not portal.mxid:
+            self.log.warning("Couldn't find portal for message referenced in decryption error")
+            return
+
+        evt = await portal.main_intent.get_event(message.mx_room, message.mxid)
+        if evt.content.get("fi.mau.double_puppet_source"):
+            self.log.debug(
+                "Message requested in decryption error is double-puppeted, not sending checkpoint"
+            )
+            return
+
+        user.send_remote_checkpoint(
+            status=MessageSendCheckpointStatus.DELIVERY_FAILED,
+            event_id=message.mxid,
+            room_id=message.mx_room,
+            event_type=EventType.ROOM_MESSAGE,
+            error=f"{sender.uuid} sent a decryption error message for this message",
+        )
+
     async def start(self) -> None:
         await self.connect()
         known_usernames = set()
         async for user in u.User.all_logged_in():
             # TODO report errors to user?
             known_usernames.add(user.username)
             if await self.subscribe(user.username):
                 self.log.info(
                     f"Successfully subscribed {user.username}, running sync in background"
                 )
-                asyncio.create_task(user.sync())
+                background_task.create(user.sync())
+            else:
+                user.username = None
         if self.delete_unknown_accounts:
             self.log.debug("Checking for unknown accounts to delete")
             for account in await self.list_accounts():
                 if account.account_id not in known_usernames:
                     self.log.warning(f"Unknown account ID {account.account_id}, deleting...")
                     await self.delete_account(account.account_id)
             else:
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/user.py` & `mautrix-signal-0.4.3/mautrix_signal/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 from uuid import UUID
 import asyncio
 
 from mausignald.errors import AuthorizationFailedError, ProfileUnavailableError
 from mausignald.types import (
     Account,
     Address,
-    Group,
     GroupV2,
+    MessageResendSuccessEvent,
     Profile,
     WebsocketConnectionState,
     WebsocketConnectionStateChangeEvent,
 )
 from mautrix.appservice import AppService
 from mautrix.bridge import AutologinError, BaseUser, async_getter_lock
-from mautrix.types import RoomID, UserID
+from mautrix.types import EventType, RoomID, UserID
+from mautrix.util import background_task
 from mautrix.util.bridge_state import BridgeState, BridgeStateEvent
+from mautrix.util.message_send_checkpoint import MessageSendCheckpointStatus
 from mautrix.util.opt_prometheus import Gauge
 
 from . import portal as po, puppet as pu
 from .config import Config
-from .db import User as DBUser
+from .db import Message as DBMessage, User as DBUser
 
 if TYPE_CHECKING:
     from .__main__ import SignalBridge
 
 METRIC_CONNECTED = Gauge("bridge_connected", "Bridge users connected to Signal")
 METRIC_LOGGED_IN = Gauge("bridge_logged_in", "Bridge users logged into Signal")
 
@@ -67,30 +69,36 @@
     relay_whitelisted: bool
     is_admin: bool
     permission_level: str
 
     _sync_lock: asyncio.Lock
     _notice_room_lock: asyncio.Lock
     _connected: bool
+    _state_id: str | None
     _websocket_connection_state: BridgeStateEvent | None
-    _latest_non_transient_disconnect_state: datetime | None
+    _latest_non_transient_bridge_state: datetime | None
+
+    challenge_token: str | None
 
     def __init__(
         self,
         mxid: UserID,
         username: str | None = None,
         uuid: UUID | None = None,
         notice_room: RoomID | None = None,
     ) -> None:
         super().__init__(mxid=mxid, username=username, uuid=uuid, notice_room=notice_room)
         BaseUser.__init__(self)
         self._notice_room_lock = asyncio.Lock()
         self._sync_lock = asyncio.Lock()
         self._connected = False
+        self._state_id = self.username
         self._websocket_connection_state = None
+        self._latest_non_transient_bridge_state = None
+        self.challenge_token = None
         perms = self.config.get_permissions(mxid)
         self.relay_whitelisted, self.is_whitelisted, self.is_admin, self.permission_level = perms
 
     @classmethod
     def init_cls(cls, bridge: "SignalBridge") -> None:
         cls.bridge = bridge
         cls.config = bridge.config
@@ -128,15 +136,15 @@
         await self.bridge.signal.delete_account(username)
         self._track_metric(METRIC_LOGGED_IN, False)
         await self.push_bridge_state(BridgeStateEvent.LOGGED_OUT, remote_id=username)
 
     async def fill_bridge_state(self, state: BridgeState) -> None:
         await super().fill_bridge_state(state)
         if not state.remote_id:
-            state.remote_id = self.username
+            state.remote_id = self._state_id
         if self.address:
             puppet = await self.get_puppet()
             state.remote_name = puppet.name or self.username
 
     async def get_bridge_states(self) -> list[BridgeState]:
         if not self.username:
             return []
@@ -145,34 +153,41 @@
             state.state_event = BridgeStateEvent.CONNECTED
         else:
             state.state_event = BridgeStateEvent.TRANSIENT_DISCONNECT
         return [state]
 
     async def handle_auth_failure(self, e: Exception) -> None:
         if isinstance(e, AuthorizationFailedError):
+            self.username = None
             await self.push_bridge_state(BridgeStateEvent.BAD_CREDENTIALS, error=str(e))
 
     async def get_puppet(self) -> pu.Puppet | None:
         if not self.address:
             return None
         return await pu.Puppet.get_by_address(self.address)
 
     async def get_portal_with(self, puppet: pu.Puppet, create: bool = True) -> po.Portal | None:
         if not self.username:
             return None
         return await po.Portal.get_by_chat_id(puppet.uuid, receiver=self.username, create=create)
 
     async def on_signin(self, account: Account) -> None:
         self.username = account.account_id
+        self._state_id = account.account_id
         self.uuid = account.address.uuid
         self._add_to_cache()
         await self.update()
-        await self.bridge.signal.subscribe(self.username)
-        asyncio.create_task(self.sync())
-        self._track_metric(METRIC_LOGGED_IN, True)
+        self.log.debug(f"Subscribing to {self.username} / {self.uuid}")
+        if await self.bridge.signal.subscribe(self.username):
+            background_task.create(self.sync(is_startup=True))
+            self._track_metric(METRIC_LOGGED_IN, True)
+            self.log.debug("Successfully subscribed")
+        else:
+            self.log.warning("Failed to subscribe")
+            self.username = None
 
     def on_websocket_connection_state_change(
         self, evt: WebsocketConnectionStateChangeEvent
     ) -> None:
         if evt.state == WebsocketConnectionState.CONNECTED:
             self.log.info(f"Connected to Signal (ws: {evt.socket})")
             self._track_metric(METRIC_CONNECTED, True)
@@ -206,52 +221,78 @@
             WebsocketConnectionState.FAILED: BridgeStateEvent.TRANSIENT_DISCONNECT,
         }.get(evt.state)
         if bridge_state is None:
             self.log.info(f"Websocket state {evt.state} seen, not reporting new bridge state")
             return
 
         now = datetime.now()
-        if bridge_state == BridgeStateEvent.TRANSIENT_DISCONNECT:
+        if bridge_state in (BridgeStateEvent.TRANSIENT_DISCONNECT, BridgeStateEvent.CONNECTING):
+            self.log.debug(
+                f"New bridge state {bridge_state} is likely transient. Waiting 15 seconds to send."
+            )
+
+            async def wait_report_bridge_state():
+                # Wait for 15 seconds (that should be enough for the bridge to get connected)
+                # before sending a TRANSIENT_DISCONNECT/CONNECTING.
+                await sleep(15)
+                if (
+                    self._latest_non_transient_bridge_state
+                    and now > self._latest_non_transient_bridge_state
+                ):
+                    background_task.create(self.push_bridge_state(bridge_state))
+
+                self._websocket_connection_state = bridge_state
 
-            async def wait_report_transient_disconnect():
-                # Wait for 10 seconds (that should be enough for the bridge to get connected)
-                # before sending a TRANSIENT_DISCONNECT.
-                # self._latest_non_transient_disconnect_state will only be None if the bridge is
-                # still starting.
-                if self._latest_non_transient_disconnect_state is None:
-                    await sleep(15)
-                    if self._latest_non_transient_disconnect_state is None:
-                        asyncio.create_task(self.push_bridge_state(bridge_state))
-
-                # Wait for another minute. If the bridge stays in TRANSIENT_DISCONNECT for that
-                # long, something terrible has happened (signald failed to restart, the internet
-                # broke, etc.)
+                # Wait for another minute. If the bridge stays in TRANSIENT_DISCONNECT/CONNECTING
+                # for that long, something terrible has happened (signald failed to restart, the
+                # internet broke, etc.)
                 await sleep(60)
                 if (
-                    self._latest_non_transient_disconnect_state
-                    and now > self._latest_non_transient_disconnect_state
+                    self._latest_non_transient_bridge_state
+                    and now > self._latest_non_transient_bridge_state
                 ):
-                    asyncio.create_task(
+                    background_task.create(
                         self.push_bridge_state(
                             BridgeStateEvent.UNKNOWN_ERROR,
                             message="Failed to restore connection to Signal",
                         )
                     )
+                    self._websocket_connection_state = BridgeStateEvent.UNKNOWN_ERROR
                 else:
                     self.log.info(
-                        "New state since last TRANSIENT_DISCONNECT push, "
+                        f"New state since last {bridge_state} push, "
                         "not transitioning to UNKNOWN_ERROR."
                     )
 
-            asyncio.create_task(wait_report_transient_disconnect())
+            background_task.create(wait_report_bridge_state())
+        elif self._websocket_connection_state == bridge_state:
+            self.log.info("Websocket state unchanged, not reporting new bridge state")
+            self._latest_non_transient_bridge_state = now
         else:
-            asyncio.create_task(self.push_bridge_state(bridge_state))
-            self._latest_non_transient_disconnect_state = now
-
-        self._websocket_connection_state = bridge_state
+            if bridge_state == BridgeStateEvent.BAD_CREDENTIALS:
+                self.username = None
+            background_task.create(self.push_bridge_state(bridge_state))
+            self._latest_non_transient_bridge_state = now
+            self._websocket_connection_state = bridge_state
+
+    async def on_message_resend_success(self, evt: MessageResendSuccessEvent):
+        # These messages mean we need to resend the message to that user.
+        my_uuid = self.address.uuid
+        self.log.debug(f"Successfully resent message {my_uuid}/{evt.timestamp}")
+        message = await DBMessage.find_by_sender_timestamp(my_uuid, evt.timestamp)
+        if not message:
+            self.log.warning("Couldn't find message that was resent")
+            return
+        self.log.debug(f"Successfully resent {message.mxid} in {message.mx_room}")
+        self.send_remote_checkpoint(
+            status=MessageSendCheckpointStatus.SUCCESS,
+            event_id=message.mxid,
+            room_id=message.mx_room,
+            event_type=EventType.ROOM_MESSAGE,
+        )
 
     async def _sync_puppet(self) -> None:
         puppet = await self.get_puppet()
         if not puppet:
             self.log.warning(f"Didn't find puppet for own address {self.address}")
             return
         if puppet.uuid and not self.uuid:
@@ -260,31 +301,31 @@
         if puppet.custom_mxid != self.mxid and puppet.can_auto_login(self.mxid):
             self.log.info("Automatically enabling custom puppet")
             try:
                 await puppet.switch_mxid(access_token="auto", mxid=self.mxid)
             except AutologinError as e:
                 self.log.warning(f"Failed to enable custom puppet: {e}")
 
-    async def sync(self) -> None:
+    async def sync(self, is_startup: bool = False) -> None:
         await self.sync_puppet()
-        await self.sync_contacts()
+        await self.sync_contacts(is_startup=is_startup)
         await self.sync_groups()
         self.log.debug("Sync complete")
 
     async def sync_puppet(self) -> None:
         try:
             async with self._sync_lock:
                 await self._sync_puppet()
         except Exception:
             self.log.exception("Error while syncing own puppet")
 
-    async def sync_contacts(self) -> None:
+    async def sync_contacts(self, is_startup: bool = False) -> None:
         try:
             async with self._sync_lock:
-                await self._sync_contacts()
+                await self._sync_contacts(is_startup)
         except Exception as e:
             self.log.exception("Error while syncing contacts")
             await self.handle_auth_failure(e)
 
     async def sync_groups(self) -> None:
         try:
             async with self._sync_lock:
@@ -330,17 +371,36 @@
         self.log.trace("Syncing group %s", group.id)
         portal = await po.Portal.get_by_chat_id(group.id, create=True)
         if create_portals:
             await portal.create_matrix_room(self, group)
         elif portal.mxid:
             await portal.update_matrix_room(self, group)
 
-    async def _sync_contacts(self) -> None:
+    async def _hacky_duplicate_contact_check(
+        self, contacts: list[Profile], is_startup: bool
+    ) -> None:
+        name_map: dict[str, list[Profile]] = {}
+        for contact in contacts:
+            if contact.contact_name:
+                name_map.setdefault(contact.contact_name, []).append(contact)
+        duplicates = {name: profiles for name, profiles in name_map.items() if len(profiles) > 1}
+        if duplicates:
+            self.log.warning(f"Found duplicate contact names, potential name mixup: {duplicates}")
+            if is_startup:
+                self.log.debug("Requesting contact sync to resolve potential name mixup")
+                await self.bridge.signal.request_sync(self.username)
+        else:
+            self.log.debug("No duplicate contact names found")
+
+    async def _sync_contacts(self, is_startup: bool) -> None:
         create_contact_portal = self.config["bridge.autocreate_contact_portal"]
-        for contact in await self.bridge.signal.list_contacts(self.username):
+        contacts = await self.bridge.signal.list_contacts(self.username)
+        if self.config["bridge.hacky_contact_name_mixup_detection"]:
+            await self._hacky_duplicate_contact_check(contacts, is_startup=is_startup)
+        for contact in contacts:
             try:
                 await self.sync_contact(contact, create_contact_portal)
             except Exception:
                 self.log.exception(f"Failed to sync contact {contact.address}")
 
     async def _sync_groups(self) -> None:
         create_group_portal = self.config["bridge.autocreate_group_portal"]
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/util/color_log.py` & `mautrix-signal-0.4.3/mautrix_signal/util/color_log.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/util/normalize_number.py` & `mautrix-signal-0.4.3/mautrix_signal/util/normalize_number.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/util/user_has_power_level.py` & `mautrix-signal-0.4.3/mautrix_signal/util/user_has_power_level.py`

 * *Files identical despite different names*

### Comparing `mautrix-signal-0.4.2/mautrix_signal/web/provisioning_api.py` & `mautrix-signal-0.4.3/mautrix_signal/web/provisioning_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,26 @@
 
 class ProvisioningAPI:
     log: TraceLogger = logging.getLogger("mau.web.provisioning")
     app: web.Application
     bridge: "SignalBridge"
 
     def __init__(
-        self, bridge: "SignalBridge", shared_secret: str, segment_key: str | None
+        self,
+        bridge: "SignalBridge",
+        shared_secret: str,
+        segment_key: str | None,
+        segment_user_id: str | None,
     ) -> None:
         self.bridge = bridge
         self.app = web.Application()
         self.shared_secret = shared_secret
 
         if segment_key:
-            init_segment(segment_key)
+            init_segment(segment_key, segment_user_id)
 
         # Whoami
         self.app.router.add_get("/v1/api/whoami", self.status)
         self.app.router.add_get("/v2/whoami", self.status)
 
         # Logout
         self.app.router.add_options("/v1/api/logout", self.login_options)
@@ -77,14 +81,15 @@
         self.app.router.add_options("/v2/link/wait/account", self.login_options)
         self.app.router.add_post("/v2/link/new", self.link_new)
         self.app.router.add_post("/v2/link/wait/scan", self.link_wait_for_scan)
         self.app.router.add_post("/v2/link/wait/account", self.link_wait_for_account)
 
         # Start new chat API
         self.app.router.add_get("/v2/contacts", self.list_contacts)
+        self.app.router.add_get("/v2/sync", self.request_sync)
         self.app.router.add_get("/v2/resolve_identifier/{number}", self.resolve_identifier)
         self.app.router.add_post("/v2/pm/{number}", self.start_pm)
 
     @property
     def _acao_headers(self) -> dict[str, str]:
         return {
             "Access-Control-Allow-Origin": "*",
@@ -351,17 +356,20 @@
             raise web.HTTPBadRequest(text=json.dumps(error), headers=self._headers)
 
     # endregion
 
     # region Logout
 
     async def logout(self, request: web.Request) -> web.Response:
-        user = await self.check_token_and_logged_in(request)
-        await user.logout()
-        return web.json_response({}, headers=self._acao_headers)
+        try:
+            user = await self.check_token_and_logged_in(request)
+            await user.logout()
+            return web.json_response({}, headers=self._acao_headers)
+        except web.HTTPNotFound:
+            return web.json_response({"error": "You're not logged in"}, headers=self._acao_headers)
 
     # endregion
 
     # region Start new chat API
 
     async def list_contacts(self, request: web.Request) -> web.Response:
         user = await self.check_token_and_logged_in(request)
@@ -384,14 +392,19 @@
                 c.address.number: await transform(c)
                 for c in contacts
                 if c.address and c.address.number
             },
             headers=self._acao_headers,
         )
 
+    async def request_sync(self, request: web.Request) -> web.Response:
+        user = await self.check_token_and_logged_in(request)
+        await self.bridge.signal.request_sync(user.username)
+        return web.json_response({}, headers=self._acao_headers)
+
     async def _resolve_identifier(self, number: str, user: u.User) -> pu.Puppet:
         try:
             number = normalize_number(number)
         except Exception as e:
             raise web.HTTPBadRequest(text=json.dumps({"error": str(e)}), headers=self._headers)
 
         try:
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal/web/segment_analytics.py` & `mautrix-signal-0.4.3/mautrix_signal/web/segment_analytics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from __future__ import annotations
 
-import asyncio
 import logging
 
 from yarl import URL
 import aiohttp
 
+from mautrix.util import background_task
+
 from .. import user as u
 
 log = logging.getLogger("mau.web.public.analytics")
 segment_url: URL = URL("https://api.segment.io/v1/track")
 http: aiohttp.ClientSession | None = None
 segment_key: str | None = None
+segment_user_id: str | None = None
 
 
 async def _track(user: u.User, event: str, properties: dict) -> None:
     await http.post(
         segment_url,
         json={
-            "userId": user.mxid,
+            "userId": segment_user_id or user.mxid,
             "event": event,
             "properties": {"bridge": "signal", **properties},
         },
         auth=aiohttp.BasicAuth(login=segment_key, encoding="utf-8"),
     )
     log.debug(f"Tracked {event}")
 
 
 def track(user: u.User, event: str, properties: dict | None = None):
     if segment_key:
-        asyncio.create_task(_track(user, event, properties or {}))
+        background_task.create(_track(user, event, properties or {}))
 
 
-def init(key):
-    global segment_key, http
+def init(key, user_id: str | None = None):
+    global segment_key, segment_user_id, http
     segment_key = key
+    segment_user_id = user_id
     http = aiohttp.ClientSession()
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal.egg-info/PKG-INFO` & `mautrix-signal-0.4.3/mautrix_signal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mautrix-signal
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Matrix-Signal puppeting bridge.
 Home-page: https://github.com/mautrix/signal
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/mautrix/signal/blob/master/CHANGELOG.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -49,9 +47,7 @@
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/signal/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#signal:maunium.net`](https://matrix.to/#/#signal:maunium.net)
-
-
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal.egg-info/SOURCES.txt` & `mautrix-signal-0.4.3/mautrix_signal.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 mautrix_signal.egg-info/requires.txt
 mautrix_signal.egg-info/top_level.txt
 mautrix_signal/commands/__init__.py
 mautrix_signal/commands/auth.py
 mautrix_signal/commands/conn.py
 mautrix_signal/commands/signal.py
 mautrix_signal/commands/typehint.py
+mautrix_signal/commands/util.py
 mautrix_signal/db/__init__.py
 mautrix_signal/db/disappearing_message.py
 mautrix_signal/db/message.py
 mautrix_signal/db/portal.py
 mautrix_signal/db/puppet.py
 mautrix_signal/db/reaction.py
 mautrix_signal/db/user.py
@@ -50,14 +51,15 @@
 mautrix_signal/db/upgrade/v05_puppet_avatar_info.py
 mautrix_signal/db/upgrade/v06_portal_revision.py
 mautrix_signal/db/upgrade/v07_portal_relay_user.py
 mautrix_signal/db/upgrade/v08_disappearing_messages.py
 mautrix_signal/db/upgrade/v09_group_topic.py
 mautrix_signal/db/upgrade/v10_puppet_name_quality.py
 mautrix_signal/db/upgrade/v11_drop_number_support.py
+mautrix_signal/db/upgrade/v12_add_contact_info_to_puppet.py
 mautrix_signal/util/__init__.py
 mautrix_signal/util/color_log.py
 mautrix_signal/util/normalize_number.py
 mautrix_signal/util/user_has_power_level.py
 mautrix_signal/web/__init__.py
 mautrix_signal/web/provisioning_api.py
 mautrix_signal/web/segment_analytics.py
```

### Comparing `mautrix-signal-0.4.2/mautrix_signal.egg-info/requires.txt` & `mautrix-signal-0.4.3/mautrix_signal.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 aiohttp<4,>=3
 asyncpg<0.28,>=0.20
 attrs>=19.1
 commonmark<0.10,>=0.8
-mautrix<0.19,>=0.18.6
+mautrix<0.20,>=0.19.14
 python-magic<0.5,>=0.4
 ruamel.yaml<0.18,>=0.15.35
 yarl<2,>=1
 
 [all]
 Pillow<10,>=4
-aiosqlite<0.18,>=0.16
+aiosqlite<0.20,>=0.16
 phonenumbers<9,>=8
-prometheus_client<0.16,>=0.6
+prometheus_client<0.17,>=0.6
 pycryptodome<4,>=3
 python-olm<4,>=3
 qrcode<8,>=6
 signalstickers-client<4,>=3
 unpaddedbase64<3,>=1
 
 [e2be]
@@ -23,18 +23,18 @@
 python-olm<4,>=3
 unpaddedbase64<3,>=1
 
 [formattednumbers]
 phonenumbers<9,>=8
 
 [metrics]
-prometheus_client<0.16,>=0.6
+prometheus_client<0.17,>=0.6
 
 [qrlink]
 Pillow<10,>=4
 qrcode<8,>=6
 
 [sqlite]
-aiosqlite<0.18,>=0.16
+aiosqlite<0.20,>=0.16
 
 [stickers]
 signalstickers-client<4,>=3
```

### Comparing `mautrix-signal-0.4.2/setup.py` & `mautrix-signal-0.4.3/setup.py`

 * *Files identical despite different names*

