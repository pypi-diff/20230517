# Comparing `tmp/yalexs-1.4.3.tar.gz` & `tmp/yalexs-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.4.3.tar", last modified: Wed May 17 17:48:55 2023, max compression
+gzip compressed data, was "yalexs-1.4.4.tar", last modified: Wed May 17 18:55:19 2023, max compression
```

## Comparing `yalexs-1.4.3.tar` & `yalexs-1.4.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.434891 yalexs-1.4.3/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.420162 yalexs-1.4.3/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.422808 yalexs-1.4.3/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.3/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.3/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.3/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.3/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 17:48:55.434982 yalexs-1.4.3/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.3/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.3/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.3/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.3/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.3/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.4.3/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 17:48:55.435291 yalexs-1.4.3/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 17:48:40.000000 yalexs-1.4.3/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.424701 yalexs-1.4.3/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.430817 yalexs-1.4.3/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.3/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.3/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    42239 2023-05-17 15:01:17.000000 yalexs-1.4.3/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.3/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-05-17 04:41:53.000000 yalexs-1.4.3/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.3/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.3/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.433867 yalexs-1.4.3/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 17:48:40.000000 yalexs-1.4.3/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 17:35:49.000000 yalexs-1.4.3/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9931 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14480 2023-05-17 17:48:35.000000 yalexs-1.4.3/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    11408 2023-05-17 17:48:35.000000 yalexs-1.4.3/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 17:48:35.000000 yalexs-1.4.3/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.3/yalexs/authenticator_common.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.434754 yalexs-1.4.3/yalexs/backports/
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/backports/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/backports/enum.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)      489 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      717 2023-05-17 15:01:17.000000 yalexs-1.4.3/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.3/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-05-17 04:41:53.000000 yalexs-1.4.3/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.3/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.434547 yalexs-1.4.3/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.359963 yalexs-1.4.4/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.345369 yalexs-1.4.4/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.348039 yalexs-1.4.4/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.4/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.4/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.4/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.4/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 18:55:19.360039 yalexs-1.4.4/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.4/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.4/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.4/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.4/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.4/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.4.4/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 18:55:19.360323 yalexs-1.4.4/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 18:54:46.000000 yalexs-1.4.4/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.349897 yalexs-1.4.4/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.356003 yalexs-1.4.4/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.4/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.4/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    42239 2023-05-17 15:01:17.000000 yalexs-1.4.4/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.4/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.4/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-05-17 04:41:53.000000 yalexs-1.4.4/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.4/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.4/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.359027 yalexs-1.4.4/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 18:54:46.000000 yalexs-1.4.4/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 17:35:49.000000 yalexs-1.4.4/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.4.4/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14528 2023-05-17 18:54:43.000000 yalexs-1.4.4/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11611 2023-05-17 18:54:43.000000 yalexs-1.4.4/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.4/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.4.4/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.4/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.359838 yalexs-1.4.4/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.4/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.4/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.4/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      593 2023-05-17 18:54:43.000000 yalexs-1.4.4/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.4/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.4/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      717 2023-05-17 15:01:17.000000 yalexs-1.4.4/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.4/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.4/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.4/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-05-17 04:41:53.000000 yalexs-1.4.4/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.4.4/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.4/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.4/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 18:55:19.359635 yalexs-1.4.4/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 18:55:19.000000 yalexs-1.4.4/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 18:55:19.000000 yalexs-1.4.4/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 18:55:19.000000 yalexs-1.4.4/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 18:55:19.000000 yalexs-1.4.4/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 18:55:19.000000 yalexs-1.4.4/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.4.3/.github/workflows/ci.yaml` & `yalexs-1.4.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/.gitignore` & `yalexs-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/LICENSE` & `yalexs-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/PKG-INFO` & `yalexs-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.3/README.md` & `yalexs-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/known_activities.md` & `yalexs-1.4.4/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/pylintrc` & `yalexs-1.4.4/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/setup.cfg` & `yalexs-1.4.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.3
+current_version = 1.4.4
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.4.3/setup.py` & `yalexs-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.4.3",
+    version="1.4.4",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-1.4.3/tests/fixtures/auto_relock_activity.json` & `yalexs-1.4.4/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.4.4/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.4.4/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/door_closed_activity.json` & `yalexs-1.4.4/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.4.4/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.4.4/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/door_open_activity.json` & `yalexs-1.4.4/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.4.4/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.4.4/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.4.4/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.4.4/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.4.4/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.4.4/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.4.4/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbell.json` & `yalexs-1.4.4/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.4.4/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.4.4/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_doorbells.json` & `yalexs-1.4.4/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_house_activities.json` & `yalexs-1.4.4/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.4.4/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.4.4/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock.offline.json` & `yalexs-1.4.4/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock.online.json` & `yalexs-1.4.4/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.4.4/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.4.4/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.4.4/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/get_pins.json` & `yalexs-1.4.4/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.4.4/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/lock.json` & `yalexs-1.4.4/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/lock_activity.json` & `yalexs-1.4.4/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.4.4/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/remote_lock_activity.json` & `yalexs-1.4.4/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.4.4/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/unlock.json` & `yalexs-1.4.4/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/unlock_activity.json` & `yalexs-1.4.4/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.4.4/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_activity.py` & `yalexs-1.4.4/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_api.py` & `yalexs-1.4.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_api_async.py` & `yalexs-1.4.4/tests/test_api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_authenticator.py` & `yalexs-1.4.4/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_authenticator_async.py` & `yalexs-1.4.4/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_pubnub_activity.py` & `yalexs-1.4.4/tests/test_pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tests/test_util.py` & `yalexs-1.4.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/tox.ini` & `yalexs-1.4.4/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/activity.py` & `yalexs-1.4.4/yalexs/activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/api.py` & `yalexs-1.4.4/yalexs/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,17 @@
         del api_dict["method"]
         if access_token:
             del api_dict["access_token"]
 
         payload = api_dict.get("params") or api_dict.get("json")
 
         if "headers" not in api_dict:
