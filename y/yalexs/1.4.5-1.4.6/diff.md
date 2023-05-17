# Comparing `tmp/yalexs-1.4.5.tar.gz` & `tmp/yalexs-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.4.5.tar", last modified: Wed May 17 20:48:40 2023, max compression
+gzip compressed data, was "yalexs-1.4.6.tar", last modified: Wed May 17 21:49:22 2023, max compression
```

## Comparing `yalexs-1.4.5.tar` & `yalexs-1.4.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.484943 yalexs-1.4.5/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.469934 yalexs-1.4.5/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.472470 yalexs-1.4.5/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.5/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.5/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.5/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.5/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 20:48:40.485030 yalexs-1.4.5/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.5/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.5/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.5/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.5/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.5/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.4.5/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 20:48:40.485317 yalexs-1.4.5/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 20:48:19.000000 yalexs-1.4.5/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.474428 yalexs-1.4.5/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.480459 yalexs-1.4.5/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.5/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.5/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    42239 2023-05-17 15:01:17.000000 yalexs-1.4.5/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.5/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.5/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-05-17 04:41:53.000000 yalexs-1.4.5/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.5/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.5/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.483966 yalexs-1.4.5/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 20:48:19.000000 yalexs-1.4.5/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 17:35:49.000000 yalexs-1.4.5/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.4.5/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14528 2023-05-17 18:54:43.000000 yalexs-1.4.5/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    11611 2023-05-17 18:54:43.000000 yalexs-1.4.5/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.5/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.4.5/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.5/yalexs/authenticator_common.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.484825 yalexs-1.4.5/yalexs/backports/
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.5/yalexs/backports/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.5/yalexs/backports/enum.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.5/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1100 2023-05-17 20:48:17.000000 yalexs-1.4.5/yalexs/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.5/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.5/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      717 2023-05-17 15:01:17.000000 yalexs-1.4.5/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.5/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.5/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.5/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-05-17 04:41:53.000000 yalexs-1.4.5/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4502 2023-05-17 20:48:17.000000 yalexs-1.4.5/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.5/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.5/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 20:48:40.484636 yalexs-1.4.5/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 20:48:40.000000 yalexs-1.4.5/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 20:48:40.000000 yalexs-1.4.5/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 20:48:40.000000 yalexs-1.4.5/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 20:48:40.000000 yalexs-1.4.5/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 20:48:40.000000 yalexs-1.4.5/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.451650 yalexs-1.4.6/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.438040 yalexs-1.4.6/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.440323 yalexs-1.4.6/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.4.6/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.4.6/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.4.6/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.4.6/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 21:49:22.451727 yalexs-1.4.6/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.4.6/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.4.6/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.4.6/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.4.6/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.4.6/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-05-17 21:24:49.000000 yalexs-1.4.6/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-17 21:49:22.452006 yalexs-1.4.6/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1027 2023-05-17 21:45:28.000000 yalexs-1.4.6/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.441727 yalexs-1.4.6/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.447492 yalexs-1.4.6/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.4.6/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.4.6/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    42924 2023-05-17 21:45:20.000000 yalexs-1.4.6/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.4.6/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.4.6/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    16539 2023-05-17 21:25:12.000000 yalexs-1.4.6/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.4.6/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.4.6/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.450786 yalexs-1.4.6/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-17 21:45:28.000000 yalexs-1.4.6/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14168 2023-05-17 17:35:49.000000 yalexs-1.4.6/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.4.6/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15146 2023-05-17 21:45:20.000000 yalexs-1.4.6/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11642 2023-05-17 21:45:20.000000 yalexs-1.4.6/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.4.6/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5279 2023-05-17 16:13:22.000000 yalexs-1.4.6/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.451541 yalexs-1.4.6/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1100 2023-05-17 20:48:17.000000 yalexs-1.4.6/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4278 2023-05-17 14:08:38.000000 yalexs-1.4.6/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      776 2023-05-17 21:45:20.000000 yalexs-1.4.6/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.4.6/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4555 2023-05-17 21:25:12.000000 yalexs-1.4.6/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4502 2023-05-17 20:48:17.000000 yalexs-1.4.6/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.4.6/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.4.6/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-17 21:49:22.451373 yalexs-1.4.6/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2869 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-17 21:49:22.000000 yalexs-1.4.6/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.4.5/.github/workflows/ci.yaml` & `yalexs-1.4.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/.gitignore` & `yalexs-1.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/LICENSE` & `yalexs-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/PKG-INFO` & `yalexs-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.5/README.md` & `yalexs-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/known_activities.md` & `yalexs-1.4.6/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/pylintrc` & `yalexs-1.4.6/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/setup.cfg` & `yalexs-1.4.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.5
+current_version = 1.4.6
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.4.5/setup.py` & `yalexs-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.4.5",
+    version="1.4.6",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-1.4.5/tests/fixtures/auto_relock_activity.json` & `yalexs-1.4.6/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.4.6/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.4.6/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/door_closed_activity.json` & `yalexs-1.4.6/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.4.6/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/door_open_activity.json` & `yalexs-1.4.6/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.4.6/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.4.6/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.4.6/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.4.6/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbell.json` & `yalexs-1.4.6/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.4.6/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.4.6/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_doorbells.json` & `yalexs-1.4.6/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_house_activities.json` & `yalexs-1.4.6/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.4.6/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.4.6/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock.offline.json` & `yalexs-1.4.6/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock.online.json` & `yalexs-1.4.6/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.4.6/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.4.6/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/get_pins.json` & `yalexs-1.4.6/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.4.6/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/lock.json` & `yalexs-1.4.6/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/lock_activity.json` & `yalexs-1.4.6/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.4.6/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/remote_lock_activity.json` & `yalexs-1.4.6/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.4.6/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/unlock.json` & `yalexs-1.4.6/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/unlock_activity.json` & `yalexs-1.4.6/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.4.6/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/test_activity.py` & `yalexs-1.4.6/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/test_api.py` & `yalexs-1.4.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/test_api_async.py` & `yalexs-1.4.6/tests/test_api_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from datetime import datetime
 import os
 from unittest import mock
