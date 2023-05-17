# Comparing `tmp/yalexs-1.3.3.tar.gz` & `tmp/yalexs-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.3.3.tar", last modified: Sun Apr 30 06:11:18 2023, max compression
+gzip compressed data, was "yalexs-1.4.0.tar", last modified: Wed May 17 14:09:08 2023, max compression
```

## Comparing `yalexs-1.3.3.tar` & `yalexs-1.4.0.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.492865 yalexs-1.3.3/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.474817 yalexs-1.3.3/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.477979 yalexs-1.3.3/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2383 2023-02-17 14:33:57.000000 yalexs-1.3.3/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.3.3/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.3.3/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.3.3/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-30 06:11:18.492962 yalexs-1.3.3/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.3.3/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.3.3/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.3.3/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.3.3/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       46 2023-02-17 14:03:08.000000 yalexs-1.3.3/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.3.3/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 06:11:18.493293 yalexs-1.3.3/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)      972 2023-04-30 06:11:07.000000 yalexs-1.3.3/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.479852 yalexs-1.3.3/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.487983 yalexs-1.3.3/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14702 2023-04-24 17:14:19.000000 yalexs-1.3.3/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    31589 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38166 2023-02-17 14:33:57.000000 yalexs-1.3.3/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8411 2023-02-17 14:03:08.000000 yalexs-1.3.3/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-04-24 17:36:15.000000 yalexs-1.3.3/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.3.3/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.3.3/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.492190 yalexs-1.3.3/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-04-30 06:11:07.000000 yalexs-1.3.3/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14180 2023-04-30 06:10:58.000000 yalexs-1.3.3/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9792 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12351 2023-02-17 14:03:08.000000 yalexs-1.3.3/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10480 2023-04-14 19:36:42.000000 yalexs-1.3.3/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4740 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5057 2023-02-17 14:03:08.000000 yalexs-1.3.3/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5080 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/authenticator_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4284 2023-02-17 14:03:08.000000 yalexs-1.3.3/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      273 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.3.3/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-04-24 17:36:15.000000 yalexs-1.3.3/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.3.3/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.492765 yalexs-1.3.3/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2799 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.490343 yalexs-1.4.0/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.479360 yalexs-1.4.0/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.481114 yalexs-1.4.0/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.0/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 14:09:08.490393 yalexs-1.4.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.0/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.0/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.0/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.4.0/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 14:09:08.490686 yalexs-1.4.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 14:08:57.000000 yalexs-1.4.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.482005 yalexs-1.4.0/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.487238 yalexs-1.4.0/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.0/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.0/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    42227 2023-05-17 14:08:38.000000 yalexs-1.4.0/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.0/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.0/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-05-17 04:41:53.000000 yalexs-1.4.0/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.0/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.0/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.489510 yalexs-1.4.0/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 14:08:57.000000 yalexs-1.4.0/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9931 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    12514 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10895 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5030 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.490252 yalexs-1.4.0/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      489 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.0/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      273 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.0/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-05-17 04:41:53.000000 yalexs-1.4.0/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.0/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.0/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 14:09:08.490052 yalexs-1.4.0/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 14:09:08.000000 yalexs-1.4.0/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 14:09:08.000000 yalexs-1.4.0/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 14:09:08.000000 yalexs-1.4.0/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:09:08.000000 yalexs-1.4.0/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 14:09:08.000000 yalexs-1.4.0/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.3.3/.github/workflows/ci.yaml` & `yalexs-1.4.0/.github/workflows/ci.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -62,23 +62,20 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
       run: TOXENV=codecov tox
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v3
       with:
-        files: ./coverage.xml
-        directory: ./coverage/reports/
         flags: unittests
         env_vars: OS,PYTHON
         name: codecov-umbrella
         fail_ci_if_error: true
-        path_to_write_report: ./coverage/codecov_report.txt
         verbose: true
 
   bandit:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
```

### Comparing `yalexs-1.3.3/.gitignore` & `yalexs-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/LICENSE` & `yalexs-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/PKG-INFO` & `yalexs-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.3.3
+Version: 1.4.0
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.3.3/README.md` & `yalexs-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/known_activities.md` & `yalexs-1.4.0/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/pylintrc` & `yalexs-1.4.0/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/setup.cfg` & `yalexs-1.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.3
+current_version = 1.4.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.3.3/setup.py` & `yalexs-1.4.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.3.3",
+    version="1.4.0",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
@@ -15,18 +15,19 @@
         "Programming Language :: Python :: 3.11",
     ],
     url="https://github.com/bdraco/yalexs",
     license="MIT",
     author="bdraco",
     author_email="nick@koston.org",
     description="Python API for Yale Access (formerly August) Smart Lock and Doorbell",
-    packages=find_packages(include=["yalexs", "yalexs.*"]),
+    packages=find_packages(include=["yalexs", "yalexs.backports", "yalexs.*"]),
     install_requires=[
         "pyjwt",
         "requests",
         "vol",
         "python-dateutil",
         "aiohttp",
         "aiofiles",
-        "pubnub>=5.5.0",
+        "pubnub>=7.1.0",
+        "typing_extensions>=4.5.0"
     ],
 )
```

### Comparing `yalexs-1.3.3/tests/fixtures/auto_relock_activity.json` & `yalexs-1.4.0/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.4.0/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.4.0/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/door_closed_activity.json` & `yalexs-1.4.0/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.4.0/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.4.0/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/door_open_activity.json` & `yalexs-1.4.0/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.4.0/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.4.0/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.4.0/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.4.0/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.4.0/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.4.0/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.4.0/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbell.json` & `yalexs-1.4.0/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.4.0/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.4.0/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_doorbells.json` & `yalexs-1.4.0/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_house_activities.json` & `yalexs-1.4.0/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.4.0/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.4.0/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock.offline.json` & `yalexs-1.4.0/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock.online.json` & `yalexs-1.4.0/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.4.0/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.4.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.4.0/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/get_pins.json` & `yalexs-1.4.0/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.4.0/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/lock.json` & `yalexs-1.4.0/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/lock_activity.json` & `yalexs-1.4.0/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.4.0/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/remote_lock_activity.json` & `yalexs-1.4.0/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.4.0/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/unlock.json` & `yalexs-1.4.0/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/unlock_activity.json` & `yalexs-1.4.0/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.4.0/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/test_activity.py` & `yalexs-1.4.0/tests/test_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     ACTIVITY_ACTIONS_DOORBELL_VIEW,
     ACTIVITY_ACTIONS_LOCK_OPERATION,
     SOURCE_LOG,
     ActivityType,
     LockOperationActivity,
 )
 from yalexs.api_async import ApiAsync
-from yalexs.api_common import API_GET_LOCK_URL
+from yalexs.api_common import API_GET_LOCK_URL, ApiCommon
+from yalexs.const import DEFAULT_BRAND
 from yalexs.lock import LockDoorStatus, LockStatus
 
 ACCESS_TOKEN = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9"
 
 
 def load_fixture(filename):
     """Load a fixture."""
@@ -329,15 +330,17 @@
         assert auto_relock_operation_activity.operated_keypad is False
 
 
 class TestActivityApiAsync(aiounittest.AsyncTestCase):
     @aioresponses()
     async def test_async_get_lock_detail_bridge_online(self, mock):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
             body=load_fixture("get_lock.online.json"),
         )
 
         api = ApiAsync(ClientSession())
         await api.async_get_lock_detail(
             ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
         )
```

### Comparing `yalexs-1.3.3/tests/test_api.py` & `yalexs-1.4.0/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     API_GET_LOCK_STATUS_URL,
     API_GET_LOCK_URL,
     API_GET_LOCKS_URL,
     API_GET_PINS_URL,
     API_GET_USER_URL,
     API_LOCK_URL,
     API_UNLOCK_URL,
+    ApiCommon,
 )
 from yalexs.bridge import BridgeDetail, BridgeStatus, BridgeStatusDetail
+from yalexs.const import DEFAULT_BRAND
 from yalexs.exceptions import AugustApiHTTPError
 from yalexs.lock import LockDoorStatus, LockStatus
 
 ACCESS_TOKEN = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9"
 
 
 def load_fixture(filename):
@@ -41,15 +43,17 @@
     return datetime(year, month, day, hour, minute, second, microsecond, tzinfo=tzutc())
 
 
 class TestApi(unittest.TestCase):
     @requests_mock.Mocker()
     def test_get_doorbells(self, mock):
         mock.register_uri(
-            "get", API_GET_DOORBELLS_URL, text=load_fixture("get_doorbells.json")
+            "get",
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_DOORBELLS_URL),
+            text=load_fixture("get_doorbells.json"),
         )
 
         api = Api()
         doorbells = sorted(api.get_doorbells(ACCESS_TOKEN), key=lambda d: d.device_id)
 
         self.assertEqual(2, len(doorbells))
 
@@ -72,15 +76,17 @@
         self.assertEqual("3dd2accaea08", second.house_id)
 
     @requests_mock.Mocker()
     def test_get_doorbell_detail(self, mock):
         expected_doorbell_image_url = "https://image.com/vmk16naaaa7ibuey7sar.jpg"
         mock.register_uri(
             "get",
-            API_GET_DOORBELL_URL.format(doorbell_id="K98GiDT45GUL"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="K98GiDT45GUL"),
             text=load_fixture("get_doorbell.json"),
         )
         mock.register_uri(
             "get", expected_doorbell_image_url, text="doorbell_image_mocked"
         )
 
         api = Api()
