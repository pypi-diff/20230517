# Comparing `tmp/yalexs-1.4.2.tar.gz` & `tmp/yalexs-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.4.2.tar", last modified: Wed May 17 16:20:58 2023, max compression
+gzip compressed data, was "yalexs-1.4.3.tar", last modified: Wed May 17 17:48:55 2023, max compression
```

## Comparing `yalexs-1.4.2.tar` & `yalexs-1.4.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.084012 yalexs-1.4.2/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.071039 yalexs-1.4.2/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.073579 yalexs-1.4.2/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.2/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.2/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.2/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.2/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 16:20:58.084096 yalexs-1.4.2/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.2/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.2/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.2/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.2/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.2/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.4.2/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 16:20:58.084385 yalexs-1.4.2/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 16:20:36.000000 yalexs-1.4.2/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.075319 yalexs-1.4.2/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.081311 yalexs-1.4.2/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.2/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.2/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    42239 2023-05-17 15:01:17.000000 yalexs-1.4.2/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.2/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.2/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-05-17 04:41:53.000000 yalexs-1.4.2/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.2/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.2/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.083259 yalexs-1.4.2/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 16:20:36.000000 yalexs-1.4.2/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9931 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12989 2023-05-17 15:01:17.000000 yalexs-1.4.2/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10895 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5235 2023-05-17 16:20:33.000000 yalexs-1.4.2/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.2/yalexs/authenticator_common.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.083902 yalexs-1.4.2/yalexs/backports/
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/backports/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/backports/enum.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.2/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)      489 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.2/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.2/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      717 2023-05-17 15:01:17.000000 yalexs-1.4.2/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.2/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.2/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.2/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-05-17 04:41:53.000000 yalexs-1.4.2/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.4.2/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.2/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.2/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 16:20:58.083733 yalexs-1.4.2/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 16:20:57.000000 yalexs-1.4.2/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 16:20:58.000000 yalexs-1.4.2/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 16:20:57.000000 yalexs-1.4.2/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 16:20:57.000000 yalexs-1.4.2/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 16:20:57.000000 yalexs-1.4.2/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.434891 yalexs-1.4.3/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.420162 yalexs-1.4.3/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.422808 yalexs-1.4.3/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.3/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.3/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.3/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.3/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 17:48:55.434982 yalexs-1.4.3/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.3/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.3/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.3/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.3/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.3/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.4.3/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 17:48:55.435291 yalexs-1.4.3/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 17:48:40.000000 yalexs-1.4.3/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.424701 yalexs-1.4.3/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.430817 yalexs-1.4.3/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.3/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.3/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    42239 2023-05-17 15:01:17.000000 yalexs-1.4.3/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.3/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.3/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-05-17 04:41:53.000000 yalexs-1.4.3/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.3/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.3/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.433867 yalexs-1.4.3/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 17:48:40.000000 yalexs-1.4.3/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 17:35:49.000000 yalexs-1.4.3/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9931 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14480 2023-05-17 17:48:35.000000 yalexs-1.4.3/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11408 2023-05-17 17:48:35.000000 yalexs-1.4.3/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 17:48:35.000000 yalexs-1.4.3/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.3/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.434754 yalexs-1.4.3/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      489 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.3/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      717 2023-05-17 15:01:17.000000 yalexs-1.4.3/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.3/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-05-17 04:41:53.000000 yalexs-1.4.3/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.3/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.3/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 17:48:55.434547 yalexs-1.4.3/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 17:48:55.000000 yalexs-1.4.3/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.4.2/.github/workflows/ci.yaml` & `yalexs-1.4.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/.gitignore` & `yalexs-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/LICENSE` & `yalexs-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/PKG-INFO` & `yalexs-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.2/README.md` & `yalexs-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/known_activities.md` & `yalexs-1.4.3/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/pylintrc` & `yalexs-1.4.3/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/setup.cfg` & `yalexs-1.4.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.2
+current_version = 1.4.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.4.2/setup.py` & `yalexs-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.4.2",
+    version="1.4.3",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-1.4.2/tests/fixtures/auto_relock_activity.json` & `yalexs-1.4.3/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.4.3/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.4.3/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/door_closed_activity.json` & `yalexs-1.4.3/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.4.3/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/door_open_activity.json` & `yalexs-1.4.3/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.4.3/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.4.3/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.4.3/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.4.3/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbell.json` & `yalexs-1.4.3/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.4.3/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.4.3/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_doorbells.json` & `yalexs-1.4.3/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_house_activities.json` & `yalexs-1.4.3/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.4.3/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.4.3/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock.offline.json` & `yalexs-1.4.3/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock.online.json` & `yalexs-1.4.3/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.4.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.4.3/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/get_pins.json` & `yalexs-1.4.3/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.4.3/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/lock.json` & `yalexs-1.4.3/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/lock_activity.json` & `yalexs-1.4.3/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.4.3/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/remote_lock_activity.json` & `yalexs-1.4.3/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.4.3/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/unlock.json` & `yalexs-1.4.3/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/unlock_activity.json` & `yalexs-1.4.3/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.4.3/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_activity.py` & `yalexs-1.4.3/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_api.py` & `yalexs-1.4.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_api_async.py` & `yalexs-1.4.3/tests/test_api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_authenticator.py` & `yalexs-1.4.3/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_authenticator_async.py` & `yalexs-1.4.3/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_pubnub_activity.py` & `yalexs-1.4.3/tests/test_pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tests/test_util.py` & `yalexs-1.4.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/tox.ini` & `yalexs-1.4.3/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/activity.py` & `yalexs-1.4.3/yalexs/activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/api.py` & `yalexs-1.4.3/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/api_async.py` & `yalexs-1.4.3/yalexs/api_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Api calls for sync."""
 
 import asyncio
 from http import HTTPStatus
 import logging
+from typing import Any, Dict, List, Tuple, Union
 
 from aiohttp import (
     ClientResponse,
     ClientResponseError,
     ClientSession,
     ServerDisconnectedError,
 )
@@ -18,30 +19,48 @@
     API_RETRY_TIME,
     API_STATUS_ASYNC_URL,
     API_UNLOCK_ASYNC_URL,
     API_UNLOCK_URL,
     HEADER_ACCEPT_VERSION,
     HEADER_AUGUST_ACCESS_TOKEN,
     HYPER_BRIDGE_PARAM,
+    ActivityType,
     ApiCommon,
     _api_headers,
     _convert_lock_result_to_activities,
     _process_activity_json,
     _process_doorbells_json,
     _process_locks_json,
 )
 from .const import DEFAULT_BRAND
-from .doorbell import DoorbellDetail
+from .doorbell import Doorbell, DoorbellDetail
 from .exceptions import AugustApiAIOHTTPError
-from .lock import LockDetail, determine_door_state, determine_lock_status
+from .lock import (
+    Lock,
+    LockDetail,
+    LockDoorStatus,
+    LockStatus,
+    determine_door_state,
+    determine_lock_status,
+)
 from .pin import Pin
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def _obscure_payload(payload: Dict[str, Any]) -> Dict[str, Any]:
+    """Obscure the payload for logging."""
+    if payload is None:
+        return None
+    if "password" in payload:
+        payload = payload.copy()
+        payload["password"] = "****"  # nosec
+    return payload
+
+
 class ApiAsync(ApiCommon):
     """Async api."""
 
     def __init__(
         self,
         aiohttp_session: ClientSession,
         timeout=10,
@@ -49,241 +68,273 @@
         brand=DEFAULT_BRAND,
     ) -> None:
         self._timeout = timeout
         self._command_timeout = command_timeout
         self._aiohttp_session = aiohttp_session
         super().__init__(brand)
 
-    async def async_get_session(self, install_id, identifier, password):
+    async def async_get_session(
+        self, install_id: str, identifier: str, password: str
+    ) -> ClientResponse:
         return await self._async_dict_to_api(
             self._build_get_session_request(install_id, identifier, password)
         )
 
-    async def async_send_verification_code(self, access_token, login_method, username):
+    async def async_send_verification_code(
+        self, access_token: str, login_method: str, username: str
+    ) -> ClientResponse:
         return await self._async_dict_to_api(
             self._build_send_verification_code_request(
                 access_token, login_method, username
             )
         )
 
     async def async_validate_verification_code(
-        self, access_token, login_method, username, verification_code
-    ):
+        self,
+        access_token: str,
+        login_method: str,
+        username: str,
+        verification_code: str,
+    ) -> ClientResponse:
         return await self._async_dict_to_api(
             self._build_validate_verification_code_request(
                 access_token, login_method, username, verification_code
             )
         )
 
-    async def async_get_doorbells(self, access_token):
+    async def async_get_doorbells(self, access_token: str) -> Doorbell:
         response = await self._async_dict_to_api(
             self._build_get_doorbells_request(access_token)
         )
         return _process_doorbells_json(await response.json())
 
-    async def async_get_doorbell_detail(self, access_token, doorbell_id):
+    async def async_get_doorbell_detail(
+        self, access_token: str, doorbell_id: str
+    ) -> DoorbellDetail:
         response = await self._async_dict_to_api(
             self._build_get_doorbell_detail_request(access_token, doorbell_id)
         )
         return DoorbellDetail(await response.json())
 
-    async def async_wakeup_doorbell(self, access_token, doorbell_id):
+    async def async_wakeup_doorbell(
+        self, access_token: str, doorbell_id: str
+    ) -> ClientResponse:
         await self._async_dict_to_api(
             self._build_wakeup_doorbell_request(access_token, doorbell_id)
         )
         return True
 
-    async def async_get_user(self, access_token):
+    async def async_get_user(self, access_token: str) -> dict[str, Any]:
         response = await self._async_dict_to_api(
             self._build_get_user_request(access_token)
         )
         return await response.json()
 
-    async def async_get_houses(self, access_token):
+    async def async_get_houses(self, access_token: str) -> ClientResponse:
         return await self._async_dict_to_api(
             self._build_get_houses_request(access_token)
         )
 
-    async def async_get_house(self, access_token, house_id):
+    async def async_get_house(self, access_token: str, house_id: str) -> Dict[str, Any]:
         response = await self._async_dict_to_api(
             self._build_get_house_request(access_token, house_id)
         )
         return await response.json()
 
-    async def async_get_house_activities(self, access_token, house_id, limit=8):
+    async def async_get_house_activities(
+        self, access_token: str, house_id: str, limit: int = 8
+    ) -> List[ActivityType]:
         response = await self._async_dict_to_api(
             self._build_get_house_activities_request(
                 access_token, house_id, limit=limit
             )
         )
         return _process_activity_json(await response.json())
 
-    async def async_get_locks(self, access_token):
+    async def async_get_locks(self, access_token: str) -> List[Lock]:
         response = await self._async_dict_to_api(
             self._build_get_locks_request(access_token)
         )
         return _process_locks_json(await response.json())
 
-    async def async_get_operable_locks(self, access_token):
+    async def async_get_operable_locks(self, access_token: str) -> List[Lock]:
         locks = await self.async_get_locks(access_token)
 
         return [lock for lock in locks if lock.is_operable]
 
-    async def async_get_lock_detail(self, access_token, lock_id):
+    async def async_get_lock_detail(
+        self, access_token: str, lock_id: str
+    ) -> LockDetail:
         response = await self._async_dict_to_api(
             self._build_get_lock_detail_request(access_token, lock_id)
         )
         return LockDetail(await response.json())
 
-    async def async_get_lock_status(self, access_token, lock_id, door_status=False):
+    async def async_get_lock_status(
+        self, access_token: str, lock_id: str, door_status=False
+    ) -> LockStatus:
         response = await self._async_dict_to_api(
             self._build_get_lock_status_request(access_token, lock_id)
         )
         json_dict = await response.json()
 
         if door_status:
             return (
                 determine_lock_status(json_dict.get("status")),
                 determine_door_state(json_dict.get("doorState")),
             )
 
         return determine_lock_status(json_dict.get("status"))
 
     async def async_get_lock_door_status(
-        self, access_token, lock_id, lock_status=False
-    ):
+        self, access_token: str, lock_id: str, lock_status=False
+    ) -> Union[LockDoorStatus, Tuple[LockDoorStatus, LockStatus]]:
         response = await self._async_dict_to_api(
             self._build_get_lock_status_request(access_token, lock_id)
         )
         json_dict = await response.json()
 
         if lock_status:
             return (
                 determine_door_state(json_dict.get("doorState")),
                 determine_lock_status(json_dict.get("status")),
             )
 
         return determine_door_state(json_dict.get("doorState"))
 
-    async def async_get_pins(self, access_token, lock_id):
+    async def async_get_pins(self, access_token: str, lock_id: str) -> List[Pin]:
         response = await self._async_dict_to_api(
             self._build_get_pins_request(access_token, lock_id)
         )
         json_dict = await response.json()
 
         return [Pin(pin_json) for pin_json in json_dict.get("loaded", [])]
 
-    async def _async_call_lock_operation(self, url_str, access_token, lock_id):
+    async def _async_call_lock_operation(
+        self, url_str: str, access_token: str, lock_id: str
+    ) -> dict[str, Any]:
         response = await self._async_dict_to_api(
             self._build_call_lock_operation_request(
                 url_str, access_token, lock_id, self._command_timeout
             )
         )
         return await response.json()
 
-    async def _async_call_async_lock_operation(self, url_str, access_token, lock_id):
+    async def _async_call_async_lock_operation(
+        self, url_str: str, access_token: str, lock_id: str
+    ) -> str:
         """Call an operation that will queue."""
         response = await self._async_dict_to_api(
             self._build_call_lock_operation_request(
                 url_str, access_token, lock_id, self._command_timeout
             )
         )
         return await response.text()
 
-    async def _async_lock(self, access_token, lock_id):
+    async def _async_lock(self, access_token: str, lock_id: str) -> str:
         return await self._async_call_lock_operation(
             API_LOCK_URL, access_token, lock_id
         )
 
-    async def async_lock(self, access_token, lock_id):
+    async def async_lock(self, access_token: str, lock_id: str) -> str:
         """Execute a remote lock operation.
 
         Returns a LockStatus state.
         """
         return determine_lock_status(
             (await self._async_lock(access_token, lock_id)).get("status")
         )
 
-    async def async_lock_async(self, access_token, lock_id, hyper_bridge=True):
+    async def async_lock_async(
+        self, access_token: str, lock_id: str, hyper_bridge=True
+    ) -> str:
         """Queue a remote lock operation and get the response via pubnub."""
         if hyper_bridge:
             return await self._async_call_async_lock_operation(
                 f"{API_LOCK_ASYNC_URL}{HYPER_BRIDGE_PARAM}", access_token, lock_id
             )
         return await self._async_call_async_lock_operation(
             API_LOCK_ASYNC_URL, access_token, lock_id
         )
 
-    async def async_lock_return_activities(self, access_token, lock_id):
+    async def async_lock_return_activities(
+        self, access_token: str, lock_id: str
+    ) -> List[ActivityType]:
         """Execute a remote lock operation.
 
         Returns an array of one or more yalexs.activity.Activity objects
 
         If the lock supports door sense one of the activities
         will include the current door state.
         """
         return _convert_lock_result_to_activities(
             await self._async_lock(access_token, lock_id)
         )
 
-    async def _async_unlock(self, access_token, lock_id):
+    async def _async_unlock(self, access_token: str, lock_id: str) -> dict[str, Any]:
         return await self._async_call_lock_operation(
             API_UNLOCK_URL, access_token, lock_id
         )
 
-    async def async_unlock(self, access_token, lock_id):
+    async def async_unlock(self, access_token: str, lock_id: str) -> LockStatus:
         """Execute a remote unlock operation.
 
         Returns a LockStatus state.
         """
         return determine_lock_status(
             (await self._async_unlock(access_token, lock_id)).get("status")
         )
 
-    async def async_unlock_async(self, access_token, lock_id, hyper_bridge=True):
+    async def async_unlock_async(
+        self, access_token: str, lock_id: str, hyper_bridge=True
+    ) -> str:
         """Queue a remote unlock operation and get the response via pubnub."""
         if hyper_bridge:
             return await self._async_call_async_lock_operation(
                 f"{API_UNLOCK_ASYNC_URL}{HYPER_BRIDGE_PARAM}", access_token, lock_id
             )
         return await self._async_call_async_lock_operation(
             API_UNLOCK_ASYNC_URL, access_token, lock_id
         )
 
-    async def async_unlock_return_activities(self, access_token, lock_id):
+    async def async_unlock_return_activities(
+        self, access_token: str, lock_id: str
+    ) -> List[ActivityType]:
         """Execute a remote lock operation.
 
         Returns an array of one or more yalexs.activity.Activity objects
 
         If the lock supports door sense one of the activities
         will include the current door state.
         """
         return _convert_lock_result_to_activities(
             await self._async_unlock(access_token, lock_id)
         )
 
-    async def async_status_async(self, access_token, lock_id, hyper_bridge=True):
+    async def async_status_async(
+        self, access_token: str, lock_id: str, hyper_bridge=True
+    ) -> str:
         """Queue a remote unlock operation and get the status via pubnub."""
         if hyper_bridge:
             return await self._async_call_async_lock_operation(
                 f"{API_STATUS_ASYNC_URL}{HYPER_BRIDGE_PARAM}", access_token, lock_id
             )
         return await self._async_call_async_lock_operation(
             API_STATUS_ASYNC_URL, access_token, lock_id
         )
 
-    async def async_refresh_access_token(self, access_token):
+    async def async_refresh_access_token(self, access_token: str) -> str:
         """Obtain a new api token."""
         return (
             await self._async_dict_to_api(
                 self._build_refresh_access_token_request(access_token)
             )
         ).headers[HEADER_AUGUST_ACCESS_TOKEN]
 
-    async def _async_dict_to_api(self, api_dict):
+    async def _async_dict_to_api(self, api_dict: dict[str, Any]) -> ClientResponse:
         url = api_dict["url"]
         method = api_dict["method"]
         access_token = api_dict.get("access_token", None)
         del api_dict["url"]
         del api_dict["method"]
         if access_token:
             del api_dict["access_token"]
@@ -296,23 +347,25 @@
         if "version" in api_dict:
             api_dict["headers"][HEADER_ACCEPT_VERSION] = api_dict["version"]
             del api_dict["version"]
 
         if "timeout" not in api_dict:
             api_dict["timeout"] = self._timeout
 
-        _LOGGER.debug(
-            "About to call %s with header=%s and payload=%s",
-            url,
-            api_dict["headers"],
-            payload,
-        )
+        debug_enabled = _LOGGER.isEnabledFor(logging.DEBUG)
+
+        if debug_enabled:
+            _LOGGER.debug(
+                "About to call %s with header=%s and payload=%s",
+                url,
+                api_dict["headers"],
+                _obscure_payload(payload),
+            )
 
         attempts = 0
-        debug_enabled = _LOGGER.isEnabledFor(logging.DEBUG)
         while attempts < API_RETRY_ATTEMPTS:
             attempts += 1
             try:
                 response = await self._aiohttp_session.request(method, url, **api_dict)
             except ServerDisconnectedError:
                 # Try again if we get disconnected
                 continue
```

### Comparing `yalexs-1.4.2/yalexs/api_common.py` & `yalexs-1.4.3/yalexs/api_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Api functions common between sync and async."""
+import datetime
 import logging