+from unittest.mock import patch
 
-from aiohttp import ClientResponse, ClientSession
+from aiohttp import ClientOSError, ClientResponse, ClientSession
 from aiohttp.helpers import TimerNoop
 from aioresponses import CallbackResult, aioresponses
 import aiounittest
 import dateutil.parser
 from dateutil.tz import tzlocal, tzutc
+import pytest
 from yarl import URL
 
+from yalexs import api_async
 import yalexs.activity
 from yalexs.api_async import ApiAsync, _raise_response_exceptions
 from yalexs.api_common import (
     API_GET_DOORBELL_URL,
     API_GET_DOORBELLS_URL,
     API_GET_HOUSE_ACTIVITIES_URL,
     API_GET_HOUSES_URL,
@@ -975,14 +978,32 @@
         self.assertIsInstance(activities[5], yalexs.activity.DoorOperationActivity)
         self.assertIsInstance(activities[6], yalexs.activity.DoorOperationActivity)
         self.assertIsInstance(activities[7], yalexs.activity.DoorOperationActivity)
         self.assertIsInstance(activities[8], yalexs.activity.LockOperationActivity)
         self.assertIsInstance(activities[9], yalexs.activity.LockOperationActivity)
 
     @aioresponses()
+    async def test_async_get_retry_raises_our_exception_class(self, mock):
+        house_id = 1234
+
+        mock.get(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_HOUSE_ACTIVITIES_URL)
+            .format(house_id=house_id)
+            + "?limit=8",
+            exception=ClientOSError("any"),
+        )
+
+        api = ApiAsync(ClientSession())
+        with patch.object(api_async, "API_EXCEPTION_RETRY_TIME", 0), pytest.raises(
+            AugustApiAIOHTTPError
+        ):
+            await api.async_get_house_activities(ACCESS_TOKEN, house_id)
+
+    @aioresponses()
     async def test_async_refresh_access_token(self, mock):
         mock.get(
             ApiCommon(DEFAULT_BRAND).get_brand_url(API_GET_HOUSES_URL),
             body="{}",
             headers={"x-august-access-token": "xyz"},
         )
```

### Comparing `yalexs-1.4.5/tests/test_authenticator.py` & `yalexs-1.4.6/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/test_authenticator_async.py` & `yalexs-1.4.6/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tests/test_pubnub_activity.py` & `yalexs-1.4.6/tests/test_pubnub_activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -394,7 +394,42 @@
                     "doorbellName": "Front Door",
                     "origin": "mars-api",
                 },
             },
         )
         assert isinstance(activities[0], DoorbellDingActivity)
         assert "DoorbellDingActivity" in str(activities[0])