@@ -107,15 +113,17 @@
             doorbell.get_doorbell_image(timeout=50), b"doorbell_image_mocked"
         )
 
     @requests_mock.Mocker()
     def test_get_doorbell_detail_missing_image(self, mock):
         mock.register_uri(
             "get",
-            API_GET_DOORBELL_URL.format(doorbell_id="K98GiDT45GUL"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="K98GiDT45GUL"),
             text=load_fixture("get_doorbell_missing_image.json"),
         )
 
         api = Api()
         doorbell = api.get_doorbell_detail(ACCESS_TOKEN, "K98GiDT45GUL")
 
         self.assertEqual("K98GiDT45GUL", doorbell.device_id)
@@ -131,15 +139,17 @@
         self.assertEqual(True, doorbell.has_subscription)
         self.assertEqual(None, doorbell.image_url)
 
     @requests_mock.Mocker()
     def test_get_doorbell_offline(self, mock):
         mock.register_uri(
             "get",
-            API_GET_DOORBELL_URL.format(doorbell_id="231ee2168dd0"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="231ee2168dd0"),
             text=load_fixture("get_doorbell.offline.json"),
         )
 
         api = Api()
         doorbell = api.get_doorbell_detail(ACCESS_TOKEN, "231ee2168dd0")
 
         self.assertEqual("231ee2168dd0", doorbell.device_id)
@@ -159,52 +169,62 @@
         self.assertEqual("https://res.cloudinary.com/x.jpg", doorbell.image_url)
         self.assertEqual("hydra1", doorbell.model)
 
     @requests_mock.Mocker()
     def test_get_doorbell_gen2_full_battery_detail(self, mock):
         mock.register_uri(
             "get",
-            API_GET_DOORBELL_URL.format(doorbell_id="did"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="did"),
             text=load_fixture("get_doorbell.battery_full.json"),
         )
 
         api = Api()
         doorbell = api.get_doorbell_detail(ACCESS_TOKEN, "did")
 
         self.assertEqual(100, doorbell.battery_level)
 
     @requests_mock.Mocker()
     def test_get_doorbell_gen2_medium_battery_detail(self, mock):
         mock.register_uri(
             "get",
-            API_GET_DOORBELL_URL.format(doorbell_id="did"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="did"),
             text=load_fixture("get_doorbell.battery_medium.json"),
         )
 
         api = Api()
         doorbell = api.get_doorbell_detail(ACCESS_TOKEN, "did")
 
         self.assertEqual(75, doorbell.battery_level)
 
     @requests_mock.Mocker()
     def test_get_doorbell_gen2_low_battery_detail(self, mock):
         mock.register_uri(
             "get",
-            API_GET_DOORBELL_URL.format(doorbell_id="did"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="did"),
             text=load_fixture("get_doorbell.battery_low.json"),
         )
 
         api = Api()
         doorbell = api.get_doorbell_detail(ACCESS_TOKEN, "did")
 
         self.assertEqual(10, doorbell.battery_level)
 
     @requests_mock.Mocker()
     def test_get_locks(self, mock):
-        mock.register_uri("get", API_GET_LOCKS_URL, text=load_fixture("get_locks.json"))
+        mock.register_uri(
+            "get",
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_LOCKS_URL),
+            text=load_fixture("get_locks.json"),
+        )
 
         api = Api()
         locks = sorted(api.get_locks(ACCESS_TOKEN), key=lambda d: d.device_id)
 
         self.assertEqual(2, len(locks))
 
         first = locks[0]
@@ -217,15 +237,19 @@
         self.assertEqual("A6697750D607098BAE8D6BAA11EF9999", second.device_id)
         self.assertEqual("Back Door Lock", second.device_name)
         self.assertEqual("000000000011", second.house_id)
         self.assertEqual(False, second.is_operable)
 
     @requests_mock.Mocker()
     def test_get_operable_locks(self, mock):
-        mock.register_uri("get", API_GET_LOCKS_URL, text=load_fixture("get_locks.json"))
+        mock.register_uri(
+            "get",
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_LOCKS_URL),
+            text=load_fixture("get_locks.json"),
+        )
 
         api = Api()
         locks = api.get_operable_locks(ACCESS_TOKEN)
 
         self.assertEqual(1, len(locks))
 
         first = locks[0]
@@ -234,15 +258,17 @@
         self.assertEqual("000000000000", first.house_id)
         self.assertEqual(True, first.is_operable)
 
     @requests_mock.Mocker()
     def test_get_lock_detail_with_doorsense_bridge_online(self, mock):
         mock.register_uri(
             "get",
-            API_GET_LOCK_URL.format(lock_id="ABC"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="ABC"),
             text=load_fixture("get_lock.online_with_doorsense.json"),
         )
 
         api = Api()
         lock = api.get_lock_detail(ACCESS_TOKEN, "ABC")
 
         self.assertEqual("ABC", lock.device_id)
@@ -269,15 +295,17 @@
             dateutil.parser.parse("2017-12-10T04:48:30.272Z"), lock.door_state_datetime
         )
 
     @requests_mock.Mocker()
     def test_get_lock_detail_bridge_online(self, mock):
         mock.register_uri(
             "get",
-            API_GET_LOCK_URL.format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
             text=load_fixture("get_lock.online.json"),
         )
 
         api = Api()
         lock = api.get_lock_detail(ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063")
 
         self.assertEqual("A6697750D607098BAE8D6BAA11EF8063", lock.device_id)
@@ -332,15 +360,17 @@
         self.assertEqual(None, lock.lock_status_datetime)
         self.assertEqual(None, lock.door_state_datetime)
 
     @requests_mock.Mocker()
     def test_get_lock_detail_doorsense_init_state(self, mock):
         mock.register_uri(
             "get",
-            API_GET_LOCK_URL.format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
             text=load_fixture("get_lock.doorsense_init.json"),
         )
 
         api = Api()
         lock = api.get_lock_detail(ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063")
 
         self.assertEqual("A6697750D607098BAE8D6BAA11EF8063", lock.device_id)
@@ -406,29 +436,33 @@
         }
 
     @requests_mock.Mocker()
     def test_get_lock_status_with_locked_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"status": "kAugLockState_Locked"}',
         )
 
         api = Api()
         status = api.get_lock_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.LOCKED, status)
 
     @requests_mock.Mocker()
     def test_get_lock_and_door_status_with_locked_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"status": "kAugLockState_Locked"'
             ',"doorState": "kAugLockDoorState_Closed"}',
         )
 
         api = Api()
         status, door_status = api.get_lock_status(ACCESS_TOKEN, lock_id, True)
 
@@ -436,71 +470,81 @@
         self.assertEqual(LockDoorStatus.CLOSED, door_status)
 
     @requests_mock.Mocker()
     def test_get_lock_status_with_unlocked_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"status": "kAugLockState_Unlocked"}',
         )
 
         api = Api()
         status = api.get_lock_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @requests_mock.Mocker()
     def test_get_lock_status_with_unknown_status_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"status": "not_advertising"}',
         )
 
         api = Api()
         status = api.get_lock_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNKNOWN, status)
 
     @requests_mock.Mocker()
     def test_get_lock_door_status_with_closed_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"doorState": "kAugLockDoorState_Closed"}',
         )
 
         api = Api()
         door_status = api.get_lock_door_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockDoorStatus.CLOSED, door_status)
 
     @requests_mock.Mocker()
     def test_get_lock_door_status_with_open_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"doorState": "kAugLockDoorState_Open"}',
         )
 
         api = Api()
         door_status = api.get_lock_door_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockDoorStatus.OPEN, door_status)
 
     @requests_mock.Mocker()
     def test_get_lock_and_door_status_with_open_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"status": "kAugLockState_Unlocked"'
             ',"doorState": "kAugLockDoorState_Open"}',
         )
 
         api = Api()
         door_status, status = api.get_lock_door_status(ACCESS_TOKEN, lock_id, True)
 