-            api_dict["headers"] = _api_headers(access_token=access_token)
+            api_dict["headers"] = _api_headers(
+                access_token=access_token, brand=self.brand
+            )
 
         if "version" in api_dict:
             api_dict["headers"][HEADER_ACCEPT_VERSION] = api_dict["version"]
             del api_dict["version"]
 
         if "timeout" not in api_dict:
             api_dict["timeout"] = self._timeout
```

### Comparing `yalexs-1.4.3/yalexs/api_async.py` & `yalexs-1.4.4/yalexs/api_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,17 @@
         del api_dict["method"]
         if access_token:
             del api_dict["access_token"]
 
         payload = api_dict.get("params") or api_dict.get("json")
 
         if "headers" not in api_dict:
-            api_dict["headers"] = _api_headers(access_token=access_token)
+            api_dict["headers"] = _api_headers(
+                access_token=access_token, brand=self.brand
+            )
 
         if "version" in api_dict:
             api_dict["headers"][HEADER_ACCEPT_VERSION] = api_dict["version"]
             del api_dict["version"]
 
         if "timeout" not in api_dict:
             api_dict["timeout"] = self._timeout
```

### Comparing `yalexs-1.4.3/yalexs/api_common.py` & `yalexs-1.4.4/yalexs/api_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,32 @@
     DoorbellDingActivity,
     DoorbellImageCaptureActivity,
     DoorbellMotionActivity,
     DoorbellViewActivity,
     DoorOperationActivity,
     LockOperationActivity,
 )
-from .const import BASE_URLS, Brand
+from .const import BASE_URLS, BRANDING, Brand
 from .doorbell import Doorbell
 from .lock import Lock, LockDoorStatus, determine_door_state, door_state_to_string
 
 API_RETRY_TIME = 2.5
 API_RETRY_ATTEMPTS = 10
 
 HEADER_ACCEPT_VERSION = "Accept-Version"
 HEADER_AUGUST_ACCESS_TOKEN = "x-august-access-token"  # nosec
 HEADER_AUGUST_API_KEY = "x-august-api-key"
 HEADER_AUGUST_BRANDING = "x-august-branding"
 HEADER_AUGUST_COUNTRY = "x-august-country"
 HEADER_CONTENT_TYPE = "Content-Type"
 HEADER_USER_AGENT = "User-Agent"
 