+
+
+class TestBridge(unittest.TestCase):
+    def test_update_bridge_details_from_pubnub_message(self):
+        lock = LockDetail(json.loads(load_fixture("get_lock.doorsense_init.json")))
+        self.assertEqual("A6697750D607098BAE8D6BAA11EF8063", lock.device_id)
+        self.assertEqual(LockStatus.LOCKED, lock.lock_status)
+        self.assertEqual(LockDoorStatus.DISABLED, lock.door_state)
+
+        activities = activities_from_pubnub_message(
+            lock,
+            dateutil.parser.parse("2017-12-10T05:48:30.272Z"),
+            {
+                "remoteEvent": 1,
+                "status": "unknown",
+                "result": "failed",
+                "error": {
+                    "jse_shortmsg": "",
+                    "jse_info": {},
+                    "message": "Bridge is offline",
+                    "statusCode": 422,
+                    "body": {"code": 98, "message": "Bridge is offline"},
+                    "restCode": 98,
+                    "name": "ERRNO_BRIDGE_OFFLINE",
+                    "code": "Error",
+                },
+                "info": {
+                    "lockID": "45E3635D35B9471FAF1218885816E90D",
+                    "action": "status",
+                },
+            },
+        )
+        assert isinstance(activities[0], BridgeOperationActivity)
+        assert "BridgeOperationActivity" in str(activities[0])
+        assert activities[0].action == "associated_bridge_offline"
```

### Comparing `yalexs-1.4.5/tests/test_util.py` & `yalexs-1.4.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/tox.ini` & `yalexs-1.4.6/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/activity.py` & `yalexs-1.4.6/yalexs/activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/api.py` & `yalexs-1.4.6/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/api_async.py` & `yalexs-1.4.6/yalexs/api_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import asyncio
 from http import HTTPStatus
 import logging
 from typing import Any, Dict, List, Tuple, Union
 
 from aiohttp import (
+    ClientConnectionError,
+    ClientOSError,
     ClientResponse,
     ClientResponseError,
     ClientSession,
+    ClientSSLError,
     ServerDisconnectedError,
 )
 
 from .api_common import (
+    API_EXCEPTION_RETRY_TIME,
     API_LOCK_ASYNC_URL,
     API_LOCK_URL,
     API_RETRY_ATTEMPTS,
     API_RETRY_TIME,
     API_STATUS_ASYNC_URL,
     API_UNLOCK_ASYNC_URL,
     API_UNLOCK_URL,
@@ -364,16 +368,28 @@
             )
 
         attempts = 0
         while attempts < API_RETRY_ATTEMPTS:
             attempts += 1
             try:
                 response = await self._aiohttp_session.request(method, url, **api_dict)
-            except ServerDisconnectedError:
+            except (
+                ClientOSError,
+                ClientSSLError,
+                ServerDisconnectedError,
+                ClientConnectionError,
+            ) as ex:
                 # Try again if we get disconnected
+                # We may get [Errno 104] Connection reset by peer or a
+                # transient disconnect/SSL error
+                if attempts == API_RETRY_ATTEMPTS:
+                    raise AugustApiAIOHTTPError(
+                        f"Failed to connect to August API: {ex}", ex
+                    ) from ex
+                await asyncio.sleep(API_EXCEPTION_RETRY_TIME)
                 continue
             if debug_enabled:
                 _LOGGER.debug(
                     "Received API response from url: %s, code: %s, headers: %s, content: %s",
                     url,
                     response.status,
                     response.headers,
```

### Comparing `yalexs-1.4.5/yalexs/api_common.py` & `yalexs-1.4.6/yalexs/api_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     DoorOperationActivity,
     LockOperationActivity,
 )
 from .const import BASE_URLS, BRANDING, Brand
 from .doorbell import Doorbell
 from .lock import Lock, LockDoorStatus, determine_door_state, door_state_to_string
 
+API_EXCEPTION_RETRY_TIME = 0.1
 API_RETRY_TIME = 2.5
 API_RETRY_ATTEMPTS = 10
 
 HEADER_ACCEPT_VERSION = "Accept-Version"
 HEADER_AUGUST_ACCESS_TOKEN = "x-august-access-token"  # nosec
 HEADER_AUGUST_API_KEY = "x-august-api-key"
 HEADER_AUGUST_BRANDING = "x-august-branding"
```

### Comparing `yalexs-1.4.5/yalexs/authenticator.py` & `yalexs-1.4.6/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/authenticator_async.py` & `yalexs-1.4.6/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/authenticator_common.py` & `yalexs-1.4.6/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/backports/enum.py` & `yalexs-1.4.6/yalexs/backports/enum.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/bridge.py` & `yalexs-1.4.6/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/const.py` & `yalexs-1.4.6/yalexs/const.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/device.py` & `yalexs-1.4.6/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/doorbell.py` & `yalexs-1.4.6/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/exceptions.py` & `yalexs-1.4.6/yalexs/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from http import HTTPStatus
 