@@ -508,54 +552,66 @@
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @requests_mock.Mocker()
     def test_get_lock_door_status_with_unknown_response(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             text='{"doorState": "not_advertising"}',
         )
 
         api = Api()
         door_status = api.get_lock_door_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockDoorStatus.UNKNOWN, door_status)
 
     @requests_mock.Mocker()
     def test_lock_from_fixture(self, mock):
         lock_id = 1234
         mock.register_uri(
-            "put", API_LOCK_URL.format(lock_id=lock_id), text=load_fixture("lock.json")
+            "put",
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
+            text=load_fixture("lock.json"),
         )
 
         api = Api()
         status = api.lock(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.LOCKED, status)
 
     @requests_mock.Mocker()
     def test_unlock_from_fixture(self, mock):
         lock_id = 1234
         mock.register_uri(
             "put",
-            API_UNLOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
             text=load_fixture("unlock.json"),
         )
 
         api = Api()
         status = api.unlock(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @requests_mock.Mocker()
     def test_lock_return_activities_from_fixture(self, mock):
         lock_id = 1234
         mock.register_uri(
-            "put", API_LOCK_URL.format(lock_id=lock_id), text=load_fixture("lock.json")
+            "put",
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
+            text=load_fixture("lock.json"),
         )
 
         api = Api()
         activities = api.lock_return_activities(ACCESS_TOKEN, lock_id)
         expected_lock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:54.371Z")
             .astimezone(tz=tzlocal())
@@ -577,15 +633,17 @@
         self.assertEqual(activities[0].activity_end_time, expected_lock_dt)
 
     @requests_mock.Mocker()
     def test_unlock_return_activities_from_fixture(self, mock):
         lock_id = 1234
         mock.register_uri(
             "put",
-            API_UNLOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
             text=load_fixture("unlock.json"),
         )
 
         api = Api()
         activities = api.unlock_return_activities(ACCESS_TOKEN, lock_id)
         expected_unlock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:26.745Z")
@@ -608,15 +666,17 @@
         self.assertEqual(activities[1].activity_end_time, expected_unlock_dt)
 
     @requests_mock.Mocker()
     def test_lock_return_activities_from_fixture_with_no_doorstate(self, mock):
         lock_id = 1234
         mock.register_uri(
             "put",
-            API_LOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
             text=load_fixture("lock_without_doorstate.json"),
         )
 
         api = Api()
         activities = api.lock_return_activities(ACCESS_TOKEN, lock_id)
         expected_lock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:54.371Z")
@@ -633,15 +693,17 @@
         self.assertEqual(activities[0].activity_end_time, expected_lock_dt)
 
     @requests_mock.Mocker()
     def test_unlock_return_activities_from_fixture_with_no_doorstate(self, mock):
         lock_id = 1234
         mock.register_uri(
             "put",
-            API_UNLOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
             text=load_fixture("unlock_without_doorstate.json"),
         )
 
         api = Api()
         activities = api.unlock_return_activities(ACCESS_TOKEN, lock_id)
         expected_unlock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:26.745Z")
@@ -658,15 +720,17 @@
         self.assertEqual(activities[0].activity_end_time, expected_unlock_dt)
 
     @requests_mock.Mocker()
     def test_lock(self, mock):
         lock_id = 1234
         mock.register_uri(
             "put",
-            API_LOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
             text='{"status":"locked",'
             '"dateTime":"2017-12-10T07:43:39.056Z",'
             '"isLockStatusChanged":false,'
             '"valid":true}',
         )
 
         api = Api()
@@ -674,28 +738,34 @@
 
         self.assertEqual(LockStatus.LOCKED, status)
 
     @requests_mock.Mocker()
     def test_unlock(self, mock):
         lock_id = 1234
         mock.register_uri(
-            "put", API_UNLOCK_URL.format(lock_id=lock_id), text='{"status": "unlocked"}'
+            "put",
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
+            text='{"status": "unlocked"}',
         )
 
         api = Api()
         status = api.unlock(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @requests_mock.Mocker()
     def test_get_pins(self, mock):
         lock_id = 1234
         mock.register_uri(
             "get",
-            API_GET_PINS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_PINS_URL)
+            .format(lock_id=lock_id),
             text=load_fixture("get_pins.json"),
         )
 
         api = Api()
         pins = api.get_pins(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(1, len(pins))
@@ -719,15 +789,17 @@
         self.assertEqual(utc_of(2018, 11, 5, 10, 2, 41, 684000), first.access_times)
 
     @requests_mock.Mocker()
     def test_get_house_activities(self, mock):
         house_id = 1234
         mock.register_uri(
             "get",
-            API_GET_HOUSE_ACTIVITIES_URL.format(house_id=house_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_HOUSE_ACTIVITIES_URL)
+            .format(house_id=house_id),
             text=load_fixture("get_house_activities.json"),
         )
 
         api = Api()
         activities = api.get_house_activities(ACCESS_TOKEN, house_id)
 
         self.assertEqual(10, len(activities))
@@ -784,15 +856,15 @@
             except AugustApiHTTPError as err:
                 self.assertEqual(str(err), ERROR_MAP[status_code])
 
     @requests_mock.Mocker()
     def test_get_user(self, mock):
         mock.register_uri(
             "get",
-            API_GET_USER_URL,
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_USER_URL),
             text='{"UserID": "abc"}',
         )
 
         user_details = Api().get_user(ACCESS_TOKEN)
 
         self.assertEqual(user_details, {"UserID": "abc"})
```

### Comparing `yalexs-1.3.3/tests/test_api_async.py` & `yalexs-1.4.0/tests/test_api_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     API_LOCK_ASYNC_URL,
     API_LOCK_URL,
     API_STATUS_ASYNC_URL,
     API_UNLOCK_ASYNC_URL,
     API_UNLOCK_URL,
     API_VALIDATE_VERIFICATION_CODE_URLS,
     HYPER_BRIDGE_PARAM,
+    ApiCommon,
 )
 from yalexs.bridge import BridgeDetail, BridgeStatus, BridgeStatusDetail
+from yalexs.const import DEFAULT_BRAND, Brand
 from yalexs.exceptions import AugustApiAIOHTTPError
 from yalexs.lock import LockDoorStatus, LockStatus
 
 ACCESS_TOKEN = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9"
 
 
 def load_fixture(filename):
@@ -47,15 +49,18 @@
 def utc_of(year, month, day, hour, minute, second, microsecond):
     return datetime(year, month, day, hour, minute, second, microsecond, tzinfo=tzutc())
 
 
 class TestApiAsync(aiounittest.AsyncTestCase):
     @aioresponses()
     async def test_async_get_doorbells(self, mock):
-        mock.get(API_GET_DOORBELLS_URL, body=load_fixture("get_doorbells.json"))
+        mock.get(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_DOORBELLS_URL),
+            body=load_fixture("get_doorbells.json"),
+        )
 
         api = ApiAsync(ClientSession())
         doorbells = sorted(
             await api.async_get_doorbells(ACCESS_TOKEN), key=lambda d: d.device_id
         )
 
         self.assertEqual(2, len(doorbells))
@@ -78,15 +83,17 @@
         self.assertEqual("https://image.com/vmk16naaaa7ibuey7sar.jpg", second.image_url)
         self.assertEqual("3dd2accaea08", second.house_id)
 
     @aioresponses()
     async def test_async_get_doorbell_detail(self, mock):
         expected_doorbell_image_url = "https://image.com/vmk16naaaa7ibuey7sar.jpg"
         mock.get(
-            API_GET_DOORBELL_URL.format(doorbell_id="K98GiDT45GUL"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="K98GiDT45GUL"),
             body=load_fixture("get_doorbell.json"),
         )
         mock.get(expected_doorbell_image_url, body="doorbell_image_mocked")
 
         api = ApiAsync(ClientSession())
         doorbell = await api.async_get_doorbell_detail(ACCESS_TOKEN, "K98GiDT45GUL")
 
@@ -110,15 +117,17 @@
             await doorbell.async_get_doorbell_image(ClientSession()),
             b"doorbell_image_mocked",
         )
 
     @aioresponses()
     async def test_async_get_doorbell_detail_missing_image(self, mock):
         mock.get(
-            API_GET_DOORBELL_URL.format(doorbell_id="K98GiDT45GUL"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="K98GiDT45GUL"),
             body=load_fixture("get_doorbell_missing_image.json"),
         )
 
         api = ApiAsync(ClientSession())
         doorbell = await api.async_get_doorbell_detail(ACCESS_TOKEN, "K98GiDT45GUL")
 
         self.assertEqual("K98GiDT45GUL", doorbell.device_id)
@@ -133,15 +142,17 @@
         self.assertEqual(None, doorbell.image_created_at_datetime)
         self.assertEqual(True, doorbell.has_subscription)
         self.assertEqual(None, doorbell.image_url)
 
     @aioresponses()
     async def test_async_get_doorbell_offline(self, mock):
         mock.get(
-            API_GET_DOORBELL_URL.format(doorbell_id="231ee2168dd0"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="231ee2168dd0"),
             body=load_fixture("get_doorbell.offline.json"),
         )
 
         api = ApiAsync(ClientSession())
         doorbell = await api.async_get_doorbell_detail(ACCESS_TOKEN, "231ee2168dd0")
 
         self.assertEqual("231ee2168dd0", doorbell.device_id)
@@ -160,50 +171,59 @@
         self.assertEqual(True, doorbell.has_subscription)
         self.assertEqual("https://res.cloudinary.com/x.jpg", doorbell.image_url)
         self.assertEqual("hydra1", doorbell.model)
 
     @aioresponses()
     async def test_async_get_doorbell_gen2_full_battery_detail(self, mock):
         mock.get(
-            API_GET_DOORBELL_URL.format(doorbell_id="did"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="did"),
             body=load_fixture("get_doorbell.battery_full.json"),
         )
 
         api = ApiAsync(ClientSession())
         doorbell = await api.async_get_doorbell_detail(ACCESS_TOKEN, "did")
 
         self.assertEqual(100, doorbell.battery_level)
 
     @aioresponses()
     async def test_async_get_doorbell_gen2_medium_battery_detail(self, mock):
         mock.get(
-            API_GET_DOORBELL_URL.format(doorbell_id="did"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="did"),
             body=load_fixture("get_doorbell.battery_medium.json"),
         )
 
         api = ApiAsync(ClientSession())
         doorbell = await api.async_get_doorbell_detail(ACCESS_TOKEN, "did")
 
         self.assertEqual(75, doorbell.battery_level)
 
     @aioresponses()
     async def test_async_get_doorbell_gen2_low_battery_detail(self, mock):
         mock.get(
-            API_GET_DOORBELL_URL.format(doorbell_id="did"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_DOORBELL_URL)
+            .format(doorbell_id="did"),
             body=load_fixture("get_doorbell.battery_low.json"),
         )
 
         api = ApiAsync(ClientSession())
         doorbell = await api.async_get_doorbell_detail(ACCESS_TOKEN, "did")
 
         self.assertEqual(10, doorbell.battery_level)
 
     @aioresponses()
     async def test_async_get_locks(self, mock):