-from typing import Any, Dict
+from typing import Any, Dict, List, Optional, Union
 
 import dateutil.parser
 
 from .activity import (
     ACTIVITY_ACTIONS_BRIDGE_OPERATION,
     ACTIVITY_ACTIONS_DOOR_OPERATION,
     ACTIVITY_ACTIONS_DOORBELL_DING,
@@ -71,14 +72,23 @@
 API_STATUS_ASYNC_URL = (
     "/remoteoperate/{lock_id}/status?v=2.3.1&type=async&intent=wakeup"
 )
 HYPER_BRIDGE_PARAM = "&connection=persistent"
 API_GET_USER_URL = "/users/me"
 
 _LOGGER = logging.getLogger(__name__)
+ActivityType = Union[
+    DoorbellDingActivity,
+    DoorbellMotionActivity,
+    DoorbellImageCaptureActivity,
+    DoorbellViewActivity,
+    LockOperationActivity,
+    DoorOperationActivity,
+    BridgeOperationActivity,
+]
 
 
 def _api_headers(access_token=None):
     headers = {
         HEADER_ACCEPT_VERSION: HEADER_VALUE_ACCEPT_VERSION,
         HEADER_AUGUST_API_KEY: HEADER_VALUE_API_KEY,
         HEADER_CONTENT_TYPE: HEADER_VALUE_CONTENT_TYPE,
@@ -89,15 +99,17 @@
 
     if access_token:
         headers[HEADER_AUGUST_ACCESS_TOKEN] = access_token
 
     return headers
 
 
-def _convert_lock_result_to_activities(lock_json_dict):
+def _convert_lock_result_to_activities(
+    lock_json_dict: Dict[str, Any]
+) -> List[ActivityType]:
     activities = []
     lock_info_json_dict = lock_json_dict.get("info", {})
     lock_id = lock_info_json_dict.get("lockID")
     lock_action_text = lock_info_json_dict.get("action")
     activity_epoch = _datetime_string_to_epoch(lock_info_json_dict.get("startTime"))
     activity_lock_dict = _map_lock_result_to_activity(
         lock_id, activity_epoch, lock_action_text
@@ -110,15 +122,17 @@
             lock_id, activity_epoch, door_state_to_string(door_state)
         )
         activities.append(activity_door_dict)
 
     return activities
 
 
-def _activity_from_dict(source: str, activity_dict: Dict[str, Any]):
+def _activity_from_dict(
+    source: str, activity_dict: Dict[str, Any]
+) -> Optional[ActivityType]:
     _LOGGER.debug("Processing activity: %s", activity_dict)
     action = activity_dict.get("action")
 
     if action in ACTIVITY_ACTIONS_DOORBELL_DING:
         return DoorbellDingActivity(source, activity_dict)
     if action in ACTIVITY_ACTIONS_DOORBELL_MOTION:
         return DoorbellMotionActivity(source, activity_dict)
@@ -133,46 +147,48 @@
     if action in ACTIVITY_ACTIONS_BRIDGE_OPERATION:
         return BridgeOperationActivity(source, activity_dict)
 
     _LOGGER.debug("Unknown activity: %s", activity_dict)
     return None
 
 
-def _map_lock_result_to_activity(lock_id, activity_epoch, action_text):
+def _map_lock_result_to_activity(
+    lock_id: str, activity_epoch: float, action_text: str
+) -> Optional[ActivityType]:
     """Create an yale access activity from a lock result."""
     mapped_dict = {
         "dateTime": activity_epoch,
         "deviceID": lock_id,
         "deviceType": "lock",
         "action": action_text,
     }
     return _activity_from_dict(SOURCE_LOCK_OPERATE, mapped_dict)
 
 
-def _datetime_string_to_epoch(datetime_string):
+def _datetime_string_to_epoch(datetime_string: str) -> datetime.datetime:
     return dateutil.parser.parse(datetime_string).timestamp() * 1000
 
 
-def _process_activity_json(json_dict):
+def _process_activity_json(json_dict: Dict[str, Any]) -> List[ActivityType]:
     if "events" in json_dict:
         json_dict = json_dict["events"]
     activities = []
     for activity_json in json_dict:
         activity = _activity_from_dict(SOURCE_LOG, activity_json)
         if activity:
             activities.append(activity)
 
     return activities
 
 
-def _process_doorbells_json(json_dict):
+def _process_doorbells_json(json_dict: Dict[str, Any]) -> List[Doorbell]:
     return [Doorbell(device_id, data) for device_id, data in json_dict.items()]
 
 
-def _process_locks_json(json_dict):
+def _process_locks_json(json_dict: Dict[str, Any]) -> List[Lock]:
     return [Lock(device_id, data) for device_id, data in json_dict.items()]
 
 
 class ApiCommon:
     """Api dict shared between async and sync."""
 
     def __init__(self, brand: Brand) -> None:
```

### Comparing `yalexs-1.4.2/yalexs/authenticator.py` & `yalexs-1.4.3/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/authenticator_async.py` & `yalexs-1.4.3/yalexs/authenticator_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Authentication,
     AuthenticationState,
     AuthenticatorCommon,
     ValidationResult,
     from_authentication_json,
     to_authentication_json,
 )
+from .exceptions import AugustApiAIOHTTPError
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AuthenticatorAsync(AuthenticatorCommon):
     """Class to manage authentication with the August API."""
 
@@ -100,15 +101,15 @@
         try:
             await self._api.async_validate_verification_code(
                 self._authentication.access_token,
                 self._login_method,
                 self._username,
                 verification_code,
             )
-        except ClientError:
+        except (AugustApiAIOHTTPError, ClientError):
             return ValidationResult.INVALID_VERIFICATION_CODE
 
         return ValidationResult.VALIDATED
 
     async def async_send_verification_code(self) -> bool:
         await self._api.async_send_verification_code(
             self._authentication.access_token, self._login_method, self._username
```

### Comparing `yalexs-1.4.2/yalexs/authenticator_common.py` & `yalexs-1.4.3/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/backports/enum.py` & `yalexs-1.4.3/yalexs/backports/enum.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/bridge.py` & `yalexs-1.4.3/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/device.py` & `yalexs-1.4.3/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/doorbell.py` & `yalexs-1.4.3/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/exceptions.py` & `yalexs-1.4.3/yalexs/exceptions.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/keypad.py` & `yalexs-1.4.3/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/lock.py` & `yalexs-1.4.3/yalexs/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/pin.py` & `yalexs-1.4.3/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/pubnub_activity.py` & `yalexs-1.4.3/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/pubnub_async.py` & `yalexs-1.4.3/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/users.py` & `yalexs-1.4.3/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs/util.py` & `yalexs-1.4.3/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.2/yalexs.egg-info/PKG-INFO` & `yalexs-1.4.3/yalexs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.2/yalexs.egg-info/SOURCES.txt` & `yalexs-1.4.3/yalexs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