-from aiohttp import ClientResponseError
+from aiohttp import ClientError, ClientResponseError
 from requests.exceptions import HTTPError
 
 
 class AugustApiAIOHTTPError(Exception):
     """An yale access api error with a friendly user consumable string."""
 
-    def __init__(
-        self, message: str, aiohttp_client_response_exception: ClientResponseError
-    ) -> None:
+    def __init__(self, message: str, aiohttp_client_error: ClientError) -> None:
         """Initialize the error."""
         super().__init__(message)
-        self.status = aiohttp_client_response_exception.status
+        self.status = (
+            isinstance(aiohttp_client_error, ClientResponseError)
+            and aiohttp_client_error.status
+        )
         self.auth_failed = self.status in (
             HTTPStatus.UNAUTHORIZED,
             HTTPStatus.FORBIDDEN,
         )
 
 
 class AugustApiHTTPError(HTTPError):
```

### Comparing `yalexs-1.4.5/yalexs/keypad.py` & `yalexs-1.4.6/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/lock.py` & `yalexs-1.4.6/yalexs/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/pin.py` & `yalexs-1.4.6/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/pubnub_activity.py` & `yalexs-1.4.6/yalexs/pubnub_activity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from datetime import datetime
 from typing import Any, Dict
 
-from yalexs.activity import (
+from .activity import (
     ACTION_BRIDGE_OFFLINE,
     ACTION_BRIDGE_ONLINE,
     ACTION_DOOR_CLOSED,
     ACTION_DOOR_OPEN,
     ACTION_DOORBELL_BUTTON_PUSHED,
     ACTION_DOORBELL_IMAGE_CAPTURE,
     ACTION_DOORBELL_MOTION_DETECTED,
     ACTION_LOCK_JAMMED,
     ACTION_LOCK_LOCK,
     ACTION_LOCK_LOCKING,
     ACTION_LOCK_UNLOCK,
     ACTION_LOCK_UNLOCKING,
     SOURCE_PUBNUB,
 )
-from yalexs.api_common import _activity_from_dict
-from yalexs.doorbell import DOORBELL_STATUS_KEY, DoorbellDetail
-from yalexs.lock import (
+from .api_common import _activity_from_dict, _datetime_string_to_epoch
+from .device import Device
+from .doorbell import DOORBELL_STATUS_KEY, DoorbellDetail
+from .lock import (
     DOOR_STATE_KEY,
     LOCK_STATUS_KEY,
     LockDetail,
     LockDoorStatus,
     LockStatus,
     determine_door_state,
     determine_lock_status,
 )
 
-from .api_common import _datetime_string_to_epoch
-from .device import Device
-
 
 def activities_from_pubnub_message(
     device: Device, date_time: datetime, message: Dict[str, Any]
 ):
     """Create activities from pubnub."""
     activities = []
     activity_dict = {
@@ -61,16 +59,18 @@
         # Only accept a UserID if we have a date/time
         # as otherwise it is a duplicate of the previous
         # activity
         if accept_user and calling_user_id:
             activity_dict["callingUser"] = {"UserID": calling_user_id}
         if "remoteEvent" in message:
             activity_dict["info"]["remote"] = True
-
-        if LOCK_STATUS_KEY in message:
+        error = message.get("error") or {}
+        if error.get("restCode") == 98 or error.get("name") == "ERRNO_BRIDGE_OFFLINE":
+            _add_activity(activities, activity_dict, ACTION_BRIDGE_OFFLINE)
+        elif LOCK_STATUS_KEY in message:
             status = message[LOCK_STATUS_KEY]
             if status == ACTION_BRIDGE_ONLINE:
                 _add_activity(activities, activity_dict, ACTION_BRIDGE_ONLINE)
             elif status == ACTION_BRIDGE_OFFLINE:
                 _add_activity(activities, activity_dict, ACTION_BRIDGE_OFFLINE)
             lock_status = determine_lock_status(status)
             if lock_status == LockStatus.LOCKED:
```

### Comparing `yalexs-1.4.5/yalexs/pubnub_async.py` & `yalexs-1.4.6/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/users.py` & `yalexs-1.4.6/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs/util.py` & `yalexs-1.4.6/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.4.5/yalexs.egg-info/PKG-INFO` & `yalexs-1.4.6/yalexs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.4.5/yalexs.egg-info/SOURCES.txt` & `yalexs-1.4.6/yalexs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