-        mock.get(API_GET_LOCKS_URL, body=load_fixture("get_locks.json"))
+        mock.get(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_LOCKS_URL),
+            body=load_fixture("get_locks.json"),
+        )
 
         api = ApiAsync(ClientSession())
         locks = sorted(
             await api.async_get_locks(ACCESS_TOKEN), key=lambda d: d.device_id
         )
 
         self.assertEqual(2, len(locks))
@@ -217,16 +237,45 @@
         second = locks[1]
         self.assertEqual("A6697750D607098BAE8D6BAA11EF9999", second.device_id)
         self.assertEqual("Back Door Lock", second.device_name)
         self.assertEqual("000000000011", second.house_id)
         self.assertEqual(False, second.is_operable)
 
     @aioresponses()
+    async def test_async_get_locks_yale_home_brand(self, mock):
+        mock.get(
+            ApiCommon(Brand.YALE_HOME).get_brand_url(API_GET_LOCKS_URL),
+            body=load_fixture("get_locks.json"),
+        )
+
+        api = ApiAsync(ClientSession(), brand=Brand.YALE_HOME)
+        locks = sorted(
+            await api.async_get_locks(ACCESS_TOKEN), key=lambda d: d.device_id
+        )
+
+        self.assertEqual(2, len(locks))
+
+        first = locks[0]
+        self.assertEqual("A6697750D607098BAE8D6BAA11EF8063", first.device_id)
+        self.assertEqual("Front Door Lock", first.device_name)
+        self.assertEqual("000000000000", first.house_id)
+        self.assertEqual(True, first.is_operable)
+
+        second = locks[1]
+        self.assertEqual("A6697750D607098BAE8D6BAA11EF9999", second.device_id)
+        self.assertEqual("Back Door Lock", second.device_name)
+        self.assertEqual("000000000011", second.house_id)
+        self.assertEqual(False, second.is_operable)
+
+    @aioresponses()
     async def test_async_get_operable_locks(self, mock):
-        mock.get(API_GET_LOCKS_URL, body=load_fixture("get_locks.json"))
+        mock.get(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_LOCKS_URL),
+            body=load_fixture("get_locks.json"),
+        )
 
         api = ApiAsync(ClientSession())
         locks = await api.async_get_operable_locks(ACCESS_TOKEN)
 
         self.assertEqual(1, len(locks))
 
         first = locks[0]
@@ -234,15 +283,17 @@
         self.assertEqual("Front Door Lock", first.device_name)
         self.assertEqual("000000000000", first.house_id)
         self.assertEqual(True, first.is_operable)
 
     @aioresponses()
     async def test_async_get_lock_detail_with_doorsense_bridge_online(self, mock):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="ABC"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="ABC"),
             body=load_fixture("get_lock.online_with_doorsense.json"),
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(ACCESS_TOKEN, "ABC")
 
         self.assertEqual("ABC", lock.device_id)
@@ -270,15 +321,17 @@
         )
 
     @aioresponses()
     async def test_async_get_lock_detail_with_doorsense_disabled_bridge_online(
         self, mock
     ):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="ABC"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="ABC"),
             body=load_fixture("get_lock.online_with_doorsense_disabled.json"),
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(ACCESS_TOKEN, "ABC")
 
         self.assertEqual("ABC", lock.device_id)
@@ -305,15 +358,17 @@
         self.assertEqual(
             dateutil.parser.parse("2017-12-10T04:48:30.272Z"), lock.door_state_datetime
         )
 
     @aioresponses()
     async def test_async_get_lock_detail_bridge_online(self, mock):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
             body=load_fixture("get_lock.online.json"),
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(
             ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
         )
@@ -342,15 +397,17 @@
         self.assertEqual(
             dateutil.parser.parse("2017-12-10T04:48:30.272Z"), lock.door_state_datetime
         )
 
     @aioresponses()
     async def test_async_get_v2_lock_detail_bridge_online(self, mock):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="snip"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="snip"),
             body=load_fixture("get_lock_v2.online.json"),
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(ACCESS_TOKEN, "snip")
 
         self.assertEqual("snip", lock.device_id)
@@ -400,15 +457,17 @@
         self.assertEqual(lock.offline_key, "XXXXXX")
         self.assertEqual(lock.offline_slot, 1)
         self.assertEqual(lock.mac_address, "SNIP")
 
     @aioresponses()
     async def test_async_get_lock_detail_bridge_offline(self, mock):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="ABC"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="ABC"),
             body=load_fixture("get_lock.offline.json"),
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(ACCESS_TOKEN, "ABC")
 
         self.assertEqual("ABC", lock.device_id)
@@ -427,15 +486,17 @@
         self.assertEqual(LockDoorStatus.DISABLED, lock.door_state)
         self.assertEqual(None, lock.lock_status_datetime)
         self.assertEqual(None, lock.door_state_datetime)
 
     @aioresponses()
     async def test_async_get_lock_detail_doorsense_init_state(self, mock):
         mock.get(
-            API_GET_LOCK_URL.format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
             body=load_fixture("get_lock.doorsense_init.json"),
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(
             ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
         )
@@ -480,28 +541,32 @@
         )
         assert isinstance(lock.raw, dict)
 
     @aioresponses()
     async def test_async_get_lock_status_with_locked_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"status": "kAugLockState_Locked"}',
         )
 
         api = ApiAsync(ClientSession())
         status = await api.async_get_lock_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.LOCKED, status)
 
     @aioresponses()
     async def test_async_get_lock_and_door_status_with_locked_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"status": "kAugLockState_Locked"'
             ',"doorState": "kAugLockDoorState_Closed"}',
         )
 
         api = ApiAsync(ClientSession())
         status, door_status = await api.async_get_lock_status(
             ACCESS_TOKEN, lock_id, True
@@ -510,67 +575,77 @@
         self.assertEqual(LockStatus.LOCKED, status)
         self.assertEqual(LockDoorStatus.CLOSED, door_status)
 
     @aioresponses()
     async def test_async_get_lock_status_with_unlocked_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"status": "kAugLockState_Unlocked"}',
         )
 
         api = ApiAsync(ClientSession())
         status = await api.async_get_lock_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @aioresponses()
     async def test_async_get_lock_status_with_unknown_status_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"status": "not_advertising"}',
         )
 
         api = ApiAsync(ClientSession())
         status = await api.async_get_lock_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNKNOWN, status)
 
     @aioresponses()
     async def test_async_get_lock_door_status_with_closed_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"doorState": "kAugLockDoorState_Closed"}',
         )
 
         api = ApiAsync(ClientSession())
         door_status = await api.async_get_lock_door_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockDoorStatus.CLOSED, door_status)
 
     @aioresponses()
     async def test_async_get_lock_door_status_with_open_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"doorState": "kAugLockDoorState_Open"}',
         )
 
         api = ApiAsync(ClientSession())
         door_status = await api.async_get_lock_door_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockDoorStatus.OPEN, door_status)
 
     @aioresponses()
     async def test_async_get_lock_and_door_status_with_open_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"status": "kAugLockState_Unlocked"'
             ',"doorState": "kAugLockDoorState_Open"}',
         )
 
         api = ApiAsync(ClientSession())
         door_status, status = await api.async_get_lock_door_status(
             ACCESS_TOKEN, lock_id, True
@@ -579,50 +654,64 @@
         self.assertEqual(LockDoorStatus.OPEN, door_status)
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @aioresponses()
     async def test_async_get_lock_door_status_with_unknown_response(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_STATUS_URL)
+            .format(lock_id=lock_id),
             body='{"doorState": "not_advertising"}',
         )
 
         api = ApiAsync(ClientSession())
         door_status = await api.async_get_lock_door_status(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockDoorStatus.UNKNOWN, door_status)
 
     @aioresponses()
     async def test_async_lock_from_fixture(self, mock):
         lock_id = 1234
-        mock.put(API_LOCK_URL.format(lock_id=lock_id), body=load_fixture("lock.json"))
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
+            body=load_fixture("lock.json"),
+        )
 
         api = ApiAsync(ClientSession())
         status = await api.async_lock(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.LOCKED, status)
 
     @aioresponses()
     async def test_async_unlock_from_fixture(self, mock):
         lock_id = 1234
         mock.put(
-            API_UNLOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
             body=load_fixture("unlock.json"),
         )
 
         api = ApiAsync(ClientSession())
         status = await api.async_unlock(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @aioresponses()
     async def test_async_lock_return_activities_from_fixture(self, mock):
         lock_id = 1234
-        mock.put(API_LOCK_URL.format(lock_id=lock_id), body=load_fixture("lock.json"))
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
+            body=load_fixture("lock.json"),
+        )
 
         api = ApiAsync(ClientSession())
         activities = await api.async_lock_return_activities(ACCESS_TOKEN, lock_id)
         expected_lock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:54.371Z")
             .astimezone(tz=tzlocal())
             .replace(tzinfo=None)