-HEADER_VALUE_API_KEY = "7cab4bbd-2693-4fc1-b99b-dec0fb20f9d4"
+
+HEADER_VALUE_API_KEY_OLD = "7cab4bbd-2693-4fc1-b99b-dec0fb20f9d4"
+HEADER_VALUE_API_KEY = "d9984f29-07a6-816e-e1c9-44ec9d1be431"
 HEADER_VALUE_CONTENT_TYPE = "application/json; charset=UTF-8"
 HEADER_VALUE_USER_AGENT = "August/Luna-22.17.0 (Android; SDK 31; gphone64_arm64)"
 HEADER_VALUE_ACCEPT_VERSION = "0.0.1"
 HEADER_VALUE_AUGUST_BRANDING = "august"
 HEADER_VALUE_AUGUST_COUNTRY = "US"
 
 
@@ -83,24 +85,27 @@
     DoorbellViewActivity,
     LockOperationActivity,
     DoorOperationActivity,
     BridgeOperationActivity,
 ]
 
 
-def _api_headers(access_token=None):
+def _api_headers(
+    access_token: Optional[str] = None, brand: Optional[Brand] = None
+) -> Dict[str, str]:
     headers = {
         HEADER_ACCEPT_VERSION: HEADER_VALUE_ACCEPT_VERSION,
         HEADER_AUGUST_API_KEY: HEADER_VALUE_API_KEY,
         HEADER_CONTENT_TYPE: HEADER_VALUE_CONTENT_TYPE,
         HEADER_USER_AGENT: HEADER_VALUE_USER_AGENT,
-        HEADER_AUGUST_BRANDING: HEADER_VALUE_AUGUST_BRANDING,
         HEADER_AUGUST_COUNTRY: HEADER_VALUE_AUGUST_COUNTRY,
     }
 
+    headers[HEADER_AUGUST_BRANDING] = BRANDING.get(brand, HEADER_VALUE_AUGUST_BRANDING)
+
     if access_token:
         headers[HEADER_AUGUST_ACCESS_TOKEN] = access_token
 
     return headers
 
 
 def _convert_lock_result_to_activities(
@@ -190,14 +195,15 @@
 
 class ApiCommon:
     """Api dict shared between async and sync."""
 
     def __init__(self, brand: Brand) -> None:
         """Init."""
         self._base_url = BASE_URLS[brand]
+        self.brand = brand
 
     def get_brand_url(self, url_str: str) -> str:
         """Get url."""
         return self._base_url + url_str
 
     def _build_get_session_request(self, install_id, identifier, password):
         return {
```

### Comparing `yalexs-1.4.3/yalexs/authenticator.py` & `yalexs-1.4.4/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/authenticator_async.py` & `yalexs-1.4.4/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/authenticator_common.py` & `yalexs-1.4.4/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/backports/enum.py` & `yalexs-1.4.4/yalexs/backports/enum.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/bridge.py` & `yalexs-1.4.4/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/device.py` & `yalexs-1.4.4/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/doorbell.py` & `yalexs-1.4.4/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/exceptions.py` & `yalexs-1.4.4/yalexs/exceptions.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/keypad.py` & `yalexs-1.4.4/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/lock.py` & `yalexs-1.4.4/yalexs/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/pin.py` & `yalexs-1.4.4/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/pubnub_activity.py` & `yalexs-1.4.4/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/pubnub_async.py` & `yalexs-1.4.4/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/users.py` & `yalexs-1.4.4/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs/util.py` & `yalexs-1.4.4/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.3/yalexs.egg-info/PKG-INFO` & `yalexs-1.4.4/yalexs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.3/yalexs.egg-info/SOURCES.txt` & `yalexs-1.4.4/yalexs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