@@ -642,15 +731,17 @@
         self.assertEqual(activities[0].activity_start_time, expected_lock_dt)
         self.assertEqual(activities[0].activity_end_time, expected_lock_dt)
 
     @aioresponses()
     async def test_async_unlock_return_activities_from_fixture(self, mock):
         lock_id = 1234
         mock.put(
-            API_UNLOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
             body=load_fixture("unlock.json"),
         )
 
         api = ApiAsync(ClientSession())
         activities = await api.async_unlock_return_activities(ACCESS_TOKEN, lock_id)
         expected_unlock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:26.745Z")
@@ -674,15 +765,17 @@
 
     @aioresponses()
     async def test_async_lock_return_activities_from_fixture_with_no_doorstate(
         self, mock
     ):
         lock_id = 1234
         mock.put(
-            API_LOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
             body=load_fixture("lock_without_doorstate.json"),
         )
 
         api = ApiAsync(ClientSession())
         activities = await api.async_lock_return_activities(ACCESS_TOKEN, lock_id)
         expected_lock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:54.371Z")
@@ -700,15 +793,17 @@
 
     @aioresponses()
     async def test_async_unlock_return_activities_from_fixture_with_no_doorstate(
         self, mock
     ):
         lock_id = 1234
         mock.put(
-            API_UNLOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
             body=load_fixture("unlock_without_doorstate.json"),
         )
 
         api = ApiAsync(ClientSession())
         activities = await api.async_unlock_return_activities(ACCESS_TOKEN, lock_id)
         expected_unlock_dt = (
             dateutil.parser.parse("2020-02-19T19:44:26.745Z")
@@ -724,15 +819,17 @@
         self.assertEqual(activities[0].activity_start_time, expected_unlock_dt)
         self.assertEqual(activities[0].activity_end_time, expected_unlock_dt)
 
     @aioresponses()
     async def test_async_lock(self, mock):
         lock_id = 1234
         mock.put(
-            API_LOCK_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_URL)
+            .format(lock_id=lock_id),
             body='{"status":"locked",'
             '"dateTime":"2017-12-10T07:43:39.056Z",'
             '"isLockStatusChanged":false,'
             '"valid":true}',
         )
 
         api = ApiAsync(ClientSession())
@@ -740,75 +837,97 @@
 
         self.assertEqual(LockStatus.LOCKED, status)
 
     @aioresponses()
     async def test_async_lock_async_old_bridge(self, mock):
         lock_id = 1234
         mock.put(
-            API_LOCK_ASYNC_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_LOCK_ASYNC_URL)
+            .format(lock_id=lock_id),
         )
 
         api = ApiAsync(ClientSession())
         await api.async_lock_async(ACCESS_TOKEN, lock_id, hyper_bridge=False)
 
     @aioresponses()
     async def test_async_lock_async_new_bridge(self, mock):
         lock_id = 1234
-        mock.put(f"{API_LOCK_ASYNC_URL}{HYPER_BRIDGE_PARAM}".format(lock_id=lock_id))
+        base_url = ApiCommon(DEFAULT_BRAND).get_brand_url(API_LOCK_ASYNC_URL)
+        mock.put(f"{base_url}{HYPER_BRIDGE_PARAM}".format(lock_id=lock_id))
 
         api = ApiAsync(ClientSession())
         await api.async_lock_async(ACCESS_TOKEN, lock_id)
 
     @aioresponses()
     async def test_async_unlock(self, mock):
         lock_id = 1234
-        mock.put(API_UNLOCK_URL.format(lock_id=lock_id), body='{"status": "unlocked"}')
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_URL)
+            .format(lock_id=lock_id),
+            body='{"status": "unlocked"}',
+        )
 
         api = ApiAsync(ClientSession())
         status = await api.async_unlock(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(LockStatus.UNLOCKED, status)
 
     @aioresponses()
     async def test_async_unlock_async_old_bridge(self, mock):
         lock_id = 1234
-        mock.put(API_UNLOCK_ASYNC_URL.format(lock_id=lock_id))
+
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_UNLOCK_ASYNC_URL)
+            .format(lock_id=lock_id)
+        )
 
         api = ApiAsync(ClientSession())
         await api.async_unlock_async(ACCESS_TOKEN, lock_id, hyper_bridge=False)
 
     @aioresponses()
     async def test_async_unlock_async_new_bridge(self, mock):
         lock_id = 1234
-        mock.put(f"{API_UNLOCK_ASYNC_URL}{HYPER_BRIDGE_PARAM}".format(lock_id=lock_id))
+        base_url = ApiCommon(DEFAULT_BRAND).get_brand_url(API_UNLOCK_ASYNC_URL)
+        mock.put(f"{base_url}{HYPER_BRIDGE_PARAM}".format(lock_id=lock_id))
 
         api = ApiAsync(ClientSession())
         await api.async_unlock_async(ACCESS_TOKEN, lock_id, hyper_bridge=True)
 
     @aioresponses()
     async def test_async_status_async_old_bridge(self, mock):
         lock_id = 1234
-        mock.put(API_STATUS_ASYNC_URL.format(lock_id=lock_id))
+
+        mock.put(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_STATUS_ASYNC_URL)
+            .format(lock_id=lock_id)
+        )
 
         api = ApiAsync(ClientSession())
         await api.async_status_async(ACCESS_TOKEN, lock_id, hyper_bridge=False)
 
     @aioresponses()
     async def test_async_status_async_new_bridge(self, mock):
         lock_id = 1234
-        mock.put(f"{API_STATUS_ASYNC_URL}{HYPER_BRIDGE_PARAM}".format(lock_id=lock_id))
+        base_url = ApiCommon(DEFAULT_BRAND).get_brand_url(API_STATUS_ASYNC_URL)
+        mock.put(f"{base_url}{HYPER_BRIDGE_PARAM}".format(lock_id=lock_id))
 
         api = ApiAsync(ClientSession())
         await api.async_status_async(ACCESS_TOKEN, lock_id)
 
     @aioresponses()
     async def test_async_get_pins(self, mock):
         lock_id = 1234
         mock.get(
-            API_GET_PINS_URL.format(lock_id=lock_id),
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_PINS_URL)
+            .format(lock_id=lock_id),
             body=load_fixture("get_pins.json"),
         )
 
         api = ApiAsync(ClientSession())
         pins = await api.async_get_pins(ACCESS_TOKEN, lock_id)
 
         self.assertEqual(1, len(pins))
@@ -830,16 +949,20 @@
         self.assertEqual(utc_of(2018, 1, 1, 1, 1, 1, 563000), first.access_start_time)
         self.assertEqual(utc_of(2018, 12, 1, 1, 1, 1, 563000), first.access_end_time)
         self.assertEqual(utc_of(2018, 11, 5, 10, 2, 41, 684000), first.access_times)
 
     @aioresponses()
     async def test_async_get_house_activities(self, mock):
         house_id = 1234
+
         mock.get(
-            API_GET_HOUSE_ACTIVITIES_URL.format(house_id=house_id) + "?limit=8",
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_HOUSE_ACTIVITIES_URL)
+            .format(house_id=house_id)
+            + "?limit=8",
             body=load_fixture("get_house_activities.json"),
         )
 
         api = ApiAsync(ClientSession())
         activities = await api.async_get_house_activities(ACCESS_TOKEN, house_id)
 
         self.assertEqual(10, len(activities))
@@ -854,15 +977,17 @@
         self.assertIsInstance(activities[7], yalexs.activity.DoorOperationActivity)
         self.assertIsInstance(activities[8], yalexs.activity.LockOperationActivity)
         self.assertIsInstance(activities[9], yalexs.activity.LockOperationActivity)
 
     @aioresponses()
     async def test_async_refresh_access_token(self, mock):
         mock.get(
-            API_GET_HOUSES_URL, body="{}", headers={"x-august-access-token": "xyz"}
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_HOUSES_URL),
+            body="{}",
+            headers={"x-august-access-token": "xyz"},
         )
 
         api = ApiAsync(ClientSession())
         new_token = await api.async_refresh_access_token("token")
         assert new_token == "xyz"
 
     @aioresponses()
@@ -870,15 +995,18 @@
         last_args = {}
 
         def response_callback(url, **kwargs):
             last_args.update(kwargs)
             return CallbackResult(status=200, body="{}")
 
         mock.post(
-            API_VALIDATE_VERIFICATION_CODE_URLS["email"], callback=response_callback
+            ApiCommon(DEFAULT_BRAND).get_brand_url(
+                API_VALIDATE_VERIFICATION_CODE_URLS["email"]
+            ),
+            callback=response_callback,
         )
 
         api = ApiAsync(ClientSession())
         await api.async_validate_verification_code(
             ACCESS_TOKEN, "email", "emailaddress", 123456
         )
         assert last_args["json"] == {"code": "123456", "email": "emailaddress"}
@@ -930,15 +1058,18 @@
             try:
                 _raise_response_exceptions(mocked_response)
             except AugustApiAIOHTTPError as err:
                 self.assertEqual(str(err), ERROR_MAP[status_code])
 
     @aioresponses()
     async def test_async_get_usern(self, mock):
-        mock.get(API_GET_USER_URL, body='{"UserID": "abc"}')
+        mock.get(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_USER_URL),
+            body='{"UserID": "abc"}',
+        )
 
         api = ApiAsync(ClientSession())
         user_details = await api.async_get_user("token")
         assert user_details == {"UserID": "abc"}
 
 
 class MockedResponse(ClientResponse):
```

### Comparing `yalexs-1.3.3/tests/test_authenticator.py` & `yalexs-1.4.0/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/test_authenticator_async.py` & `yalexs-1.4.0/tests/test_authenticator_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from yalexs.api_async import ApiAsync
 from yalexs.api_common import (
     API_GET_HOUSES_URL,
     API_GET_SESSION_URL,
     API_SEND_VERIFICATION_CODE_URLS,
     API_VALIDATE_VERIFICATION_CODE_URLS,
     HEADER_AUGUST_ACCESS_TOKEN,
+    ApiCommon,
 )
 from yalexs.authenticator_async import (
     AuthenticationState,
     AuthenticatorAsync,
     ValidationResult,
 )
+from yalexs.const import DEFAULT_BRAND
 
 
 def format_datetime(dt):
     return dt.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3] + "Z"
 
 
 class TestAuthenticatorAsync(aiounittest.AsyncTestCase):
@@ -40,15 +42,15 @@
         self,
         mock_aioresponses,
         v_password,
         v_install_id,
         expires_at=format_datetime(datetime.utcnow()),
     ):
         mock_aioresponses.post(
-            API_GET_SESSION_URL,
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_SESSION_URL),
             headers={"x-august-access-token": "access_token"},
             body=json.dumps(
                 {
                     "expiresAt": expires_at,
                     "vPassword": v_password,
                     "vInstallId": v_install_id,
                 }
@@ -96,15 +98,17 @@
         self._setup_session_response(mock_aioresponses, True, True)
 
         authenticator = await self._async_create_authenticator_async(mock_aioresponses)
         await authenticator.async_authenticate()
 
         token = "e30=.eyJleHAiOjEzMzd9.e30="
         mock_aioresponses.get(
-            API_GET_HOUSES_URL, body=token, headers={HEADER_AUGUST_ACCESS_TOKEN: token}
+            ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_HOUSES_URL),
+            body=token,
+            headers={HEADER_AUGUST_ACCESS_TOKEN: token},
         )
 
         access_token = await authenticator.async_refresh_access_token(force=False)
 
         self.assertEqual(token, access_token.access_token)
         self.assertEqual(
             datetime.fromtimestamp(1337, tz=tzutc()),
@@ -167,58 +171,76 @@
         self.assertEqual(AuthenticationState.AUTHENTICATED, authentication.state)
 
     @aioresponses()
     async def test_async_send_verification_code(self, mock_aioresponses):
         self._setup_session_response(mock_aioresponses, True, False)
 
         authenticator = await self._async_create_authenticator_async(mock_aioresponses)
-        mock_aioresponses.post(API_SEND_VERIFICATION_CODE_URLS["phone"], body="{}")
+        mock_aioresponses.post(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(
+                API_SEND_VERIFICATION_CODE_URLS["phone"]
+            ),
+            body="{}",
+        )
         await authenticator.async_authenticate()
         result = await authenticator.async_send_verification_code()
 
         self.assertEqual(True, result)
 
     @aioresponses()
     async def test_async_validate_verification_code_with_no_code(
         self, mock_aioresponses
     ):
         self._setup_session_response(mock_aioresponses, True, False)
 
         authenticator = await self._async_create_authenticator_async(mock_aioresponses)
         await authenticator.async_authenticate()
 
-        mock_aioresponses.post(API_VALIDATE_VERIFICATION_CODE_URLS["phone"], body="{}")
+        mock_aioresponses.post(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(
+                API_VALIDATE_VERIFICATION_CODE_URLS["phone"]
+            ),
+            body="{}",
+        )
         result = await authenticator.async_validate_verification_code("")
 
         # mock_aioresponses.async_validate_verification_code.assert_not_called()
 
         self.assertEqual(ValidationResult.INVALID_VERIFICATION_CODE, result)
 
     @aioresponses()
     async def test_async_validate_verification_code_with_validated_response(
         self, mock_aioresponses
     ):
         self._setup_session_response(mock_aioresponses, True, False)
 
-        mock_aioresponses.post(API_VALIDATE_VERIFICATION_CODE_URLS["phone"], body="{}")
+        mock_aioresponses.post(
+            ApiCommon(DEFAULT_BRAND).get_brand_url(
+                API_VALIDATE_VERIFICATION_CODE_URLS["phone"]
+            ),
+            body="{}",
+        )
 
         authenticator = await self._async_create_authenticator_async(mock_aioresponses)
         await authenticator.async_authenticate()
         result = await authenticator.async_validate_verification_code("123456")
 
         self.assertEqual(ValidationResult.VALIDATED, result)
 
     @aioresponses()
     async def test_async_validate_verification_code_with_invalid_code_response(
         self, mock_aioresponses
     ):
         self._setup_session_response(mock_aioresponses, True, False)
 
         mock_aioresponses.post(
-            API_VALIDATE_VERIFICATION_CODE_URLS["phone"], exception=ClientError()
+            ApiCommon(DEFAULT_BRAND).get_brand_url(
+                API_VALIDATE_VERIFICATION_CODE_URLS["phone"]
+            ),
+            exception=ClientError(),
         )
 
         authenticator = await self._async_create_authenticator_async(mock_aioresponses)
         await authenticator.async_authenticate()
         result = await authenticator.async_validate_verification_code("123456")
 
         self.assertEqual(ValidationResult.INVALID_VERIFICATION_CODE, result)
```

### Comparing `yalexs-1.3.3/tests/test_pubnub_activity.py` & `yalexs-1.4.0/tests/test_pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tests/test_util.py` & `yalexs-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/tox.ini` & `yalexs-1.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/activity.py` & `yalexs-1.4.0/yalexs/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 
 import dateutil.parser
 
-from yalexs.lock import LockDoorStatus, LockStatus
-from yalexs.users import get_user_info
+from .lock import LockDoorStatus, LockStatus
+from .users import get_user_info
 
 ACTION_LOCK_ONETOUCHLOCK = "onetouchlock"
 ACTION_LOCK_ONETOUCHLOCK_2 = "one_touch_lock"
 ACTION_LOCK_LOCK = "lock"
 ACTION_RF_LOCK = "rf_lock"
 ACTION_RF_SECURE = "rf_secure"
 ACTION_RF_UNLOCK = "rf_unlock"
```

### Comparing `yalexs-1.3.3/yalexs/api.py` & `yalexs-1.4.0/yalexs/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,51 @@
 import json
 import logging
 import time
 
 from requests import Session, request
 from requests.exceptions import HTTPError
 
-from yalexs.api_common import (
+from .api_common import (
     API_LOCK_URL,
     API_RETRY_ATTEMPTS,
     API_RETRY_TIME,
     API_UNLOCK_URL,
     HEADER_ACCEPT_VERSION,
     HEADER_AUGUST_ACCESS_TOKEN,
     ApiCommon,
     _api_headers,
     _convert_lock_result_to_activities,
     _process_activity_json,
     _process_doorbells_json,
     _process_locks_json,
 )
-from yalexs.doorbell import DoorbellDetail
-from yalexs.exceptions import AugustApiHTTPError
-from yalexs.lock import LockDetail, determine_door_state, determine_lock_status
-from yalexs.pin import Pin
+from .const import DEFAULT_BRAND
+from .doorbell import DoorbellDetail
+from .exceptions import AugustApiHTTPError
+from .lock import LockDetail, determine_door_state, determine_lock_status
+from .pin import Pin
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Api(ApiCommon):
-    def __init__(self, timeout=10, command_timeout=60, http_session: Session = None):
+    """Legacy sync api."""
+
+    def __init__(
+        self,
+        timeout=10,
+        command_timeout=60,
+        http_session: Session = None,
+        brand=DEFAULT_BRAND,
+    ) -> None:
         self._timeout = timeout
         self._command_timeout = command_timeout
         self._http_session = http_session
+        super().__init__(brand)
 
     def get_session(self, install_id, identifier, password):
         return self._dict_to_api(
             self._build_get_session_request(install_id, identifier, password)
         )
 
     def send_verification_code(self, access_token, login_method, username):
```

### Comparing `yalexs-1.3.3/yalexs/api_async.py` & `yalexs-1.4.0/yalexs/api_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Api calls for sync."""
 
 import asyncio
 import logging
 
-from aiohttp import ClientResponseError, ServerDisconnectedError
+from aiohttp import ClientResponseError, ClientSession, ServerDisconnectedError
 
-from yalexs.api_common import (
+from .api_common import (
     API_LOCK_ASYNC_URL,
     API_LOCK_URL,
     API_RETRY_ATTEMPTS,
     API_RETRY_TIME,
     API_STATUS_ASYNC_URL,
     API_UNLOCK_ASYNC_URL,
     API_UNLOCK_URL,
@@ -19,27 +19,37 @@
     ApiCommon,
     _api_headers,
     _convert_lock_result_to_activities,
     _process_activity_json,
     _process_doorbells_json,
     _process_locks_json,
 )
-from yalexs.doorbell import DoorbellDetail
-from yalexs.exceptions import AugustApiAIOHTTPError
-from yalexs.lock import LockDetail, determine_door_state, determine_lock_status
-from yalexs.pin import Pin
+from .const import DEFAULT_BRAND
+from .doorbell import DoorbellDetail
+from .exceptions import AugustApiAIOHTTPError
+from .lock import LockDetail, determine_door_state, determine_lock_status
+from .pin import Pin
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ApiAsync(ApiCommon):
-    def __init__(self, aiohttp_session, timeout=10, command_timeout=60):
+    """Async api."""
+
+    def __init__(
+        self,
+        aiohttp_session: ClientSession,
+        timeout=10,
+        command_timeout=60,
+        brand=DEFAULT_BRAND,
+    ) -> None:
         self._timeout = timeout
         self._command_timeout = command_timeout
         self._aiohttp_session = aiohttp_session
+        super().__init__(brand)
 
     async def async_get_session(self, install_id, identifier, password):
         return await self._async_dict_to_api(
             self._build_get_session_request(install_id, identifier, password)
         )
 
     async def async_send_verification_code(self, access_token, login_method, username):
```

### Comparing `yalexs-1.3.3/yalexs/api_common.py` & `yalexs-1.4.0/yalexs/api_common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Api functions common between sync and async."""
 import logging
 from typing import Any, Dict
 
 import dateutil.parser
 
-from yalexs.activity import (
+from .activity import (
     ACTIVITY_ACTIONS_BRIDGE_OPERATION,
     ACTIVITY_ACTIONS_DOOR_OPERATION,
     ACTIVITY_ACTIONS_DOORBELL_DING,
     ACTIVITY_ACTIONS_DOORBELL_IMAGE_CAPTURE,
     ACTIVITY_ACTIONS_DOORBELL_MOTION,
     ACTIVITY_ACTIONS_DOORBELL_VIEW,
     ACTIVITY_ACTIONS_LOCK_OPERATION,
@@ -18,16 +18,17 @@
     DoorbellDingActivity,
     DoorbellImageCaptureActivity,
     DoorbellMotionActivity,
     DoorbellViewActivity,
     DoorOperationActivity,
     LockOperationActivity,
 )
-from yalexs.doorbell import Doorbell
-from yalexs.lock import Lock, LockDoorStatus, determine_door_state, door_state_to_string
+from .const import BASE_URLS, Brand
+from .doorbell import Doorbell
+from .lock import Lock, LockDoorStatus, determine_door_state, door_state_to_string
 
 API_RETRY_TIME = 2.5
 API_RETRY_ATTEMPTS = 10
 
 HEADER_ACCEPT_VERSION = "Accept-Version"
 HEADER_AUGUST_ACCESS_TOKEN = "x-august-access-token"  # nosec
 HEADER_AUGUST_API_KEY = "x-august-api-key"
@@ -39,45 +40,43 @@
 HEADER_VALUE_API_KEY = "7cab4bbd-2693-4fc1-b99b-dec0fb20f9d4"
 HEADER_VALUE_CONTENT_TYPE = "application/json; charset=UTF-8"
 HEADER_VALUE_USER_AGENT = "August/Luna-22.17.0 (Android; SDK 31; gphone64_arm64)"
 HEADER_VALUE_ACCEPT_VERSION = "0.0.1"
 HEADER_VALUE_AUGUST_BRANDING = "august"
 HEADER_VALUE_AUGUST_COUNTRY = "US"
 
-API_BASE_URL = "https://api-production.august.com"
-API_GET_SESSION_URL = API_BASE_URL + "/session"
+
+API_GET_SESSION_URL = "/session"
 API_SEND_VERIFICATION_CODE_URLS = {
-    "phone": API_BASE_URL + "/validation/phone",
-    "email": API_BASE_URL + "/validation/email",
+    "phone": "/validation/phone",
+    "email": "/validation/email",
 }
 API_VALIDATE_VERIFICATION_CODE_URLS = {
-    "phone": API_BASE_URL + "/validate/phone",
-    "email": API_BASE_URL + "/validate/email",
+    "phone": "/validate/phone",
+    "email": "/validate/email",
 }
-API_GET_HOUSE_ACTIVITIES_URL = API_BASE_URL + "/houses/{house_id}/activities"
-API_GET_DOORBELLS_URL = API_BASE_URL + "/users/doorbells/mine"
-API_GET_DOORBELL_URL = API_BASE_URL + "/doorbells/{doorbell_id}"
-API_WAKEUP_DOORBELL_URL = API_BASE_URL + "/doorbells/{doorbell_id}/wakeup"
-API_GET_HOUSES_URL = API_BASE_URL + "/users/houses/mine"
-API_GET_HOUSE_URL = API_BASE_URL + "/houses/{house_id}"
-API_GET_LOCKS_URL = API_BASE_URL + "/users/locks/mine"
-API_GET_LOCK_URL = API_BASE_URL + "/locks/{lock_id}"
-API_GET_LOCK_STATUS_URL = API_BASE_URL + "/locks/{lock_id}/status"
-API_GET_PINS_URL = API_BASE_URL + "/locks/{lock_id}/pins"
-API_LOCK_URL = API_BASE_URL + "/remoteoperate/{lock_id}/lock"
-API_UNLOCK_URL = API_BASE_URL + "/remoteoperate/{lock_id}/unlock"
-API_LOCK_ASYNC_URL = API_BASE_URL + "/remoteoperate/{lock_id}/lock?v=2.3.1&type=async"
-API_UNLOCK_ASYNC_URL = (
-    API_BASE_URL + "/remoteoperate/{lock_id}/unlock?v=2.3.1&type=async"
-)
+API_GET_HOUSE_ACTIVITIES_URL = "/houses/{house_id}/activities"
+API_GET_DOORBELLS_URL = "/users/doorbells/mine"
+API_GET_DOORBELL_URL = "/doorbells/{doorbell_id}"
+API_WAKEUP_DOORBELL_URL = "/doorbells/{doorbell_id}/wakeup"
+API_GET_HOUSES_URL = "/users/houses/mine"
+API_GET_HOUSE_URL = "/houses/{house_id}"
+API_GET_LOCKS_URL = "/users/locks/mine"
+API_GET_LOCK_URL = "/locks/{lock_id}"
+API_GET_LOCK_STATUS_URL = "/locks/{lock_id}/status"
+API_GET_PINS_URL = "/locks/{lock_id}/pins"
+API_LOCK_URL = "/remoteoperate/{lock_id}/lock"
+API_UNLOCK_URL = "/remoteoperate/{lock_id}/unlock"
+API_LOCK_ASYNC_URL = "/remoteoperate/{lock_id}/lock?v=2.3.1&type=async"
+API_UNLOCK_ASYNC_URL = "/remoteoperate/{lock_id}/unlock?v=2.3.1&type=async"
 API_STATUS_ASYNC_URL = (
-    API_BASE_URL + "/remoteoperate/{lock_id}/status?v=2.3.1&type=async&intent=wakeup"
+    "/remoteoperate/{lock_id}/status?v=2.3.1&type=async&intent=wakeup"
 )
 HYPER_BRIDGE_PARAM = "&connection=persistent"
-API_GET_USER_URL = API_BASE_URL + "/users/me"
+API_GET_USER_URL = "/users/me"
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def _api_headers(access_token=None):
     headers = {
         HEADER_ACCEPT_VERSION: HEADER_VALUE_ACCEPT_VERSION,
@@ -172,18 +171,26 @@
 def _process_locks_json(json_dict):
     return [Lock(device_id, data) for device_id, data in json_dict.items()]
 
 
 class ApiCommon:
     """Api dict shared between async and sync."""
 
+    def __init__(self, brand: Brand) -> None:
+        """Init."""
+        self._base_url = BASE_URLS[brand]
+
+    def get_brand_url(self, url_str: str) -> str:
+        """Get url."""
+        return self._base_url + url_str
+
     def _build_get_session_request(self, install_id, identifier, password):
         return {
             "method": "post",
-            "url": API_GET_SESSION_URL,
+            "url": self.get_brand_url(API_GET_SESSION_URL),
             "json": {
                 "installId": install_id,
                 "identifier": identifier,
                 "password": password,
             },
         }
 
@@ -193,105 +200,121 @@
         if login_method == "phone":
             json = {"smsHashString": "anY0ZsRmXw+", "value": username}
         else:
             json = {"value": username}
 
         return {
             "method": "post",
-            "url": API_SEND_VERIFICATION_CODE_URLS[login_method],
+            "url": self.get_brand_url(API_SEND_VERIFICATION_CODE_URLS[login_method]),
             "access_token": access_token,
             "json": json,
         }
 
     def _build_validate_verification_code_request(
         self, access_token, login_method, username, verification_code
     ):
         return {
             "method": "post",
-            "url": API_VALIDATE_VERIFICATION_CODE_URLS[login_method],
+            "url": self.get_brand_url(
+                API_VALIDATE_VERIFICATION_CODE_URLS[login_method]
+            ),
             "access_token": access_token,
             "json": {login_method: username, "code": str(verification_code)},
         }
 
     def _build_get_doorbells_request(self, access_token):
         return {
             "method": "get",
-            "url": API_GET_DOORBELLS_URL,
+            "url": self.get_brand_url(API_GET_DOORBELLS_URL),
             "access_token": access_token,
         }
 
     def _build_get_doorbell_detail_request(self, access_token, doorbell_id):
         return {
             "method": "get",
-            "url": API_GET_DOORBELL_URL.format(doorbell_id=doorbell_id),
+            "url": self.get_brand_url(
+                API_GET_DOORBELL_URL.format(doorbell_id=doorbell_id)
+            ),
             "access_token": access_token,
         }
 
     def _build_wakeup_doorbell_request(self, access_token, doorbell_id):
         return {
             "method": "put",
-            "url": API_WAKEUP_DOORBELL_URL.format(doorbell_id=doorbell_id),
+            "url": self.get_brand_url(
+                API_WAKEUP_DOORBELL_URL.format(doorbell_id=doorbell_id)
+            ),
             "access_token": access_token,
         }
 
     def _build_get_houses_request(self, access_token):
         return {"method": "get", "access_token": access_token}
 
     def _build_get_house_request(self, access_token, house_id):
         return {
             "method": "get",
-            "url": API_GET_HOUSE_URL.format(house_id=house_id),
+            "url": self.get_brand_url(API_GET_HOUSE_URL.format(house_id=house_id)),
             "access_token": access_token,
         }
 
     def _build_get_house_activities_request(self, access_token, house_id, limit=8):
         return {
             "method": "get",
-            "url": API_GET_HOUSE_ACTIVITIES_URL.format(house_id=house_id),
+            "url": self.get_brand_url(
+                API_GET_HOUSE_ACTIVITIES_URL.format(house_id=house_id)
+            ),
             "version": "4.0.0",
             "access_token": access_token,
             "params": {"limit": limit},
         }
 
     def _build_get_locks_request(self, access_token):
-        return {"method": "get", "url": API_GET_LOCKS_URL, "access_token": access_token}
+        return {
+            "method": "get",
+            "url": self.get_brand_url(API_GET_LOCKS_URL),
+            "access_token": access_token,
+        }
 
     def _build_get_user_request(self, access_token):
-        return {"method": "get", "url": API_GET_USER_URL, "access_token": access_token}
+        return {
+            "method": "get",
+            "url": self.get_brand_url(API_GET_USER_URL),
+            "access_token": access_token,
+        }
 
     def _build_get_lock_detail_request(self, access_token, lock_id):
         return {
             "method": "get",
-            "url": API_GET_LOCK_URL.format(lock_id=lock_id),
+            "url": self.get_brand_url(API_GET_LOCK_URL.format(lock_id=lock_id)),
             "access_token": access_token,
         }
 
     def _build_get_lock_status_request(self, access_token, lock_id):
         return {
             "method": "get",
-            "url": API_GET_LOCK_STATUS_URL.format(lock_id=lock_id),
+            "url": self.get_brand_url(API_GET_LOCK_STATUS_URL.format(lock_id=lock_id)),
             "access_token": access_token,
         }
 
     def _build_get_pins_request(self, access_token, lock_id):
         return {
             "method": "get",
-            "url": API_GET_PINS_URL.format(lock_id=lock_id),
+            "url": self.get_brand_url(API_GET_PINS_URL.format(lock_id=lock_id)),
             "access_token": access_token,
         }
 
     def _build_refresh_access_token_request(self, access_token):
         return {
             "method": "get",
-            "url": API_GET_HOUSES_URL,
+            "url": self.get_brand_url(API_GET_HOUSES_URL),
             "access_token": access_token,
         }
 
     def _build_call_lock_operation_request(
-        self, url_str, access_token, lock_id, timeout
-    ):
+        self, url_str: str, access_token: str, lock_id: str, timeout
+    ) -> Dict[str, Any]:
         return {
             "method": "put",
-            "url": url_str.format(lock_id=lock_id),
+            "url": self.get_brand_url(url_str.format(lock_id=lock_id)),
             "access_token": access_token,
             "timeout": timeout,
         }
```

### Comparing `yalexs-1.3.3/yalexs/authenticator.py` & `yalexs-1.4.0/yalexs/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from datetime import datetime, timedelta, timezone
 import json
 import logging
 import os
+from typing import Any
 
 import requests
 
-from yalexs.authenticator_common import (
+from .authenticator_common import (
     Authentication,
     AuthenticationState,
     AuthenticatorCommon,
     ValidationResult,
     from_authentication_json,
     to_authentication_json,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Authenticator(AuthenticatorCommon):
-    def __init__(self, *args, **kwargs):
+    """Class to manage authentication with the August API."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._setup_authentication()
 
     def _setup_authentication(self):
         access_token_cache_file = self._access_token_cache_file
         if access_token_cache_file is not None and os.path.exists(
             access_token_cache_file
```

### Comparing `yalexs-1.3.3/yalexs/authenticator_async.py` & `yalexs-1.4.0/yalexs/authenticator_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 import json
 import logging
 import os
 
 import aiofiles
 from aiohttp import ClientError
 
-from yalexs.authenticator_common import (
+from .authenticator_common import (
     Authentication,
     AuthenticationState,
     AuthenticatorCommon,
     ValidationResult,
     from_authentication_json,
     to_authentication_json,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AuthenticatorAsync(AuthenticatorCommon):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    """Class to manage authentication with the August API."""
 
     async def async_setup_authentication(self):
         access_token_cache_file = self._access_token_cache_file
         if access_token_cache_file is not None and os.path.exists(
             access_token_cache_file
         ):
             async with aiofiles.open(access_token_cache_file, "r") as file:
```

### Comparing `yalexs-1.3.3/yalexs/authenticator_common.py` & `yalexs-1.4.0/yalexs/authenticator_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime, timedelta, timezone
 from enum import Enum
 import json
 import logging
+from typing import Any, Optional
 import uuid
 
 import dateutil.parser
 import jwt
 
-from yalexs.api import HEADER_AUGUST_ACCESS_TOKEN
+from .api import HEADER_AUGUST_ACCESS_TOKEN, ApiCommon
 
 # The default time before expiration to refresh a token
 DEFAULT_RENEWAL_THRESHOLD = timedelta(days=7)
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -90,34 +91,37 @@
     VALIDATED = "validated"
     INVALID_VERIFICATION_CODE = "invalid_verification_code"
 
 
 class AuthenticatorCommon:
     def __init__(
         self,
-        api,
-        login_method,
-        username,
-        password,
-        install_id=None,
-        access_token_cache_file=None,
-        access_token_renewal_threshold=DEFAULT_RENEWAL_THRESHOLD,
-    ):
+        api: ApiCommon,
+        login_method: str,
+        username: str,
+        password: str,
+        install_id: Optional[str] = None,
+        access_token_cache_file: Optional[str] = None,
+        access_token_renewal_threshold: timedelta = DEFAULT_RENEWAL_THRESHOLD,
+    ) -> None:
         self._api = api
         self._login_method = login_method
         self._username = username
         self._password = password
         self._install_id = install_id
         self._access_token_cache_file = access_token_cache_file
         self._access_token_renewal_threshold = access_token_renewal_threshold
         self._authentication = None
 
     def _authentication_from_session_response(
-        self, install_id, response_headers, json_dict
-    ):
+        self,
+        install_id: str,
+        response_headers: dict[str, Any],
+        json_dict: dict[str, Any],
+    ) -> Authentication:
         access_token = response_headers[HEADER_AUGUST_ACCESS_TOKEN]
         access_token_expires = json_dict["expiresAt"]
         v_password = json_dict["vPassword"]
         v_install_id = json_dict["vInstallId"]
 
         if not v_password:
             state = AuthenticationState.BAD_PASSWORD
```

### Comparing `yalexs-1.3.3/yalexs/bridge.py` & `yalexs-1.4.0/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/device.py` & `yalexs-1.4.0/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/doorbell.py` & `yalexs-1.4.0/yalexs/doorbell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 import dateutil.parser
 import requests
 
-from yalexs.device import Device, DeviceDetail
+from .device import Device, DeviceDetail
 
 DOORBELL_STATUS_KEY = "status"
 
 
 class Doorbell(Device):
     def __init__(self, device_id, data):
         super().__init__(device_id, data["name"], data["HouseID"])
```

### Comparing `yalexs-1.3.3/yalexs/keypad.py` & `yalexs-1.4.0/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/lock.py` & `yalexs-1.4.0/yalexs/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/pin.py` & `yalexs-1.4.0/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/pubnub_activity.py` & `yalexs-1.4.0/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/pubnub_async.py` & `yalexs-1.4.0/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/users.py` & `yalexs-1.4.0/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs/util.py` & `yalexs-1.4.0/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.3/yalexs.egg-info/PKG-INFO` & `yalexs-1.4.0/yalexs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.3.3
+Version: 1.4.0
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.3.3/yalexs.egg-info/SOURCES.txt` & `yalexs-1.4.0/yalexs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,25 @@
 yalexs/api.py
 yalexs/api_async.py
 yalexs/api_common.py
 yalexs/authenticator.py
 yalexs/authenticator_async.py
 yalexs/authenticator_common.py
 yalexs/bridge.py
+yalexs/const.py
 yalexs/device.py
 yalexs/doorbell.py
 yalexs/exceptions.py
 yalexs/keypad.py
 yalexs/lock.py
 yalexs/pin.py
 yalexs/pubnub_activity.py
 yalexs/pubnub_async.py
 yalexs/users.py
 yalexs/util.py
 yalexs.egg-info/PKG-INFO
 yalexs.egg-info/SOURCES.txt
 yalexs.egg-info/dependency_links.txt
 yalexs.egg-info/requires.txt
-yalexs.egg-info/top_level.txt
+yalexs.egg-info/top_level.txt
+yalexs/backports/__init__.py
+yalexs/backports/enum.py
```

