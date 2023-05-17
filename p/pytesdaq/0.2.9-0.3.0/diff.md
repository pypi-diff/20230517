# Comparing `tmp/pytesdaq-0.2.9.tar.gz` & `tmp/pytesdaq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesdaq-0.2.9.tar", last modified: Wed Jan 25 20:39:40 2023, max compression
+gzip compressed data, was "pytesdaq-0.3.0.tar", last modified: Fri Feb  3 00:34:24 2023, max compression
```

## Comparing `pytesdaq-0.2.9.tar` & `pytesdaq-0.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.203915 pytesdaq-0.2.9/pytesdaq/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.203915 pytesdaq-0.2.9/pytesdaq/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/analyzer/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.203915 pytesdaq-0.2.9/pytesdaq/config/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25099 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/daq/daq.py
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/daq/nidaqtask.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/daq/polaris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/display/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/display/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    78448 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/feb/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/feb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/feb/feb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/imacrt/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/imacrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/imacrt/imacrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/imacrt/macrtmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/keysight/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/keysight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/keysight/keysight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/lakeshore/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/lakeshore/lakeshore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/magnicon/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/magnicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/magnicon/magnicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.207915 pytesdaq-0.2.9/pytesdaq/instruments/niadc/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/niadc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/instruments/niadc/nidevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/pytesdaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23183 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/io/filter_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    67076 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/io/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/pytesdaq/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61215 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/processing/_iv_didv_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/processing/_iv_didv_tools_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/processing/_process_iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/processing/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/pytesdaq/scope/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/scope/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/scope/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/pytesdaq/sequencer/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/sequencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32482 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/sequencer/iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/sequencer/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/sequencer/tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/pytesdaq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/pytesdaq/utils/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:40.203915 pytesdaq-0.2.9/pytesdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-25 20:39:40.000000 pytesdaq-0.2.9/pytesdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-01-25 20:39:40.000000 pytesdaq-0.2.9/pytesdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:39:40.000000 pytesdaq-0.2.9/pytesdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:39:39.000000 pytesdaq-0.2.9/pytesdaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-25 20:39:40.000000 pytesdaq-0.2.9/pytesdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-25 20:39:40.000000 pytesdaq-0.2.9/pytesdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:39:40.211916 pytesdaq-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-25 20:39:30.000000 pytesdaq-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.520010 pytesdaq-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-03 00:34:24.520010 pytesdaq-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.508010 pytesdaq-0.3.0/pytesdaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.512010 pytesdaq-0.3.0/pytesdaq/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/analyzer/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.512010 pytesdaq-0.3.0/pytesdaq/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25099 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.512010 pytesdaq-0.3.0/pytesdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/daq/daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/daq/nidaqtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/daq/polaris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.512010 pytesdaq-0.3.0/pytesdaq/display/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/display/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.512010 pytesdaq-0.3.0/pytesdaq/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78448 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/instruments/feb/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/feb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/feb/feb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/instruments/imacrt/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/imacrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/imacrt/imacrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/imacrt/macrtmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/instruments/keysight/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/keysight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/keysight/keysight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/instruments/lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/lakeshore/lakeshore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/instruments/magnicon/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/magnicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/magnicon/magnicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/instruments/niadc/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/niadc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/instruments/niadc/nidevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23183 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/io/filter_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65885 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/io/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61215 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/processing/_iv_didv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/processing/_iv_didv_tools_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/processing/_process_iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/processing/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/scope/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/scope/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.516010 pytesdaq-0.3.0/pytesdaq/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/sequencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32482 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/sequencer/iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/sequencer/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/sequencer/tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.520010 pytesdaq-0.3.0/pytesdaq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/pytesdaq/utils/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:34:24.512010 pytesdaq-0.3.0/pytesdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-03 00:34:24.000000 pytesdaq-0.3.0/pytesdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-03 00:34:24.000000 pytesdaq-0.3.0/pytesdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 00:34:24.000000 pytesdaq-0.3.0/pytesdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 00:34:24.000000 pytesdaq-0.3.0/pytesdaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-03 00:34:24.000000 pytesdaq-0.3.0/pytesdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-03 00:34:24.000000 pytesdaq-0.3.0/pytesdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 00:34:24.520010 pytesdaq-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-03 00:34:13.000000 pytesdaq-0.3.0/setup.py
```

### Comparing `pytesdaq-0.2.9/PKG-INFO` & `pytesdaq-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.2.9
+Version: 0.3.0
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.2.9/README.md` & `pytesdaq-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/analyzer/analyzer.py` & `pytesdaq-0.3.0/pytesdaq/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/config/settings.py` & `pytesdaq-0.3.0/pytesdaq/config/settings.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/daq/daq.py` & `pytesdaq-0.3.0/pytesdaq/daq/daq.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/daq/nidaqtask.py` & `pytesdaq-0.3.0/pytesdaq/daq/nidaqtask.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/daq/polaris.py` & `pytesdaq-0.3.0/pytesdaq/daq/polaris.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/display/series.py` & `pytesdaq-0.3.0/pytesdaq/display/series.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/communication.py` & `pytesdaq-0.3.0/pytesdaq/instruments/communication.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/control.py` & `pytesdaq-0.3.0/pytesdaq/instruments/control.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/feb/feb.py` & `pytesdaq-0.3.0/pytesdaq/instruments/feb/feb.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/imacrt/imacrt.py` & `pytesdaq-0.3.0/pytesdaq/instruments/imacrt/imacrt.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/imacrt/macrtmodule.py` & `pytesdaq-0.3.0/pytesdaq/instruments/imacrt/macrtmodule.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/keysight/keysight.py` & `pytesdaq-0.3.0/pytesdaq/instruments/keysight/keysight.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/lakeshore/lakeshore.py` & `pytesdaq-0.3.0/pytesdaq/instruments/lakeshore/lakeshore.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/magnicon/magnicon.py` & `pytesdaq-0.3.0/pytesdaq/instruments/magnicon/magnicon.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/instruments/niadc/nidevice.py` & `pytesdaq-0.3.0/pytesdaq/instruments/niadc/nidevice.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/io/filter_hdf5.py` & `pytesdaq-0.3.0/pytesdaq/io/filter_hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/io/hdf5.py` & `pytesdaq-0.3.0/pytesdaq/io/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -800,3394 +800,3319 @@
 000031f0: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
 00003200: 6620 696e 636c 7564 655f 6d65 7461 6461  f include_metada
 00003210: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
 00003220: 7265 7475 726e 2061 7272 6179 2c20 696e  return array, in
 00003230: 666f 0a20 2020 2020 2020 2065 6c73 653a  fo.        else:
 00003240: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
 00003250: 7572 6e20 6172 7261 790a 2020 2020 2020  urn array.      
-00003260: 2020 0a0a 0a0a 0a0a 0a20 2020 200a 2020    .......    .  
-00003270: 2020 0a20 2020 2064 6566 2072 6561 645f    .    def read_
-00003280: 6d61 6e79 5f65 7665 6e74 7328 7365 6c66  many_events(self
-00003290: 2c20 6669 6c65 7061 7468 3d4e 6f6e 652c  , filepath=None,
-000032a0: 206e 6576 656e 7473 3d30 2c20 6f75 7470   nevents=0, outp
-000032b0: 7574 5f66 6f72 6d61 743d 312c 0a20 2020  ut_format=1,.   
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2020 2020 6465 7465 6374 6f72 5f63        detector_c
-000032e0: 6861 6e73 3d4e 6f6e 652c 0a20 2020 2020  hans=None,.     
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 2020 6576 656e 745f 6e75 6d73 3d4e      event_nums=N
-00003310: 6f6e 652c 2073 6572 6965 735f 6e75 6d73  one, series_nums
-00003320: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 696e 636c 7564 655f 6d65 7461 6461 7461  include_metadata
-00003350: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003370: 2061 6463 746f 766f 6c74 3d46 616c 7365   adctovolt=False
-00003380: 2c20 6164 6374 6f61 6d70 3d46 616c 7365  , adctoamp=False
-00003390: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000033a0: 2020 2020 2020 2020 2020 2062 6173 656c             basel
-000033b0: 696e 6573 7562 3d46 616c 7365 2c20 6261  inesub=False, ba
-000033c0: 7365 6c69 6e65 696e 6473 3d4e 6f6e 652c  selineinds=None,
-000033d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033e0: 2020 2020 2020 2020 2020 6d65 6d6f 7279            memory
-000033f0: 5f6c 696d 6974 3d32 2c20 6164 635f 6e61  _limit=2, adc_na
-00003400: 6d65 3d27 6164 6331 2729 3a0a 2020 2020  me='adc1'):.    
-00003410: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003420: 5265 6164 206d 756c 7469 706c 6520 6576  Read multiple ev
-00003430: 656e 7473 2028 6465 6661 756c 7420 7265  ents (default re
-00003440: 6164 2061 6c6c 2065 7665 6e74 7329 0a20  ad all events). 
-00003450: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003460: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00003470: 2020 202d 2d2d 2d2d 2d2d 2d2d 0a20 2020     ---------.   
-00003480: 2020 2020 2066 696c 6570 6174 683a 2073       filepath: s
-00003490: 7472 696e 6720 6f72 206c 6973 7420 206f  tring or list  o
-000034a0: 6620 7374 7269 6e67 730a 2020 2020 2020  f strings.      
-000034b0: 2020 2020 2066 696c 652f 7061 7468 206f       file/path o
-000034c0: 7220 6c69 7374 206f 6620 6669 6c65 732f  r list of files/
-000034d0: 7061 7468 7320 2864 6566 6175 6c74 3a20  paths (default: 
-000034e0: 7573 6520 6375 7272 656e 7420 6669 6c65  use current file
-000034f0: 290a 2020 2020 2020 2020 2020 0a20 2020  ).          .   
-00003500: 2020 2020 206e 6576 656e 7473 3a20 696e       nevents: in
-00003510: 7465 6765 720a 2020 2020 2020 2020 2020  teger.          
-00003520: 206e 756d 6265 7220 6f66 2065 7665 6e74   number of event
-00003530: 7320 746f 2072 6561 6420 2028 6465 6661  s to read  (defa
-00003540: 756c 7420 6e62 5f65 7665 6e74 733d 3020  ult nb_events=0 
-00003550: 2d3e 2061 6c6c 2065 7665 6e74 7320 696e  -> all events in
-00003560: 2064 756d 7073 290a 0a20 2020 2020 2020   dumps)..       
-00003570: 206f 7574 7075 745f 666f 726d 6174 3a20   output_format: 
-00003580: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-00003590: 2020 2020 313a 206c 6973 7420 6f66 2032      1: list of 2
-000035a0: 4420 6e64 6172 7261 795b 6368 616e 2c20  D ndarray[chan, 
-000035b0: 7361 6d70 6c65 735d 0a20 2020 2020 2020  samples].       
-000035c0: 2020 2020 2032 3a20 3344 206e 6461 7272       2: 3D ndarr
-000035d0: 6179 5b65 7665 6e74 2c20 6368 616e 2c20  ay[event, chan, 
-000035e0: 7361 6d70 6c65 735d 0a20 0a20 2020 2020  samples]. .     
-000035f0: 2020 2064 6574 6563 746f 725f 6368 616e     detector_chan
-00003600: 733a 2073 7472 696e 672f 696e 7420 6f72  s: string/int or
-00003610: 206c 6973 7420 6f66 2073 7472 696e 672f   list of string/
-00003620: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00003630: 6465 7465 6374 6f72 2063 6861 6e6e 656c  detector channel
-00003640: 206e 616d 6529 2873 2920 2865 7861 6d70   name)(s) (examp
-00003650: 6c65 2027 5a31 5041 5331 272c 2027 5044  le 'Z1PAS1', 'PD
-00003660: 3227 2c20 6f72 2031 290a 2020 2020 2020  2', or 1).      
-00003670: 2020 2020 2020 666f 6c6c 6f77 696e 6720        following 
-00003680: 666f 726d 6174 2069 6e20 7365 7475 702e  format in setup.
-00003690: 696e 6920 6669 6c65 0a20 2020 2020 2020  ini file.       
-000036a0: 2020 2020 2049 6620 4e6f 6e65 2c20 7265       If None, re
-000036b0: 6164 2061 6c6c 2063 6861 6e6e 656c 7320  ad all channels 
-000036c0: 6176 6169 6c61 626c 6520 0a0a 2020 2020  available ..    
-000036d0: 2020 2020 6576 656e 745f 6e75 6d73 3a20      event_nums: 
-000036e0: 6c69 7374 206f 7220 6e75 6d70 7920 6172  list or numpy ar
-000036f0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00003700: 4576 656e 7420 6e75 6d62 6572 7320 2866  Event numbers (f
-00003710: 6f72 6d61 743a 2064 756d 705f 6e75 6d20  ormat: dump_num 
-00003720: 2a20 3130 3030 3030 202b 2065 7665 6e74  * 100000 + event
-00003730: 5f69 6e64 6578 290a 2020 2020 2020 2020  _index).        
-00003740: 2020 2020 2020 0a20 2020 2020 2020 2073        .        s
-00003750: 6572 6965 735f 6e75 6d73 3a20 6c69 7374  eries_nums: list
-00003760: 206f 7220 6e75 6d70 7920 6172 7261 790a   or numpy array.
-00003770: 2020 2020 2020 2020 2020 2020 5365 7269              Seri
-00003780: 6573 206e 756d 6265 7273 2028 666f 726d  es numbers (form
-00003790: 6174 3a20 7879 7979 796d 6d64 6468 686d  at: xyyyymmddhhm
-000037a0: 6d73 7329 0a20 2020 2020 2020 2020 2020  mss).           
-000037b0: 2069 6620 6576 656e 745f 6e75 6d73 2061   if event_nums a
-000037c0: 7267 756d 656e 7420 7072 6f76 6964 6564  rgument provided
-000037d0: 2c20 7365 7269 6573 5f6e 756d 7320 7368  , series_nums sh
-000037e0: 6f75 6c64 2068 6176 6520 7361 6d65 206c  ould have same l
-000037f0: 656e 6774 6821 290a 0a20 2020 2020 2020  ength!)..       
-00003800: 2069 6e63 6c75 6465 5f6d 6574 6164 6174   include_metadat
-00003810: 613a 2062 6f6f 6c20 0a20 2020 2020 2020  a: bool .       
-00003820: 2020 2020 2069 6e63 6c75 6465 2066 696c       include fil
-00003830: 652f 6772 6f75 702f 6461 7461 7365 7420  e/group/dataset 
-00003840: 6d65 7461 6461 7461 2028 6465 6661 756c  metadata (defaul
-00003850: 7420 3d20 4661 6c73 6529 0a0a 2020 2020  t = False)..    
-00003860: 2020 2020 6164 6374 6f76 6f6c 743a 2042      adctovolt: B
-00003870: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00003880: 436f 6e76 6572 7420 2066 726f 6d20 4144  Convert  from AD
-00003890: 4320 746f 2076 6f6c 7420 2844 6566 6175  C to volt (Defau
-000038a0: 6c74 3d46 616c 7365 2920 0a20 2020 2020  lt=False) .     
-000038b0: 2020 200a 2020 2020 2020 2020 6164 6374     .        adct
-000038c0: 6f61 6d70 3a20 426f 6f6c 0a20 2020 2020  oamp: Bool.     
-000038d0: 2020 2020 2020 2043 6f6e 7665 7274 2020         Convert  
-000038e0: 6672 6f6d 2041 4443 2074 6f20 636c 6f73  from ADC to clos
-000038f0: 6520 6c6f 6f70 2f46 4c4c 2061 6d70 7320  e loop/FLL amps 
-00003900: 2844 6566 6175 6c74 3d46 616c 7365 2920  (Default=False) 
-00003910: 0a0a 2020 2020 2020 2020 6261 7365 6c69  ..        baseli
-00003920: 6e65 7375 623a 2042 6f6f 6c0a 2020 2020  nesub: Bool.    
-00003930: 2020 2020 2020 2020 4170 706c 7920 6261          Apply ba
-00003940: 7365 6c69 6e65 2073 7562 7472 6163 7469  seline subtracti
-00003950: 6f6e 0a0a 2020 2020 2020 2020 6261 7365  on..        base
-00003960: 6c69 6e65 696e 6473 3a20 7475 706c 6520  lineinds: tuple 
-00003970: 2869 6e74 2c20 696e 7429 206f 7220 6c69  (int, int) or li
-00003980: 7374 205b 696e 742c 2069 6e74 5d0a 2020  st [int, int].  
-00003990: 2020 2020 2020 2020 2020 7374 6172 742f            start/
-000039a0: 7374 6f70 2062 6173 656c 696e 6520 6361  stop baseline ca
-000039b0: 6c63 756c 6174 696f 6e20 2864 6566 6175  lculation (defau
-000039c0: 6c74 3a20 2831 302c 2030 2e38 2a70 7265  lt: (10, 0.8*pre
-000039d0: 7472 6967 6765 7220 6c65 6e67 7468 2929  trigger length))
-000039e0: 0a20 2020 2020 2020 2020 200a 2020 2020  .          .    
-000039f0: 2020 2020 6d65 6d6f 7279 5f6c 696d 6974      memory_limit
-00003a00: 3a20 466c 6f61 740a 2020 2020 2020 2020  : Float.        
-00003a10: 2020 2020 5075 6c73 6520 6461 7461 206d      Pulse data m
-00003a20: 656d 6f72 7920 6c69 6d69 7420 696e 2047  emory limit in G
-00003a30: 4220 5b64 6566 6175 6c74 3a20 3247 425d  B [default: 2GB]
-00003a40: 0a0a 2020 2020 2020 2020 6164 635f 6e61  ..        adc_na
-00003a50: 6d65 3a20 7374 7269 6e67 0a20 2020 2020  me: string.     
-00003a60: 2020 2020 2020 2020 2041 4443 2069 6420           ADC id 
-00003a70: 2864 6566 6175 6c74 3a20 2761 6463 3127  (default: 'adc1'
-00003a80: 290a 2020 2020 2020 2020 2020 0a0a 2020  ).          ..  
-00003a90: 2020 2020 2020 5265 7475 726e 0a20 2020        Return.   
-00003aa0: 2020 2020 202d 2d2d 2d2d 2d0a 200a 2020       ------. .  
-00003ab0: 2020 2020 2020 6f75 7470 7574 5f64 6174        output_dat
-00003ac0: 6120 3a20 6c69 7374 206f 7220 7061 6e64  a : list or pand
-00003ad0: 6173 2064 6174 6166 7261 6d65 0a20 2020  as dataframe.   
-00003ae0: 2020 2020 2020 2020 7472 6163 6573 2066          traces f
-00003af0: 6f72 2065 6163 6820 6368 616e 6e65 6c73  or each channels
-00003b00: 2061 6e64 2065 7665 6e74 730a 0a20 2020   and events..   
-00003b10: 2020 2020 2069 6e66 6f20 3a20 6c69 7374       info : list
-00003b20: 0a20 2020 2020 2020 2020 2020 6669 6c65  .           file
-00003b30: 2f65 7665 6e74 2f64 6574 6563 746f 7220  /event/detector 
-00003b40: 6d65 7461 6461 7461 200a 2020 2020 2020  metadata .      
-00003b50: 2020 2020 2028 6966 2022 696e 636c 7564       (if "includ
-00003b60: 655f 6d65 7461 6461 7461 2220 3d20 5472  e_metadata" = Tr
-00003b70: 7565 290a 0a0a 2020 2020 2020 2020 2222  ue)...        ""
-00003b80: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
-00003b90: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
-00003ba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003bb0: 3d3d 3d3d 0a20 2020 2020 2020 2023 2043  ====.        # C
-00003bc0: 6865 636b 2061 7267 756d 656e 7473 0a20  heck arguments. 
-00003bd0: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-00003be0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003bf0: 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020 2020  ========..      
-00003c00: 2020 2320 2066 696c 6520 6c69 7374 0a20    #  file list. 
-00003c10: 2020 2020 2020 2063 7572 7265 6e74 5f66         current_f
-00003c20: 696c 655f 6c69 7374 203d 204e 6f6e 6520  ile_list = None 
-00003c30: 200a 2020 2020 2020 2020 6966 2066 696c   .        if fil
-00003c40: 6570 6174 6820 6973 206e 6f74 204e 6f6e  epath is not Non
-00003c50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00003c60: 656c 662e 7365 745f 6669 6c65 7328 6669  elf.set_files(fi
-00003c70: 6c65 7061 7468 290a 2020 2020 2020 2020  lepath).        
-00003c80: 656c 6966 206e 6f74 2073 656c 662e 5f66  elif not self._f
-00003c90: 696c 655f 6c69 7374 3a0a 2020 2020 2020  ile_list:.      
-00003ca0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00003cb0: 6545 7272 6f72 2827 4552 524f 523a 204e  eError('ERROR: N
-00003cc0: 6f20 6669 6c65 7320 7365 6c65 6374 6564  o files selected
-00003cd0: 2127 290a 2020 2020 2020 2020 656c 7365  !').        else
-00003ce0: 3a0a 2020 2020 2020 2020 2020 2020 6375  :.            cu
-00003cf0: 7272 656e 745f 6669 6c65 5f6c 6973 7420  rrent_file_list 
-00003d00: 3d20 7365 6c66 2e5f 6669 6c65 5f6c 6973  = self._file_lis
-00003d10: 742e 636f 7079 2829 0a20 2020 2020 2020  t.copy().       
-00003d20: 2020 2020 200a 0a20 2020 2020 2020 2023       ..        #
-00003d30: 2064 6574 6563 746f 722f 6368 616e 6e65   detector/channe
-00003d40: 6c0a 2020 2020 2020 2020 6966 2028 6465  l.        if (de
-00003d50: 7465 6374 6f72 5f63 6861 6e73 2069 7320  tector_chans is 
-00003d60: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-00003d70: 2020 2020 2061 6e64 206e 6f74 2028 6973       and not (is
-00003d80: 696e 7374 616e 6365 2864 6574 6563 746f  instance(detecto
-00003d90: 725f 6368 616e 732c 206c 6973 7429 0a20  r_chans, list). 
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 2020 6f72 2069 7369 6e73 7461 6e63      or isinstanc
-00003dc0: 6528 6465 7465 6374 6f72 5f63 6861 6e73  e(detector_chans
-00003dd0: 2c20 6e70 2e6e 6461 7272 6179 2929 293a  , np.ndarray))):
-00003de0: 0a20 2020 2020 2020 2020 2020 2064 6574  .            det
-00003df0: 6563 746f 725f 6368 616e 7320 3d20 5b64  ector_chans = [d
-00003e00: 6574 6563 746f 725f 6368 616e 735d 0a20  etector_chans]. 
-00003e10: 2020 200a 0a20 2020 2020 2020 2023 2073     ..        # s
-00003e20: 6572 6965 7320 6e75 6d73 0a20 2020 2020  eries nums.     
-00003e30: 2020 2069 6620 7365 7269 6573 5f6e 756d     if series_num
-00003e40: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00003e50: 2020 2020 2020 2020 2020 2069 6620 286e             if (n
-00003e60: 6f74 2069 7369 6e73 7461 6e63 6528 7365  ot isinstance(se
-00003e70: 7269 6573 5f6e 756d 732c 206c 6973 7429  ries_nums, list)
-00003e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003e90: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
-00003ea0: 6e63 6528 7365 7269 6573 5f6e 756d 732c  nce(series_nums,
-00003eb0: 206e 702e 6e64 6172 7261 7929 293a 0a20   np.ndarray)):. 
-00003ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003ed0: 6572 6965 735f 6e75 6d73 203d 205b 7365  eries_nums = [se
-00003ee0: 7269 6573 5f6e 756d 735d 0a0a 2020 2020  ries_nums]..    
-00003ef0: 2020 2020 2020 2020 2320 6d61 6b65 2073          # make s
-00003f00: 7572 6520 7765 2061 7265 2075 7369 6e67  ure we are using
-00003f10: 2069 6e74 6567 6572 730a 2020 2020 2020   integers.      
-00003f20: 2020 2020 2020 666f 7220 6973 6572 6965        for iserie
-00003f30: 7320 696e 2072 616e 6765 286c 656e 2873  s in range(len(s
-00003f40: 6572 6965 735f 6e75 6d73 2929 3a0a 2020  eries_nums)):.  
-00003f50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003f60: 7269 6573 5f6e 756d 735b 6973 6572 6965  ries_nums[iserie
-00003f70: 735d 203d 2069 6e74 2873 6572 6965 735f  s] = int(series_
-00003f80: 6e75 6d73 5b69 7365 7269 6573 5d29 0a0a  nums[iseries])..
-00003f90: 2020 2020 2020 2020 2320 6576 656e 7420          # event 
-00003fa0: 6e75 6d73 3a0a 2020 2020 2020 2020 2320  nums:.        # 
-00003fb0: 2020 6173 736f 6369 6174 6520 6120 6475    associate a du
-00003fc0: 6d70 206c 6973 740a 2020 2020 2020 2020  mp list.        
-00003fd0: 2320 2020 636f 6e76 6572 7420 746f 206c  #   convert to l
-00003fe0: 6973 7420 6f66 2069 6e74 2069 6620 6e65  ist of int if ne
-00003ff0: 6564 6564 0a20 2020 2020 2020 200a 2020  eded.        .  
-00004000: 2020 2020 2020 6475 6d70 5f6e 756d 7320        dump_nums 
-00004010: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-00004020: 6620 6576 656e 745f 6e75 6d73 2069 7320  f event_nums is 
-00004030: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004040: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00004050: 2020 2023 2063 6f6e 7665 7274 2074 6f20     # convert to 
-00004060: 6c69 7374 2069 6620 6e6f 7420 6172 7261  list if not arra
-00004070: 792f 6c69 7374 0a20 2020 2020 2020 2020  y/list.         
-00004080: 2020 2069 6620 286e 6f74 2069 7369 6e73     if (not isins
-00004090: 7461 6e63 6528 6576 656e 745f 6e75 6d73  tance(event_nums
-000040a0: 2c20 6c69 7374 290a 2020 2020 2020 2020  , list).        
-000040b0: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
-000040c0: 6973 696e 7374 616e 6365 2865 7665 6e74  isinstance(event
-000040d0: 5f6e 756d 732c 6e70 2e6e 6461 7272 6179  _nums,np.ndarray
-000040e0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000040f0: 2020 2020 6576 656e 745f 6e75 6d73 203d      event_nums =
-00004100: 205b 6576 656e 745f 6e75 6d73 5d0a 2020   [event_nums].  
-00004110: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00004120: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-00004130: 6572 6965 735f 6e75 6d73 2069 7320 6e6f  eries_nums is no
-00004140: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-00004150: 2020 2020 2020 2061 6e64 2020 6c65 6e28         and  len(
-00004160: 6576 656e 745f 6e75 6d73 2921 3d6c 656e  event_nums)!=len
-00004170: 2873 6572 6965 735f 6e75 6d73 2929 3a0a  (series_nums)):.
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004190: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000041a0: 2827 4552 524f 523a 2073 6572 6965 735f  ('ERROR: series_
-000041b0: 6e75 6d73 2061 6e64 2065 7665 6e74 5f6e  nums and event_n
-000041c0: 756d 7320 6e65 6564 2074 6f20 6265 2073  ums need to be s
-000041d0: 616d 6520 6c65 6e67 7468 2127 290a 0a20  ame length!').. 
-000041e0: 2020 2020 2020 2020 2020 2064 756d 705f             dump_
-000041f0: 6e75 6d73 203d 206c 6973 7428 290a 2020  nums = list().  
-00004200: 2020 2020 2020 2020 2020 666f 7220 6965            for ie
-00004210: 7665 6e74 2069 6e20 7261 6e67 6528 6c65  vent in range(le
-00004220: 6e28 6576 656e 745f 6e75 6d73 2929 3a0a  n(event_nums)):.
-00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 6576 656e 745f 6e75 6d73 5b69 6576 656e  event_nums[ieven
-00004250: 745d 203d 2069 6e74 2865 7665 6e74 5f6e  t] = int(event_n
-00004260: 756d 735b 6965 7665 6e74 5d29 0a20 2020  ums[ievent]).   
-00004270: 2020 2020 2020 2020 2020 2020 2064 756d               dum
-00004280: 705f 6e75 6d20 3d20 696e 7428 6576 656e  p_num = int(even
-00004290: 745f 6e75 6d73 5b69 6576 656e 745d 2f31  t_nums[ievent]/1
-000042a0: 3030 3030 3029 0a20 2020 2020 2020 2020  00000).         
-000042b0: 2020 2020 2020 2069 6620 6475 6d70 5f6e         if dump_n
-000042c0: 756d 203d 3d20 303a 0a20 2020 2020 2020  um == 0:.       
-000042d0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-000042e0: 7365 2056 616c 7565 4572 726f 7228 2745  se ValueError('E
-000042f0: 5252 4f52 3a20 556e 6578 7065 6374 6564  RROR: Unexpected
-00004300: 2065 7665 6e74 206e 756d 6265 7220 666f   event number fo
-00004310: 726d 6174 2127 202b 0a20 2020 2020 2020  rmat!' +.       
-00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004330: 2020 2020 2020 2020 2020 2020 2020 2720                ' 
-00004340: 5265 7175 6972 6564 2066 6f72 6d61 7420  Required format 
-00004350: 3d20 2264 756d 705f 6e75 6d2a 3130 3030  = "dump_num*1000
-00004360: 3030 2b65 7665 6e74 5f69 6e64 6578 2227  00+event_index"'
-00004370: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004380: 2020 6475 6d70 5f6e 756d 732e 6170 7065    dump_nums.appe
-00004390: 6e64 2864 756d 705f 6e75 6d29 0a20 2020  nd(dump_num).   
-000043a0: 2020 2020 2020 200a 0a0a 2020 2020 2020         ...      
-000043b0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-000043c0: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
-000043d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000043e0: 3d3d 3d3d 3d0a 2020 2020 2020 2020 2320  =====.        # 
-000043f0: 5261 7720 6461 7461 2063 6865 636b 7320  Raw data checks 
-00004400: 7573 696e 6720 6d65 7461 6461 7461 0a20  using metadata. 
-00004410: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-00004420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004430: 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020 2020  ========..      
-00004440: 2020 2320 696e 6974 6961 6c69 7a65 2075    # initialize u
-00004450: 7365 6675 6c20 7061 7261 6d65 7465 7273  seful parameters
-00004460: 0a20 2020 2020 2020 206e 625f 6576 656e  .        nb_even
-00004470: 7473 5f74 6f74 203d 2030 0a20 2020 2020  ts_tot = 0.     
-00004480: 2020 206e 625f 6368 616e 6e65 6c73 203d     nb_channels =
-00004490: 2030 0a20 2020 2020 2020 206e 625f 7361   0.        nb_sa
-000044a0: 6d70 6c65 7320 3d20 300a 2020 2020 2020  mples = 0.      
-000044b0: 2020 6172 7261 795f 696e 6469 6365 7320    array_indices 
-000044c0: 3d20 6c69 7374 2829 0a0a 2020 2020 2020  = list()..      
-000044d0: 2020 2320 7365 6c65 6374 6564 2066 696c    # selected fil
-000044e0: 6573 2028 6361 7365 2073 6572 6965 7320  es (case series 
-000044f0: 6e75 6d62 6572 206f 6e6c 7920 7072 6f76  number only prov
-00004500: 6964 6564 290a 2020 2020 2020 2020 2320  ided).        # 
-00004510: 6f72 2074 7570 6c65 2028 6576 656e 7420  or tuple (event 
-00004520: 696e 6465 782c 2066 696c 6529 2069 6620  index, file) if 
-00004530: 6576 656e 7420 7072 6f76 6964 6564 0a20  event provided. 
-00004540: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-00004550: 6669 6c65 7320 3d20 4e6f 6e65 0a20 2020  files = None.   
-00004560: 2020 2020 2073 656c 6563 7465 645f 6576       selected_ev
-00004570: 656e 745f 6669 6c65 7320 3d20 4e6f 6e65  ent_files = None
-00004580: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
-00004590: 745f 6e75 6d73 2069 7320 4e6f 6e65 3a0a  t_nums is None:.
-000045a0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-000045b0: 6374 6564 5f66 696c 6573 203d 206c 6973  cted_files = lis
-000045c0: 7428 290a 2020 2020 2020 2020 656c 7365  t().        else
-000045d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000045e0: 6c65 6374 6564 5f65 7665 6e74 5f66 696c  lected_event_fil
-000045f0: 6573 203d 206c 6973 7428 290a 2020 2020  es = list().    
-00004600: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-00004610: 2020 0a20 2020 2020 2020 2023 206c 6f6f    .        # loo
-00004620: 7020 6669 6c65 730a 2020 2020 2020 2020  p files.        
-00004630: 666f 7220 6669 6c65 5f6e 616d 6520 696e  for file_name in
-00004640: 2073 656c 662e 5f66 696c 655f 6c69 7374   self._file_list
-00004650: 3a0a 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00004660: 2067 6574 206d 6574 6164 6174 610a 2020   get metadata.  
-00004670: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
-00004680: 7461 203d 2073 656c 662e 6765 745f 6d65  ta = self.get_me
-00004690: 7461 6461 7461 2866 696c 655f 6e61 6d65  tadata(file_name
-000046a0: 290a 2020 2020 2020 2020 2020 2020 6164  ).            ad
-000046b0: 635f 6d65 7461 6461 7461 203d 206d 6574  c_metadata = met
-000046c0: 6164 6174 615b 2767 726f 7570 7327 5d5b  adata['groups'][
-000046d0: 6164 635f 6e61 6d65 5d0a 0a20 2020 2020  adc_name]..     
-000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
-00004700: 6578 7472 6163 7420 7365 7269 6573 206e  extract series n
-00004710: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
-00004720: 2020 6669 6c65 5f73 6572 6965 735f 6e75    file_series_nu
-00004730: 6d20 3d20 4e6f 6e65 0a20 2020 2020 2020  m = None.       
-00004740: 2020 2020 2069 6620 2773 6572 6965 735f       if 'series_
-00004750: 6e75 6d27 2069 6e20 6d65 7461 6461 7461  num' in metadata
-00004760: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004770: 2020 6669 6c65 5f73 6572 6965 735f 6e75    file_series_nu
-00004780: 6d20 3d20 696e 7428 6d65 7461 6461 7461  m = int(metadata
-00004790: 5b27 7365 7269 6573 5f6e 756d 275d 290a  ['series_num']).
-000047a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000047b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000047c0: 2020 6669 6c65 5f73 6572 6965 735f 6e75    file_series_nu
-000047d0: 6d20 3d20 696e 7428 6578 7472 6163 745f  m = int(extract_
-000047e0: 7365 7269 6573 5f6e 756d 2866 696c 655f  series_num(file_
-000047f0: 6e61 6d65 2929 0a0a 2020 2020 2020 2020  name))..        
-00004800: 2020 2020 6966 2073 6572 6965 735f 6e75      if series_nu
-00004810: 6d73 2069 7320 6e6f 7420 4e6f 6e65 2061  ms is not None a
-00004820: 6e64 2066 696c 655f 7365 7269 6573 5f6e  nd file_series_n
-00004830: 756d 2069 7320 4e6f 6e65 3a0a 2020 2020  um is None:.    
-00004840: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00004850: 6520 5661 6c75 6545 7272 6f72 2827 4552  e ValueError('ER
-00004860: 524f 523a 2075 6e61 626c 6520 746f 2067  ROR: unable to g
-00004870: 6574 2073 6572 6965 7320 6e75 6d62 6572  et series number
-00004880: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
-00004890: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
-000048a0: 7874 7261 6374 2064 756d 7020 6e75 6d62  xtract dump numb
-000048b0: 6572 0a20 2020 2020 2020 2020 2020 2066  er.            f
-000048c0: 696c 655f 6475 6d70 5f6e 756d 203d 204e  ile_dump_num = N
-000048d0: 6f6e 6520 200a 2020 2020 2020 2020 2020  one  .          
-000048e0: 2020 6966 2027 6475 6d70 5f6e 756d 2720    if 'dump_num' 
-000048f0: 696e 206d 6574 6164 6174 613a 0a20 2020  in metadata:.   
-00004900: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00004910: 655f 6475 6d70 5f6e 756d 203d 2069 6e74  e_dump_num = int
-00004920: 286d 6574 6164 6174 615b 2764 756d 705f  (metadata['dump_
-00004930: 6e75 6d27 5d29 0a20 2020 2020 2020 2020  num']).         
-00004940: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004950: 2020 2020 2020 2020 2066 696c 655f 6475           file_du
-00004960: 6d70 5f6e 756d 203d 2069 6e74 2865 7874  mp_num = int(ext
-00004970: 7261 6374 5f64 756d 705f 6e75 6d28 6669  ract_dump_num(fi
-00004980: 6c65 5f6e 616d 6529 290a 0a20 2020 2020  le_name))..     
-00004990: 2020 2020 2020 2069 6620 6475 6d70 5f6e         if dump_n
-000049a0: 756d 7320 6973 206e 6f74 204e 6f6e 6520  ums is not None 
-000049b0: 616e 6420 6669 6c65 5f64 756d 705f 6e75  and file_dump_nu
-000049c0: 6d20 6973 204e 6f6e 653a 0a20 2020 2020  m is None:.     
-000049d0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000049e0: 2056 616c 7565 4572 726f 7228 2745 5252   ValueError('ERR
-000049f0: 4f52 3a20 756e 6162 6c65 2074 6f20 6765  OR: unable to ge
-00004a00: 7420 6475 6d70 206e 756d 6265 7221 2729  t dump number!')
-00004a10: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00004a20: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00004a30: 2020 2020 2020 2023 2073 6b69 7020 6669         # skip fi
-00004a40: 6c65 7320 7468 6174 2061 7265 206e 6f74  les that are not
-00004a50: 206e 6565 6465 640a 2020 2020 2020 2020   needed.        
-00004a60: 2020 2020 6966 2028 7365 7269 6573 5f6e      if (series_n
-00004a70: 756d 7320 6973 206e 6f74 204e 6f6e 650a  ums is not None.
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 616e 6420 6669 6c65 5f73 6572 6965 735f  and file_series_
-00004aa0: 6e75 6d20 6e6f 7420 696e 2073 6572 6965  num not in serie
-00004ab0: 735f 6e75 6d73 293a 0a20 2020 2020 2020  s_nums):.       
-00004ac0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00004ad0: 650a 2020 2020 2020 2020 2020 2020 0a20  e.            . 
-00004ae0: 2020 2020 2020 2020 2020 2069 6620 2864             if (d
-00004af0: 756d 705f 6e75 6d73 2069 7320 6e6f 7420  ump_nums is not 
-00004b00: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00004b10: 2020 2020 2061 6e64 2066 696c 655f 6475       and file_du
-00004b20: 6d70 5f6e 756d 206e 6f74 2069 6e20 6475  mp_num not in du
-00004b30: 6d70 5f6e 756d 7329 3a0a 2020 2020 2020  mp_nums):.      
-00004b40: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00004b50: 7565 0a20 2020 2020 2020 2020 2020 200a  ue.            .
-00004b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004b80: 2020 2020 2320 6966 2065 7665 6e74 5f6e      # if event_n
-00004b90: 756d 733a 2020 6368 6563 6b20 6669 6c65  ums:  check file
-00004ba0: 2069 6620 6176 6169 6c61 626c 6520 616e   if available an
-00004bb0: 6420 7374 6f72 6520 6974 0a20 2020 2020  d store it.     
-00004bc0: 2020 2020 2020 2069 6620 6576 656e 745f         if event_
-00004bd0: 6e75 6d73 2069 7320 6e6f 7420 4e6f 6e65  nums is not None
-00004be0: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004bf0: 2020 206b 6565 705f 6669 6c65 203d 2046     keep_file = F
-00004c00: 616c 7365 0a0a 2020 2020 2020 2020 2020  alse..          
-00004c10: 2020 2020 2020 666f 7220 6965 7665 6e74        for ievent
-00004c20: 2069 6e20 7261 6e67 6528 6c65 6e28 6576   in range(len(ev
-00004c30: 656e 745f 6e75 6d73 2929 3a0a 0a20 2020  ent_nums)):..   
-00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2023 2063 6865 636b 2069 6620 6475 6d70   # check if dump
-00004c60: 206e 756d 6265 7220 6d61 7463 6820 6375   number match cu
-00004c70: 7272 656e 7420 6669 6c65 0a20 2020 2020  rrent file.     
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004c90: 756d 705f 6e75 6d20 3d20 2064 756d 705f  ump_num =  dump_
-00004ca0: 6e75 6d73 5b69 6576 656e 745d 0a20 2020  nums[ievent].   
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2069 6620 6475 6d70 5f6e 756d 2021 3d20   if dump_num != 
-00004cd0: 6669 6c65 5f64 756d 705f 6e75 6d3a 0a20  file_dump_num:. 
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00004d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d10: 2020 2020 2023 2063 6865 636b 2073 6572       # check ser
-00004d20: 6965 7320 6d61 7463 6820 6375 7272 656e  ies match curren
-00004d30: 7420 6669 6c65 0a20 2020 2020 2020 2020  t file.         
-00004d40: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00004d50: 7269 6573 5f6e 756d 7320 6973 206e 6f74  ries_nums is not
-00004d60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004d80: 6572 6965 735f 6e75 6d20 3d20 7365 7269  eries_num = seri
-00004d90: 6573 5f6e 756d 735b 6965 7665 6e74 5d0a  es_nums[ievent].
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004db0: 2020 2020 2020 2020 6966 2073 6572 6965          if serie
-00004dc0: 735f 6e75 6d20 213d 2066 696c 655f 7365  s_num != file_se
-00004dd0: 7269 6573 5f6e 756d 3a0a 2020 2020 2020  ries_num:.      
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004e20: 2020 2020 2020 2020 2020 2020 2320 466f              # Fo
-00004e30: 756e 6420 6669 6c65 210a 2020 2020 2020  und file!.      
-00004e40: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
-00004e50: 6570 5f66 696c 6520 203d 2054 7275 650a  ep_file  = True.
-00004e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e70: 2020 2020 2023 2063 6865 636b 2069 6e64       # check ind
-00004e80: 6578 2061 7661 696c 6162 6c65 0a20 2020  ex available.   
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2065 7665 6e74 5f6e 756d 203d 2065 7665   event_num = eve
-00004eb0: 6e74 5f6e 756d 735b 6965 7665 6e74 5d0a  nt_nums[ievent].
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2020 2020 6576 656e 745f 696e 6465 7820      event_index 
-00004ee0: 3d20 696e 7428 6576 656e 745f 6e75 6d20  = int(event_num 
-00004ef0: 2520 3130 3030 3030 290a 2020 2020 2020  % 100000).      
-00004f00: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2069 6620 6576 656e 745f 696e 6465     if event_inde
-00004f30: 783e 696e 7428 6164 635f 6d65 7461 6461  x>int(adc_metada
-00004f40: 7461 5b27 6e62 5f65 7665 6e74 7327 5d29  ta['nb_events'])
-00004f50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004f60: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004f70: 5661 6c75 6545 7272 6f72 2827 4552 524f  ValueError('ERRO
-00004f80: 523a 2046 696e 6420 6669 6c65 2066 6f72  R: Find file for
-00004f90: 2065 7665 6e74 206e 756d 6265 7220 270a   event number '.
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fc0: 2020 2020 2020 2020 202b 2073 7472 2865           + str(e
-00004fd0: 7665 6e74 5f6e 756d 290a 2020 2020 2020  vent_num).      
-00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 202b 2027 2068 6f77 6576 6572 2c20     + ' however, 
-00005010: 6576 656e 7420 646f 6573 206e 6f74 2065  event does not e
-00005020: 7869 7374 2127 290a 2020 2020 2020 2020  xist!').        
-00005030: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005050: 2023 2073 746f 7265 2069 6e20 6c69 7374   # store in list
-00005060: 2061 7320 6120 7475 706c 650a 2020 2020   as a tuple.    
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 7365 6c65 6374 6564 5f65 7665 6e74 5f66  selected_event_f
-00005090: 696c 6573 2e61 7070 656e 6428 2865 7665  iles.append((eve
-000050a0: 6e74 5f69 6e64 6578 2c20 6669 6c65 5f6e  nt_index, file_n
-000050b0: 616d 6529 290a 0a20 2020 2020 2020 2020  ame))..         
-000050c0: 2020 2020 2020 2020 2020 2023 2069 6e63             # inc
-000050d0: 7265 6d65 6e74 2074 6f74 206e 756d 6265  rement tot numbe
-000050e0: 7220 6f66 2065 7665 6e74 730a 2020 2020  r of events.    
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 6e62 5f65 7665 6e74 735f 746f 7420 2b3d  nb_events_tot +=
-00005110: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00005120: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
-00005130: 2020 2020 2020 2020 2023 2063 6f6e 7469           # conti
-00005140: 6e75 6520 6669 6c65 206c 6f6f 7020 6966  nue file loop if
-00005150: 206e 6f74 206e 6565 6465 640a 2020 2020   not needed.    
-00005160: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005170: 6f74 206b 6565 705f 6669 6c65 203a 0a20  ot keep_file :. 
-00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
-000051a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000051b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000051c0: 625f 6576 656e 7473 5f74 6f74 202b 3d20  b_events_tot += 
-000051d0: 6164 635f 6d65 7461 6461 7461 5b27 6e62  adc_metadata['nb
-000051e0: 5f65 7665 6e74 7327 5d0a 2020 2020 2020  _events'].      
-000051f0: 2020 2020 2020 2020 2020 6966 206e 6576            if nev
-00005200: 656e 7473 3e30 2020 616e 6420 6e62 5f65  ents>0  and nb_e
-00005210: 7665 6e74 735f 746f 743e 3d6e 6576 656e  vents_tot>=neven
-00005220: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00005230: 2020 2020 2020 2020 6e62 5f65 7665 6e74          nb_event
-00005240: 735f 746f 7420 3d20 6e65 7665 6e74 730a  s_tot = nevents.
-00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 7365 6c65 6374 6564 5f66 696c 6573 2e61  selected_files.a
-00005270: 7070 656e 6428 6669 6c65 5f6e 616d 6529  ppend(file_name)
-00005280: 0a0a 2020 2020 2020 2020 2020 200a 2020  ..           .  
-00005290: 2020 2020 2020 2020 2020 2320 6368 616e            # chan
-000052a0: 6e65 6c73 0a20 2020 2020 2020 2020 2020  nels.           
-000052b0: 2061 7272 6179 5f69 6e64 6963 6573 5f66   array_indices_f
-000052c0: 696c 6520 3d20 6c69 7374 2829 0a20 2020  ile = list().   
-000052d0: 2020 2020 2020 2020 206e 625f 6368 616e           nb_chan
-000052e0: 6e65 6c73 5f66 696c 6520 3d20 6164 635f  nels_file = adc_
-000052f0: 6d65 7461 6461 7461 5b27 6e62 5f63 6861  metadata['nb_cha
-00005300: 6e6e 656c 7327 5d0a 2020 2020 2020 2020  nnels'].        
-00005310: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00005320: 2069 6620 6465 7465 6374 6f72 5f63 6861   if detector_cha
-00005330: 6e73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ns is not None:.
-00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00005360: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005370: 2061 7661 696c 6162 6c65 2061 6463 2063   available adc c
-00005380: 6861 6e6e 656c 7320 200a 2020 2020 2020  hannels  .      
-00005390: 2020 2020 2020 2020 2020 6164 635f 6368            adc_ch
-000053a0: 616e 5f6c 6973 7420 3d20 6164 635f 6d65  an_list = adc_me
-000053b0: 7461 6461 7461 5b27 6164 635f 6368 616e  tadata['adc_chan
-000053c0: 6e65 6c5f 696e 6469 6365 7327 5d0a 2020  nel_indices'].  
-000053d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000053e0: 2028 6e6f 7420 6973 696e 7374 616e 6365   (not isinstance
-000053f0: 2861 6463 5f63 6861 6e5f 6c69 7374 2c20  (adc_chan_list, 
-00005400: 6c69 7374 290a 2020 2020 2020 2020 2020  list).          
-00005410: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
-00005420: 7420 6973 696e 7374 616e 6365 2861 6463  t isinstance(adc
-00005430: 5f63 6861 6e5f 6c69 7374 2c20 6e70 2e6e  _chan_list, np.n
-00005440: 6461 7272 6179 2929 3a0a 2020 2020 2020  darray)):.      
-00005450: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00005460: 635f 6368 616e 5f6c 6973 7420 3d20 6e70  c_chan_list = np
-00005470: 2e61 7272 6179 285b 6164 635f 6368 616e  .array([adc_chan
-00005480: 5f6c 6973 745d 290a 2020 2020 2020 2020  _list]).        
-00005490: 2020 2020 2020 2020 2020 2020 0a0a 2020              ..  
-000054a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000054b0: 636f 6e6e 6563 7469 6f6e 730a 2020 2020  connections.    
-000054c0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-000054d0: 6563 7469 6f6e 7320 3d20 7365 6c66 2e67  ections = self.g
-000054e0: 6574 5f63 6f6e 6e65 6374 696f 6e5f 6469  et_connection_di
-000054f0: 6374 2861 6463 5f6e 616d 653d 6164 635f  ct(adc_name=adc_
-00005500: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005530: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00005540: 6164 6174 613d 6d65 7461 6461 7461 290a  adata=metadata).
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2020 0a0a 2020 2020 0a20 2020 2064 6566    ..    .    def
+00003270: 2072 6561 645f 6d61 6e79 5f65 7665 6e74   read_many_event
+00003280: 7328 7365 6c66 2c20 6669 6c65 7061 7468  s(self, filepath
+00003290: 3d4e 6f6e 652c 206e 6576 656e 7473 3d30  =None, nevents=0
+000032a0: 2c20 6f75 7470 7574 5f66 6f72 6d61 743d  , output_format=
+000032b0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+000032c0: 2020 2020 2020 2020 2020 2020 6465 7465              dete
+000032d0: 6374 6f72 5f63 6861 6e73 3d4e 6f6e 652c  ctor_chans=None,
+000032e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000032f0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
+00003300: 6e75 6d73 3d4e 6f6e 652c 2073 6572 6965  nums=None, serie
+00003310: 735f 6e75 6d73 3d4e 6f6e 652c 0a20 2020  s_nums=None,.   
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 2020 2020 2020 696e 636c 7564 655f 6d65        include_me
+00003340: 7461 6461 7461 3d46 616c 7365 2c0a 2020  tadata=False,.  
+00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003360: 2020 2020 2020 2061 6463 746f 766f 6c74         adctovolt
+00003370: 3d46 616c 7365 2c20 6164 6374 6f61 6d70  =False, adctoamp
+00003380: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033a0: 2062 6173 656c 696e 6573 7562 3d46 616c   baselinesub=Fal
+000033b0: 7365 2c20 6261 7365 6c69 6e65 696e 6473  se, baselineinds
+000033c0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033e0: 6d65 6d6f 7279 5f6c 696d 6974 3d32 2c20  memory_limit=2, 
+000033f0: 6164 635f 6e61 6d65 3d27 6164 6331 2729  adc_name='adc1')
+00003400: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00003410: 2020 2020 2020 5265 6164 206d 756c 7469        Read multi
+00003420: 706c 6520 6576 656e 7473 2028 6465 6661  ple events (defa
+00003430: 756c 7420 7265 6164 2061 6c6c 2065 7665  ult read all eve
+00003440: 6e74 7329 0a20 2020 2020 2020 200a 2020  nts).        .  
+00003450: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00003460: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00003470: 2d2d 0a20 2020 2020 2020 2066 696c 6570  --.        filep
+00003480: 6174 683a 2073 7472 696e 6720 6f72 206c  ath: string or l
+00003490: 6973 7420 206f 6620 7374 7269 6e67 730a  ist  of strings.
+000034a0: 2020 2020 2020 2020 2020 2066 696c 652f             file/
+000034b0: 7061 7468 206f 7220 6c69 7374 206f 6620  path or list of 
+000034c0: 6669 6c65 732f 7061 7468 7320 2864 6566  files/paths (def
+000034d0: 6175 6c74 3a20 7573 6520 6375 7272 656e  ault: use curren
+000034e0: 7420 6669 6c65 290a 2020 2020 2020 2020  t file).        
+000034f0: 2020 0a20 2020 2020 2020 206e 6576 656e    .        neven
+00003500: 7473 3a20 696e 7465 6765 720a 2020 2020  ts: integer.    
+00003510: 2020 2020 2020 206e 756d 6265 7220 6f66         number of
+00003520: 2065 7665 6e74 7320 746f 2072 6561 6420   events to read 
+00003530: 2028 6465 6661 756c 7420 6e62 5f65 7665   (default nb_eve
+00003540: 6e74 733d 3020 2d3e 2061 6c6c 2065 7665  nts=0 -> all eve
+00003550: 6e74 7320 696e 2064 756d 7073 290a 0a20  nts in dumps).. 
+00003560: 2020 2020 2020 206f 7574 7075 745f 666f         output_fo
+00003570: 726d 6174 3a20 696e 7465 6765 720a 2020  rmat: integer.  
+00003580: 2020 2020 2020 2020 2020 313a 206c 6973            1: lis
+00003590: 7420 6f66 2032 4420 6e64 6172 7261 795b  t of 2D ndarray[
+000035a0: 6368 616e 2c20 7361 6d70 6c65 735d 0a20  chan, samples]. 
+000035b0: 2020 2020 2020 2020 2020 2032 3a20 3344             2: 3D
+000035c0: 206e 6461 7272 6179 5b65 7665 6e74 2c20   ndarray[event, 
+000035d0: 6368 616e 2c20 7361 6d70 6c65 735d 0a20  chan, samples]. 
+000035e0: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
+000035f0: 725f 6368 616e 733a 2073 7472 696e 672f  r_chans: string/
+00003600: 696e 7420 6f72 206c 6973 7420 6f66 2073  int or list of s
+00003610: 7472 696e 672f 696e 740a 2020 2020 2020  tring/int.      
+00003620: 2020 2020 2020 6465 7465 6374 6f72 2063        detector c
+00003630: 6861 6e6e 656c 206e 616d 6529 2873 2920  hannel name)(s) 
+00003640: 2865 7861 6d70 6c65 2027 5a31 5041 5331  (example 'Z1PAS1
+00003650: 272c 2027 5044 3227 2c20 6f72 2031 290a  ', 'PD2', or 1).
+00003660: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
+00003670: 6f77 696e 6720 666f 726d 6174 2069 6e20  owing format in 
+00003680: 7365 7475 702e 696e 6920 6669 6c65 0a20  setup.ini file. 
+00003690: 2020 2020 2020 2020 2020 2049 6620 4e6f             If No
+000036a0: 6e65 2c20 7265 6164 2061 6c6c 2063 6861  ne, read all cha
+000036b0: 6e6e 656c 7320 6176 6169 6c61 626c 6520  nnels available 
+000036c0: 0a0a 2020 2020 2020 2020 6576 656e 745f  ..        event_
+000036d0: 6e75 6d73 3a20 6c69 7374 206f 7220 6e75  nums: list or nu
+000036e0: 6d70 7920 6172 7261 790a 2020 2020 2020  mpy array.      
+000036f0: 2020 2020 2020 4576 656e 7420 6e75 6d62        Event numb
+00003700: 6572 7320 2866 6f72 6d61 743a 2064 756d  ers (format: dum
+00003710: 705f 6e75 6d20 2a20 3130 3030 3030 202b  p_num * 100000 +
+00003720: 2065 7665 6e74 5f69 6e64 6578 290a 2020   event_index).  
+00003730: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00003740: 2020 2020 2073 6572 6965 735f 6e75 6d73       series_nums
+00003750: 3a20 6c69 7374 206f 7220 6e75 6d70 7920  : list or numpy 
+00003760: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
+00003770: 2020 5365 7269 6573 206e 756d 6265 7273    Series numbers
+00003780: 2028 666f 726d 6174 3a20 7879 7979 796d   (format: xyyyym
+00003790: 6d64 6468 686d 6d73 7329 0a20 2020 2020  mddhhmmss).     
+000037a0: 2020 2020 2020 2069 6620 6576 656e 745f         if event_
+000037b0: 6e75 6d73 2061 7267 756d 656e 7420 7072  nums argument pr
+000037c0: 6f76 6964 6564 2c20 7365 7269 6573 5f6e  ovided, series_n
+000037d0: 756d 7320 7368 6f75 6c64 2068 6176 6520  ums should have 
+000037e0: 7361 6d65 206c 656e 6774 6821 290a 0a20  same length!).. 
+000037f0: 2020 2020 2020 2069 6e63 6c75 6465 5f6d         include_m
+00003800: 6574 6164 6174 613a 2062 6f6f 6c20 0a20  etadata: bool . 
+00003810: 2020 2020 2020 2020 2020 2069 6e63 6c75             inclu
+00003820: 6465 2066 696c 652f 6772 6f75 702f 6461  de file/group/da
+00003830: 7461 7365 7420 6d65 7461 6461 7461 2028  taset metadata (
+00003840: 6465 6661 756c 7420 3d20 4661 6c73 6529  default = False)
+00003850: 0a0a 2020 2020 2020 2020 6164 6374 6f76  ..        adctov
+00003860: 6f6c 743a 2042 6f6f 6c0a 2020 2020 2020  olt: Bool.      
+00003870: 2020 2020 2020 436f 6e76 6572 7420 2066        Convert  f
+00003880: 726f 6d20 4144 4320 746f 2076 6f6c 7420  rom ADC to volt 
+00003890: 2844 6566 6175 6c74 3d46 616c 7365 2920  (Default=False) 
+000038a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000038b0: 2020 6164 6374 6f61 6d70 3a20 426f 6f6c    adctoamp: Bool
+000038c0: 0a20 2020 2020 2020 2020 2020 2043 6f6e  .            Con
+000038d0: 7665 7274 2020 6672 6f6d 2041 4443 2074  vert  from ADC t
+000038e0: 6f20 636c 6f73 6520 6c6f 6f70 2f46 4c4c  o close loop/FLL
+000038f0: 2061 6d70 7320 2844 6566 6175 6c74 3d46   amps (Default=F
+00003900: 616c 7365 2920 0a0a 2020 2020 2020 2020  alse) ..        
+00003910: 6261 7365 6c69 6e65 7375 623a 2042 6f6f  baselinesub: Boo
+00003920: 6c0a 2020 2020 2020 2020 2020 2020 4170  l.            Ap
+00003930: 706c 7920 6261 7365 6c69 6e65 2073 7562  ply baseline sub
+00003940: 7472 6163 7469 6f6e 0a0a 2020 2020 2020  traction..      
+00003950: 2020 6261 7365 6c69 6e65 696e 6473 3a20    baselineinds: 
+00003960: 7475 706c 6520 2869 6e74 2c20 696e 7429  tuple (int, int)
+00003970: 206f 7220 6c69 7374 205b 696e 742c 2069   or list [int, i
+00003980: 6e74 5d0a 2020 2020 2020 2020 2020 2020  nt].            
+00003990: 7374 6172 742f 7374 6f70 2062 6173 656c  start/stop basel
+000039a0: 696e 6520 6361 6c63 756c 6174 696f 6e20  ine calculation 
+000039b0: 2864 6566 6175 6c74 3a20 2831 302c 2030  (default: (10, 0
+000039c0: 2e38 2a70 7265 7472 6967 6765 7220 6c65  .8*pretrigger le
+000039d0: 6e67 7468 2929 0a20 2020 2020 2020 2020  ngth)).         
+000039e0: 200a 2020 2020 2020 2020 6d65 6d6f 7279   .        memory
+000039f0: 5f6c 696d 6974 3a20 466c 6f61 740a 2020  _limit: Float.  
+00003a00: 2020 2020 2020 2020 2020 5075 6c73 6520            Pulse 
+00003a10: 6461 7461 206d 656d 6f72 7920 6c69 6d69  data memory limi
+00003a20: 7420 696e 2047 4220 5b64 6566 6175 6c74  t in GB [default
+00003a30: 3a20 3247 425d 0a0a 2020 2020 2020 2020  : 2GB]..        
+00003a40: 6164 635f 6e61 6d65 3a20 7374 7269 6e67  adc_name: string
+00003a50: 0a20 2020 2020 2020 2020 2020 2020 2041  .              A
+00003a60: 4443 2069 6420 2864 6566 6175 6c74 3a20  DC id (default: 
+00003a70: 2761 6463 3127 290a 2020 2020 2020 2020  'adc1').        
+00003a80: 2020 0a0a 2020 2020 2020 2020 5265 7475    ..        Retu
+00003a90: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
+00003aa0: 2d0a 200a 2020 2020 2020 2020 6f75 7470  -. .        outp
+00003ab0: 7574 5f64 6174 6120 3a20 6c69 7374 206f  ut_data : list o
+00003ac0: 7220 7061 6e64 6173 2064 6174 6166 7261  r pandas datafra
+00003ad0: 6d65 0a20 2020 2020 2020 2020 2020 7472  me.           tr
+00003ae0: 6163 6573 2066 6f72 2065 6163 6820 6368  aces for each ch
+00003af0: 616e 6e65 6c73 2061 6e64 2065 7665 6e74  annels and event
+00003b00: 730a 0a20 2020 2020 2020 2069 6e66 6f20  s..        info 
+00003b10: 3a20 6c69 7374 0a20 2020 2020 2020 2020  : list.         
+00003b20: 2020 6669 6c65 2f65 7665 6e74 2f64 6574    file/event/det
+00003b30: 6563 746f 7220 6d65 7461 6461 7461 200a  ector metadata .
+00003b40: 2020 2020 2020 2020 2020 2028 6966 2022             (if "
+00003b50: 696e 636c 7564 655f 6d65 7461 6461 7461  include_metadata
+00003b60: 2220 3d20 5472 7565 290a 0a0a 2020 2020  " = True)...    
+00003b70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00003b80: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
+00003b90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003ba0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020  ==========.     
+00003bb0: 2020 2023 2043 6865 636b 2061 7267 756d     # Check argum
+00003bc0: 656e 7473 0a20 2020 2020 2020 2023 203d  ents.        # =
+00003bd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003be0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
+00003bf0: 0a20 2020 2020 2020 2023 2073 6574 2066  .        # set f
+00003c00: 696c 6520 7061 7468 2069 6620 7072 6f76  ile path if prov
+00003c10: 6964 6564 0a20 2020 2020 2020 2069 6620  ided.        if 
+00003c20: 6669 6c65 7061 7468 2069 7320 6e6f 7420  filepath is not 
+00003c30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003c40: 2020 7365 6c66 2e73 6574 5f66 696c 6573    self.set_files
+00003c50: 2866 696c 6570 6174 6829 0a0a 2020 2020  (filepath)..    
+00003c60: 2020 2020 2320 6368 6563 6b20 0a20 2020      # check .   
+00003c70: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00003c80: 2e5f 6669 6c65 5f6c 6973 743a 0a20 2020  ._file_list:.   
+00003c90: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00003ca0: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
+00003cb0: 3a20 4e6f 2066 696c 6573 2073 656c 6563  : No files selec
+00003cc0: 7465 6421 2729 0a0a 2020 2020 2020 2020  ted!')..        
+00003cd0: 2320 6c65 7427 7320 6b65 6570 2061 2063  # let's keep a c
+00003ce0: 6f70 7920 6f66 2063 7572 7265 6e74 2066  opy of current f
+00003cf0: 696c 6520 6c69 7374 0a20 2020 2020 2020  ile list.       
+00003d00: 2063 7572 7265 6e74 5f66 696c 655f 6c69   current_file_li
+00003d10: 7374 203d 204e 6f6e 650a 2020 2020 2020  st = None.      
+00003d20: 2020 6966 2073 656c 662e 5f66 696c 655f    if self._file_
+00003d30: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+00003d40: 2020 6375 7272 656e 745f 6669 6c65 5f6c    current_file_l
+00003d50: 6973 7420 3d20 7365 6c66 2e5f 6669 6c65  ist = self._file
+00003d60: 5f6c 6973 742e 636f 7079 2829 0a0a 0a20  _list.copy()... 
+00003d70: 2020 2020 2020 2023 2064 6574 6563 746f         # detecto
+00003d80: 722f 6368 616e 6e65 6c0a 2020 2020 2020  r/channel.      
+00003d90: 2020 6966 2028 6465 7465 6374 6f72 5f63    if (detector_c
+00003da0: 6861 6e73 2069 7320 6e6f 7420 4e6f 6e65  hans is not None
+00003db0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00003dc0: 206e 6f74 2028 6973 696e 7374 616e 6365   not (isinstance
+00003dd0: 2864 6574 6563 746f 725f 6368 616e 732c  (detector_chans,
+00003de0: 206c 6973 7429 0a20 2020 2020 2020 2020   list).         
+00003df0: 2020 2020 2020 2020 2020 2020 6f72 2069              or i
+00003e00: 7369 6e73 7461 6e63 6528 6465 7465 6374  sinstance(detect
+00003e10: 6f72 5f63 6861 6e73 2c20 6e70 2e6e 6461  or_chans, np.nda
+00003e20: 7272 6179 2929 293a 0a20 2020 2020 2020  rray))):.       
+00003e30: 2020 2020 2064 6574 6563 746f 725f 6368       detector_ch
+00003e40: 616e 7320 3d20 5b64 6574 6563 746f 725f  ans = [detector_
+00003e50: 6368 616e 735d 0a20 2020 200a 0a20 2020  chans].    ..   
+00003e60: 2020 2020 2023 206c 6574 2773 2066 696c       # let's fil
+00003e70: 7465 7220 6669 6c65 7320 6261 7365 6420  ter files based 
+00003e80: 0a20 2020 2020 2020 2023 2073 6572 6965  .        # serie
+00003e90: 735f 6e75 6d73 2061 6e64 2065 7665 6e74  s_nums and event
+00003ea0: 5f6e 756d 7320 696e 7075 740a 2020 2020  _nums input.    
+00003eb0: 2020 2020 6669 6c74 6572 6564 5f66 696c      filtered_fil
+00003ec0: 655f 6c69 7374 203d 206c 6973 7428 290a  e_list = list().
+00003ed0: 2020 2020 2020 2020 6966 2073 6572 6965          if serie
+00003ee0: 735f 6e75 6d73 2069 7320 6e6f 7420 4e6f  s_nums is not No
+00003ef0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003f00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003f10: 2020 2020 2023 2063 6f6e 7665 7274 2074       # convert t
+00003f20: 6f20 6172 7261 790a 2020 2020 2020 2020  o array.        
+00003f30: 2020 2020 6966 2028 6e6f 7420 6973 696e      if (not isin
+00003f40: 7374 616e 6365 2873 6572 6965 735f 6e75  stance(series_nu
+00003f50: 6d73 2c20 6c69 7374 290a 2020 2020 2020  ms, list).      
+00003f60: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+00003f70: 7420 6973 696e 7374 616e 6365 2873 6572  t isinstance(ser
+00003f80: 6965 735f 6e75 6d73 2c20 6e70 2e6e 6461  ies_nums, np.nda
+00003f90: 7272 6179 2929 3a0a 2020 2020 2020 2020  rray)):.        
+00003fa0: 2020 2020 2020 2020 7365 7269 6573 5f6e          series_n
+00003fb0: 756d 7320 3d20 5b73 6572 6965 735f 6e75  ums = [series_nu
+00003fc0: 6d73 5d0a 2020 2020 2020 2020 2020 2020  ms].            
+00003fd0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00003fe0: 2023 206c 6f6f 7020 7365 7269 6573 2061   # loop series a
+00003ff0: 6e64 2063 6f6e 7665 7274 2074 6f20 7365  nd convert to se
+00004000: 7269 6573 206e 616d 650a 2020 2020 2020  ries name.      
+00004010: 2020 2020 2020 2320 2861 6e64 2063 6865        # (and che
+00004020: 636b 2069 6e74 6567 6572 290a 2020 2020  ck integer).    
+00004030: 2020 2020 2020 2020 7365 7269 6573 5f6e          series_n
+00004040: 616d 6573 203d 206c 6973 7428 290a 2020  ames = list().  
+00004050: 2020 2020 2020 2020 2020 666f 7220 6973            for is
+00004060: 6572 6965 7320 696e 2072 616e 6765 286c  eries in range(l
+00004070: 656e 2873 6572 6965 735f 6e75 6d73 2929  en(series_nums))
+00004080: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004090: 2020 7365 7269 6573 203d 2069 6e74 2873    series = int(s
+000040a0: 6572 6965 735f 6e75 6d73 5b69 7365 7269  eries_nums[iseri
+000040b0: 6573 5d29 0a20 2020 2020 2020 2020 2020  es]).           
+000040c0: 2020 2020 2073 6572 6965 735f 6e61 6d65       series_name
+000040d0: 732e 6170 7065 6e64 2865 7874 7261 6374  s.append(extract
+000040e0: 5f73 6572 6965 735f 6e61 6d65 2873 6572  _series_name(ser
+000040f0: 6965 7329 290a 2020 2020 2020 2020 2020  ies)).          
+00004100: 2020 2020 2020 7365 7269 6573 5f6e 756d        series_num
+00004110: 735b 6973 6572 6965 735d 203d 2073 6572  s[iseries] = ser
+00004120: 6965 730a 0a20 2020 2020 2020 2020 2020  ies..           
+00004130: 2023 206c 6f6f 7020 6669 6c65 7320 616e   # loop files an
+00004140: 6420 6368 6563 6b20 6966 2070 6172 7420  d check if part 
+00004150: 6f66 2073 656c 6563 7465 6420 7365 7269  of selected seri
+00004160: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
+00004170: 6f72 2066 696c 655f 6e61 6d65 2069 6e20  or file_name in 
+00004180: 7365 6c66 2e5f 6669 6c65 5f6c 6973 743a  self._file_list:
+00004190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041a0: 2066 6f72 2073 6572 6965 7320 696e 2073   for series in s
+000041b0: 6572 6965 735f 6e61 6d65 733a 0a20 2020  eries_names:.   
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041d0: 2069 6620 7365 7269 6573 2069 6e20 6669   if series in fi
+000041e0: 6c65 5f6e 616d 653a 0a20 2020 2020 2020  le_name:.       
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 2066 696c 7465 7265 645f 6669 6c65 5f6c   filtered_file_l
+00004210: 6973 742e 6170 7065 6e64 2866 696c 655f  ist.append(file_
+00004220: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+00004230: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00004240: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00004250: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004260: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00004270: 6669 6c74 6572 2062 6173 6564 206f 6e20  filter based on 
+00004280: 6576 656e 7420 6e75 6d73 0a20 2020 2020  event nums.     
+00004290: 2020 2023 2028 7365 7269 6573 206e 616d     # (series nam
+000042a0: 6573 2073 686f 756c 6420 6265 2073 616d  es should be sam
+000042b0: 6520 6c65 6e67 7468 290a 0a20 2020 2020  e length)..     
+000042c0: 2020 2064 756d 705f 6e75 6d73 203d 206c     dump_nums = l
+000042d0: 6973 7428 290a 2020 2020 2020 2020 6576  ist().        ev
+000042e0: 656e 745f 696e 6469 6365 7320 3d20 6c69  ent_indices = li
+000042f0: 7374 2829 0a20 2020 2020 2020 2069 6620  st().        if 
+00004300: 6576 656e 745f 6e75 6d73 2069 7320 6e6f  event_nums is no
+00004310: 7420 4e6f 6e65 3a0a 0a20 2020 2020 2020  t None:..       
+00004320: 2020 2020 2073 6572 6965 735f 6475 6d70       series_dump
+00004330: 5f6e 616d 6573 203d 206c 6973 7428 290a  _names = list().
+00004340: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00004350: 2020 2020 2020 2020 2023 2063 6f6e 7665           # conve
+00004360: 7274 2074 6f20 6c69 7374 2069 6620 6e6f  rt to list if no
+00004370: 7420 6172 7261 792f 6c69 7374 0a20 2020  t array/list.   
+00004380: 2020 2020 2020 2020 2069 6620 286e 6f74           if (not
+00004390: 2069 7369 6e73 7461 6e63 6528 6576 656e   isinstance(even
+000043a0: 745f 6e75 6d73 2c20 6c69 7374 290a 2020  t_nums, list).  
+000043b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+000043c0: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
+000043d0: 2865 7665 6e74 5f6e 756d 732c 6e70 2e6e  (event_nums,np.n
+000043e0: 6461 7272 6179 2929 3a0a 2020 2020 2020  darray)):.      
+000043f0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
+00004400: 6e75 6d73 203d 205b 6576 656e 745f 6e75  nums = [event_nu
+00004410: 6d73 5d0a 2020 2020 2020 2020 2020 2020  ms].            
+00004420: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00004430: 2069 6620 2873 6572 6965 735f 6e75 6d73   if (series_nums
+00004440: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
+00004450: 2020 2020 2020 2020 206f 7220 6c65 6e28           or len(
+00004460: 6576 656e 745f 6e75 6d73 2921 3d6c 656e  event_nums)!=len
+00004470: 2873 6572 6965 735f 6e75 6d73 2929 3a0a  (series_nums)):.
+00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004490: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000044a0: 2827 4552 524f 523a 2073 6572 6965 735f  ('ERROR: series_
+000044b0: 6e75 6d73 2061 6e64 2065 7665 6e74 5f6e  nums and event_n
+000044c0: 756d 7320 270a 2020 2020 2020 2020 2020  ums '.          
+000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044e0: 2020 2020 2020 202b 2027 6e65 6564 2074         + 'need t
+000044f0: 6f20 6265 2073 616d 6520 6c65 6e67 7468  o be same length
+00004500: 2127 290a 0a20 2020 2020 2020 2020 2020  !')..           
+00004510: 2073 6572 6965 735f 6475 6d70 5f6e 616d   series_dump_nam
+00004520: 6573 203d 206c 6973 7428 290a 2020 2020  es = list().    
+00004530: 2020 2020 2020 2020 666f 7220 6965 7665          for ieve
+00004540: 6e74 2069 6e20 7261 6e67 6528 6c65 6e28  nt in range(len(
+00004550: 6576 656e 745f 6e75 6d73 2929 3a0a 2020  event_nums)):.  
+00004560: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00004570: 656e 745f 6e75 6d73 5b69 6576 656e 745d  ent_nums[ievent]
+00004580: 203d 2069 6e74 2865 7665 6e74 5f6e 756d   = int(event_num
+00004590: 735b 6965 7665 6e74 5d29 0a20 2020 2020  s[ievent]).     
+000045a0: 2020 2020 2020 2020 2020 2064 756d 705f             dump_
+000045b0: 6e75 6d20 3d20 696e 7428 6576 656e 745f  num = int(event_
+000045c0: 6e75 6d73 5b69 6576 656e 745d 2f31 3030  nums[ievent]/100
+000045d0: 3030 3029 0a20 2020 2020 2020 2020 2020  000).           
+000045e0: 2020 2020 2065 7665 6e74 5f69 6e64 6578       event_index
+000045f0: 203d 2069 6e74 2865 7665 6e74 5f6e 756d   = int(event_num
+00004600: 735b 6965 7665 6e74 5d25 3130 3030 3030  s[ievent]%100000
+00004610: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004620: 2020 6966 2064 756d 705f 6e75 6d20 3d3d    if dump_num ==
+00004630: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00004640: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00004650: 6c75 6545 7272 6f72 2827 4552 524f 523a  lueError('ERROR:
+00004660: 2055 6e65 7870 6563 7465 6420 6576 656e   Unexpected even
+00004670: 7420 6e75 6d62 6572 2066 6f72 6d61 7421  t number format!
+00004680: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 2020 202b 2027 2052 6571 7569         + ' Requi
+000046b0: 7265 6420 666f 726d 6174 203d 2027 0a20  red format = '. 
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2020 2b20 2722 6475 6d70 5f6e 756d      + '"dump_num
+000046f0: 2a31 3030 3030 302b 6576 656e 745f 696e  *100000+event_in
+00004700: 6465 7822 2729 0a20 2020 2020 2020 2020  dex"').         
+00004710: 2020 2020 2020 2064 756d 705f 6e75 6d73         dump_nums
+00004720: 2e61 7070 656e 6428 6475 6d70 5f6e 756d  .append(dump_num
+00004730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004740: 2020 6576 656e 745f 696e 6469 6365 732e    event_indices.
+00004750: 6170 7065 6e64 2865 7665 6e74 5f69 6e64  append(event_ind
+00004760: 6578 290a 2020 2020 2020 2020 2020 2020  ex).            
+00004770: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00004780: 2020 2020 2023 2064 756d 7020 7374 720a       # dump str.
+00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047a0: 6475 6d70 5f6e 616d 6520 3d20 7374 7228  dump_name = str(
+000047b0: 6475 6d70 5f6e 756d 290a 2020 2020 2020  dump_num).      
+000047c0: 2020 2020 2020 2020 2020 666f 7220 7820            for x 
+000047d0: 696e 2072 616e 6765 2831 2c35 2d6c 656e  in range(1,5-len
+000047e0: 2864 756d 705f 6e61 6d65 2929 3a0a 2020  (dump_name)):.  
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004800: 2020 6475 6d70 5f6e 616d 6520 3d20 2730    dump_name = '0
+00004810: 272b 6475 6d70 5f6e 616d 650a 2020 2020  '+dump_name.    
+00004820: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+00004830: 6573 5f64 756d 705f 6e61 6d65 732e 6170  es_dump_names.ap
+00004840: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00004850: 2020 2020 2020 2020 2020 7365 7269 6573            series
+00004860: 5f6e 616d 6573 5b69 6576 656e 745d 202b  _names[ievent] +
+00004870: 2027 5f46 2720 2b20 6475 6d70 5f6e 616d   '_F' + dump_nam
+00004880: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00004890: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000048a0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+000048b0: 2023 2066 696c 7465 7220 6669 6c65 730a   # filter files.
+000048c0: 2020 2020 2020 2020 2020 2020 6576 656e              even
+000048d0: 745f 6669 6c74 6572 6564 5f66 696c 6573  t_filtered_files
+000048e0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+000048f0: 2020 2020 2020 666f 7220 6669 6c65 5f6e        for file_n
+00004900: 616d 6520 696e 2066 696c 7465 7265 645f  ame in filtered_
+00004910: 6669 6c65 5f6c 6973 743a 0a20 2020 2020  file_list:.     
+00004920: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+00004930: 6572 6965 735f 6475 6d70 2069 6e20 7365  eries_dump in se
+00004940: 7269 6573 5f64 756d 705f 6e61 6d65 733a  ries_dump_names:
+00004950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004960: 2020 2020 2069 6620 7365 7269 6573 5f64       if series_d
+00004970: 756d 7020 696e 2066 696c 655f 6e61 6d65  ump in file_name
+00004980: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004990: 2020 2020 2020 2020 2020 6576 656e 745f            event_
+000049a0: 6669 6c74 6572 6564 5f66 696c 6573 2e61  filtered_files.a
+000049b0: 7070 656e 6428 6669 6c65 5f6e 616d 6529  ppend(file_name)
+000049c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049d0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+000049e0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+000049f0: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
+00004a00: 5f66 696c 655f 6c69 7374 203d 2065 7665  _file_list = eve
+00004a10: 6e74 5f66 696c 7465 7265 645f 6669 6c65  nt_filtered_file
+00004a20: 730a 2020 2020 0a20 2020 2020 2020 2020  s.    .         
+00004a30: 2020 200a 2020 2020 2020 2020 2320 7265     .        # re
+00004a40: 706c 6163 6520 6669 6c65 206c 6973 740a  place file list.
+00004a50: 2020 2020 2020 2020 6966 2066 696c 7465          if filte
+00004a60: 7265 645f 6669 6c65 5f6c 6973 743a 0a20  red_file_list:. 
+00004a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004a80: 7365 745f 6669 6c65 7328 6669 6c74 6572  set_files(filter
+00004a90: 6564 5f66 696c 655f 6c69 7374 290a 2020  ed_file_list).  
+00004aa0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00004ab0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00004ac0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
+00004ad0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004ae0: 3d3d 3d3d 3d3d 0a20 2020 2020 2020 2023  ======.        #
+00004af0: 2043 6865 636b 2072 6177 2064 6174 610a   Check raw data.
+00004b00: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
+00004b10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004b20: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2020  =========.      
+00004b30: 2020 0a20 2020 2020 2020 2023 2069 6e69    .        # ini
+00004b40: 7469 616c 697a 6520 7573 6566 756c 2070  tialize useful p
+00004b50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00004b60: 2020 6e62 5f65 7665 6e74 735f 746f 7420    nb_events_tot 
+00004b70: 3d20 300a 2020 2020 2020 2020 6e62 5f63  = 0.        nb_c
+00004b80: 6861 6e6e 656c 7320 3d20 300a 2020 2020  hannels = 0.    
+00004b90: 2020 2020 6e62 5f73 616d 706c 6573 203d      nb_samples =
+00004ba0: 2030 0a20 2020 2020 2020 0a20 2020 2020   0.       .     
+00004bb0: 2020 2023 2073 656c 6563 7465 6420 6669     # selected fi
+00004bc0: 6c65 7320 2863 6173 6520 7365 7269 6573  les (case series
+00004bd0: 206e 756d 6265 7220 6f6e 6c79 2070 726f   number only pro
+00004be0: 7669 6465 6429 0a20 2020 2020 2020 2023  vided).        #
+00004bf0: 2020 2020 7475 706c 6520 2865 7665 6e74      tuple (event
+00004c00: 2069 6e64 6578 2c20 6669 6c65 2920 6966   index, file) if
+00004c10: 2065 7665 6e74 2070 726f 7669 6465 640a   event provided.
+00004c20: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00004c30: 5f65 7665 6e74 5f66 696c 6573 203d 206c  _event_files = l
+00004c40: 6973 7428 290a 2020 2020 0a20 2020 2020  ist().    .     
+00004c50: 2020 200a 2020 2020 2020 2020 2320 6c6f     .        # lo
+00004c60: 6f70 2066 696c 6573 2074 6f20 6765 7420  op files to get 
+00004c70: 6e75 6d62 6572 206f 6620 6576 656e 7473  number of events
+00004c80: 0a20 2020 2020 2020 2066 6f72 2066 696c  .        for fil
+00004c90: 655f 6e61 6d65 2069 6e20 7365 6c66 2e5f  e_name in self._
+00004ca0: 6669 6c65 5f6c 6973 743a 0a0a 2020 2020  file_list:..    
+00004cb0: 2020 2020 2020 2020 2320 6765 7420 6d65          # get me
+00004cc0: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
+00004cd0: 2020 206d 6574 6164 6174 6120 3d20 7365     metadata = se
+00004ce0: 6c66 2e67 6574 5f6d 6574 6164 6174 6128  lf.get_metadata(
+00004cf0: 6669 6c65 5f6e 616d 6529 0a20 2020 2020  file_name).     
+00004d00: 2020 2020 2020 2061 6463 5f6d 6574 6164         adc_metad
+00004d10: 6174 6120 3d20 6d65 7461 6461 7461 5b27  ata = metadata['
+00004d20: 6772 6f75 7073 275d 5b61 6463 5f6e 616d  groups'][adc_nam
+00004d30: 655d 0a0a 0a20 2020 2020 2020 2020 2020  e]...           
+00004d40: 2023 2065 7874 7261 6374 2064 756d 7020   # extract dump 
+00004d50: 616e 6420 7365 7269 6573 2062 6173 6564  and series based
+00004d60: 206f 6e20 6d65 7461 6461 7461 0a20 2020   on metadata.   
+00004d70: 2020 2020 2020 2020 2066 696c 655f 7365           file_se
+00004d80: 7269 6573 5f6e 756d 203d 204e 6f6e 650a  ries_num = None.
+00004d90: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+00004da0: 7365 7269 6573 5f6e 756d 2720 696e 206d  series_num' in m
+00004db0: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
+00004dc0: 2020 2020 2020 2020 2066 696c 655f 7365           file_se
+00004dd0: 7269 6573 5f6e 756d 203d 2069 6e74 286d  ries_num = int(m
+00004de0: 6574 6164 6174 615b 2773 6572 6965 735f  etadata['series_
+00004df0: 6e75 6d27 5d29 0a20 2020 2020 2020 2020  num']).         
+00004e00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00004e10: 2020 2020 2020 2020 2066 696c 655f 7365           file_se
+00004e20: 7269 6573 5f6e 756d 203d 2069 6e74 2865  ries_num = int(e
+00004e30: 7874 7261 6374 5f73 6572 6965 735f 6e75  xtract_series_nu
+00004e40: 6d28 6669 6c65 5f6e 616d 6529 290a 2020  m(file_name)).  
+00004e50: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00004e60: 2020 2020 2020 2023 2065 7874 7261 6374         # extract
+00004e70: 2064 756d 7020 6e75 6d62 6572 0a20 2020   dump number.   
+00004e80: 2020 2020 2020 2020 2066 696c 655f 6475           file_du
+00004e90: 6d70 5f6e 756d 203d 204e 6f6e 6520 200a  mp_num = None  .
+00004ea0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+00004eb0: 6475 6d70 5f6e 756d 2720 696e 206d 6574  dump_num' in met
+00004ec0: 6164 6174 613a 0a20 2020 2020 2020 2020  adata:.         
+00004ed0: 2020 2020 2020 2066 696c 655f 6475 6d70         file_dump
+00004ee0: 5f6e 756d 203d 2069 6e74 286d 6574 6164  _num = int(metad
+00004ef0: 6174 615b 2764 756d 705f 6e75 6d27 5d29  ata['dump_num'])
+00004f00: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00004f10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00004f20: 2020 2066 696c 655f 6475 6d70 5f6e 756d     file_dump_num
+00004f30: 203d 2069 6e74 2865 7874 7261 6374 5f64   = int(extract_d
+00004f40: 756d 705f 6e75 6d28 6669 6c65 5f6e 616d  ump_num(file_nam
+00004f50: 6529 290a 0a20 2020 2020 2020 2020 2020  e))..           
+00004f60: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00004f70: 2020 2020 2020 2020 2020 2320 6966 2065            # if e
+00004f80: 7665 6e74 5f6e 756d 733a 2020 6368 6563  vent_nums:  chec
+00004f90: 6b20 6669 6c65 2069 6620 6176 6169 6c61  k file if availa
+00004fa0: 626c 6520 616e 6420 7374 6f72 6520 6974  ble and store it
+00004fb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004fc0: 6576 656e 745f 6e75 6d73 2069 7320 6e6f  event_nums is no
+00004fd0: 7420 4e6f 6e65 3a0a 0a20 2020 2020 2020  t None:..       
+00004fe0: 2020 2020 2020 2020 206b 6565 705f 6669           keep_fi
+00004ff0: 6c65 203d 2046 616c 7365 0a0a 2020 2020  le = False..    
+00005000: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00005010: 6965 7665 6e74 2069 6e20 7261 6e67 6528  ievent in range(
+00005020: 6c65 6e28 6576 656e 745f 6e75 6d73 2929  len(event_nums))
+00005030: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005040: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
+00005050: 6620 6475 6d70 206e 756d 6265 7220 6d61  f dump number ma
+00005060: 7463 6820 6375 7272 656e 7420 6669 6c65  tch current file
+00005070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005080: 2020 2020 2069 6620 2869 6e74 2864 756d       if (int(dum
+00005090: 705f 6e75 6d73 5b69 6576 656e 745d 2921  p_nums[ievent])!
+000050a0: 3d66 696c 655f 6475 6d70 5f6e 756d 293a  =file_dump_num):
+000050b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000050c0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+000050d0: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+000050e0: 2020 2020 2020 2023 2063 6865 636b 2073         # check s
+000050f0: 6572 6965 7320 6d61 7463 6820 6375 7272  eries match curr
+00005100: 656e 7420 6669 6c65 0a20 2020 2020 2020  ent file.       
+00005110: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005120: 2869 6e74 2873 6572 6965 735f 6e75 6d73  (int(series_nums
+00005130: 5b69 6576 656e 745d 2921 3d66 696c 655f  [ievent])!=file_
+00005140: 7365 7269 6573 5f6e 756d 293a 0a20 2020  series_num):.   
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005180: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
+00005190: 2020 2020 2020 2023 2046 6f75 6e64 2066         # Found f
+000051a0: 696c 6521 0a20 2020 2020 2020 2020 2020  ile!.           
+000051b0: 2020 2020 2020 2020 206b 6565 705f 6669           keep_fi
+000051c0: 6c65 2020 3d20 5472 7565 0a0a 2020 2020  le  = True..    
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2320 6368 6563 6b20 696e 6465 7820 6176  # check index av
+000051f0: 6169 6c61 626c 650a 2020 2020 2020 2020  ailable.        
+00005200: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00005210: 745f 696e 6465 7820 3d20 6576 656e 745f  t_index = event_
+00005220: 696e 6469 6365 735b 6965 7665 6e74 5d0a  indices[ievent].
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00005250: 2020 2020 2020 2020 2069 6620 2865 7665           if (eve
+00005260: 6e74 5f69 6e64 6578 3e69 6e74 2861 6463  nt_index>int(adc
+00005270: 5f6d 6574 6164 6174 615b 276e 625f 6576  _metadata['nb_ev
+00005280: 656e 7473 275d 2929 3a0a 2020 2020 2020  ents'])):.      
+00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052a0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000052b0: 6f72 2827 4552 524f 523a 2046 6f75 6e64  or('ERROR: Found
+000052c0: 2066 696c 6520 666f 7220 6576 656e 7420   file for event 
+000052d0: 6e75 6d62 6572 2027 0a20 2020 2020 2020  number '.       
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 2020 2b20 7374 7228 6576 656e 745f 6e75    + str(event_nu
+00005310: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
+00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 2020 2020 2020 2020 2b20 2720              + ' 
+00005340: 686f 7765 7665 722c 2065 7665 6e74 2064  however, event d
+00005350: 6f65 7320 6e6f 7420 6578 6973 7421 2729  oes not exist!')
+00005360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005370: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00005380: 2020 2020 2020 2020 2020 2320 7374 6f72            # stor
+00005390: 6520 696e 206c 6973 7420 6173 2061 2074  e in list as a t
+000053a0: 7570 6c65 0a20 2020 2020 2020 2020 2020  uple.           
+000053b0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+000053c0: 645f 6576 656e 745f 6669 6c65 732e 6170  d_event_files.ap
+000053d0: 7065 6e64 2828 6576 656e 745f 696e 6465  pend((event_inde
+000053e0: 782c 2066 696c 655f 6e61 6d65 2929 0a0a  x, file_name))..
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005400: 2020 2020 2320 696e 6372 656d 656e 7420      # increment 
+00005410: 746f 7420 6e75 6d62 6572 206f 6620 6576  tot number of ev
+00005420: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00005430: 2020 2020 2020 2020 206e 625f 6576 656e           nb_even
+00005440: 7473 5f74 6f74 202b 3d20 310a 2020 2020  ts_tot += 1.    
+00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005460: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005470: 2020 2320 636f 6e74 696e 7565 2066 696c    # continue fil
+00005480: 6520 6c6f 6f70 2069 6620 6e6f 7420 6e65  e loop if not ne
+00005490: 6564 6564 0a20 2020 2020 2020 2020 2020  eded.           
+000054a0: 2020 2020 2069 6620 6e6f 7420 6b65 6570       if not keep
+000054b0: 5f66 696c 6520 3a0a 2020 2020 2020 2020  _file :.        
+000054c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000054d0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+000054e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000054f0: 2020 2020 2020 2020 6e62 5f65 7665 6e74          nb_event
+00005500: 735f 746f 7420 2b3d 2061 6463 5f6d 6574  s_tot += adc_met
+00005510: 6164 6174 615b 276e 625f 6576 656e 7473  adata['nb_events
+00005520: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+00005530: 2020 2069 6620 6e65 7665 6e74 733e 3020     if nevents>0 
+00005540: 2061 6e64 206e 625f 6576 656e 7473 5f74   and nb_events_t
+00005550: 6f74 3e3d 6e65 7665 6e74 733a 0a20 2020  ot>=nevents:.   
 00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005580: 2023 206c 6f6f 7020 6368 616e 6e65 6c73   # loop channels
-00005590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000055a0: 2063 6861 6e5f 636f 756e 7465 7220 3d20   chan_counter = 
-000055b0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-000055c0: 2020 666f 7220 6368 616e 5f6e 616d 6520    for chan_name 
-000055d0: 696e 2063 6f6e 6e65 6374 696f 6e73 5b27  in connections['
-000055e0: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
-000055f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005600: 2020 2020 2020 6966 2063 6861 6e5f 6e61        if chan_na
-00005610: 6d65 2069 6e20 6465 7465 6374 6f72 5f63  me in detector_c
-00005620: 6861 6e73 3a0a 2020 2020 2020 2020 2020  hans:.          
-00005630: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00005640: 616e 5f61 6463 203d 2069 6e74 2863 6f6e  an_adc = int(con
-00005650: 6e65 6374 696f 6e73 5b27 6164 635f 6368  nections['adc_ch
-00005660: 616e 7327 5d5b 6368 616e 5f63 6f75 6e74  ans'][chan_count
-00005670: 6572 5d29 0a20 2020 2020 2020 2020 2020  er]).           
-00005680: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005690: 6368 616e 5f61 6463 2069 6e20 6164 635f  chan_adc in adc_
-000056a0: 6368 616e 5f6c 6973 743a 0a20 2020 2020  chan_list:.     
+00005570: 206e 625f 6576 656e 7473 5f74 6f74 203d   nb_events_tot =
+00005580: 206e 6576 656e 7473 0a20 2020 2020 2020   nevents.       
+00005590: 2020 2020 2020 2020 200a 0a20 2020 2020           ..     
+000055a0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+000055b0: 2020 2023 2063 6865 636b 2063 6861 6e6e     # check chann
+000055c0: 656c 730a 2020 2020 2020 2020 2020 2020  els.            
+000055d0: 6e62 5f63 6861 6e6e 656c 735f 6669 6c65  nb_channels_file
+000055e0: 203d 2061 6463 5f6d 6574 6164 6174 615b   = adc_metadata[
+000055f0: 276e 625f 6368 616e 6e65 6c73 275d 0a20  'nb_channels']. 
+00005600: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005610: 2020 2020 6966 2064 6574 6563 746f 725f      if detector_
+00005620: 6368 616e 7320 6973 206e 6f74 204e 6f6e  chans is not Non
+00005630: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
+00005640: 2020 2020 2320 636f 6e6e 6563 7469 6f6e      # connection
+00005650: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00005660: 2020 636f 6e6e 6563 7469 6f6e 7320 3d20    connections = 
+00005670: 7365 6c66 2e67 6574 5f63 6f6e 6e65 6374  self.get_connect
+00005680: 696f 6e5f 6469 6374 2861 6463 5f6e 616d  ion_dict(adc_nam
+00005690: 653d 6164 635f 6e61 6d65 2c0a 2020 2020  e=adc_name,.    
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2020 2020 2069 6e64 203d 206e 702e         ind = np.
-000056d0: 7768 6572 6528 6164 635f 6368 616e 5f6c  where(adc_chan_l
-000056e0: 6973 743d 3d63 6861 6e5f 6164 6329 5b30  ist==chan_adc)[0
-000056f0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00005700: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005710: 206c 656e 2869 6e64 293d 3d31 3a0a 2020   len(ind)==1:.  
-00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005730: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00005740: 7261 795f 696e 6469 6365 735f 6669 6c65  ray_indices_file
-00005750: 2e61 7070 656e 6428 696e 7428 696e 6429  .append(int(ind)
-00005760: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005770: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005780: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056d0: 2020 206d 6574 6164 6174 613d 6d65 7461     metadata=meta
+000056e0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00005710: 2020 2020 2020 2023 206c 6f6f 7020 6368         # loop ch
+00005720: 616e 6e65 6c73 0a20 2020 2020 2020 2020  annels.         
+00005730: 2020 2020 2020 206e 625f 6368 616e 6e65         nb_channe
+00005740: 6c73 5f66 696c 6520 203d 2030 0a20 2020  ls_file  = 0.   
+00005750: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00005760: 2063 6861 6e5f 6e61 6d65 2069 6e20 636f   chan_name in co
+00005770: 6e6e 6563 7469 6f6e 735b 2764 6574 6563  nnections['detec
+00005780: 746f 725f 6368 616e 7327 5d3a 0a20 2020  tor_chans']:.   
 00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-000057b0: 7272 6f72 2827 5072 6f62 6c65 6d20 7769  rror('Problem wi
-000057c0: 7468 2072 6177 2064 6174 612e 2e27 290a  th raw data..').
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2020 6368 616e 5f63 6f75 6e74 6572      chan_counter
-000057f0: 2b3d 310a 2020 2020 2020 2020 2020 2020  +=1.            
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005820: 206e 625f 6368 616e 6e65 6c73 5f66 696c   nb_channels_fil
-00005830: 6520 3d20 6c65 6e28 6172 7261 795f 696e  e = len(array_in
-00005840: 6469 6365 735f 6669 6c65 290a 2020 2020  dices_file).    
-00005850: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00005860: 6e62 5f63 6861 6e6e 656c 735f 6669 6c65  nb_channels_file
-00005870: 3d3d 3029 3a0a 2020 2020 2020 2020 2020  ==0):.          
-00005880: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00005890: 6d73 6720 3d20 2827 556e 6162 6c65 2074  msg = ('Unable t
-000058a0: 6f20 6669 6e64 2073 656c 6563 7465 6420  o find selected 
-000058b0: 6368 616e 6e65 6c28 7329 2e27 0a20 2020  channel(s).'.   
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000058e0: 2720 4368 6563 6b20 636f 6e6e 6563 7469  ' Check connecti
-000058f0: 6f6e 2074 6162 6c65 2127 290a 2020 2020  on table!').    
-00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005910: 6966 2073 656c 662e 5f72 6169 7365 5f65  if self._raise_e
-00005920: 7272 6f72 733a 0a20 2020 2020 2020 2020  rrors:.         
-00005930: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00005940: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00005950: 6572 726f 725f 6d73 6729 0a20 2020 2020  error_msg).     
-00005960: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005970: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005980: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00005990: 6e74 2827 4552 524f 523a 2027 202b 2065  nt('ERROR: ' + e
-000059a0: 7272 6f72 5f6d 7367 290a 2020 2020 2020  rror_msg).      
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 6966 2069 6e63 6c75 6465 5f6d 6574    if include_met
-000059d0: 6164 6174 613a 0a20 2020 2020 2020 2020  adata:.         
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 2020 2072 6574 7572 6e20 5b5d 2c5b 5d0a     return [],[].
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005a40: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00005a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005a60: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00005a70: 7261 795f 696e 6469 6365 735f 6669 6c65  ray_indices_file
-00005a80: 2e73 6f72 7428 290a 0a20 2020 2020 2020  .sort()..       
-00005a90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00005aa0: 2020 2020 2020 2020 2020 2061 7272 6179             array
-00005ab0: 5f69 6e64 6963 6573 5f66 696c 6520 3d20  _indices_file = 
-00005ac0: 6c69 7374 2872 616e 6765 286e 625f 6368  list(range(nb_ch
-00005ad0: 616e 6e65 6c73 5f66 696c 6529 290a 0a20  annels_file)).. 
-00005ae0: 2020 2020 2020 2020 2020 2069 6620 6e62             if nb
-00005af0: 5f63 6861 6e6e 656c 733d 3d30 3a0a 2020  _channels==0:.  
-00005b00: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
-00005b10: 5f63 6861 6e6e 656c 7320 3d20 206e 625f  _channels =  nb_
-00005b20: 6368 616e 6e65 6c73 5f66 696c 650a 2020  channels_file.  
-00005b30: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00005b40: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00005b50: 7420 6172 7261 795f 696e 6469 6365 733a  t array_indices:
-00005b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005b70: 2061 7272 6179 5f69 6e64 6963 6573 203d   array_indices =
-00005b80: 2061 7272 6179 5f69 6e64 6963 6573 5f66   array_indices_f
-00005b90: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
-00005ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005bb0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
-00005bc0: 6368 6563 6b20 6368 616e 6e65 6c20 636f  check channel co
-00005bd0: 6e73 6973 7465 6e63 790a 2020 2020 2020  nsistency.      
-00005be0: 2020 2020 2020 6966 2061 7272 6179 5f69        if array_i
-00005bf0: 6e64 6963 6573 213d 6172 7261 795f 696e  ndices!=array_in
-00005c00: 6469 6365 735f 6669 6c65 3a0a 2020 2020  dices_file:.    
-00005c10: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00005c20: 725f 6d73 6720 3d20 2827 556e 6162 6c65  r_msg = ('Unable
-00005c30: 2074 6f20 7265 7475 726e 2061 7272 7261   to return arrra
-00005c40: 7920 6475 6520 746f 2069 6e63 6f6e 7369  y due to inconsi
-00005c50: 7374 656e 7420 2720 2b0a 2020 2020 2020  stent ' +.      
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 2020 2020 2027 6c69 7374 206f 6620         'list of 
-00005c80: 6368 616e 6e65 6c73 2062 6574 7765 656e  channels between
-00005c90: 2066 696c 6573 2127 290a 2020 2020 2020   files!').      
-00005ca0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005cb0: 662e 5f72 6169 7365 5f65 7272 6f72 733a  f._raise_errors:
-00005cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cd0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00005ce0: 4572 726f 7228 6572 726f 725f 6d73 6729  Error(error_msg)
-00005cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005d10: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00005d20: 2827 4552 524f 523a 2027 202b 2065 7272  ('ERROR: ' + err
-00005d30: 6f72 5f6d 7367 290a 2020 2020 2020 2020  or_msg).        
-00005d40: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00005d50: 6e63 6c75 6465 5f6d 6574 6164 6174 613a  nclude_metadata:
-00005d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005d80: 5b5d 2c5b 5d0a 2020 2020 2020 2020 2020  [],[].          
-00005d90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005db0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00005dc0: 5d0a 0a0a 2020 2020 2020 2020 2020 2020  ]...            
-00005dd0: 2320 6e75 6d62 6572 206f 6620 7361 6d70  # number of samp
-00005de0: 6c65 730a 2020 2020 2020 2020 2020 2020  les.            
-00005df0: 6e62 5f73 616d 706c 6573 5f66 696c 6520  nb_samples_file 
-00005e00: 3d20 6164 635f 6d65 7461 6461 7461 5b27  = adc_metadata['
-00005e10: 6e62 5f73 616d 706c 6573 275d 2020 200a  nb_samples']   .
-00005e20: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005e30: 625f 7361 6d70 6c65 733d 3d30 3a0a 2020  b_samples==0:.  
-00005e40: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
-00005e50: 5f73 616d 706c 6573 203d 2020 6e62 5f73  _samples =  nb_s
-00005e60: 616d 706c 6573 5f66 696c 650a 2020 2020  amples_file.    
-00005e70: 2020 2020 2020 2020 656c 6966 2020 6f75          elif  ou
-00005e80: 7470 7574 5f66 6f72 6d61 7421 3d31 2061  tput_format!=1 a
-00005e90: 6e64 206e 625f 7361 6d70 6c65 735f 6669  nd nb_samples_fi
-00005ea0: 6c65 213d 6e62 5f73 616d 706c 6573 3a0a  le!=nb_samples:.
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ec0: 6572 726f 725f 6d73 6720 3d20 2755 6e61  error_msg = 'Una
-00005ed0: 626c 6520 746f 2072 6574 7572 6e20 3344  ble to return 3D
-00005ee0: 2061 7272 7261 7920 6475 6520 746f 2069   arrray due to i
-00005ef0: 6e63 6f6e 7369 7374 656e 7420 6e62 206f  nconsistent nb o
-00005f00: 6620 7361 6d70 6c65 7321 270a 2020 2020  f samples!'.    
-00005f10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005f20: 656c 662e 5f72 6169 7365 5f65 7272 6f72  elf._raise_error
-00005f30: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00005f40: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00005f50: 7565 4572 726f 7228 6572 726f 725f 6d73  ueError(error_ms
-00005f60: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-00005f70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00005f80: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00005f90: 6e74 2827 4552 524f 523a 2027 202b 2065  nt('ERROR: ' + e
-00005fa0: 7272 6f72 5f6d 7367 290a 2020 2020 2020  rror_msg).      
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00005fc0: 696e 7428 2755 7365 206f 7574 7075 743d  int('Use output=
-00005fd0: 3120 2865 7665 6e74 206c 6973 7429 2069  1 (event list) i
-00005fe0: 6e73 7465 6164 206f 7220 6368 6563 6b20  nstead or check 
-00005ff0: 6669 6c65 7327 290a 2020 2020 2020 2020  files').        
-00006000: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00006010: 6e63 6c75 6465 5f6d 6574 6164 6174 613a  nclude_metadata:
-00006020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006030: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006040: 5b5d 2c5b 5d0a 2020 2020 2020 2020 2020  [],[].          
-00006050: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000057a0: 2069 6620 6368 616e 5f6e 616d 6520 696e   if chan_name in
+000057b0: 2064 6574 6563 746f 725f 6368 616e 733a   detector_chans:
+000057c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057d0: 2020 2020 2020 2020 206e 625f 6368 616e           nb_chan
+000057e0: 6e65 6c73 5f66 696c 6520 2b3d 310a 0a20  nels_file +=1.. 
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005810: 2020 2020 2020 2020 2320 6572 726f 7220          # error 
+00005820: 6966 206e 6f20 6368 616e 6e65 6c20 666f  if no channel fo
+00005830: 756e 640a 2020 2020 2020 2020 2020 2020  und.            
+00005840: 2020 2020 6966 2028 6e62 5f63 6861 6e6e      if (nb_chann
+00005850: 656c 735f 6669 6c65 3d3d 3029 3a0a 2020  els_file==0):.  
+00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005870: 2020 6572 726f 725f 6d73 6720 3d20 2827    error_msg = ('
+00005880: 556e 6162 6c65 2074 6f20 6669 6e64 2073  Unable to find s
+00005890: 656c 6563 7465 6420 6368 616e 6e65 6c28  elected channel(
+000058a0: 7329 2e27 0a20 2020 2020 2020 2020 2020  s).'.           
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2020 2020 2b20 2720 4368 6563 6b20        + ' Check 
+000058d0: 636f 6e6e 6563 7469 6f6e 2074 6162 6c65  connection table
+000058e0: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
+000058f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005900: 5f72 6169 7365 5f65 7272 6f72 733a 0a20  _raise_errors:. 
+00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005920: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00005930: 7565 4572 726f 7228 6572 726f 725f 6d73  ueError(error_ms
+00005940: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00005950: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005970: 2020 2020 2070 7269 6e74 2827 4552 524f       print('ERRO
+00005980: 523a 2027 202b 2065 7272 6f72 5f6d 7367  R: ' + error_msg
+00005990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000059a0: 2020 2020 2020 2020 2020 6966 2069 6e63            if inc
+000059b0: 6c75 6465 5f6d 6574 6164 6174 613a 0a20  lude_metadata:. 
+000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000059e0: 6e20 5b5d 2c5b 5d0a 2020 2020 2020 2020  n [],[].        
+000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 7265 7475 726e 205b 5d0a 2020 2020    return [].    
+00005a30: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
+00005a40: 2020 2020 2020 6966 206e 625f 6368 616e        if nb_chan
+00005a50: 6e65 6c73 3d3d 303a 0a20 2020 2020 2020  nels==0:.       
+00005a60: 2020 2020 2020 2020 206e 625f 6368 616e           nb_chan
+00005a70: 6e65 6c73 203d 2020 6e62 5f63 6861 6e6e  nels =  nb_chann
+00005a80: 656c 735f 6669 6c65 0a20 2020 2020 2020  els_file.       
+00005a90: 2020 2020 2065 6c69 6620 6e62 5f63 6861       elif nb_cha
+00005aa0: 6e6e 656c 7321 3d6e 625f 6368 616e 6e65  nnels!=nb_channe
+00005ab0: 6c73 5f66 696c 653a 0a20 2020 2020 2020  ls_file:.       
+00005ac0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00005ad0: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
+00005ae0: 3a20 696e 636f 6e73 6973 7465 6e74 206e  : inconsistent n
+00005af0: 756d 6265 7220 270a 2020 2020 2020 2020  umber '.        
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2020 2020 2020 2020 202b 2027 6f66 2063           + 'of c
+00005b20: 6861 6e6e 656c 7320 6265 7477 6565 6e20  hannels between 
+00005b30: 6669 6c65 7321 2729 0a20 2020 2020 2020  files!').       
+00005b40: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b60: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00005b70: 2020 2023 206e 756d 6265 7220 6f66 2073     # number of s
+00005b80: 616d 706c 6573 0a20 2020 2020 2020 2020  amples.         
+00005b90: 2020 206e 625f 7361 6d70 6c65 735f 6669     nb_samples_fi
+00005ba0: 6c65 203d 2061 6463 5f6d 6574 6164 6174  le = adc_metadat
+00005bb0: 615b 276e 625f 7361 6d70 6c65 7327 5d20  a['nb_samples'] 
+00005bc0: 2020 0a20 2020 2020 2020 2020 2020 2069    .            i
+00005bd0: 6620 6e62 5f73 616d 706c 6573 3d3d 303a  f nb_samples==0:
+00005be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005bf0: 206e 625f 7361 6d70 6c65 7320 3d20 206e   nb_samples =  n
+00005c00: 625f 7361 6d70 6c65 735f 6669 6c65 0a20  b_samples_file. 
+00005c10: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00005c20: 206f 7574 7075 745f 666f 726d 6174 213d   output_format!=
+00005c30: 3120 616e 6420 6e62 5f73 616d 706c 6573  1 and nb_samples
+00005c40: 5f66 696c 6521 3d6e 625f 7361 6d70 6c65  _file!=nb_sample
+00005c50: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00005c60: 2020 2065 7272 6f72 5f6d 7367 203d 2027     error_msg = '
+00005c70: 556e 6162 6c65 2074 6f20 7265 7475 726e  Unable to return
+00005c80: 2033 4420 6172 7272 6179 2064 7565 2074   3D arrray due t
+00005c90: 6f20 696e 636f 6e73 6973 7465 6e74 206e  o inconsistent n
+00005ca0: 6220 6f66 2073 616d 706c 6573 2127 0a20  b of samples!'. 
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005cc0: 6620 7365 6c66 2e5f 7261 6973 655f 6572  f self._raise_er
+00005cd0: 726f 7273 3a0a 2020 2020 2020 2020 2020  rors:.          
+00005ce0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00005cf0: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
+00005d00: 5f6d 7367 290a 2020 2020 2020 2020 2020  _msg).          
+00005d10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 7072 696e 7428 2745 5252 4f52 3a20 2720  print('ERROR: ' 
+00005d40: 2b20 6572 726f 725f 6d73 6729 0a20 2020  + error_msg).   
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2070 7269 6e74 2827 5573 6520 6f75 7470   print('Use outp
+00005d70: 7574 3d31 2028 6576 656e 7420 6c69 7374  ut=1 (event list
+00005d80: 2920 696e 7374 6561 6420 6f72 2063 6865  ) instead or che
+00005d90: 636b 2066 696c 6573 2729 0a20 2020 2020  ck files').     
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005db0: 6620 696e 636c 7564 655f 6d65 7461 6461  f include_metada
+00005dc0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00005dd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005de0: 726e 205b 5d2c 5b5d 0a20 2020 2020 2020  rn [],[].       
+00005df0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00005e00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00005e10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00005e20: 6e20 5b5d 0a0a 2020 2020 2020 2020 2020  n []..          
+00005e30: 2020 2320 6368 6563 6b20 6d61 7820 6576    # check max ev
+00005e40: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00005e50: 2069 6620 286e 6576 656e 7473 3e30 2020   if (nevents>0  
+00005e60: 616e 6420 6e62 5f65 7665 6e74 735f 746f  and nb_events_to
+00005e70: 743e 3d6e 6576 656e 7473 293a 0a20 2020  t>=nevents):.   
+00005e80: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00005e90: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
+00005ea0: 0a20 2020 2020 2020 2023 2063 6c65 6172  .        # clear
+00005eb0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+00005ec0: 6561 7228 290a 0a0a 2020 2020 2020 2020  ear()...        
+00005ed0: 2320 6368 6563 6b20 6e75 6d62 6572 206f  # check number o
+00005ee0: 6620 6576 656e 7473 0a20 2020 2020 2020  f events.       
+00005ef0: 2069 6620 6e62 5f65 7665 6e74 735f 746f   if nb_events_to
+00005f00: 7420 3d3d 2030 3a0a 2020 2020 2020 2020  t == 0:.        
+00005f10: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00005f20: 7272 6f72 2827 4552 524f 523a 204e 6f20  rror('ERROR: No 
+00005f30: 6576 656e 7473 2066 6f75 6e64 2127 290a  events found!').
+00005f40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005f50: 2069 6620 2865 7665 6e74 5f6e 756d 7320   if (event_nums 
+00005f60: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00005f70: 2020 2020 2020 2020 616e 6420 6e62 5f65          and nb_e
+00005f80: 7665 6e74 735f 746f 743c 6c65 6e28 6576  vents_tot<len(ev
+00005f90: 656e 745f 6e75 6d73 2929 3a0a 2020 2020  ent_nums)):.    
+00005fa0: 2020 2020 2020 2020 7072 696e 7428 2757          print('W
+00005fb0: 4152 4e49 4e47 3a20 4f6e 6c79 2027 202b  ARNING: Only ' +
+00005fc0: 2073 7472 286e 625f 6576 656e 7473 5f74   str(nb_events_t
+00005fd0: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
+00005fe0: 2020 2020 2020 2b20 2720 6576 656e 7473        + ' events
+00005ff0: 206f 7574 206f 6620 270a 2020 2020 2020   out of '.      
+00006000: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
+00006010: 7228 6c65 6e28 6576 656e 745f 6e75 6d73  r(len(event_nums
+00006020: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00006030: 2020 2020 202b 2027 2068 6176 6520 6265       + ' have be
+00006040: 656e 2066 6f75 6e64 2127 290a 2020 2020  en found!').    
+00006050: 2020 2020 2020 2020 0a20 2020 200a 0a0a          .    ...
 00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00006080: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
-00006090: 2063 6865 636b 206d 6178 2065 7665 6e74   check max event
-000060a0: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
-000060b0: 206e 6576 656e 7473 3e30 2020 616e 6420   nevents>0  and 
-000060c0: 6e62 5f65 7665 6e74 735f 746f 743e 3d6e  nb_events_tot>=n
-000060d0: 6576 656e 7473 3a0a 2020 2020 2020 2020  events:.        
-000060e0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-000060f0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00006100: 2020 2020 2320 636c 6561 720a 2020 2020      # clear.    
-00006110: 2020 2020 7365 6c66 2e63 6c65 6172 2829      self.clear()
-00006120: 0a0a 0a20 2020 2020 2020 2023 2063 6865  ...        # che
-00006130: 636b 206e 756d 6265 7220 6f66 2065 7665  ck number of eve
-00006140: 6e74 730a 2020 2020 2020 2020 6966 206e  nts.        if n
-00006150: 625f 6576 656e 7473 5f74 6f74 203d 3d20  b_events_tot == 
-00006160: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00006170: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00006180: 2745 5252 4f52 3a20 4e6f 2065 7665 6e74  'ERROR: No event
-00006190: 7320 666f 756e 6421 2729 0a20 2020 2020  s found!').     
-000061a0: 2020 200a 2020 2020 2020 2020 6966 2065     .        if e
-000061b0: 7665 6e74 5f6e 756d 7320 6973 206e 6f74  vent_nums is not
-000061c0: 204e 6f6e 653a 0a0a 2020 2020 2020 2020   None:..        
-000061d0: 2020 2020 6966 206e 625f 6576 656e 7473      if nb_events
-000061e0: 5f74 6f74 3e6c 656e 2865 7665 6e74 5f6e  _tot>len(event_n
-000061f0: 756d 7329 3a0a 0a20 2020 2020 2020 2020  ums):..         
-00006200: 2020 2020 2020 2069 6620 7365 7269 6573         if series
-00006210: 5f6e 756d 7320 6973 204e 6f6e 653a 0a20  _nums is None:. 
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00006240: 726f 7228 2745 5252 4f52 3a20 4d75 6c74  ror('ERROR: Mult
-00006250: 6970 6c65 2065 7665 6e74 7320 666f 756e  iple events foun
-00006260: 6420 7769 7468 2073 616d 6520 270a 2020  d with same '.  
-00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 202b 2027 6576 656e 7420 6e75 6d62     + 'event numb
-000062a0: 6572 2e20 2273 6572 6965 735f 6e75 6d73  er. "series_nums
-000062b0: 2220 6172 6775 6d65 6e74 2027 0a20 2020  " argument '.   
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2b20 2769 7320 7265 7175 6972 6564    + 'is required
-000062f0: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
-00006300: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006310: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00006320: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-00006330: 4552 524f 523a 204d 756c 7469 706c 6520  ERROR: Multiple 
-00006340: 6576 656e 7473 2066 6f75 6e64 2077 6974  events found wit
-00006350: 6820 7361 6d65 2027 0a20 2020 2020 2020  h same '.       
-00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006370: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00006380: 2765 7665 6e74 206e 756d 6265 722e 2053  'event number. S
-00006390: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
-000063a0: 6f6e 672e 2e2e 2729 0a0a 2020 2020 2020  ong...')..      
-000063b0: 2020 2020 2020 656c 6966 206e 625f 6576        elif nb_ev
-000063c0: 656e 7473 5f74 6f74 3c6c 656e 2865 7665  ents_tot<len(eve
-000063d0: 6e74 5f6e 756d 7329 3a0a 2020 2020 2020  nt_nums):.      
-000063e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000063f0: 2757 4152 4e49 4e47 3a20 4f6e 6c79 2027  'WARNING: Only '
-00006400: 202b 2073 7472 286e 625f 6576 656e 7473   + str(nb_events
-00006410: 5f74 6f74 290a 2020 2020 2020 2020 2020  _tot).          
-00006420: 2020 2020 2020 2020 2020 2020 2b20 2720              + ' 
-00006430: 6576 656e 7473 206f 7574 206f 6620 270a  events out of '.
-00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006450: 2020 2020 2020 2b20 7374 7228 6c65 6e28        + str(len(
-00006460: 6576 656e 745f 6e75 6d73 2929 0a20 2020  event_nums)).   
-00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006480: 2020 202b 2027 2068 6176 6520 6265 656e     + ' have been
-00006490: 2066 6f75 6e64 2127 290a 2020 2020 0a20   found!').    . 
-000064a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000064b0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
-000064c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000064d0: 3d0a 2020 2020 2020 2020 2320 4d65 6d6f  =.        # Memo
-000064e0: 7279 2063 6865 636b 0a20 2020 2020 2020  ry check.       
-000064f0: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   # =============
-00006500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006510: 3d3d 0a20 2020 2020 2020 2020 2020 2020  ==.             
-00006520: 2020 200a 2020 2020 2020 2020 7361 6d70     .        samp
-00006530: 6c65 5f62 7974 6573 203d 2032 0a20 2020  le_bytes = 2.   
-00006540: 2020 2020 2069 6620 6164 6374 6f76 6f6c       if adctovol
-00006550: 7420 6f72 2061 6463 746f 616d 7020 6f72  t or adctoamp or
-00006560: 2062 6173 656c 696e 6573 7562 3a0a 2020   baselinesub:.  
-00006570: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
-00006580: 5f62 7974 6573 203d 2038 0a20 2020 2020  _bytes = 8.     
-00006590: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000065a0: 6f75 7470 7574 5f6d 656d 6f72 795f 7065  output_memory_pe
-000065b0: 725f 6576 656e 7420 3d20 7361 6d70 6c65  r_event = sample
-000065c0: 5f62 7974 6573 2a6e 625f 7361 6d70 6c65  _bytes*nb_sample
-000065d0: 732a 6e62 5f63 6861 6e6e 656c 732f 3165  s*nb_channels/1e
-000065e0: 390a 2020 2020 2020 2020 6f75 7470 7574  9.        output
-000065f0: 5f6d 656d 6f72 7920 3d20 6e62 5f65 7665  _memory = nb_eve
-00006600: 6e74 735f 746f 742a 6f75 7470 7574 5f6d  nts_tot*output_m
-00006610: 656d 6f72 795f 7065 725f 6576 656e 740a  emory_per_event.
-00006620: 2020 2020 2020 2020 6966 206f 7574 7075          if outpu
-00006630: 745f 6d65 6d6f 7279 3e6d 656d 6f72 795f  t_memory>memory_
-00006640: 6c69 6d69 743a 0a20 2020 2020 2020 2020  limit:.         
-00006650: 2020 206e 625f 6576 656e 7473 5f74 6f74     nb_events_tot
-00006660: 5f74 656d 7020 3d20 696e 7428 726f 756e  _temp = int(roun
-00006670: 6428 6d65 6d6f 7279 5f6c 696d 6974 2f6f  d(memory_limit/o
-00006680: 7574 7075 745f 6d65 6d6f 7279 5f70 6572  utput_memory_per
-00006690: 5f65 7665 6e74 2929 0a20 2020 2020 2020  _event)).       
-000066a0: 2020 2020 2070 7269 6e74 2827 5741 524e       print('WARN
-000066b0: 494e 473a 204d 6178 206e 756d 6265 7220  ING: Max number 
-000066c0: 6576 656e 7473 2062 6173 6564 206f 6e20  events based on 
-000066d0: 6d65 6d6f 7279 206c 696d 6974 206f 6620  memory limit of 
-000066e0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000066f0: 2020 2020 2b20 7374 7228 6d65 6d6f 7279      + str(memory
-00006700: 5f6c 696d 6974 2920 2b20 2747 4220 6973  _limit) + 'GB is
-00006710: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00006720: 2020 2020 202b 2073 7472 286e 625f 6576       + str(nb_ev
-00006730: 656e 7473 5f74 6f74 5f74 656d 7029 202b  ents_tot_temp) +
-00006740: 2027 206f 7574 206f 6620 270a 2020 2020   ' out of '.    
-00006750: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00006760: 7374 7228 6e62 5f65 7665 6e74 735f 746f  str(nb_events_to
-00006770: 7429 202b 2721 2729 0a20 2020 2020 2020  t) +'!').       
-00006780: 2020 2020 206e 625f 6576 656e 7473 5f74       nb_events_t
-00006790: 6f74 203d 206e 625f 6576 656e 7473 5f74  ot = nb_events_t
-000067a0: 6f74 5f74 656d 700a 0a0a 0a0a 2020 2020  ot_temp.....    
-000067b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000067c0: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   # =============
-000067d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000067e0: 3d3d 0a20 2020 2020 2020 2023 2020 496e  ==.        #  In
-000067f0: 6974 6961 6c69 7a65 206f 7574 7075 740a  itialize output.
-00006800: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
-00006810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006820: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2020  =========.      
-00006830: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00006840: 2020 2020 2020 6f75 7470 7574 5f64 6174        output_dat
-00006850: 6120 3d20 6c69 7374 2829 0a20 2020 2020  a = list().     
-00006860: 2020 2069 6e66 6f5f 6c69 7374 203d 206c     info_list = l
-00006870: 6973 7428 290a 2020 2020 200a 2020 2020  ist().     .    
-00006880: 2020 2020 6966 206f 7574 7075 745f 666f      if output_fo
-00006890: 726d 6174 3d3d 323a 0a20 2020 2020 2020  rmat==2:.       
-000068a0: 2020 2020 2069 6620 6164 6374 6f76 6f6c       if adctovol
-000068b0: 7420 6f72 2061 6463 746f 616d 7020 6f72  t or adctoamp or
-000068c0: 2062 6173 656c 696e 6573 7562 3a0a 2020   baselinesub:.  
-000068d0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-000068e0: 7470 7574 5f64 6174 6120 3d20 6e70 2e7a  tput_data = np.z
-000068f0: 6572 6f73 2828 6e62 5f65 7665 6e74 735f  eros((nb_events_
-00006900: 746f 742c 206e 625f 6368 616e 6e65 6c73  tot, nb_channels
-00006910: 2c20 6e62 5f73 616d 706c 6573 292c 0a20  , nb_samples),. 
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 2020 6474 7970 653d 6e70 2e66        dtype=np.f
-00006950: 6c6f 6174 3634 290a 2020 2020 2020 2020  loat64).        
-00006960: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006970: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00006980: 5f64 6174 6120 3d20 6e70 2e7a 6572 6f73  _data = np.zeros
-00006990: 2828 6e62 5f65 7665 6e74 735f 746f 742c  ((nb_events_tot,
-000069a0: 206e 625f 6368 616e 6e65 6c73 2c20 6e62   nb_channels, nb
-000069b0: 5f73 616d 706c 6573 292c 0a20 2020 2020  _samples),.     
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 6474 7970 653d 6e70 2e69 6e74 3136    dtype=np.int16
-000069f0: 290a 0a0a 2020 2020 2020 2020 2020 2020  )...            
-00006a00: 2020 2020 0a20 2020 2020 2020 2023 203d      .        # =
-00006a10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006a20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
-00006a30: 2020 2020 2020 2023 2020 4c6f 6f70 2061         #  Loop a
-00006a40: 6e64 2072 6561 6420 6576 656e 7473 0a20  nd read events. 
-00006a50: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-00006a60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006a70: 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020 2020  ========..      
-00006a80: 2020 2320 7265 7365 7420 6c69 7374 206f    # reset list o
-00006a90: 6620 6669 6c65 7320 6966 206e 6565 6465  f files if neede
-00006aa0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00006ab0: 6563 7465 645f 6669 6c65 7320 6973 206e  ected_files is n
-00006ac0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00006ad0: 2020 2020 2073 656c 662e 7365 745f 6669       self.set_fi
-00006ae0: 6c65 7328 7365 6c65 6374 6564 5f66 696c  les(selected_fil
-00006af0: 6573 290a 0a20 2020 2020 2020 2023 206c  es)..        # l
-00006b00: 6f6f 7020 6576 656e 7473 0a20 2020 2020  oop events.     
-00006b10: 2020 2066 6f72 2069 6576 656e 7420 696e     for ievent in
-00006b20: 2072 616e 6765 286e 625f 6576 656e 7473   range(nb_events
-00006b30: 5f74 6f74 293a 0a20 2020 2020 2020 2020  _tot):.         
-00006b40: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00006b50: 2320 7265 6164 2065 7665 6e74 0a20 2020  # read event.   
-00006b60: 2020 2020 2020 2020 2074 7261 6365 7320           traces 
-00006b70: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00006b80: 2069 6e66 6f20 3d20 6469 6374 2829 0a0a   info = dict()..
-00006b90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00006ba0: 656c 6563 7465 645f 6576 656e 745f 6669  elected_event_fi
-00006bb0: 6c65 7320 6973 204e 6f6e 653a 0a20 2020  les is None:.   
-00006bc0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00006bd0: 6365 732c 2069 6e66 6f20 3d20 7365 6c66  ces, info = self
-00006be0: 2e72 6561 645f 6e65 7874 5f65 7665 6e74  .read_next_event
-00006bf0: 2864 6574 6563 746f 725f 6368 616e 733d  (detector_chans=
-00006c00: 6465 7465 6374 6f72 5f63 6861 6e73 2c0a  detector_chans,.
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 6164 6374 6f76 6f6c 743d 6164      adctovolt=ad
-00006c50: 6374 6f76 6f6c 742c 2061 6463 746f 616d  ctovolt, adctoam
-00006c60: 703d 6164 6374 6f61 6d70 2c0a 2020 2020  p=adctoamp,.    
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ca0: 6261 7365 6c69 6e65 7375 623d 6261 7365  baselinesub=base
-00006cb0: 6c69 6e65 7375 622c 0a20 2020 2020 2020  linesub,.       
-00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-00006cf0: 656c 696e 6569 6e64 733d 6261 7365 6c69  elineinds=baseli
-00006d00: 6e65 696e 6473 2c0a 2020 2020 2020 2020  neinds,.        
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d30: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-00006d40: 7564 655f 6d65 7461 6461 7461 3d54 7275  ude_metadata=Tru
-00006d50: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
-00006d60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00006d70: 2020 2020 2065 7665 6e74 5f69 6e64 6578       event_index
-00006d80: 203d 2073 656c 6563 7465 645f 6576 656e   = selected_even
-00006d90: 745f 6669 6c65 735b 6965 7665 6e74 5d5b  t_files[ievent][
-00006da0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-00006db0: 2020 2066 696c 655f 6e61 6d65 203d 2073     file_name = s
-00006dc0: 656c 6563 7465 645f 6576 656e 745f 6669  elected_event_fi
-00006dd0: 6c65 735b 6965 7665 6e74 5d5b 315d 0a20  les[ievent][1]. 
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00006df0: 7261 6365 732c 2069 6e66 6f20 3d20 7365  races, info = se
-00006e00: 6c66 2e72 6561 645f 7369 6e67 6c65 5f65  lf.read_single_e
-00006e10: 7665 6e74 2865 7665 6e74 5f69 6e64 6578  vent(event_index
-00006e20: 2c20 6669 6c65 5f6e 616d 653d 6669 6c65  , file_name=file
-00006e30: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 2020 2020 2064 6574               det
-00006e70: 6563 746f 725f 6368 616e 733d 6465 7465  ector_chans=dete
-00006e80: 6374 6f72 5f63 6861 6e73 2c0a 2020 2020  ctor_chans,.    
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 6164 6374 6f76 6f6c 743d 6164 6374    adctovolt=adct
-00006ed0: 6f76 6f6c 742c 2061 6463 746f 616d 703d  ovolt, adctoamp=
-00006ee0: 6164 6374 6f61 6d70 2c0a 2020 2020 2020  adctoamp,.      
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f20: 6261 7365 6c69 6e65 7375 623d 6261 7365  baselinesub=base
-00006f30: 6c69 6e65 7375 622c 0a20 2020 2020 2020  linesub,.       
-00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00006f70: 6173 656c 696e 6569 6e64 733d 6261 7365  aselineinds=base
-00006f80: 6c69 6e65 696e 6473 2c0a 2020 2020 2020  lineinds,.      
-00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 696e 636c 7564 655f 6d65 7461 6461 7461  include_metadata
-00006fd0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00006fe0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006ff0: 2020 2020 2320 6368 6563 6b20 6966 2072      # check if r
-00007000: 6561 6469 6e67 2065 7272 6f72 0a20 2020  eading error.   
-00007010: 2020 2020 2020 2020 2069 6620 696e 666f           if info
-00007020: 5b27 7265 6164 5f73 7461 7475 7327 5d3e  ['read_status']>
-00007030: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00007040: 2020 2070 7269 6e74 2827 5741 524e 494e     print('WARNIN
-00007050: 473a 2055 6e61 626c 6520 746f 2072 6561  G: Unable to rea
-00007060: 6420 6576 656e 7420 2327 202b 2073 7472  d event #' + str
-00007070: 2869 6576 656e 7429 202b 2027 2120 4572  (ievent) + '! Er
-00007080: 726f 7220 6d65 7373 6167 653a 2027 290a  ror message: ').
-00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 7072 696e 7428 2757 4152 4e49 4e47 3a20  print('WARNING: 
-000070b0: 2227 202b 2069 6e66 6f5b 2765 7272 6f72  "' + info['error
-000070c0: 5f6d 7367 275d 202b 2027 222e 2053 746f  _msg'] + '". Sto
-000070d0: 7070 696e 6720 6576 656e 7420 6c6f 6f70  pping event loop
-000070e0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-000070f0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-00007100: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00007110: 2020 2023 2061 6464 2074 6f20 6d65 7461     # add to meta
-00007120: 6461 7461 206c 6973 740a 2020 2020 2020  data list.      
-00007130: 2020 2020 2020 6966 2069 6e63 6c75 6465        if include
-00007140: 5f6d 6574 6164 6174 613a 0a20 2020 2020  _metadata:.     
-00007150: 2020 2020 2020 2020 2020 2069 6e66 6f5f             info_
-00007160: 6c69 7374 2e61 7070 656e 6428 696e 666f  list.append(info
-00007170: 290a 0a20 2020 2020 2020 2020 2020 200a  )..            .
-00007180: 2020 2020 2020 2020 2020 2020 2320 7374              # st
-00007190: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
-000071a0: 6966 2028 6f75 7470 7574 5f66 6f72 6d61  if (output_forma
-000071b0: 743d 3d31 206f 7220 6f75 7470 7574 5f66  t==1 or output_f
-000071c0: 6f72 6d61 743d 3d33 293a 0a20 2020 2020  ormat==3):.     
-000071d0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-000071e0: 745f 6461 7461 2e61 7070 656e 6428 7472  t_data.append(tr
-000071f0: 6163 6573 290a 2020 2020 2020 2020 2020  aces).          
-00007200: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007210: 2020 2020 2020 2020 6f75 7470 7574 5f64          output_d
-00007220: 6174 615b 6965 7665 6e74 2c3a 2c3a 5d20  ata[ievent,:,:] 
-00007230: 3d20 7472 6163 6573 0a20 2020 2020 2020  = traces.       
-00007240: 2020 2020 2020 2020 200a 0a20 2020 2020           ..     
-00007250: 2020 2023 2072 6573 6574 2066 696c 6520     # reset file 
-00007260: 6c69 7374 2074 6f20 6f72 6967 696e 616c  list to original
-00007270: 206c 6973 740a 2020 2020 2020 2020 2320   list.        # 
-00007280: 6966 206e 6565 6465 640a 2020 2020 2020  if needed.      
-00007290: 2020 6966 2063 7572 7265 6e74 5f66 696c    if current_fil
-000072a0: 655f 6c69 7374 2069 7320 6e6f 7420 4e6f  e_list is not No
-000072b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000072c0: 7365 6c66 2e73 6574 5f66 696c 6573 2863  self.set_files(c
-000072d0: 7572 7265 6e74 5f66 696c 655f 6c69 7374  urrent_file_list
-000072e0: 290a 0a0a 2020 2020 2020 2020 6966 2069  )...        if i
-000072f0: 6e63 6c75 6465 5f6d 6574 6164 6174 613a  nclude_metadata:
-00007300: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007310: 7572 6e20 6f75 7470 7574 5f64 6174 612c  urn output_data,
-00007320: 2069 6e66 6f5f 6c69 7374 0a20 2020 2020   info_list.     
-00007330: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007340: 2020 2020 2072 6574 7572 6e20 6f75 7470       return outp
-00007350: 7574 5f64 6174 610a 2020 2020 2020 2020  ut_data.        
-00007360: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007370: 2020 0a20 2020 2020 2020 2020 2020 200a    .            .
-00007380: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00007390: 2020 2020 200a 0a20 2020 2064 6566 2067       ..    def g
-000073a0: 6574 5f63 7572 7265 6e74 5f66 696c 655f  et_current_file_
-000073b0: 6e61 6d65 2873 656c 6629 3a0a 2020 2020  name(self):.    
-000073c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000073d0: 4765 7420 6375 7272 656e 7420 6669 6c65  Get current file
-000073e0: 206e 616d 650a 2020 2020 2020 2020 0a20   name.        . 
-000073f0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00007400: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00007410: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00007420: 650a 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-00007430: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
-00007440: 2d0a 2020 2020 2020 2020 0a20 2020 2020  -.        .     
-00007450: 2020 2066 696c 655f 6e61 6d65 203a 2073     file_name : s
-00007460: 7472 0a20 2020 2020 2020 2020 2063 7572  tr.          cur
-00007470: 7265 6e74 2066 696c 6520 6e61 6d65 0a0a  rent file name..
-00007480: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007490: 2020 2020 0a20 2020 2020 2020 2072 6574      .        ret
-000074a0: 7572 6e20 7365 6c66 2e5f 6375 7272 656e  urn self._curren
-000074b0: 745f 6669 6c65 5f6e 616d 650a 2020 2020  t_file_name.    
-000074c0: 2020 2020 0a0a 0a20 2020 200a 2020 2020      ...    .    
-000074d0: 6465 6620 6765 745f 6d65 7461 6461 7461  def get_metadata
-000074e0: 2873 656c 662c 2066 696c 655f 6e61 6d65  (self, file_name
-000074f0: 3d4e 6f6e 652c 2067 726f 7570 5f6e 616d  =None, group_nam
-00007500: 653d 4e6f 6e65 2c20 6461 7461 7365 745f  e=None, dataset_
-00007510: 6e61 6d65 3d4e 6f6e 652c 200a 2020 2020  name=None, .    
-00007520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007530: 2069 6e63 6c75 6465 5f64 6174 6173 6574   include_dataset
-00007540: 5f6d 6574 6164 6174 613d 4661 6c73 6529  _metadata=False)
-00007550: 3a0a 0a20 2020 2020 2020 2022 2222 0a20  :..        """. 
-00007560: 2020 2020 2020 2046 756e 6374 696f 6e20         Function 
-00007570: 746f 2067 6574 206d 6574 6164 6174 612e  to get metadata.
-00007580: 0a20 2020 2020 2020 0a20 2020 2020 2020  .       .       
-00007590: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000075a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000075b0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-000075c0: 2020 6669 6c65 5f6e 616d 653a 2073 7472    file_name: str
-000075d0: 696e 672c 206f 7074 696f 6e61 6c0a 2020  ing, optional.  
-000075e0: 2020 2020 2020 2020 2020 6966 206e 6f20            if no 
-000075f0: 6669 6c65 206e 616d 6520 7072 6f76 6964  file name provid
-00007600: 6564 3a20 7573 6520 6375 7272 656e 7420  ed: use current 
-00007610: 6669 6c65 0a0a 2020 2020 2020 2020 6772  file..        gr
-00007620: 6f75 705f 6e61 6d65 3a20 2073 7472 696e  oup_name:  strin
-00007630: 672c 206f 7074 696f 6e61 6c0a 2020 2020  g, optional.    
-00007640: 2020 2020 2020 2020 4835 2022 4772 6f75          H5 "Grou
-00007650: 7022 206e 616d 650a 2020 2020 2020 2020  p" name.        
-00007660: 2020 2020 4465 6661 756c 743a 204e 6f6e      Default: Non
-00007670: 652c 2072 6561 6420 616c 6c20 6772 6f75  e, read all grou
-00007680: 7073 0a20 2020 2020 2020 2020 200a 2020  ps.          .  
-00007690: 2020 2020 2020 6461 7461 7365 745f 6e61        dataset_na
-000076a0: 6d65 3a20 7374 7269 6e67 2c20 6f70 7469  me: string, opti
-000076b0: 6f6e 616c 2c20 0a20 2020 2020 2020 2020  onal, .         
-000076c0: 2020 2048 3520 2244 6174 6173 6574 2220     H5 "Dataset" 
-000076d0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-000076e0: 2044 6566 6175 6c74 3a20 616c 6c20 6461   Default: all da
-000076f0: 7461 7365 7473 0a20 2020 2020 2020 2020  tasets.         
-00007700: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
-00007710: 5f64 6174 6173 6574 5f6d 6574 6164 6174  _dataset_metadat
-00007720: 6120 3a20 626f 6f6c 2c20 6f70 7469 6f6e  a : bool, option
-00007730: 616c 0a20 2020 2020 2020 2020 2020 2049  al.            I
-00007740: 6620 5472 7565 2c20 696e 636c 7564 6520  f True, include 
-00007750: 6461 7461 7365 7420 6d65 7461 6461 7461  dataset metadata
-00007760: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
-00007770: 6175 6c74 3a20 4661 6c73 650a 2020 2020  ault: False.    
-00007780: 2020 2020 0a0a 2020 2020 2020 2020 5265      ..        Re
-00007790: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
-000077a0: 2d2d 2d0a 2020 2020 2020 2020 0a20 2020  ---.        .   
-000077b0: 2020 2020 206d 6574 6164 6174 613a 2064       metadata: d
-000077c0: 6963 740a 2020 2020 2020 2020 2020 2064  ict.           d
-000077d0: 6963 7469 6f6e 6172 7920 7769 7468 2061  ictionary with a
-000077e0: 6c6c 206d 6574 6164 6174 610a 0a20 2020  ll metadata..   
-000077f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00007800: 2020 6d65 7461 6461 7461 203d 2064 6963    metadata = dic
-00007810: 7428 290a 0a0a 2020 2020 2020 2020 2320  t()...        # 
-00007820: 6368 6563 6b20 696e 7075 7420 0a20 2020  check input .   
-00007830: 2020 2020 2069 6620 6669 6c65 5f6e 616d       if file_nam
-00007840: 6520 6973 204e 6f6e 6520 616e 6420 7365  e is None and se
-00007850: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-00007860: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00007870: 2020 2020 2020 6572 726f 725f 6d73 6720        error_msg 
-00007880: 3d20 274e 6f20 6669 6c65 2063 7572 7265  = 'No file curre
-00007890: 6e74 6c79 206f 7065 6e20 616e 6420 6e6f  ntly open and no
-000078a0: 2022 6669 6c65 5f6e 616d 6522 2061 7267   "file_name" arg
-000078b0: 756d 656e 7420 6e6f 7420 7072 6f76 6964  ument not provid
-000078c0: 6564 2127 0a20 2020 2020 2020 2020 2020  ed!'.           
-000078d0: 2069 6620 7365 6c66 2e5f 7261 6973 655f   if self._raise_
-000078e0: 6572 726f 7273 3a0a 2020 2020 2020 2020  errors:.        
-000078f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00007900: 6520 5661 6c75 6545 7272 6f72 2865 7272  e ValueError(err
-00007910: 6f72 5f6d 7367 290a 2020 2020 2020 2020  or_msg).        
-00007920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00007930: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00007940: 2745 5252 4f52 3a20 2720 2b20 6572 726f  'ERROR: ' + erro
-00007950: 725f 6d73 6729 0a20 2020 2020 2020 2020  r_msg).         
-00007960: 2020 2020 2020 2070 7269 6e74 2827 506c         print('Pl
-00007970: 6561 7365 206f 7065 6e20 6120 6669 6c65  ease open a file
-00007980: 206f 7220 7072 6f76 6964 6520 6120 6669   or provide a fi
-00007990: 6c65 206e 616d 6521 2729 0a20 2020 2020  le name!').     
-000079a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000079b0: 6e20 6d65 7461 6461 7461 0a0a 2020 2020  n metadata..    
-000079c0: 2020 2020 2320 6f70 656e 2066 696c 6520      # open file 
-000079d0: 6966 206e 6565 6465 640a 2020 2020 2020  if needed.      
-000079e0: 2020 6966 2028 6669 6c65 5f6e 616d 6520    if (file_name 
-000079f0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00007a00: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
-00007a10: 2e5f 6375 7272 656e 745f 6669 6c65 5f6e  ._current_file_n
-00007a20: 616d 6521 3d66 696c 655f 6e61 6d65 293a  ame!=file_name):
-00007a30: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00007a40: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
-00007a50: 6b20 6966 2061 2066 696c 6520 616c 7265  k if a file alre
-00007a60: 6164 7920 6f70 656e 0a20 2020 2020 2020  ady open.       
-00007a70: 2020 2020 2069 6620 7365 6c66 2e5f 6375       if self._cu
-00007a80: 7272 656e 745f 6669 6c65 2069 7320 6e6f  rrent_file is no
-00007a90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00007aa0: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
-00007ab0: 6f73 655f 6669 6c65 2829 0a20 2020 2020  ose_file().     
-00007ac0: 2020 2020 2020 2023 206f 7065 6e0a 2020         # open.  
-00007ad0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007ae0: 6f70 656e 5f66 696c 6528 6669 6c65 5f6e  open_file(file_n
-00007af0: 616d 652c 206c 6f61 645f 6d65 7461 6461  ame, load_metada
-00007b00: 7461 3d46 616c 7365 290a 2020 2020 2020  ta=False).      
-00007b10: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
-00007b20: 2320 6c6f 6164 206d 6574 6164 6174 6120  # load metadata 
-00007b30: 2869 6620 2264 6174 6173 6574 2220 6d65  (if "dataset" me
-00007b40: 7461 6461 7461 2072 6571 7565 7374 6564  tadata requested
-00007b50: 202d 3e20 7265 6c6f 6164 290a 2020 2020   -> reload).    
-00007b60: 2020 2020 6966 2064 6174 6173 6574 5f6e      if dataset_n
-00007b70: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00007b80: 0a20 2020 2020 2020 2020 2020 2069 6e63  .            inc
-00007b90: 6c75 6465 5f64 6174 6173 6574 5f6d 6574  lude_dataset_met
-00007ba0: 6164 6174 6120 3d20 5472 7565 0a0a 2020  adata = True..  
-00007bb0: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
-00007bc0: 7572 7265 6e74 5f66 696c 655f 6d65 7461  urrent_file_meta
-00007bd0: 6461 7461 2069 7320 4e6f 6e65 206f 7220  data is None or 
-00007be0: 696e 636c 7564 655f 6461 7461 7365 745f  include_dataset_
-00007bf0: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
-00007c00: 2020 2020 2020 7365 6c66 2e5f 6c6f 6164        self._load
-00007c10: 5f6d 6574 6164 6174 6128 696e 636c 7564  _metadata(includ
-00007c20: 655f 6461 7461 7365 745f 6d65 7461 6461  e_dataset_metada
-00007c30: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-00007c40: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00007c50: 200a 2020 2020 2020 2020 2320 6669 6e64   .        # find
-00007c60: 2073 7065 6369 6669 6320 6d65 7461 6461   specific metada
-00007c70: 7461 0a20 2020 2020 2020 206d 6574 6164  ta.        metad
-00007c80: 6174 6120 3d20 6469 6374 2829 0a20 2020  ata = dict().   
-00007c90: 2020 2020 2069 6620 6772 6f75 705f 6e61       if group_na
-00007ca0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00007cb0: 2020 2020 2020 2020 2020 2020 6966 2067              if g
-00007cc0: 726f 7570 5f6e 616d 6520 696e 2073 656c  roup_name in sel
-00007cd0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-00007ce0: 6d65 7461 6461 7461 5b27 6772 6f75 705f  metadata['group_
-00007cf0: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
-00007d00: 2020 2020 2020 2020 6772 6f75 705f 6d65          group_me
-00007d10: 7461 6461 7461 203d 2073 656c 662e 5f63  tadata = self._c
-00007d20: 7572 7265 6e74 5f66 696c 655f 6d65 7461  urrent_file_meta
-00007d30: 6461 7461 5b27 6772 6f75 7073 275d 5b67  data['groups'][g
-00007d40: 726f 7570 5f6e 616d 655d 0a20 2020 2020  roup_name].     
-00007d50: 2020 2020 2020 2020 2020 2069 6620 6461             if da
-00007d60: 7461 7365 745f 6e61 6d65 2069 7320 6e6f  taset_name is no
-00007d70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00007d80: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00007d90: 6174 6173 6574 5f6e 616d 6520 696e 2067  ataset_name in g
-00007da0: 726f 7570 5f6d 6574 6164 6174 615b 2764  roup_metadata['d
-00007db0: 6174 6173 6574 5f6c 6973 7427 5d3a 0a20  ataset_list']:. 
-00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007dd0: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-00007de0: 3d20 6772 6f75 705f 6d65 7461 6461 7461  = group_metadata
-00007df0: 5b27 6461 7461 7365 7473 275d 5b64 6174  ['datasets'][dat
-00007e00: 6173 6574 5f6e 616d 655d 0a20 2020 2020  aset_name].     
-00007e10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e30: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
-00007e40: 6772 6f75 705f 6d65 7461 6461 7461 0a20  group_metadata. 
-00007e50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007e60: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00007e70: 6120 3d20 7365 6c66 2e5f 6375 7272 656e  a = self._curren
-00007e80: 745f 6669 6c65 5f6d 6574 6164 6174 610a  t_file_metadata.
-00007e90: 0a0a 2020 2020 2020 2020 2320 636c 6f73  ..        # clos
-00007ea0: 6520 6669 6c65 0a20 2020 2020 2020 2069  e file.        i
-00007eb0: 6620 6669 6c65 5f6e 616d 6520 6973 206e  f file_name is n
-00007ec0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007ed0: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
-00007ee0: 5f66 696c 6528 290a 2020 2020 2020 2020  _file().        
-00007ef0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00007f00: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
-00007f10: 2020 2020 2020 0a0a 0a0a 2020 2020 6465        ....    de
-00007f20: 6620 6765 745f 6465 7465 6374 6f72 5f63  f get_detector_c
-00007f30: 6f6e 6669 6728 7365 6c66 2c20 6669 6c65  onfig(self, file
-00007f40: 5f6e 616d 653d 4e6f 6e65 2c0a 2020 2020  _name=None,.    
-00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f60: 2020 2020 2020 2020 6164 635f 6e61 6d65          adc_name
-00007f70: 3d27 6164 6331 272c 0a20 2020 2020 2020  ='adc1',.       
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 2020 2075 7365 5f63 6861 6e5f 6469       use_chan_di
-00007fa0: 6374 3d54 7275 6529 3a20 2020 0a20 2020  ct=True):   .   
-00007fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007fc0: 2047 6574 2064 6574 6563 746f 7220 636f   Get detector co
-00007fd0: 6e66 6967 7572 6174 696f 6e0a 2020 2020  nfiguration.    
-00007fe0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007ff0: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
-00008000: 725f 636f 6e66 6967 203d 2064 6963 7428  r_config = dict(
-00008010: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00008020: 2020 2023 2067 6574 206d 6574 6164 6174     # get metadat
-00008030: 610a 2020 2020 2020 2020 6d65 7461 6461  a.        metada
-00008040: 7461 203d 204e 6f6e 650a 2020 2020 2020  ta = None.      
-00008050: 2020 6966 2066 696c 655f 6e61 6d65 2069    if file_name i
-00008060: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00008070: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00008080: 203d 2073 656c 662e 6765 745f 6d65 7461   = self.get_meta
-00008090: 6461 7461 2866 696c 655f 6e61 6d65 3d66  data(file_name=f
-000080a0: 696c 655f 6e61 6d65 290a 2020 2020 2020  ile_name).      
-000080b0: 2020 656c 6966 2073 656c 662e 5f63 7572    elif self._cur
-000080c0: 7265 6e74 5f66 696c 655f 6d65 7461 6461  rent_file_metada
-000080d0: 7461 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ta is not None:.
-000080e0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-000080f0: 6461 7461 203d 2073 656c 662e 5f63 7572  data = self._cur
-00008100: 7265 6e74 5f66 696c 655f 6d65 7461 6461  rent_file_metada
-00008110: 7461 0a20 2020 2020 2020 2065 6c73 653a  ta.        else:
-00008120: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00008130: 7365 2056 616c 7565 4572 726f 7228 2745  se ValueError('E
-00008140: 5252 4f52 2069 6e20 6765 745f 6465 7465  RROR in get_dete
-00008150: 6374 6f72 5f63 6f6e 6669 673a 2061 2066  ctor_config: a f
-00008160: 696c 6520 6e61 6d65 206e 6565 6473 2074  ile name needs t
-00008170: 6f20 6265 2070 726f 7669 6465 6421 2729  o be provided!')
-00008180: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00008190: 2020 0a0a 2020 2020 2020 2020 2320 636f    ..        # co
-000081a0: 6e66 6967 206e 616d 650a 2020 2020 2020  nfig name.      
-000081b0: 2020 636f 6e66 6967 5f6e 616d 6520 3d20    config_name = 
-000081c0: 2764 6574 636f 6e66 6967 3127 0a20 2020  'detconfig1'.   
-000081d0: 2020 2020 2069 6620 6164 635f 6e61 6d65       if adc_name
-000081e0: 213d 2761 6463 3127 3a0a 2020 2020 2020  !='adc1':.      
-000081f0: 2020 2020 2020 636f 6e66 6967 5f6e 616d        config_nam
-00008200: 6520 3d20 2764 6574 636f 6e66 6967 2720  e = 'detconfig' 
-00008210: 2b20 6164 635f 6e61 6d65 5b33 3a5d 0a0a  + adc_name[3:]..
-00008220: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-00008230: 6966 2061 7661 696c 6162 6c65 0a20 2020  if available.   
-00008240: 2020 2020 2069 6620 636f 6e66 6967 5f6e       if config_n
-00008250: 616d 6520 6e6f 7420 696e 206d 6574 6164  ame not in metad
-00008260: 6174 615b 2767 726f 7570 5f6c 6973 7427  ata['group_list'
-00008270: 5d3a 0a20 2020 2020 2020 2020 2020 2070  ]:.            p
-00008280: 7269 6e74 2827 4552 524f 523a 2075 6e61  rint('ERROR: una
-00008290: 626c 6520 746f 2066 696e 6420 6465 7465  ble to find dete
-000082a0: 6374 6f72 2063 6f6e 6669 6721 2729 0a20  ctor config!'). 
-000082b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000082c0: 6e20 5b5d 0a0a 2020 2020 2020 2020 2320  n []..        # 
-000082d0: 6772 6f75 7020 6d65 7461 6461 7461 0a20  group metadata. 
-000082e0: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
-000082f0: 636f 6e66 6967 5f64 6963 7420 3d20 6d65  config_dict = me
-00008300: 7461 6461 7461 5b27 6772 6f75 7073 275d  tadata['groups']
-00008310: 5b63 6f6e 6669 675f 6e61 6d65 5d0a 2020  [config_name].  
-00008320: 2020 2020 2020 2369 6620 2761 6463 5f6e        #if 'adc_n
-00008330: 616d 6527 2069 6e20 6465 7465 6374 6f72  ame' in detector
-00008340: 5f63 6f6e 6669 675f 6469 6374 2061 6e64  _config_dict and
-00008350: 2061 6463 5f6e 616d 6521 3d64 6574 6563   adc_name!=detec
-00008360: 746f 725f 636f 6e66 6967 5f64 6963 745b  tor_config_dict[
-00008370: 2761 6463 5f6e 616d 6527 5d3a 0a20 2020  'adc_name']:.   
-00008380: 2020 2020 2023 2020 2020 7072 696e 7428       #    print(
-00008390: 2745 5252 4f52 3a20 556e 6578 7065 6374  'ERROR: Unexpect
-000083a0: 6564 2064 6574 6563 746f 7220 636f 6e66  ed detector conf
-000083b0: 6967 7572 6174 696f 6e20 666f 726d 6174  iguration format
-000083c0: 2127 290a 2020 2020 2020 2020 2320 2020  !').        #   
-000083d0: 2072 6574 7572 6e20 5b5d 0a0a 0a20 2020   return []...   
-000083e0: 2020 2020 2023 2061 6464 2064 6574 6563       # add detec
-000083f0: 746f 722f 6368 616e 6e65 6c20 6c69 7374  tor/channel list
-00008400: 2066 726f 6d20 6164 6320 6d65 7461 6461   from adc metada
-00008410: 7461 2c20 6e65 6564 7320 746f 206d 6174  ta, needs to mat
-00008420: 6368 0a20 2020 2020 2020 2023 2064 6574  ch.        # det
-00008430: 6563 746f 7220 7365 7474 696e 6773 2061  ector settings a
-00008440: 7272 6179 206f 7264 6572 0a20 2020 2020  rray order.     
-00008450: 2020 2074 6573 5f63 6861 6e73 203d 206c     tes_chans = l
-00008460: 6973 7428 290a 2020 2020 2020 2020 6465  ist().        de
-00008470: 7465 6374 6f72 5f63 6861 6e73 203d 206c  tector_chans = l
-00008480: 6973 7428 290a 2020 2020 2020 2020 636f  ist().        co
-00008490: 6e74 726f 6c6c 6572 5f63 6861 6e73 203d  ntroller_chans =
-000084a0: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
-000084b0: 636f 6e6e 6563 7469 6f6e 5f64 6963 7420  connection_dict 
-000084c0: 3d20 7365 6c66 2e67 6574 5f63 6f6e 6e65  = self.get_conne
-000084d0: 6374 696f 6e5f 6469 6374 2861 6463 5f6e  ction_dict(adc_n
-000084e0: 616d 653d 6164 635f 6e61 6d65 2c0a 2020  ame=adc_name,.  
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008520: 206d 6574 6164 6174 613d 6d65 7461 6461   metadata=metada
-00008530: 7461 290a 0a20 2020 2020 2020 2069 6620  ta)..        if 
-00008540: 636f 6e6e 6563 7469 6f6e 5f64 6963 743a  connection_dict:
-00008550: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-00008560: 6e5f 6c69 7374 203d 2064 6574 6563 746f  n_list = detecto
-00008570: 725f 636f 6e66 6967 5f64 6963 745b 2763  r_config_dict['c
-00008580: 6861 6e6e 656c 5f6c 6973 7427 5d0a 2020  hannel_list'].  
-00008590: 2020 2020 2020 2020 2020 6966 2028 6e6f            if (no
-000085a0: 7420 6973 696e 7374 616e 6365 2863 6861  t isinstance(cha
-000085b0: 6e5f 6c69 7374 2c20 6e70 2e6e 6461 7272  n_list, np.ndarr
-000085c0: 6179 290a 2020 2020 2020 2020 2020 2020  ay).            
-000085d0: 2020 2020 616e 6420 6e6f 7420 6973 696e      and not isin
-000085e0: 7374 616e 6365 2863 6861 6e5f 6c69 7374  stance(chan_list
-000085f0: 2c20 6c69 7374 2929 3a0a 2020 2020 2020  , list)):.      
-00008600: 2020 2020 2020 2020 2020 6368 616e 5f6c            chan_l
-00008610: 6973 7420 203d 205b 6368 616e 5f6c 6973  ist  = [chan_lis
-00008620: 745d 0a20 2020 2020 2020 2020 2020 2066  t].            f
-00008630: 6f72 2063 6861 6e20 696e 2063 6861 6e5f  or chan in chan_
-00008640: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-00008650: 2020 2020 2020 6966 2063 6861 6e20 696e        if chan in
-00008660: 2063 6f6e 6e65 6374 696f 6e5f 6469 6374   connection_dict
-00008670: 5b27 6164 635f 6368 616e 7327 5d3a 0a20  ['adc_chans']:. 
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2069 6e64 203d 2063 6f6e 6e65 6374     ind = connect
-000086a0: 696f 6e5f 6469 6374 5b27 6164 635f 6368  ion_dict['adc_ch
-000086b0: 616e 7327 5d2e 696e 6465 7828 696e 7428  ans'].index(int(
-000086c0: 6368 616e 2929 0a20 2020 2020 2020 2020  chan)).         
-000086d0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-000086e0: 6e6e 6563 7469 6f6e 5f64 6963 745b 2763  nnection_dict['c
-000086f0: 6f6e 7472 6f6c 6c65 725f 6368 616e 7327  ontroller_chans'
-00008700: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00008710: 2020 2020 2020 2020 2020 2063 6f6e 7472             contr
-00008720: 6f6c 6c65 725f 6368 616e 732e 6170 7065  oller_chans.appe
-00008730: 6e64 2863 6f6e 6e65 6374 696f 6e5f 6469  nd(connection_di
-00008740: 6374 5b27 636f 6e74 726f 6c6c 6572 5f63  ct['controller_c
-00008750: 6861 6e73 275d 5b69 6e64 5d29 0a20 2020  hans'][ind]).   
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2069 6620 636f 6e6e 6563 7469 6f6e 5f64   if connection_d
-00008780: 6963 745b 2774 6573 5f63 6861 6e73 275d  ict['tes_chans']
-00008790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000087a0: 2020 2020 2020 2020 2020 7465 735f 6368            tes_ch
-000087b0: 616e 732e 6170 7065 6e64 2863 6f6e 6e65  ans.append(conne
-000087c0: 6374 696f 6e5f 6469 6374 5b27 7465 735f  ction_dict['tes_
-000087d0: 6368 616e 7327 5d5b 696e 645d 290a 2020  chans'][ind]).  
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087f0: 2020 6966 2063 6f6e 6e65 6374 696f 6e5f    if connection_
-00008800: 6469 6374 5b27 6465 7465 6374 6f72 5f63  dict['detector_c
-00008810: 6861 6e73 275d 3a0a 2020 2020 2020 2020  hans']:.        
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 6465 7465 6374 6f72 5f63 6861 6e73 2e61  detector_chans.a
-00008840: 7070 656e 6428 636f 6e6e 6563 7469 6f6e  ppend(connection
-00008850: 5f64 6963 745b 2764 6574 6563 746f 725f  _dict['detector_
-00008860: 6368 616e 7327 5d5b 696e 645d 290a 2020  chans'][ind]).  
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000088b0: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-000088c0: 5f64 6963 745b 2774 6573 5f63 6861 6e73  _dict['tes_chans
-000088d0: 275d 203d 2020 7465 735f 6368 616e 730a  '] =  tes_chans.
-000088e0: 2020 2020 2020 2020 6465 7465 6374 6f72          detector
-000088f0: 5f63 6f6e 6669 675f 6469 6374 5b27 6465  _config_dict['de
-00008900: 7465 6374 6f72 5f63 6861 6e73 275d 203d  tector_chans'] =
-00008910: 2020 6465 7465 6374 6f72 5f63 6861 6e73    detector_chans
-00008920: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
-00008930: 725f 636f 6e66 6967 5f64 6963 745b 2763  r_config_dict['c
-00008940: 6f6e 7472 6f6c 6c65 725f 6368 616e 7327  ontroller_chans'
-00008950: 5d20 3d20 2063 6f6e 7472 6f6c 6c65 725f  ] =  controller_
-00008960: 6368 616e 7320 2020 0a0a 2020 2020 2020  chans   ..      
-00008970: 2020 2320 636f 6e76 6572 7420 746f 206c    # convert to l
-00008980: 6973 7420 6966 206e 6565 6465 6420 2873  ist if needed (s
-00008990: 697a 6520 6f66 206e 6220 6368 616e 6e65  ize of nb channe
-000089a0: 6c73 290a 2020 2020 2020 2020 6e62 5f63  ls).        nb_c
-000089b0: 6861 6e20 3d20 6c65 6e28 6465 7465 6374  han = len(detect
-000089c0: 6f72 5f63 6f6e 6669 675f 6469 6374 5b27  or_config_dict['
-000089d0: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
-000089e0: 290a 2020 2020 2020 2020 666f 7220 636f  ).        for co
-000089f0: 6e66 6967 2069 6e20 6465 7465 6374 6f72  nfig in detector
-00008a00: 5f63 6f6e 6669 675f 6469 6374 2e6b 6579  _config_dict.key
-00008a10: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00008a20: 2070 6172 616d 203d 2064 6574 6563 746f   param = detecto
-00008a30: 725f 636f 6e66 6967 5f64 6963 745b 636f  r_config_dict[co
-00008a40: 6e66 6967 5d0a 2020 2020 2020 2020 2020  nfig].          
-00008a50: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00008a60: 6e63 6528 7061 7261 6d2c 206c 6973 7429  nce(param, list)
-00008a70: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
-00008a80: 6e63 6528 7061 7261 6d2c 206e 702e 6e64  nce(param, np.nd
-00008a90: 6172 7261 7929 3a0a 2020 2020 2020 2020  array):.        
-00008aa0: 2020 2020 2020 2020 6465 7465 6374 6f72          detector
-00008ab0: 5f63 6f6e 6669 675f 6469 6374 5b63 6f6e  _config_dict[con
-00008ac0: 6669 675d 203d 205b 6465 7465 6374 6f72  fig] = [detector
-00008ad0: 5f63 6f6e 6669 675f 6469 6374 5b63 6f6e  _config_dict[con
-00008ae0: 6669 675d 5d2a 6e62 5f63 6861 6e0a 2020  fig]]*nb_chan.  
-00008af0: 2020 0a20 2020 2020 2020 2023 2063 6f6e    .        # con
-00008b00: 7665 7274 2074 6f20 6469 6374 696f 6e61  vert to dictiona
-00008b10: 7279 0a20 2020 2020 2020 2064 6574 6563  ry.        detec
-00008b20: 746f 725f 636f 6e66 6967 203d 2064 6963  tor_config = dic
-00008b30: 7428 290a 2020 2020 2020 2020 6966 2075  t().        if u
-00008b40: 7365 5f63 6861 6e5f 6469 6374 3a0a 2020  se_chan_dict:.  
-00008b50: 2020 2020 2020 2020 2020 6368 616e 5f6c            chan_l
-00008b60: 6973 7420 3d20 6465 7465 6374 6f72 5f63  ist = detector_c
-00008b70: 6f6e 6669 675f 6469 6374 5b27 6465 7465  onfig_dict['dete
-00008b80: 6374 6f72 5f63 6861 6e73 275d 0a20 2020  ctor_chans'].   
-00008b90: 2020 2020 2020 2020 2066 6f72 2063 6861           for cha
-00008ba0: 6e20 696e 2063 6861 6e5f 6c69 7374 3a0a  n in chan_list:.
-00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bc0: 6368 616e 5f69 6e64 6578 203d 2064 6574  chan_index = det
-00008bd0: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
-00008be0: 745b 2764 6574 6563 746f 725f 6368 616e  t['detector_chan
-00008bf0: 7327 5d2e 696e 6465 7828 6368 616e 290a  s'].index(chan).
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c10: 6465 7465 6374 6f72 5f63 6f6e 6669 675b  detector_config[
-00008c20: 6368 616e 5d20 3d20 6469 6374 2829 0a20  chan] = dict(). 
-00008c30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00008c40: 6f72 2063 6f6e 6669 6720 696e 2064 6574  or config in det
-00008c50: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
-00008c60: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00008c70: 2020 2020 2020 2069 6620 6c65 6e28 6465         if len(de
-00008c80: 7465 6374 6f72 5f63 6f6e 6669 675f 6469  tector_config_di
-00008c90: 6374 5b63 6f6e 6669 675d 293d 3d6e 625f  ct[config])==nb_
-00008ca0: 6368 616e 3a0a 2020 2020 2020 2020 2020  chan:.          
-00008cb0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00008cc0: 7465 6374 6f72 5f63 6f6e 6669 675b 6368  tector_config[ch
-00008cd0: 616e 5d5b 636f 6e66 6967 5d20 3d20 6465  an][config] = de
-00008ce0: 7465 6374 6f72 5f63 6f6e 6669 675f 6469  tector_config_di
-00008cf0: 6374 5b63 6f6e 6669 675d 5b63 6861 6e5f  ct[config][chan_
-00008d00: 696e 6465 785d 0a20 2020 2020 2020 2065  index].        e
-00008d10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008d20: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-00008d30: 203d 2064 6574 6563 746f 725f 636f 6e66   = detector_conf
-00008d40: 6967 5f64 6963 740a 2020 2020 2020 2020  ig_dict.        
-00008d50: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00008d60: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00008d70: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008d80: 2072 6574 7572 6e20 6465 7465 6374 6f72   return detector
-00008d90: 5f63 6f6e 6669 670a 0a0a 2020 2020 2020  _config...      
-00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008db0: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00008dc0: 2020 2064 6566 2067 6574 5f63 6f6e 6e65     def get_conne
-00008dd0: 6374 696f 6e5f 6469 6374 2873 656c 662c  ction_dict(self,
-00008de0: 2066 696c 655f 6e61 6d65 3d4e 6f6e 652c   file_name=None,
-00008df0: 2061 6463 5f6e 616d 653d 2761 6463 3127   adc_name='adc1'
-00008e00: 2c20 6d65 7461 6461 7461 3d4e 6f6e 6529  , metadata=None)
-00008e10: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00008e20: 2020 2020 2020 4765 7420 636f 6e6e 6563        Get connec
-00008e30: 7469 6f6e 2064 6963 7469 6f6e 6172 7920  tion dictionary 
-00008e40: 666f 7220 7370 6563 6966 6964 2061 6463  for specifid adc
-00008e50: 206e 616d 650a 2020 2020 2020 2020 2222   name.        ""
-00008e60: 220a 0a20 2020 2020 2020 2023 2069 6e69  "..        # ini
-00008e70: 7469 616c 697a 650a 2020 2020 2020 2020  tialize.        
-00008e80: 636f 6e6e 6563 7469 6f6e 5f64 6963 743d  connection_dict=
-00008e90: 6469 6374 2829 0a0a 2020 2020 2020 2020  dict()..        
-00008ea0: 2320 6d65 7461 6461 7461 0a20 2020 2020  # metadata.     
-00008eb0: 2020 2061 6463 5f6d 6574 6164 6174 6120     adc_metadata 
-00008ec0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-00008ed0: 6620 6d65 7461 6461 7461 2069 7320 4e6f  f metadata is No
-00008ee0: 6e65 206f 7220 2767 726f 7570 5f6c 6973  ne or 'group_lis
-00008ef0: 7427 206e 6f74 2069 6e20 6d65 7461 6461  t' not in metada
-00008f00: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00008f10: 6d65 7461 6461 7461 203d 2073 656c 662e  metadata = self.
-00008f20: 6765 745f 6d65 7461 6461 7461 2866 696c  get_metadata(fil
-00008f30: 655f 6e61 6d65 3d66 696c 655f 6e61 6d65  e_name=file_name
-00008f40: 290a 0a20 2020 2020 2020 2069 6620 2767  )..        if 'g
-00008f50: 726f 7570 5f6c 6973 7427 2069 6e20 6d65  roup_list' in me
-00008f60: 7461 6461 7461 2061 6e64 2061 6463 5f6e  tadata and adc_n
-00008f70: 616d 6520 696e 206d 6574 6164 6174 615b  ame in metadata[
-00008f80: 2767 726f 7570 5f6c 6973 7427 5d3a 0a20  'group_list']:. 
-00008f90: 2020 2020 2020 2020 2020 2061 6463 5f6d             adc_m
-00008fa0: 6574 6164 6174 6120 203d 206d 6574 6164  etadata  = metad
-00008fb0: 6174 615b 2767 726f 7570 7327 5d5b 6164  ata['groups'][ad
-00008fc0: 635f 6e61 6d65 5d0a 0a20 2020 2020 2020  c_name]..       
-00008fd0: 2069 6620 6164 635f 6d65 7461 6461 7461   if adc_metadata
-00008fe0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00008ff0: 2020 2020 2020 6572 726f 725f 6d73 6720        error_msg 
-00009000: 3d20 2741 4443 206d 6574 6164 6174 6120  = 'ADC metadata 
-00009010: 6e6f 7420 666f 756e 6421 270a 2020 2020  not found!'.    
-00009020: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009030: 5f72 6169 7365 5f65 7272 6f72 733a 0a20  _raise_errors:. 
-00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009050: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00009060: 726f 7228 6572 726f 725f 6d73 6729 0a20  ror(error_msg). 
-00009070: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00009080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009090: 2070 7269 6e74 2827 5741 524e 494e 473a   print('WARNING:
-000090a0: 2027 202b 2065 7272 6f72 5f6d 7367 290a   ' + error_msg).
-000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090c0: 7265 7475 726e 2063 6f6e 6563 7469 6f6e  return conection
-000090d0: 5f64 6963 740a 0a0a 2020 2020 2020 2020  _dict...        
-000090e0: 636f 6e6e 6563 7469 6f6e 5f64 6963 745b  connection_dict[
-000090f0: 2761 6463 5f63 6861 6e73 275d 203d 206c  'adc_chans'] = l
-00009100: 6973 7428 290a 2020 2020 2020 2020 636f  ist().        co
-00009110: 6e6e 6563 7469 6f6e 5f64 6963 745b 2763  nnection_dict['c
-00009120: 6f6e 7472 6f6c 6c65 725f 6368 616e 7327  ontroller_chans'
-00009130: 5d20 3d20 6c69 7374 2829 0a20 2020 2020  ] = list().     
-00009140: 2020 2063 6f6e 6e65 6374 696f 6e5f 6469     connection_di
-00009150: 6374 5b27 7465 735f 6368 616e 7327 5d20  ct['tes_chans'] 
-00009160: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
-00009170: 2063 6f6e 6e65 6374 696f 6e5f 6469 6374   connection_dict
-00009180: 5b27 6465 7465 6374 6f72 5f63 6861 6e73  ['detector_chans
-00009190: 275d 203d 206c 6973 7428 290a 2020 2020  '] = list().    
-000091a0: 2020 2020 0a20 2020 2020 2020 2023 206c      .        # l
-000091b0: 6f6f 7020 6d65 7461 6461 7461 2074 6f20  oop metadata to 
-000091c0: 6669 6e64 2063 6f6e 6e65 6374 696f 6e73  find connections
-000091d0: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-000091e0: 2c76 616c 7565 2069 6e20 6164 635f 6d65  ,value in adc_me
-000091f0: 7461 6461 7461 2e69 7465 6d73 2829 3a0a  tadata.items():.
-00009200: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00009210: 6579 2e66 696e 6428 2763 6f6e 6e65 6374  ey.find('connect
-00009220: 696f 6e27 2921 3d2d 313a 0a20 2020 2020  ion')!=-1:.     
-00009230: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-00009240: 6374 696f 6e5f 6469 6374 5b27 6164 635f  ction_dict['adc_
-00009250: 6368 616e 7327 5d2e 6170 7065 6e64 2869  chans'].append(i
-00009260: 6e74 286b 6579 5b31 303a 5d29 290a 2020  nt(key[10:])).  
-00009270: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00009280: 7220 636f 6e6e 6563 7469 6f6e 5f74 7970  r connection_typ
-00009290: 6520 696e 2076 616c 7565 3a0a 2020 2020  e in value:.    
-000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092b0: 6368 616e 6e65 6c5f 6e61 6d65 203d 2063  channel_name = c
-000092c0: 6f6e 6e65 6374 696f 6e5f 7479 7065 5b63  onnection_type[c
-000092d0: 6f6e 6e65 6374 696f 6e5f 7479 7065 2e66  onnection_type.f
-000092e0: 696e 6428 273a 2729 2b31 3a5d 0a20 2020  ind(':')+1:].   
-000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2069 6620 636f 6e6e 6563 7469 6f6e 5f74   if connection_t
-00009310: 7970 652e 6669 6e64 2827 7465 733a 2729  ype.find('tes:')
-00009320: 213d 2d31 3a0a 2020 2020 2020 2020 2020  !=-1:.          
-00009330: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00009340: 6e6e 6563 7469 6f6e 5f64 6963 745b 2774  nnection_dict['t
-00009350: 6573 5f63 6861 6e73 275d 2e61 7070 656e  es_chans'].appen
-00009360: 6428 6368 616e 6e65 6c5f 6e61 6d65 290a  d(channel_name).
-00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 2020 2020 6966 2063 6f6e 6e65 6374 696f      if connectio
-00009390: 6e5f 7479 7065 2e66 696e 6428 2764 6574  n_type.find('det
-000093a0: 6563 746f 723a 2729 213d 2d31 3a0a 2020  ector:')!=-1:.  
-000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093c0: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-000093d0: 5f64 6963 745b 2764 6574 6563 746f 725f  _dict['detector_
-000093e0: 6368 616e 7327 5d2e 6170 7065 6e64 2863  chans'].append(c
-000093f0: 6861 6e6e 656c 5f6e 616d 6529 0a20 2020  hannel_name).   
-00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009410: 2069 6620 636f 6e6e 6563 7469 6f6e 5f74   if connection_t
-00009420: 7970 652e 6669 6e64 2827 636f 6e74 726f  ype.find('contro
-00009430: 6c6c 6572 3a27 2921 3d2d 313a 0a20 2020  ller:')!=-1:.   
-00009440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009450: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
-00009460: 6469 6374 5b27 636f 6e74 726f 6c6c 6572  dict['controller
-00009470: 5f63 6861 6e73 275d 2e61 7070 656e 6428  _chans'].append(
-00009480: 6368 616e 6e65 6c5f 6e61 6d65 290a 0a20  channel_name).. 
-00009490: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-000094a0: 6e6e 6563 7469 6f6e 5f64 6963 7420 2020  nnection_dict   
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2020 2020 200a 0a0a 2020             ...  
-000094d0: 2020 0a0a 2020 2020 6465 6620 6765 745f    ..    def get_
-000094e0: 636f 6e6e 6563 7469 6f6e 5f74 6162 6c65  connection_table
-000094f0: 2873 656c 662c 2066 696c 655f 6e61 6d65  (self, file_name
-00009500: 3d4e 6f6e 652c 206d 6574 6164 6174 613d  =None, metadata=
-00009510: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-00009520: 2222 0a20 2020 2020 2020 2047 6574 2063  "".        Get c
-00009530: 6f6e 6e65 6374 696f 6e20 7461 626c 650a  onnection table.
-00009540: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009550: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
-00009560: 6d65 7461 6461 7461 2069 7320 4e6f 6e65  metadata is None
-00009570: 3a0a 2020 2020 2020 2020 2020 2020 6d65  :.            me
-00009580: 7461 6461 7461 203d 2073 656c 662e 6765  tadata = self.ge
-00009590: 745f 6d65 7461 6461 7461 2866 696c 655f  t_metadata(file_
-000095a0: 6e61 6d65 3d66 696c 655f 6e61 6d65 290a  name=file_name).
-000095b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000095c0: 2023 2063 6865 636b 2061 6463 206c 6973   # check adc lis
-000095d0: 7420 6578 6973 7420 0a20 2020 2020 2020  t exist .       
-000095e0: 2069 6620 2761 6463 5f6c 6973 7427 206e   if 'adc_list' n
-000095f0: 6f74 2069 6e20 6d65 7461 6461 7461 3a0a  ot in metadata:.
-00009600: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00009610: 7428 2745 5252 4f52 3a20 4e6f 2041 4443  t('ERROR: No ADC
-00009620: 206d 6574 6164 6174 6120 666f 756e 6420   metadata found 
-00009630: 696e 2074 6865 2066 696c 6521 2729 0a20  in the file!'). 
-00009640: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009650: 6e0a 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00009660: 2020 2020 2320 6c6f 6f70 2061 6463 2061      # loop adc a
-00009670: 6e64 2066 696e 6420 636f 6e6e 6563 7469  nd find connecti
-00009680: 6f6e 0a20 2020 2020 2020 2063 6f6e 6e65  on.        conne
-00009690: 6374 696f 6e5f 6c69 7374 203d 206c 6973  ction_list = lis
-000096a0: 7428 290a 2020 2020 2020 2020 636f 6e6e  t().        conn
-000096b0: 6563 7469 6f6e 5f6e 616d 655f 6c69 7374  ection_name_list
-000096c0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
-000096d0: 2020 666f 7220 6164 635f 6964 2069 6e20    for adc_id in 
-000096e0: 6d65 7461 6461 7461 5b27 6164 635f 6c69  metadata['adc_li
-000096f0: 7374 275d 3a0a 2020 2020 2020 2020 2020  st']:.          
-00009700: 2020 6164 635f 6d65 7461 6461 7461 203d    adc_metadata =
-00009710: 206d 6574 6164 6174 615b 2767 726f 7570   metadata['group
-00009720: 7327 5d5b 6164 635f 6964 5d0a 2020 2020  s'][adc_id].    
-00009730: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-00009740: 7661 6c20 696e 2061 6463 5f6d 6574 6164  val in adc_metad
-00009750: 6174 612e 6974 656d 7328 293a 0a20 2020  ata.items():.   
-00009760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009770: 6b65 795b 303a 3130 5d3d 3d27 636f 6e6e  key[0:10]=='conn
-00009780: 6563 7469 6f6e 273a 0a20 2020 2020 2020  ection':.       
-00009790: 2020 2020 2020 2020 2020 2020 2061 6463               adc
-000097a0: 5f63 6861 6e20 3d20 7265 2e73 7562 2872  _chan = re.sub(r
-000097b0: 275c 732b 272c 2727 2c20 7374 7228 6b65  '\s+','', str(ke
-000097c0: 7929 295b 3130 3a5d 0a20 2020 2020 2020  y))[10:].       
-000097d0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-000097e0: 655f 7661 6c5f 6c69 7374 2c20 6e61 6d65  e_val_list, name
-000097f0: 5f6c 6973 742c 2076 616c 5f6c 6973 7420  _list, val_list 
-00009800: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00009810: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-00009820: 6563 7469 6f6e 5f75 7469 6c73 2e65 7874  ection_utils.ext
-00009830: 7261 6374 5f61 6463 5f63 6f6e 6e65 6374  ract_adc_connect
-00009840: 696f 6e28 6c69 7374 2876 616c 2929 290a  ion(list(val))).
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2020 2020 7661 6c5f 6c69 7374 2020 3d20      val_list  = 
-00009870: 5b61 6463 5f69 642c 6164 635f 6368 616e  [adc_id,adc_chan
-00009880: 5d20 2b20 7661 6c5f 6c69 7374 0a20 2020  ] + val_list.   
-00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098a0: 206e 616d 655f 6c69 7374 203d 205b 2761   name_list = ['a
-000098b0: 6463 5f69 6427 2c27 6164 635f 6368 616e  dc_id','adc_chan
-000098c0: 6e65 6c27 5d20 2b20 6e61 6d65 5f6c 6973  nel'] + name_lis
-000098d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000098e0: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-000098f0: 5f6c 6973 742e 6170 7065 6e64 2876 616c  _list.append(val
-00009900: 5f6c 6973 7429 0a20 2020 2020 2020 2020  _list).         
-00009910: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00009920: 7420 636f 6e6e 6563 7469 6f6e 5f6e 616d  t connection_nam
-00009930: 655f 6c69 7374 3a0a 2020 2020 2020 2020  e_list:.        
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 636f 6e6e 6563 7469 6f6e 5f6e 616d 655f  connection_name_
-00009960: 6c69 7374 203d 206e 616d 655f 6c69 7374  list = name_list
-00009970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009980: 2020 2020 2065 6c69 6620 636f 6e6e 6563       elif connec
-00009990: 7469 6f6e 5f6e 616d 655f 6c69 7374 213d  tion_name_list!=
-000099a0: 6e61 6d65 5f6c 6973 743a 0a20 2020 2020  name_list:.     
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099c0: 2020 2070 7269 6e74 2827 4552 524f 523a     print('ERROR:
-000099d0: 206d 6973 7369 6e67 2061 6463 2063 6f6e   missing adc con
-000099e0: 6e65 6374 696f 6e20 7661 6c75 6573 2127  nection values!'
-000099f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009a00: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00009a10: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00009a20: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
-00009a30: 6f6e 5f74 6162 6c65 203d 2070 642e 4461  on_table = pd.Da
-00009a40: 7461 4672 616d 6528 636f 6e6e 6563 7469  taFrame(connecti
-00009a50: 6f6e 5f6c 6973 742c 0a20 2020 2020 2020  on_list,.       
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2063 6f6c 756d 6e73 3d63 6f6e 6e65 6374   columns=connect
-00009a90: 696f 6e5f 6e61 6d65 5f6c 6973 7420 290a  ion_name_list ).
-00009aa0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00009ab0: 6f6e 6e65 6374 696f 6e5f 7461 626c 650a  onnection_table.
-00009ac0: 0a0a 2020 2020 0a20 200a 0a20 2020 2064  ..    .  ..    d
-00009ad0: 6566 205f 6f70 656e 5f66 696c 6528 7365  ef _open_file(se
-00009ae0: 6c66 2c20 6669 6c65 5f6e 616d 652c 2072  lf, file_name, r
-00009af0: 775f 7374 7269 6e67 3d27 7227 2c20 6c6f  w_string='r', lo
-00009b00: 6164 5f6d 6574 6164 6174 613d 5472 7565  ad_metadata=True
-00009b10: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00009b20: 2020 2020 2020 206f 7065 6e20 6669 6c65         open file
-00009b30: 200a 2020 2020 2020 2020 2222 220a 2020   .        """.  
-00009b40: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
-00009b50: 7572 7265 6e74 5f66 696c 6520 6973 206e  urrent_file is n
-00009b60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00009b70: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
-00009b80: 5f66 696c 6528 290a 2020 2020 2020 2020  _file().        
-00009b90: 2020 2020 0a20 2020 2020 2020 2066 696c      .        fil
-00009ba0: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
-00009bb0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00009bc0: 2020 6669 6c65 203d 2068 3570 792e 4669    file = h5py.Fi
-00009bd0: 6c65 2866 696c 655f 6e61 6d65 2c72 775f  le(file_name,rw_
-00009be0: 7374 7269 6e67 290a 2020 2020 2020 2020  string).        
-00009bf0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00009c00: 2020 2020 7072 696e 7428 2745 5252 4f52      print('ERROR
-00009c10: 3a20 756e 6162 6c65 2074 6f20 6f70 656e  : unable to open
-00009c20: 2066 696c 6520 2720 2b20 6669 6c65 5f6e   file ' + file_n
-00009c30: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00009c40: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00009c50: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-00009c60: 696c 6520 3d20 6669 6c65 0a20 2020 2020  ile = file.     
-00009c70: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-00009c80: 5f66 696c 655f 6e61 6d65 203d 2066 696c  _file_name = fil
-00009c90: 655f 6e61 6d65 0a20 2020 2020 2020 2073  e_name.        s
-00009ca0: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
-00009cb0: 655f 6e62 5f65 7665 6e74 7320 3d20 300a  e_nb_events = 0.
-00009cc0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00009cd0: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
-00009ce0: 5f63 6f75 6e74 6572 203d 2030 0a20 2020  _counter = 0.   
-00009cf0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00009d00: 6c6f 6164 206d 6574 6164 6174 610a 2020  load metadata.  
-00009d10: 2020 2020 2020 6966 206c 6f61 645f 6d65        if load_me
-00009d20: 7461 6461 7461 3a0a 0a20 2020 2020 2020  tadata:..       
-00009d30: 2020 2020 2073 656c 662e 5f6c 6f61 645f       self._load_
-00009d40: 6d65 7461 6461 7461 2829 0a20 2020 2020  metadata().     
-00009d50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009d60: 2020 2020 2320 6368 6563 6b20 6576 656e      # check even
-00009d70: 7473 0a20 2020 2020 2020 2020 2020 2069  ts.            i
-00009d80: 6620 2761 6463 5f6c 6973 7427 206e 6f74  f 'adc_list' not
-00009d90: 2069 6e20 7365 6c66 2e5f 6375 7272 656e   in self._curren
-00009da0: 745f 6669 6c65 5f6d 6574 6164 6174 613a  t_file_metadata:
-00009db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009dc0: 2070 7269 6e74 2827 5741 524e 494e 473a   print('WARNING:
-00009dd0: 204e 6f20 4144 4320 696e 666f 726d 6174   No ADC informat
-00009de0: 696f 6e20 666f 756e 6420 696e 2074 6865  ion found in the
-00009df0: 2066 696c 6527 290a 2020 2020 2020 2020   file').        
-00009e00: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00009e10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009e20: 6164 635f 6e61 6d65 2069 6e20 7365 6c66  adc_name in self
-00009e30: 2e5f 6375 7272 656e 745f 6669 6c65 5f6d  ._current_file_m
-00009e40: 6574 6164 6174 615b 2761 6463 5f6c 6973  etadata['adc_lis
-00009e50: 7427 5d3a 0a20 2020 2020 2020 2020 2020  t']:.           
-00009e60: 2020 2020 206e 625f 6576 656e 7473 5f61       nb_events_a
-00009e70: 6463 203d 2073 656c 662e 5f63 7572 7265  dc = self._curre
-00009e80: 6e74 5f66 696c 655f 6d65 7461 6461 7461  nt_file_metadata
-00009e90: 5b27 6772 6f75 7073 275d 5b61 6463 5f6e  ['groups'][adc_n
-00009ea0: 616d 655d 5b27 6e62 5f64 6174 6173 6574  ame]['nb_dataset
-00009eb0: 7327 5d0a 2020 2020 2020 2020 2020 2020  s'].            
-00009ec0: 2020 2020 6966 2073 656c 662e 5f63 7572      if self._cur
-00009ed0: 7265 6e74 5f66 696c 655f 6e62 5f65 7665  rent_file_nb_eve
-00009ee0: 6e74 733d 3d30 3a0a 2020 2020 2020 2020  nts==0:.        
-00009ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009f00: 2e5f 6375 7272 656e 745f 6669 6c65 5f6e  ._current_file_n
-00009f10: 625f 6576 656e 7473 203d 206e 625f 6576  b_events = nb_ev
-00009f20: 656e 7473 5f61 6463 0a20 2020 2020 2020  ents_adc.       
-00009f30: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
-00009f40: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-00009f50: 5f6e 625f 6576 656e 7473 2021 3d20 6e62  _nb_events != nb
-00009f60: 5f65 7665 6e74 735f 6164 633a 0a20 2020  _events_adc:.   
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2070 7269 6e74 2827 4552 524f 523a 2049   print('ERROR: I
-00009f90: 6e63 6f6e 7369 7374 656e 7420 6e75 6d62  nconsistent numb
-00009fa0: 6572 206f 6620 6576 656e 7473 2062 6574  er of events bet
-00009fb0: 7765 656e 2041 4443 2064 6576 6963 6573  ween ADC devices
-00009fc0: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
-00009fd0: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
-00009fe0: 6f73 655f 6669 6c65 2829 0a20 2020 2020  ose_file().     
-00009ff0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a000: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-0000a010: 2020 2020 2073 656c 662e 5f66 696c 655f       self._file_
-0000a020: 636f 756e 7465 7220 2b3d 2031 200a 2020  counter += 1 .  
-0000a030: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000a040: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
-0000a050: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-0000a060: 0a20 2020 200a 0a20 2020 2064 6566 205f  .    ..    def _
-0000a070: 636c 6f73 655f 6669 6c65 2873 656c 6629  close_file(self)
-0000a080: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000a090: 2020 2020 2020 436c 6f73 6520 6375 7272        Close curr
-0000a0a0: 656e 7420 6669 6c65 2061 6e64 2072 6573  ent file and res
-0000a0b0: 6574 0a20 2020 2020 2020 2063 7572 7265  et.        curre
-0000a0c0: 6e74 2066 696c 6520 7061 7261 6d65 7465  nt file paramete
-0000a0d0: 7273 0a0a 2020 2020 2020 2020 5061 7261  rs..        Para
-0000a0e0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000a0f0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000a100: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
-0000a110: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
-0000a120: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0000a130: 6e65 0a0a 2020 2020 2020 2020 2222 220a  ne..        """.
-0000a140: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000a150: 2e5f 6375 7272 656e 745f 6669 6c65 2069  ._current_file i
-0000a160: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000a170: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-0000a180: 7272 656e 745f 6669 6c65 2e63 6c6f 7365  rrent_file.close
-0000a190: 2829 0a20 200a 2020 2020 2020 2020 2320  ().  .        # 
-0000a1a0: 696e 6974 6961 6c69 7a65 0a20 2020 2020  initialize.     
-0000a1b0: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000a1c0: 5f66 696c 6520 3d20 4e6f 6e65 0a20 2020  _file = None.   
-0000a1d0: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000a1e0: 6e74 5f66 696c 655f 6e61 6d65 203d 204e  nt_file_name = N
-0000a1f0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000a200: 2e5f 6375 7272 656e 745f 6669 6c65 5f6d  ._current_file_m
-0000a210: 6574 6164 6174 6120 3d20 4e6f 6e65 0a20  etadata = None. 
-0000a220: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
-0000a230: 7265 6e74 5f66 696c 655f 6e62 5f65 7665  rent_file_nb_eve
-0000a240: 6e74 7320 3d20 300a 2020 2020 2020 2020  nts = 0.        
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2020 2020 0a20 2020 2020 2020 200a 0a0a      .        ...
-0000a270: 2020 2020 6465 6620 5f6c 6f61 645f 6d65      def _load_me
-0000a280: 7461 6461 7461 2873 656c 662c 2069 6e63  tadata(self, inc
-0000a290: 6c75 6465 5f64 6174 6173 6574 5f6d 6574  lude_dataset_met
-0000a2a0: 6164 6174 613d 4661 6c73 6529 3a0a 0a20  adata=False):.. 
-0000a2b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000a2c0: 2020 2046 756e 6374 696f 6e20 746f 206c     Function to l
-0000a2d0: 6f61 6420 616c 6c20 6d65 7461 6461 7461  oad all metadata
-0000a2e0: 2066 726f 6d20 6375 7272 656e 7420 6669   from current fi
-0000a2f0: 6c65 2e20 5374 6f72 6520 696e 200a 2020  le. Store in .  
-0000a300: 2020 2020 2020 616e 2069 6e74 6572 6e61        an interna
-0000a310: 6c20 6469 6374 696f 6e61 7279 0a0a 2020  l dictionary..  
-0000a320: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000a330: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000a340: 2d2d 2d0a 0a20 2020 2020 2020 2069 6e63  ---..        inc
-0000a350: 6c75 6465 5f64 6174 6173 6574 5f6d 6574  lude_dataset_met
-0000a360: 6164 6174 6120 3a20 626f 6f6c 2c20 6f70  adata : bool, op
-0000a370: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0000a380: 2020 6966 2054 7275 652c 2072 6561 6420    if True, read 
-0000a390: 6461 7461 7365 7420 6d65 7461 6461 7461  dataset metadata
-0000a3a0: 0a20 2020 2020 2020 2020 2020 4465 6661  .           Defa
-0000a3b0: 756c 743a 2046 616c 7365 0a0a 0a20 2020  ult: False...   
-0000a3c0: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
-0000a3d0: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
-0000a3e0: 2020 200a 2020 2020 2020 2020 6d65 7461     .        meta
-0000a3f0: 6461 7461 5f64 6963 7420 3a20 6469 6374  data_dict : dict
-0000a400: 0a20 2020 2020 2020 2020 2064 6963 7469  .          dicti
-0000a410: 6f6e 6172 7920 7769 7468 206d 6574 6164  onary with metad
-0000a420: 6174 610a 2020 2020 2020 2020 0a0a 2020  ata.        ..  
-0000a430: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000a440: 2020 2023 2063 6865 636b 2069 6620 6669     # check if fi
-0000a450: 6c65 2065 7869 7374 0a20 2020 2020 2020  le exist.       
-0000a460: 2069 6620 7365 6c66 2e5f 6375 7272 656e   if self._curren
-0000a470: 745f 6669 6c65 2069 7320 4e6f 6e65 3a0a  t_file is None:.
-0000a480: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a490: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
-0000a4a0: 2020 0a20 2020 2020 2020 2023 2069 6e69    .        # ini
-0000a4b0: 7469 616c 697a 6520 636f 6e74 6169 6e6e  tialize containn
-0000a4c0: 6572 0a20 2020 2020 2020 206d 6574 6164  er.        metad
-0000a4d0: 6174 615f 6469 6374 203d 2064 6963 7428  ata_dict = dict(
-0000a4e0: 290a 2020 2020 2020 0a0a 2020 2020 2020  ).      ..      
-0000a4f0: 2020 2320 6669 6c65 206d 6174 6164 6174    # file matadat
-0000a500: 610a 2020 2020 2020 2020 6d65 7461 6461  a.        metada
-0000a510: 7461 5f64 6963 7420 3d20 7365 6c66 2e5f  ta_dict = self._
-0000a520: 6578 7472 6163 745f 6d65 7461 6461 7461  extract_metadata
-0000a530: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
-0000a540: 696c 652e 6174 7472 7329 0a20 2020 2020  ile.attrs).     
-0000a550: 200a 2020 2020 0a20 2020 2020 2020 2023   .    .        #
-0000a560: 2067 726f 7570 2f64 6174 6173 6574 206d   group/dataset m
-0000a570: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
-0000a580: 6d65 7461 6461 7461 5f64 6963 745b 2767  metadata_dict['g
-0000a590: 726f 7570 5f6c 6973 7427 5d20 3d20 6c69  roup_list'] = li
-0000a5a0: 7374 2829 0a20 2020 2020 2020 206d 6574  st().        met
-0000a5b0: 6164 6174 615f 6469 6374 5b27 6164 635f  adata_dict['adc_
-0000a5c0: 6c69 7374 275d 203d 206c 6973 7428 290a  list'] = list().
-0000a5d0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000a5e0: 5f64 6963 745b 2767 726f 7570 7327 5d20  _dict['groups'] 
-0000a5f0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000a600: 2020 2020 0a20 2020 2020 2020 2023 204c      .        # L
-0000a610: 6f6f 7020 6772 6f75 7073 0a20 2020 2020  oop groups.     
-0000a620: 2020 2066 6f72 206b 6579 2c20 6772 6f75     for key, grou
-0000a630: 7020 696e 2073 656c 662e 5f63 7572 7265  p in self._curre
-0000a640: 6e74 5f66 696c 652e 6974 656d 7328 293a  nt_file.items():
-0000a650: 0a20 2020 2020 2020 0a20 2020 2020 2020  .       .       
-0000a660: 2020 2020 2023 2075 7064 6174 6520 6c69       # update li
-0000a670: 7374 0a20 2020 2020 2020 2020 2020 206d  st.            m
-0000a680: 6574 6164 6174 615f 6469 6374 5b27 6772  etadata_dict['gr
-0000a690: 6f75 705f 6c69 7374 275d 2e61 7070 656e  oup_list'].appen
-0000a6a0: 6428 6b65 7929 0a20 2020 2020 2020 2020  d(key).         
-0000a6b0: 2020 2069 6620 6b65 795b 303a 335d 3d3d     if key[0:3]==
-0000a6c0: 2761 6463 273a 0a20 2020 2020 2020 2020  'adc':.         
-0000a6d0: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
-0000a6e0: 6469 6374 5b27 6164 635f 6c69 7374 275d  dict['adc_list']
-0000a6f0: 2e61 7070 656e 6428 6b65 7929 0a20 2020  .append(key).   
-0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a710: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-0000a720: 2020 2020 2020 2020 2020 2320 7361 7665            # save
-0000a730: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
-0000a740: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
-0000a750: 6963 745b 2767 726f 7570 7327 5d5b 6b65  ict['groups'][ke
-0000a760: 795d 203d 2064 6963 7428 290a 2020 2020  y] = dict().    
-0000a770: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000a780: 5f64 6963 745b 2767 726f 7570 7327 5d5b  _dict['groups'][
-0000a790: 6b65 795d 203d 2020 7365 6c66 2e5f 6578  key] =  self._ex
-0000a7a0: 7472 6163 745f 6d65 7461 6461 7461 2867  tract_metadata(g
-0000a7b0: 726f 7570 2e61 7474 7273 290a 2020 2020  roup.attrs).    
-0000a7c0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-0000a7d0: 2023 2064 6174 6173 6574 730a 2020 2020   # datasets.    
-0000a7e0: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-0000a7f0: 6c69 7374 203d 206c 6973 7428 6772 6f75  list = list(grou
-0000a800: 702e 6b65 7973 2829 290a 2020 2020 2020  p.keys()).      
-0000a810: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
-0000a820: 6963 745b 2767 726f 7570 7327 5d5b 6b65  ict['groups'][ke
-0000a830: 795d 5b27 6461 7461 7365 745f 6c69 7374  y]['dataset_list
-0000a840: 275d 203d 2064 6174 6173 6574 5f6c 6973  '] = dataset_lis
-0000a850: 740a 2020 2020 2020 2020 2020 2020 6d65  t.            me
-0000a860: 7461 6461 7461 5f64 6963 745b 2767 726f  tadata_dict['gro
-0000a870: 7570 7327 5d5b 6b65 795d 5b27 6e62 5f64  ups'][key]['nb_d
-0000a880: 6174 6173 6574 7327 5d20 3d20 6c65 6e28  atasets'] = len(
-0000a890: 6461 7461 7365 745f 6c69 7374 290a 2020  dataset_list).  
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 0a0a                ..
-0000a8b0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000a8c0: 6e63 6c75 6465 5f64 6174 6173 6574 5f6d  nclude_dataset_m
-0000a8d0: 6574 6164 6174 6120 616e 6420 6c65 6e28  etadata and len(
-0000a8e0: 6461 7461 7365 745f 6c69 7374 293e 303a  dataset_list)>0:
-0000a8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a900: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-0000a910: 2020 2020 2020 2320 4c6f 6f70 2064 6174        # Loop dat
-0000a920: 6173 6574 7320 616e 6420 6164 6420 6d65  asets and add me
-0000a930: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
-0000a940: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
-0000a950: 6469 6374 5b27 6772 6f75 7073 275d 5b6b  dict['groups'][k
-0000a960: 6579 5d5b 2764 6174 6173 6574 7327 5d20  ey]['datasets'] 
-0000a970: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000a980: 2020 2020 2020 2020 2066 6f72 2064 6174           for dat
-0000a990: 6173 6574 5f6b 6579 2c20 6461 7461 7365  aset_key, datase
-0000a9a0: 7420 696e 2067 726f 7570 2e69 7465 6d73  t in group.items
-0000a9b0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000a9c0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000a9d0: 5f64 6963 745b 2767 726f 7570 7327 5d5b  _dict['groups'][
-0000a9e0: 6b65 795d 5b27 6461 7461 7365 7473 275d  key]['datasets']
-0000a9f0: 5b64 6174 6173 6574 5f6b 6579 5d20 3d20  [dataset_key] = 
-0000aa00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000aa10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000aa20: 6578 7472 6163 745f 6d65 7461 6461 7461  extract_metadata
-0000aa30: 2864 6174 6173 6574 2e61 7474 7273 290a  (dataset.attrs).
-0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa50: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000aa60: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-0000aa70: 0a20 2020 2020 2020 2023 2073 6176 650a  .        # save.
-0000aa80: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-0000aa90: 7272 656e 745f 6669 6c65 5f6d 6574 6164  rrent_file_metad
-0000aaa0: 6174 6120 3d20 6d65 7461 6461 7461 5f64  ata = metadata_d
-0000aab0: 6963 740a 2020 2020 200a 0a0a 0a0a 0a0a  ict.     .......
-0000aac0: 2020 2020 6465 6620 5f65 7874 7261 6374      def _extract
-0000aad0: 5f6d 6574 6164 6174 6128 7365 6c66 2c20  _metadata(self, 
-0000aae0: 6174 7472 6962 7574 6573 293a 0a20 2020  attributes):.   
-0000aaf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ab00: 2045 7874 7261 6374 206d 6574 6164 6174   Extract metadat
-0000ab10: 6120 6672 6f6d 2061 7474 7269 6275 7465  a from attribute
-0000ab20: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
-0000ab30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ab40: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-0000ab50: 615f 6469 6374 203d 2064 6963 7428 290a  a_dict = dict().
-0000ab60: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-0000ab70: 7661 6c75 6520 696e 2061 7474 7269 6275  value in attribu
-0000ab80: 7465 732e 6974 656d 7328 293a 0a20 2020  tes.items():.   
-0000ab90: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000aba0: 7374 616e 6365 2876 616c 7565 2c20 6279  stance(value, by
-0000abb0: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
-0000abc0: 2020 2020 2020 7661 6c75 6520 3d20 7661        value = va
-0000abd0: 6c75 652e 6465 636f 6465 2829 0a20 2020  lue.decode().   
-0000abe0: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-0000abf0: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
-0000ac00: 6e70 2e6e 6461 7272 6179 293a 0a20 2020  np.ndarray):.   
-0000ac10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000ac20: 7661 6c75 652e 6474 7970 6520 3d3d 206e  value.dtype == n
-0000ac30: 702e 6f62 6a65 6374 3a0a 2020 2020 2020  p.object:.      
-0000ac40: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000ac50: 6c75 6520 3d20 7661 6c75 652e 6173 7479  lue = value.asty
-0000ac60: 7065 2873 7472 290a 2020 2020 2020 2020  pe(str).        
-0000ac70: 2020 2020 2020 2020 2320 6120 6665 7720          # a few 
-0000ac80: 7061 7274 6963 756c 6172 2063 6173 6573  particular cases
-0000ac90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aca0: 2069 6620 6b65 7920 3d3d 2027 7275 6e5f   if key == 'run_
-0000acb0: 7075 7270 6f73 6527 3a0a 2020 2020 2020  purpose':.      
-0000acc0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000acd0: 6c75 6520 3d20 2720 272e 6a6f 696e 286c  lue = ' '.join(l
-0000ace0: 6973 7428 7661 6c75 6529 2920 2020 2020  ist(value))     
-0000acf0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-0000ad00: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-0000ad10: 6461 7461 5f64 6963 745b 6b65 795d 203d  data_dict[key] =
-0000ad20: 2076 616c 7565 0a20 2020 2020 2020 2072   value.        r
-0000ad30: 6574 7572 6e20 6d65 7461 6461 7461 5f64  eturn metadata_d
-0000ad40: 6963 740a 2020 2020 2020 2020 0a0a 2020  ict.        ..  
-0000ad50: 2020 0a20 2020 2064 6566 205f 6c6f 6164    .    def _load
-0000ad60: 5f65 7665 6e74 2873 656c 662c 2065 7665  _event(self, eve
-0000ad70: 6e74 5f69 6e64 6578 2c0a 2020 2020 2020  nt_index,.      
-0000ad80: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0000ad90: 7465 6374 6f72 5f63 6861 6e73 3d4e 6f6e  tector_chans=Non
-0000ada0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000adb0: 2020 2020 2020 2061 6463 746f 766f 6c74         adctovolt
-0000adc0: 3d46 616c 7365 2c20 6164 6374 6f61 6d70  =False, adctoamp
-0000add0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000ade0: 2020 2020 2020 2020 2020 2020 6261 7365              base
-0000adf0: 6c69 6e65 7375 623d 4661 6c73 652c 2062  linesub=False, b
-0000ae00: 6173 656c 696e 6569 6e64 733d 4e6f 6e65  aselineinds=None
-0000ae10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ae20: 2020 2020 2020 6164 635f 6e61 6d65 3d27        adc_name='
-0000ae30: 6164 6331 2729 3a0a 2020 2020 2020 2020  adc1'):.        
-0000ae40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ae50: 2020 2020 204c 6f61 6420 7472 6163 6573       Load traces
-0000ae60: 2061 6e64 206d 6574 6164 6174 6120 6672   and metadata fr
-0000ae70: 6f6d 2063 7572 7265 6e74 2066 696c 6520  om current file 
-0000ae80: 2062 6173 6564 206f 6e0a 2020 2020 2020   based on.      
-0000ae90: 2020 6576 656e 7420 696e 6465 780a 200a    event index. .
-0000aea0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000aeb0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000aec0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6576  -----.        ev
-0000aed0: 656e 745f 696e 6465 7820 3a20 696e 740a  ent_index : int.
-0000aee0: 2020 2020 2020 2020 2020 6576 656e 7420            event 
-0000aef0: 2868 6466 3520 2264 6174 6173 6574 2229  (hdf5 "dataset")
-0000af00: 2020 6e75 6d62 6572 200a 2020 2020 2020    number .      
-0000af10: 2020 0a20 2020 2020 2020 2064 6574 6563    .        detec
-0000af20: 746f 725f 6368 616e 7320 3a20 7374 7220  tor_chans : str 
-0000af30: 6f72 206c 6973 742c 206f 7074 696f 6e61  or list, optiona
-0000af40: 6c0a 2020 2020 2020 2020 2020 6465 7465  l.          dete
-0000af50: 6374 6f72 2f63 6861 6e6e 656c 206e 616d  ctor/channel nam
-0000af60: 6520 6f72 206c 6973 7420 6f66 2064 6574  e or list of det
-0000af70: 6563 746f 7273 2f63 6861 6e6e 656c 730a  ectors/channels.
-0000af80: 2020 2020 2020 2020 2020 6966 204e 6f6e            if Non
-0000af90: 652c 2067 6574 2061 6c6c 2063 6861 6e6e  e, get all chann
-0000afa0: 656c 7320 2864 6566 6175 6c74 290a 0a20  els (default).. 
-0000afb0: 2020 2020 2020 2061 6463 746f 766f 6c74         adctovolt
-0000afc0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-0000afd0: 6c0a 2020 2020 2020 2020 2020 636f 6e76  l.          conv
-0000afe0: 6572 7420 6672 6f6d 2041 4443 2074 6f20  ert from ADC to 
-0000aff0: 766f 6c74 730a 2020 2020 2020 2020 2020  volts.          
-0000b000: 6465 6661 756c 743a 2046 616c 7365 0a0a  default: False..
-0000b010: 2020 2020 2020 2020 6164 6374 6f61 6d70          adctoamp
-0000b020: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-0000b030: 6c0a 2020 2020 2020 2020 2020 636f 6e76  l.          conv
-0000b040: 6572 7420 6672 6f6d 2041 4443 2074 6f20  ert from ADC to 
-0000b050: 6375 7272 656e 7420 616d 7073 0a20 2020  current amps.   
-0000b060: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
-0000b070: 4661 6c73 650a 2020 2020 2020 2020 0a20  False.        . 
-0000b080: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-0000b090: 2020 2020 2020 6261 7365 6c69 6e65 7375        baselinesu
-0000b0a0: 623a 2062 6f6f 6c2c 206f 7074 696f 6e61  b: bool, optiona
-0000b0b0: 6c0a 2020 2020 2020 2020 2020 6966 2054  l.          if T
-0000b0c0: 7275 652c 2073 7562 7472 6163 7420 7072  rue, subtract pr
-0000b0d0: 652d 7075 6c73 6520 6261 7365 6c69 6e65  e-pulse baseline
-0000b0e0: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
-0000b0f0: 6c74 3a20 4661 6c73 650a 0a20 2020 2020  lt: False..     
-0000b100: 2020 2062 6173 656c 696e 6569 6e64 733a     baselineinds:
-0000b110: 2074 7570 6c65 2028 696e 742c 2069 6e74   tuple (int, int
-0000b120: 2920 6f72 206c 6973 7420 5b69 6e74 2c20  ) or list [int, 
-0000b130: 696e 745d 0a20 2020 2020 2020 2020 206d  int].          m
-0000b140: 696e 2f6d 6178 2069 6e64 6578 2066 6f72  in/max index for
-0000b150: 2020 6261 7365 6c69 6e65 2063 616c 6375    baseline calcu
-0000b160: 6c61 7469 6f6e 200a 2020 2020 2020 2020  lation .        
-0000b170: 2020 6465 6661 756c 743a 2028 3130 2c20    default: (10, 
-0000b180: 302e 382a 7072 6574 7269 6767 6572 206c  0.8*pretrigger l
-0000b190: 656e 6774 6829 290a 2020 2020 2020 2020  ength)).        
-0000b1a0: 2020 0a20 2020 2020 2020 2061 6463 5f6e    .        adc_n
-0000b1b0: 616d 6520 3a20 7374 722c 206f 7074 696f  ame : str, optio
-0000b1c0: 6e61 6c0a 2020 2020 2020 2020 2020 6e61  nal.          na
-0000b1d0: 6d65 2f49 4420 6f66 2074 6865 2061 6463  me/ID of the adc
-0000b1e0: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
-0000b1f0: 6c74 3a20 2261 6463 3122 0a0a 2020 2020  lt: "adc1"..    
-0000b200: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
-0000b210: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
-0000b220: 2020 0a20 2020 2020 2020 2061 7272 6179    .        array
-0000b230: 203a 2032 4420 6e75 6d70 7920 6172 7261   : 2D numpy arra
-0000b240: 790a 2020 2020 2020 2020 2020 2074 7261  y.           tra
-0000b250: 6365 7320 666f 7220 6561 6368 2063 6861  ces for each cha
-0000b260: 6e6e 656c 205b 6e62 2063 6861 6e6e 656c  nnel [nb channel
-0000b270: 2c20 6e62 2073 616d 706c 6573 5d0a 0a20  , nb samples].. 
-0000b280: 2020 2020 2020 2069 6e66 6f20 3a20 6469         info : di
-0000b290: 6374 0a20 2020 2020 2020 2020 2020 6669  ct.           fi
-0000b2a0: 6c65 2f65 7665 6e74 2f64 6574 6563 746f  le/event/detecto
-0000b2b0: 7220 6d65 7461 6461 7461 2028 6966 2022  r metadata (if "
-0000b2c0: 696e 636c 7564 655f 6d65 7461 6461 7461  include_metadata
-0000b2d0: 2220 3d20 5472 7565 290a 0a0a 2020 2020  " = True)...    
-0000b2e0: 2020 2020 0a20 2020 2020 2020 2022 2222      .        """
-0000b2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b300: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-0000b310: 6368 6563 6b20 6669 6c65 206f 7065 6e0a  check file open.
-0000b320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b330: 5f63 7572 7265 6e74 5f66 696c 6520 6973  _current_file is
-0000b340: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b350: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000b360: 726f 7228 274e 6f20 6669 6c65 206f 7065  ror('No file ope
-0000b370: 6e21 2729 0a20 2020 2020 2020 200a 2020  n!').        .  
-0000b380: 2020 2020 2020 2320 6765 7420 6461 7461        # get data
-0000b390: 7365 740a 2020 2020 2020 2020 6461 7461  set.        data
-0000b3a0: 7365 745f 6e61 6d65 203d 2027 6576 656e  set_name = 'even
-0000b3b0: 745f 2720 2b20 7374 7228 6576 656e 745f  t_' + str(event_
-0000b3c0: 696e 6465 7829 0a20 2020 2020 2020 2064  index).        d
-0000b3d0: 6174 6173 6574 203d 2073 656c 662e 5f63  ataset = self._c
-0000b3e0: 7572 7265 6e74 5f66 696c 655b 6164 635f  urrent_file[adc_
-0000b3f0: 6e61 6d65 5d5b 6461 7461 7365 745f 6e61  name][dataset_na
-0000b400: 6d65 5d0a 2020 2020 2020 2020 0a20 2020  me].        .   
-0000b410: 2020 2020 2023 2072 6561 6420 6461 7461       # read data
-0000b420: 7365 740a 2020 2020 2020 2020 6469 6d73  set.        dims
-0000b430: 203d 2064 6174 6173 6574 2e73 6861 7065   = dataset.shape
-0000b440: 0a20 2020 2020 2020 2074 7261 6365 735f  .        traces_
-0000b450: 696e 7420 3d20 6e70 2e7a 6572 6f73 2828  int = np.zeros((
-0000b460: 6469 6d73 5b30 5d2c 6469 6d73 5b31 5d29  dims[0],dims[1])
-0000b470: 2c20 6474 7970 653d 6e70 2e69 6e74 3136  , dtype=np.int16
-0000b480: 290a 2020 2020 2020 2020 6461 7461 7365  ).        datase
-0000b490: 742e 7265 6164 5f64 6972 6563 7428 7472  t.read_direct(tr
-0000b4a0: 6163 6573 5f69 6e74 290a 2020 2020 2020  aces_int).      
-0000b4b0: 0a20 2020 2020 2020 2023 2067 6574 206d  .        # get m
-0000b4c0: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
-0000b4d0: 696e 666f 203d 2073 656c 662e 5f65 7874  info = self._ext
-0000b4e0: 7261 6374 5f6d 6574 6164 6174 6128 6461  ract_metadata(da
-0000b4f0: 7461 7365 742e 6174 7472 7329 0a20 2020  taset.attrs).   
-0000b500: 2020 2020 2069 6e66 6f2e 7570 6461 7465       info.update
-0000b510: 2873 656c 662e 5f65 7874 7261 6374 5f6d  (self._extract_m
-0000b520: 6574 6164 6174 6128 7365 6c66 2e5f 6375  etadata(self._cu
-0000b530: 7272 656e 745f 6669 6c65 2e61 7474 7273  rrent_file.attrs
-0000b540: 2929 0a20 2020 2020 2020 2069 6e66 6f2e  )).        info.
-0000b550: 7570 6461 7465 2873 656c 662e 5f65 7874  update(self._ext
-0000b560: 7261 6374 5f6d 6574 6164 6174 6128 7365  ract_metadata(se
-0000b570: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000b580: 5b61 6463 5f6e 616d 655d 2e61 7474 7273  [adc_name].attrs
-0000b590: 2929 0a20 2020 2020 2020 2069 6e66 6f5b  )).        info[
-0000b5a0: 2772 6561 645f 7374 6174 7573 275d 203d  'read_status'] =
-0000b5b0: 2030 0a20 2020 2020 2020 2069 6e66 6f5b   0.        info[
-0000b5c0: 2765 7272 6f72 5f6d 7367 275d 203d 2027  'error_msg'] = '
-0000b5d0: 270a 0a0a 2020 2020 2020 2020 2320 6578  '...        # ex
-0000b5e0: 7472 6163 7420 6c69 7374 206f 6620 6164  tract list of ad
-0000b5f0: 6320 6368 616e 6e65 6c73 2c20 696e 6465  c channels, inde
-0000b600: 7820 636f 7272 6573 706f 6e64 2074 6f20  x correspond to 
-0000b610: 6172 7261 7920 696e 6465 7821 0a20 2020  array index!.   
-0000b620: 2020 2020 2061 6463 5f6e 756d 735f 6669       adc_nums_fi
-0000b630: 6c65 203d 2069 6e66 6f5b 2761 6463 5f63  le = info['adc_c
-0000b640: 6861 6e6e 656c 5f69 6e64 6963 6573 275d  hannel_indices']
-0000b650: 0a20 2020 2020 2020 2069 6620 286e 6f74  .        if (not
-0000b660: 2069 7369 6e73 7461 6e63 6528 6164 635f   isinstance(adc_
-0000b670: 6e75 6d73 5f66 696c 652c 206c 6973 7429  nums_file, list)
-0000b680: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0000b690: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0000b6a0: 6164 635f 6e75 6d73 5f66 696c 652c 206e  adc_nums_file, n
-0000b6b0: 702e 6e64 6172 7261 7929 293a 0a20 2020  p.ndarray)):.   
-0000b6c0: 2020 2020 2020 2020 2061 6463 5f6e 756d           adc_num
-0000b6d0: 735f 6669 6c65 203d 206e 702e 6172 7261  s_file = np.arra
-0000b6e0: 7928 5b61 6463 5f6e 756d 735f 6669 6c65  y([adc_nums_file
-0000b6f0: 5d29 0a20 2020 2020 2020 206e 625f 6368  ]).        nb_ch
-0000b700: 616e 6e65 6c73 5f66 696c 6520 3d20 6c65  annels_file = le
-0000b710: 6e28 6164 635f 6e75 6d73 5f66 696c 6529  n(adc_nums_file)
-0000b720: 0a0a 0a20 2020 2020 2020 2023 2067 6574  ...        # get
-0000b730: 2063 6f6e 6e65 6374 696f 6e20 6d61 7020   connection map 
-0000b740: 616e 6420 636f 6e76 6572 7420 746f 206e  and convert to n
-0000b750: 756d 7079 2061 7272 6179 0a20 2020 2020  umpy array.     
-0000b760: 2020 2063 6f6e 6e65 6374 696f 6e73 203d     connections =
-0000b770: 2073 656c 662e 6765 745f 636f 6e6e 6563   self.get_connec
-0000b780: 7469 6f6e 5f64 6963 7428 6164 635f 6e61  tion_dict(adc_na
-0000b790: 6d65 3d61 6463 5f6e 616d 652c 206d 6574  me=adc_name, met
-0000b7a0: 6164 6174 613d 696e 666f 290a 2020 2020  adata=info).    
-0000b7b0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-0000b7c0: 2020 2023 2046 696c 7465 7220 6261 7365     # Filter base
-0000b7d0: 6420 6f6e 2064 6574 6563 746f 725f 6368  d on detector_ch
-0000b7e0: 616e 7320 6172 6775 6d65 6e74 0a20 2020  ans argument.   
-0000b7f0: 2020 2020 2073 656c 6563 7465 645f 6172       selected_ar
-0000b800: 7261 795f 696e 6469 6365 7320 3d20 6c69  ray_indices = li
-0000b810: 7374 2829 0a20 2020 2020 2020 2073 656c  st().        sel
-0000b820: 6563 7465 645f 6164 635f 6e75 6d73 203d  ected_adc_nums =
-0000b830: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
-0000b840: 7365 6c65 6374 6564 5f64 6574 6563 746f  selected_detecto
-0000b850: 725f 6368 616e 7320 3d20 6c69 7374 2829  r_chans = list()
-0000b860: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
-0000b870: 645f 7465 735f 6368 616e 7320 3d20 6c69  d_tes_chans = li
-0000b880: 7374 2829 0a20 2020 2020 2020 2073 656c  st().        sel
-0000b890: 6563 7465 645f 636f 6e74 726f 6c6c 6572  ected_controller
-0000b8a0: 5f63 6861 6e73 203d 206c 6973 7428 290a  _chans = list().
-0000b8b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000b8c0: 200a 2020 2020 2020 2020 6966 2064 6574   .        if det
-0000b8d0: 6563 746f 725f 6368 616e 7320 6973 206e  ector_chans is n
-0000b8e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000b8f0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-0000b900: 2020 2320 636f 6e76 6572 7420 6465 7465    # convert dete
-0000b910: 6374 6f72 5f63 6861 6e73 2074 6f20 6c69  ctor_chans to li
-0000b920: 7374 2069 6620 6e65 6564 6564 0a20 2020  st if needed.   
-0000b930: 2020 2020 2020 2020 2069 6620 286e 6f74           if (not
-0000b940: 2069 7369 6e73 7461 6e63 6528 6465 7465   isinstance(dete
-0000b950: 6374 6f72 5f63 6861 6e73 2c20 6c69 7374  ctor_chans, list
-0000b960: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b970: 2020 616e 6420 6e6f 7420 6973 696e 7374    and not isinst
-0000b980: 616e 6365 2864 6574 6563 746f 725f 6368  ance(detector_ch
-0000b990: 616e 732c 206e 702e 6e64 6172 7261 7929  ans, np.ndarray)
-0000b9a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000b9b0: 2020 2064 6574 6563 746f 725f 6368 616e     detector_chan
-0000b9c0: 7320 3d20 5b64 6574 6563 746f 725f 6368  s = [detector_ch
-0000b9d0: 616e 735d 0a20 2020 2020 2020 2020 2020  ans].           
-0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9f0: 200a 0a20 2020 2020 2020 2020 2020 2023   ..            #
-0000ba00: 206c 6f6f 7020 7365 6c65 6374 6564 2063   loop selected c
-0000ba10: 6861 6e6e 656c 730a 2020 2020 2020 2020  hannels.        
-0000ba20: 2020 2020 666f 7220 6368 616e 2069 6e20      for chan in 
-0000ba30: 6465 7465 6374 6f72 5f63 6861 6e73 3a0a  detector_chans:.
-0000ba40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ba50: 2023 2063 6865 636b 0a20 2020 2020 2020   # check.       
-0000ba60: 2020 2020 2020 2020 2069 6620 6368 616e           if chan
-0000ba70: 206e 6f74 2069 6e20 636f 6e6e 6563 7469   not in connecti
-0000ba80: 6f6e 735b 2764 6574 6563 746f 725f 6368  ons['detector_ch
-0000ba90: 616e 7327 5d3a 0a20 2020 2020 2020 2020  ans']:.         
-0000baa0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000bab0: 2056 616c 7565 4572 726f 7228 2744 6574   ValueError('Det
-0000bac0: 6563 746f 7220 6368 616e 6e65 6c20 2720  ector channel ' 
-0000bad0: 2b20 6368 616e 0a20 2020 2020 2020 2020  + chan.         
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baf0: 2020 2020 2020 2020 2020 2020 2b20 2720              + ' 
-0000bb00: 6e6f 7420 6176 6169 6c61 626c 6520 696e  not available in
-0000bb10: 2072 6177 2064 6174 612e 270a 2020 2020   raw data.'.    
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb40: 202b 2027 2043 6865 636b 2063 6f6e 6e65   + ' Check conne
-0000bb50: 6374 696f 6e20 6d61 7021 2729 0a20 2020  ction map!').   
-0000bb60: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-0000bb70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000bb80: 6669 6e64 2063 6861 6e6e 656c 2069 6e64  find channel ind
-0000bb90: 6578 2069 6e20 636f 6e6e 6563 7469 6f6e  ex in connection
-0000bba0: 206d 6170 0a20 2020 2020 2020 2020 2020   map.           
-0000bbb0: 2020 2020 2069 6e64 203d 2063 6f6e 6e65       ind = conne
-0000bbc0: 6374 696f 6e73 5b27 6465 7465 6374 6f72  ctions['detector
-0000bbd0: 5f63 6861 6e73 275d 2e69 6e64 6578 2863  _chans'].index(c
-0000bbe0: 6861 6e29 0a0a 2020 2020 2020 2020 2020  han)..          
-0000bbf0: 2020 2020 2020 2320 6578 7472 6163 7420        # extract 
-0000bc00: 7365 6c65 6374 6564 2041 4443 206e 756d  selected ADC num
-0000bc10: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
-0000bc20: 2020 2020 7365 6c65 6374 6564 5f61 6463      selected_adc
-0000bc30: 203d 2069 6e74 2863 6f6e 6e65 6374 696f   = int(connectio
-0000bc40: 6e73 5b27 6164 635f 6368 616e 7327 5d5b  ns['adc_chans'][
-0000bc50: 696e 645d 290a 2020 2020 2020 2020 2020  ind]).          
-0000bc60: 2020 2020 2020 6966 2073 656c 6563 7465        if selecte
-0000bc70: 645f 6164 6320 6e6f 7420 696e 2061 6463  d_adc not in adc
-0000bc80: 5f6e 756d 735f 6669 6c65 3a0a 2020 2020  _nums_file:.    
+00006070: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006080: 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    # ============
+00006090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000060a0: 3d3d 3d0a 2020 2020 2020 2020 2320 4d65  ===.        # Me
+000060b0: 6d6f 7279 2063 6865 636b 0a20 2020 2020  mory check.     
+000060c0: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
+000060d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000060e0: 3d3d 3d3d 0a20 2020 2020 2020 2020 2020  ====.           
+000060f0: 2020 2020 200a 2020 2020 2020 2020 7361       .        sa
+00006100: 6d70 6c65 5f62 7974 6573 203d 2032 0a20  mple_bytes = 2. 
+00006110: 2020 2020 2020 2069 6620 6164 6374 6f76         if adctov
+00006120: 6f6c 7420 6f72 2061 6463 746f 616d 7020  olt or adctoamp 
+00006130: 6f72 2062 6173 656c 696e 6573 7562 3a0a  or baselinesub:.
+00006140: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+00006150: 6c65 5f62 7974 6573 203d 2038 0a20 2020  le_bytes = 8.   
+00006160: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00006170: 2020 6f75 7470 7574 5f6d 656d 6f72 795f    output_memory_
+00006180: 7065 725f 6576 656e 7420 3d20 7361 6d70  per_event = samp
+00006190: 6c65 5f62 7974 6573 2a6e 625f 7361 6d70  le_bytes*nb_samp
+000061a0: 6c65 732a 6e62 5f63 6861 6e6e 656c 732f  les*nb_channels/
+000061b0: 3165 390a 2020 2020 2020 2020 6f75 7470  1e9.        outp
+000061c0: 7574 5f6d 656d 6f72 7920 3d20 6e62 5f65  ut_memory = nb_e
+000061d0: 7665 6e74 735f 746f 742a 6f75 7470 7574  vents_tot*output
+000061e0: 5f6d 656d 6f72 795f 7065 725f 6576 656e  _memory_per_even
+000061f0: 740a 2020 2020 2020 2020 6966 206f 7574  t.        if out
+00006200: 7075 745f 6d65 6d6f 7279 3e6d 656d 6f72  put_memory>memor
+00006210: 795f 6c69 6d69 743a 0a20 2020 2020 2020  y_limit:.       
+00006220: 2020 2020 206e 625f 6576 656e 7473 5f74       nb_events_t
+00006230: 6f74 5f74 656d 7020 3d20 696e 7428 726f  ot_temp = int(ro
+00006240: 756e 6428 6d65 6d6f 7279 5f6c 696d 6974  und(memory_limit
+00006250: 2f6f 7574 7075 745f 6d65 6d6f 7279 5f70  /output_memory_p
+00006260: 6572 5f65 7665 6e74 2929 0a20 2020 2020  er_event)).     
+00006270: 2020 2020 2020 2070 7269 6e74 2827 5741         print('WA
+00006280: 524e 494e 473a 204d 6178 206e 756d 6265  RNING: Max numbe
+00006290: 7220 6576 656e 7473 2062 6173 6564 206f  r events based o
+000062a0: 6e20 6d65 6d6f 7279 206c 696d 6974 206f  n memory limit o
+000062b0: 6620 270a 2020 2020 2020 2020 2020 2020  f '.            
+000062c0: 2020 2020 2020 2b20 7374 7228 6d65 6d6f        + str(memo
+000062d0: 7279 5f6c 696d 6974 2920 2b20 2747 4220  ry_limit) + 'GB 
+000062e0: 6973 2027 0a20 2020 2020 2020 2020 2020  is '.           
+000062f0: 2020 2020 2020 202b 2073 7472 286e 625f         + str(nb_
+00006300: 6576 656e 7473 5f74 6f74 5f74 656d 7029  events_tot_temp)
+00006310: 202b 2027 206f 7574 206f 6620 270a 2020   + ' out of '.  
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2b20 7374 7228 6e62 5f65 7665 6e74 735f  + str(nb_events_
+00006340: 746f 7429 202b 2721 2729 0a20 2020 2020  tot) +'!').     
+00006350: 2020 2020 2020 206e 625f 6576 656e 7473         nb_events
+00006360: 5f74 6f74 203d 206e 625f 6576 656e 7473  _tot = nb_events
+00006370: 5f74 6f74 5f74 656d 700a 0a0a 0a0a 2020  _tot_temp.....  
+00006380: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00006390: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
+000063a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000063b0: 3d3d 3d3d 0a20 2020 2020 2020 2023 2020  ====.        #  
+000063c0: 496e 6974 6961 6c69 7a65 206f 7574 7075  Initialize outpu
+000063d0: 740a 2020 2020 2020 2020 2320 3d3d 3d3d  t.        # ====
+000063e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000063f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
+00006400: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+00006410: 2020 2020 2020 2020 6f75 7470 7574 5f64          output_d
+00006420: 6174 6120 3d20 6c69 7374 2829 0a20 2020  ata = list().   
+00006430: 2020 2020 2069 6e66 6f5f 6c69 7374 203d       info_list =
+00006440: 206c 6973 7428 290a 2020 2020 200a 2020   list().     .  
+00006450: 2020 2020 2020 6966 206f 7574 7075 745f        if output_
+00006460: 666f 726d 6174 3d3d 323a 0a20 2020 2020  format==2:.     
+00006470: 2020 2020 2020 2069 6620 6164 6374 6f76         if adctov
+00006480: 6f6c 7420 6f72 2061 6463 746f 616d 7020  olt or adctoamp 
+00006490: 6f72 2062 6173 656c 696e 6573 7562 3a0a  or baselinesub:.
+000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064b0: 6f75 7470 7574 5f64 6174 6120 3d20 6e70  output_data = np
+000064c0: 2e7a 6572 6f73 2828 6e62 5f65 7665 6e74  .zeros((nb_event
+000064d0: 735f 746f 742c 206e 625f 6368 616e 6e65  s_tot, nb_channe
+000064e0: 6c73 2c20 6e62 5f73 616d 706c 6573 292c  ls, nb_samples),
+000064f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006510: 2020 2020 2020 2020 6474 7970 653d 6e70          dtype=np
+00006520: 2e66 6c6f 6174 3634 290a 2020 2020 2020  .float64).      
+00006530: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006540: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00006550: 7574 5f64 6174 6120 3d20 6e70 2e7a 6572  ut_data = np.zer
+00006560: 6f73 2828 6e62 5f65 7665 6e74 735f 746f  os((nb_events_to
+00006570: 742c 206e 625f 6368 616e 6e65 6c73 2c20  t, nb_channels, 
+00006580: 6e62 5f73 616d 706c 6573 292c 0a20 2020  nb_samples),.   
+00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 2020 2020 6474 7970 653d 6e70 2e69 6e74      dtype=np.int
+000065c0: 3136 290a 0a0a 2020 2020 2020 2020 2020  16)...          
+000065d0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000065e0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+000065f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006600: 0a20 2020 2020 2020 2023 2020 4c6f 6f70  .        #  Loop
+00006610: 2061 6e64 2072 6561 6420 6576 656e 7473   and read events
+00006620: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
+00006630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006640: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
+00006650: 200a 2020 2020 2020 2020 2320 6c6f 6f70   .        # loop
+00006660: 2065 7665 6e74 730a 2020 2020 2020 2020   events.        
+00006670: 666f 7220 6965 7665 6e74 2069 6e20 7261  for ievent in ra
+00006680: 6e67 6528 6e62 5f65 7665 6e74 735f 746f  nge(nb_events_to
+00006690: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000066a0: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
+000066b0: 6561 6420 6576 656e 740a 2020 2020 2020  ead event.      
+000066c0: 2020 2020 2020 7472 6163 6573 203d 205b        traces = [
+000066d0: 5d0a 2020 2020 2020 2020 2020 2020 696e  ].            in
+000066e0: 666f 203d 2064 6963 7428 290a 0a20 2020  fo = dict()..   
+000066f0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00006700: 7365 6c65 6374 6564 5f65 7665 6e74 5f66  selected_event_f
+00006710: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
+00006720: 2020 2020 2020 7472 6163 6573 2c20 696e        traces, in
+00006730: 666f 203d 2073 656c 662e 7265 6164 5f6e  fo = self.read_n
+00006740: 6578 745f 6576 656e 7428 6465 7465 6374  ext_event(detect
+00006750: 6f72 5f63 6861 6e73 3d64 6574 6563 746f  or_chans=detecto
+00006760: 725f 6368 616e 732c 0a20 2020 2020 2020  r_chans,.       
+00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006790: 2020 2020 2020 2020 2020 2020 2061 6463               adc
+000067a0: 746f 766f 6c74 3d61 6463 746f 766f 6c74  tovolt=adctovolt
+000067b0: 2c20 6164 6374 6f61 6d70 3d61 6463 746f  , adctoamp=adcto
+000067c0: 616d 702c 0a20 2020 2020 2020 2020 2020  amp,.           
+000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067f0: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
+00006800: 6573 7562 3d62 6173 656c 696e 6573 7562  esub=baselinesub
+00006810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 2020 2020 2020 6261 7365 6c69 6e65 696e        baselinein
+00006850: 6473 3d62 6173 656c 696e 6569 6e64 732c  ds=baselineinds,
+00006860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006890: 2020 2020 2069 6e63 6c75 6465 5f6d 6574       include_met
+000068a0: 6164 6174 613d 5472 7565 290a 2020 2020  adata=True).    
+000068b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000068c0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+000068d0: 656e 745f 696e 6465 7820 3d20 7365 6c65  ent_index = sele
+000068e0: 6374 6564 5f65 7665 6e74 5f66 696c 6573  cted_event_files
+000068f0: 5b69 6576 656e 745d 5b30 5d0a 2020 2020  [ievent][0].    
+00006900: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00006910: 5f6e 616d 6520 3d20 7365 6c65 6374 6564  _name = selected
+00006920: 5f65 7665 6e74 5f66 696c 6573 5b69 6576  _event_files[iev
+00006930: 656e 745d 5b31 5d0a 2020 2020 2020 2020  ent][1].        
+00006940: 2020 2020 2020 2020 7472 6163 6573 2c20          traces, 
+00006950: 696e 666f 203d 2073 656c 662e 7265 6164  info = self.read
+00006960: 5f73 696e 676c 655f 6576 656e 7428 6576  _single_event(ev
+00006970: 656e 745f 696e 6465 782c 2066 696c 655f  ent_index, file_
+00006980: 6e61 6d65 3d66 696c 655f 6e61 6d65 2c0a  name=file_name,.
+00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 2020 2020 2020 6465 7465 6374 6f72 5f63        detector_c
+000069d0: 6861 6e73 3d64 6574 6563 746f 725f 6368  hans=detector_ch
+000069e0: 616e 732c 0a20 2020 2020 2020 2020 2020  ans,.           
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a10: 2020 2020 2020 2020 2020 2061 6463 746f             adcto
+00006a20: 766f 6c74 3d61 6463 746f 766f 6c74 2c20  volt=adctovolt, 
+00006a30: 6164 6374 6f61 6d70 3d61 6463 746f 616d  adctoamp=adctoam
+00006a40: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
+00006a80: 6573 7562 3d62 6173 656c 696e 6573 7562  esub=baselinesub
+00006a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 2020 2020 2020 6261 7365 6c69 6e65          baseline
+00006ad0: 696e 6473 3d62 6173 656c 696e 6569 6e64  inds=baselineind
+00006ae0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b10: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+00006b20: 5f6d 6574 6164 6174 613d 5472 7565 290a  _metadata=True).
+00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b40: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00006b50: 6865 636b 2069 6620 7265 6164 696e 6720  heck if reading 
+00006b60: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
+00006b70: 2020 6966 2069 6e66 6f5b 2772 6561 645f    if info['read_
+00006b80: 7374 6174 7573 275d 3e30 3a0a 2020 2020  status']>0:.    
+00006b90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00006ba0: 7428 2757 4152 4e49 4e47 3a20 556e 6162  t('WARNING: Unab
+00006bb0: 6c65 2074 6f20 7265 6164 2065 7665 6e74  le to read event
+00006bc0: 2023 2720 2b20 7374 7228 6965 7665 6e74   #' + str(ievent
+00006bd0: 2920 2b20 2721 2045 7272 6f72 206d 6573  ) + '! Error mes
+00006be0: 7361 6765 3a20 2729 0a20 2020 2020 2020  sage: ').       
+00006bf0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00006c00: 5741 524e 494e 473a 2022 2720 2b20 696e  WARNING: "' + in
+00006c10: 666f 5b27 6572 726f 725f 6d73 6727 5d20  fo['error_msg'] 
+00006c20: 2b20 2722 2e20 5374 6f70 7069 6e67 2065  + '". Stopping e
+00006c30: 7665 6e74 206c 6f6f 7027 290a 2020 2020  vent loop').    
+00006c40: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00006c50: 6b0a 0a20 2020 2020 2020 2020 2020 200a  k..            .
+00006c60: 2020 2020 2020 2020 2020 2020 2320 6164              # ad
+00006c70: 6420 746f 206d 6574 6164 6174 6120 6c69  d to metadata li
+00006c80: 7374 0a20 2020 2020 2020 2020 2020 2069  st.            i
+00006c90: 6620 696e 636c 7564 655f 6d65 7461 6461  f include_metada
+00006ca0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00006cb0: 2020 2020 696e 666f 5f6c 6973 742e 6170      info_list.ap
+00006cc0: 7065 6e64 2869 6e66 6f29 0a0a 2020 2020  pend(info)..    
+00006cd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006ce0: 2020 2020 2023 2073 746f 7265 0a20 2020       # store.   
+00006cf0: 2020 2020 2020 2020 2069 6620 286f 7574           if (out
+00006d00: 7075 745f 666f 726d 6174 3d3d 3120 6f72  put_format==1 or
+00006d10: 206f 7574 7075 745f 666f 726d 6174 3d3d   output_format==
+00006d20: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
+00006d30: 2020 2020 6f75 7470 7574 5f64 6174 612e      output_data.
+00006d40: 6170 7065 6e64 2874 7261 6365 7329 0a20  append(traces). 
+00006d50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00006d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d70: 206f 7574 7075 745f 6461 7461 5b69 6576   output_data[iev
+00006d80: 656e 742c 3a2c 3a5d 203d 2074 7261 6365  ent,:,:] = trace
+00006d90: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00006da0: 2020 0a0a 2020 2020 2020 2020 2320 7265    ..        # re
+00006db0: 7365 7420 6669 6c65 206c 6973 7420 746f  set file list to
+00006dc0: 206f 7269 6769 6e61 6c20 6c69 7374 0a20   original list. 
+00006dd0: 2020 2020 2020 2023 2069 6620 6e65 6564         # if need
+00006de0: 6564 0a20 2020 2020 2020 2069 6620 6375  ed.        if cu
+00006df0: 7272 656e 745f 6669 6c65 5f6c 6973 7420  rrent_file_list 
+00006e00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00006e10: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00006e20: 745f 6669 6c65 7328 6375 7272 656e 745f  t_files(current_
+00006e30: 6669 6c65 5f6c 6973 7429 0a0a 0a20 2020  file_list)...   
+00006e40: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
+00006e50: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
+00006e60: 2020 2020 2020 7265 7475 726e 206f 7574        return out
+00006e70: 7075 745f 6461 7461 2c20 696e 666f 5f6c  put_data, info_l
+00006e80: 6973 740a 2020 2020 2020 2020 656c 7365  ist.        else
+00006e90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006ea0: 7475 726e 206f 7574 7075 745f 6461 7461  turn output_data
+00006eb0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006ec0: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
+00006ed0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006ee0: 2020 2020 200a 2020 2020 2020 2020 0a0a       .        ..
+00006ef0: 2020 2020 6465 6620 6765 745f 6375 7272      def get_curr
+00006f00: 656e 745f 6669 6c65 5f6e 616d 6528 7365  ent_file_name(se
+00006f10: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00006f20: 0a20 2020 2020 2020 2047 6574 2063 7572  .        Get cur
+00006f30: 7265 6e74 2066 696c 6520 6e61 6d65 0a20  rent file name. 
+00006f40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006f50: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00006f60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00006f70: 2020 2020 2020 4e6f 6e65 0a0a 0a20 2020        None...   
+00006f80: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
+00006f90: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
+00006fa0: 2020 200a 2020 2020 2020 2020 6669 6c65     .        file
+00006fb0: 5f6e 616d 6520 3a20 7374 720a 2020 2020  _name : str.    
+00006fc0: 2020 2020 2020 6375 7272 656e 7420 6669        current fi
+00006fd0: 6c65 206e 616d 650a 0a20 2020 2020 2020  le name..       
+00006fe0: 2022 2222 0a20 2020 2020 2020 200a 2020   """.        .  
+00006ff0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00007000: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+00007010: 6e61 6d65 0a20 2020 2020 2020 200a 0a0a  name.        ...
+00007020: 2020 2020 0a20 2020 2064 6566 2067 6574      .    def get
+00007030: 5f6d 6574 6164 6174 6128 7365 6c66 2c20  _metadata(self, 
+00007040: 6669 6c65 5f6e 616d 653d 4e6f 6e65 2c20  file_name=None, 
+00007050: 6772 6f75 705f 6e61 6d65 3d4e 6f6e 652c  group_name=None,
+00007060: 2064 6174 6173 6574 5f6e 616d 653d 4e6f   dataset_name=No
+00007070: 6e65 2c20 0a20 2020 2020 2020 2020 2020  ne, .           
+00007080: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+00007090: 655f 6461 7461 7365 745f 6d65 7461 6461  e_dataset_metada
+000070a0: 7461 3d46 616c 7365 293a 0a0a 2020 2020  ta=False):..    
+000070b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000070c0: 4675 6e63 7469 6f6e 2074 6f20 6765 7420  Function to get 
+000070d0: 6d65 7461 6461 7461 2e0a 2020 2020 2020  metadata..      
+000070e0: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
+000070f0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00007100: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00007110: 2020 0a20 2020 2020 2020 2066 696c 655f    .        file_
+00007120: 6e61 6d65 3a20 7374 7269 6e67 2c20 6f70  name: string, op
+00007130: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00007140: 2020 2069 6620 6e6f 2066 696c 6520 6e61     if no file na
+00007150: 6d65 2070 726f 7669 6465 643a 2075 7365  me provided: use
+00007160: 2063 7572 7265 6e74 2066 696c 650a 0a20   current file.. 
+00007170: 2020 2020 2020 2067 726f 7570 5f6e 616d         group_nam
+00007180: 653a 2020 7374 7269 6e67 2c20 6f70 7469  e:  string, opti
+00007190: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+000071a0: 2048 3520 2247 726f 7570 2220 6e61 6d65   H5 "Group" name
+000071b0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
+000071c0: 6175 6c74 3a20 4e6f 6e65 2c20 7265 6164  ault: None, read
+000071d0: 2061 6c6c 2067 726f 7570 730a 2020 2020   all groups.    
+000071e0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
+000071f0: 6174 6173 6574 5f6e 616d 653a 2073 7472  ataset_name: str
+00007200: 696e 672c 206f 7074 696f 6e61 6c2c 200a  ing, optional, .
+00007210: 2020 2020 2020 2020 2020 2020 4835 2022              H5 "
+00007220: 4461 7461 7365 7422 206e 616d 650a 2020  Dataset" name.  
+00007230: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00007240: 743a 2061 6c6c 2064 6174 6173 6574 730a  t: all datasets.
+00007250: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00007260: 2020 696e 636c 7564 655f 6461 7461 7365    include_datase
+00007270: 745f 6d65 7461 6461 7461 203a 2062 6f6f  t_metadata : boo
+00007280: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
+00007290: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+000072a0: 2069 6e63 6c75 6465 2064 6174 6173 6574   include dataset
+000072b0: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
+000072c0: 2020 2020 2020 4465 6661 756c 743a 2046        Default: F
+000072d0: 616c 7365 0a20 2020 2020 2020 200a 0a20  alse.        .. 
+000072e0: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
+000072f0: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
+00007300: 2020 2020 200a 2020 2020 2020 2020 6d65       .        me
+00007310: 7461 6461 7461 3a20 6469 6374 0a20 2020  tadata: dict.   
+00007320: 2020 2020 2020 2020 6469 6374 696f 6e61          dictiona
+00007330: 7279 2077 6974 6820 616c 6c20 6d65 7461  ry with all meta
+00007340: 6461 7461 0a0a 2020 2020 2020 2020 2222  data..        ""
+00007350: 220a 0a20 2020 2020 2020 206d 6574 6164  "..        metad
+00007360: 6174 6120 3d20 6469 6374 2829 0a0a 0a20  ata = dict()... 
+00007370: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
+00007380: 6e70 7574 200a 2020 2020 2020 2020 6966  nput .        if
+00007390: 2066 696c 655f 6e61 6d65 2069 7320 4e6f   file_name is No
+000073a0: 6e65 2061 6e64 2073 656c 662e 5f63 7572  ne and self._cur
+000073b0: 7265 6e74 5f66 696c 6520 6973 204e 6f6e  rent_file is Non
+000073c0: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+000073d0: 7272 6f72 5f6d 7367 203d 2027 4e6f 2066  rror_msg = 'No f
+000073e0: 696c 6520 6375 7272 656e 746c 7920 6f70  ile currently op
+000073f0: 656e 2061 6e64 206e 6f20 2266 696c 655f  en and no "file_
+00007400: 6e61 6d65 2220 6172 6775 6d65 6e74 206e  name" argument n
+00007410: 6f74 2070 726f 7669 6465 6421 270a 2020  ot provided!'.  
+00007420: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007430: 662e 5f72 6169 7365 5f65 7272 6f72 733a  f._raise_errors:
+00007440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007450: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00007460: 4572 726f 7228 6572 726f 725f 6d73 6729  Error(error_msg)
+00007470: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00007480: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007490: 2020 2070 7269 6e74 2827 4552 524f 523a     print('ERROR:
+000074a0: 2027 202b 2065 7272 6f72 5f6d 7367 290a   ' + error_msg).
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 7072 696e 7428 2750 6c65 6173 6520 6f70  print('Please op
+000074d0: 656e 2061 2066 696c 6520 6f72 2070 726f  en a file or pro
+000074e0: 7669 6465 2061 2066 696c 6520 6e61 6d65  vide a file name
+000074f0: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
+00007500: 2020 2020 7265 7475 726e 206d 6574 6164      return metad
+00007510: 6174 610a 0a20 2020 2020 2020 2023 206f  ata..        # o
+00007520: 7065 6e20 6669 6c65 2069 6620 6e65 6564  pen file if need
+00007530: 6564 0a20 2020 2020 2020 2069 6620 2866  ed.        if (f
+00007540: 696c 655f 6e61 6d65 2069 7320 6e6f 7420  ile_name is not 
+00007550: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00007560: 2061 6e64 2073 656c 662e 5f63 7572 7265   and self._curre
+00007570: 6e74 5f66 696c 655f 6e61 6d65 213d 6669  nt_file_name!=fi
+00007580: 6c65 5f6e 616d 6529 3a0a 2020 2020 2020  le_name):.      
+00007590: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+000075a0: 2020 2023 2063 6865 636b 2069 6620 6120     # check if a 
+000075b0: 6669 6c65 2061 6c72 6561 6479 206f 7065  file already ope
+000075c0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+000075d0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+000075e0: 696c 6520 6973 206e 6f74 204e 6f6e 653a  ile is not None:
+000075f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007600: 2073 656c 662e 5f63 6c6f 7365 5f66 696c   self._close_fil
+00007610: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00007620: 2320 6f70 656e 0a20 2020 2020 2020 2020  # open.         
+00007630: 2020 2073 656c 662e 5f6f 7065 6e5f 6669     self._open_fi
+00007640: 6c65 2866 696c 655f 6e61 6d65 2c20 6c6f  le(file_name, lo
+00007650: 6164 5f6d 6574 6164 6174 613d 4661 6c73  ad_metadata=Fals
+00007660: 6529 0a20 2020 2020 2020 2020 2020 200a  e).            .
+00007670: 0a20 2020 2020 2020 2023 206c 6f61 6420  .        # load 
+00007680: 6d65 7461 6461 7461 2028 6966 2022 6461  metadata (if "da
+00007690: 7461 7365 7422 206d 6574 6164 6174 6120  taset" metadata 
+000076a0: 7265 7175 6573 7465 6420 2d3e 2072 656c  requested -> rel
+000076b0: 6f61 6429 0a20 2020 2020 2020 2069 6620  oad).        if 
+000076c0: 6461 7461 7365 745f 6e61 6d65 2069 7320  dataset_name is 
+000076d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000076e0: 2020 2020 2020 696e 636c 7564 655f 6461        include_da
+000076f0: 7461 7365 745f 6d65 7461 6461 7461 203d  taset_metadata =
+00007700: 2054 7275 650a 0a20 2020 2020 2020 2069   True..        i
+00007710: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
+00007720: 6669 6c65 5f6d 6574 6164 6174 6120 6973  file_metadata is
+00007730: 204e 6f6e 6520 6f72 2069 6e63 6c75 6465   None or include
+00007740: 5f64 6174 6173 6574 5f6d 6574 6164 6174  _dataset_metadat
+00007750: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
+00007760: 656c 662e 5f6c 6f61 645f 6d65 7461 6461  elf._load_metada
+00007770: 7461 2869 6e63 6c75 6465 5f64 6174 6173  ta(include_datas
+00007780: 6574 5f6d 6574 6164 6174 6129 0a20 2020  et_metadata).   
+00007790: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000077a0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+000077b0: 2020 2023 2066 696e 6420 7370 6563 6966     # find specif
+000077c0: 6963 206d 6574 6164 6174 610a 2020 2020  ic metadata.    
+000077d0: 2020 2020 6d65 7461 6461 7461 203d 2064      metadata = d
+000077e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000077f0: 2067 726f 7570 5f6e 616d 6520 6973 206e   group_name is n
+00007800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007810: 2020 2020 2069 6620 6772 6f75 705f 6e61       if group_na
+00007820: 6d65 2069 6e20 7365 6c66 2e5f 6375 7272  me in self._curr
+00007830: 656e 745f 6669 6c65 5f6d 6574 6164 6174  ent_file_metadat
+00007840: 615b 2767 726f 7570 5f6c 6973 7427 5d3a  a['group_list']:
+00007850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007860: 2067 726f 7570 5f6d 6574 6164 6174 6120   group_metadata 
+00007870: 3d20 7365 6c66 2e5f 6375 7272 656e 745f  = self._current_
+00007880: 6669 6c65 5f6d 6574 6164 6174 615b 2767  file_metadata['g
+00007890: 726f 7570 7327 5d5b 6772 6f75 705f 6e61  roups'][group_na
+000078a0: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
+000078b0: 2020 2020 6966 2064 6174 6173 6574 5f6e      if dataset_n
+000078c0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000078d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000078e0: 2020 2020 2069 6620 6461 7461 7365 745f       if dataset_
+000078f0: 6e61 6d65 2069 6e20 6772 6f75 705f 6d65  name in group_me
+00007900: 7461 6461 7461 5b27 6461 7461 7365 745f  tadata['dataset_
+00007910: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 6d65 7461 6461 7461 203d 2067 726f 7570  metadata = group
+00007940: 5f6d 6574 6164 6174 615b 2764 6174 6173  _metadata['datas
+00007950: 6574 7327 5d5b 6461 7461 7365 745f 6e61  ets'][dataset_na
+00007960: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
+00007970: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00007980: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00007990: 7461 6461 7461 203d 2067 726f 7570 5f6d  tadata = group_m
+000079a0: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
+000079b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000079c0: 2020 6d65 7461 6461 7461 203d 2073 656c    metadata = sel
+000079d0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+000079e0: 6d65 7461 6461 7461 0a0a 0a20 2020 2020  metadata...     
+000079f0: 2020 2023 2063 6c6f 7365 2066 696c 650a     # close file.
+00007a00: 2020 2020 2020 2020 6966 2066 696c 655f          if file_
+00007a10: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+00007a20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007a30: 6c66 2e5f 636c 6f73 655f 6669 6c65 2829  lf._close_file()
+00007a40: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
+00007a50: 2020 2072 6574 7572 6e20 6d65 7461 6461     return metada
+00007a60: 7461 0a20 2020 2020 2020 2020 2020 200a  ta.            .
+00007a70: 0a0a 0a20 2020 2064 6566 2067 6574 5f64  ...    def get_d
+00007a80: 6574 6563 746f 725f 636f 6e66 6967 2873  etector_config(s
+00007a90: 656c 662c 2066 696c 655f 6e61 6d65 3d4e  elf, file_name=N
+00007aa0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 2061 6463 5f6e 616d 653d 2761 6463 3127   adc_name='adc1'
+00007ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00007af0: 655f 6368 616e 5f64 6963 743d 5472 7565  e_chan_dict=True
+00007b00: 293a 2020 200a 2020 2020 2020 2020 2222  ):   .        ""
+00007b10: 220a 2020 2020 2020 2020 4765 7420 6465  ".        Get de
+00007b20: 7465 6374 6f72 2063 6f6e 6669 6775 7261  tector configura
+00007b30: 7469 6f6e 0a20 2020 2020 2020 2022 2222  tion.        """
+00007b40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00007b50: 2020 6465 7465 6374 6f72 5f63 6f6e 6669    detector_confi
+00007b60: 6720 3d20 6469 6374 2829 0a20 2020 2020  g = dict().     
+00007b70: 2020 200a 2020 2020 2020 2020 2320 6765     .        # ge
+00007b80: 7420 6d65 7461 6461 7461 0a20 2020 2020  t metadata.     
+00007b90: 2020 206d 6574 6164 6174 6120 3d20 4e6f     metadata = No
+00007ba0: 6e65 0a20 2020 2020 2020 2069 6620 6669  ne.        if fi
+00007bb0: 6c65 5f6e 616d 6520 6973 206e 6f74 204e  le_name is not N
+00007bc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007bd0: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
+00007be0: 2e67 6574 5f6d 6574 6164 6174 6128 6669  .get_metadata(fi
+00007bf0: 6c65 5f6e 616d 653d 6669 6c65 5f6e 616d  le_name=file_nam
+00007c00: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
+00007c10: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00007c20: 6c65 5f6d 6574 6164 6174 6120 6973 206e  le_metadata is n
+00007c30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007c40: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
+00007c50: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00007c60: 6c65 5f6d 6574 6164 6174 610a 2020 2020  le_metadata.    
+00007c70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00007c80: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00007c90: 6545 7272 6f72 2827 4552 524f 5220 696e  eError('ERROR in
+00007ca0: 2067 6574 5f64 6574 6563 746f 725f 636f   get_detector_co
+00007cb0: 6e66 6967 3a20 6120 6669 6c65 206e 616d  nfig: a file nam
+00007cc0: 6520 6e65 6564 7320 746f 2062 6520 7072  e needs to be pr
+00007cd0: 6f76 6964 6564 2127 290a 2020 2020 2020  ovided!').      
+00007ce0: 2020 0a20 2020 2020 2020 200a 0a20 2020    .        ..   
+00007cf0: 2020 2020 2023 2063 6f6e 6669 6720 6e61       # config na
+00007d00: 6d65 0a20 2020 2020 2020 2063 6f6e 6669  me.        confi
+00007d10: 675f 6e61 6d65 203d 2027 6465 7463 6f6e  g_name = 'detcon
+00007d20: 6669 6731 270a 2020 2020 2020 2020 6966  fig1'.        if
+00007d30: 2061 6463 5f6e 616d 6521 3d27 6164 6331   adc_name!='adc1
+00007d40: 273a 0a20 2020 2020 2020 2020 2020 2063  ':.            c
+00007d50: 6f6e 6669 675f 6e61 6d65 203d 2027 6465  onfig_name = 'de
+00007d60: 7463 6f6e 6669 6727 202b 2061 6463 5f6e  tconfig' + adc_n
+00007d70: 616d 655b 333a 5d0a 0a20 2020 2020 2020  ame[3:]..       
+00007d80: 2023 2063 6865 636b 2069 6620 6176 6169   # check if avai
+00007d90: 6c61 626c 650a 2020 2020 2020 2020 6966  lable.        if
+00007da0: 2063 6f6e 6669 675f 6e61 6d65 206e 6f74   config_name not
+00007db0: 2069 6e20 6d65 7461 6461 7461 5b27 6772   in metadata['gr
+00007dc0: 6f75 705f 6c69 7374 275d 3a0a 2020 2020  oup_list']:.    
+00007dd0: 2020 2020 2020 2020 7072 696e 7428 2745          print('E
+00007de0: 5252 4f52 3a20 756e 6162 6c65 2074 6f20  RROR: unable to 
+00007df0: 6669 6e64 2064 6574 6563 746f 7220 636f  find detector co
+00007e00: 6e66 6967 2127 290a 2020 2020 2020 2020  nfig!').        
+00007e10: 2020 2020 7265 7475 726e 205b 5d0a 0a20      return [].. 
+00007e20: 2020 2020 2020 2023 2067 726f 7570 206d         # group m
+00007e30: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
+00007e40: 6465 7465 6374 6f72 5f63 6f6e 6669 675f  detector_config_
+00007e50: 6469 6374 203d 206d 6574 6164 6174 615b  dict = metadata[
+00007e60: 2767 726f 7570 7327 5d5b 636f 6e66 6967  'groups'][config
+00007e70: 5f6e 616d 655d 0a20 2020 2020 2020 2023  _name].        #
+00007e80: 6966 2027 6164 635f 6e61 6d65 2720 696e  if 'adc_name' in
+00007e90: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
+00007ea0: 5f64 6963 7420 616e 6420 6164 635f 6e61  _dict and adc_na
+00007eb0: 6d65 213d 6465 7465 6374 6f72 5f63 6f6e  me!=detector_con
+00007ec0: 6669 675f 6469 6374 5b27 6164 635f 6e61  fig_dict['adc_na
+00007ed0: 6d65 275d 3a0a 2020 2020 2020 2020 2320  me']:.        # 
+00007ee0: 2020 2070 7269 6e74 2827 4552 524f 523a     print('ERROR:
+00007ef0: 2055 6e65 7870 6563 7465 6420 6465 7465   Unexpected dete
+00007f00: 6374 6f72 2063 6f6e 6669 6775 7261 7469  ctor configurati
+00007f10: 6f6e 2066 6f72 6d61 7421 2729 0a20 2020  on format!').   
+00007f20: 2020 2020 2023 2020 2020 7265 7475 726e       #    return
+00007f30: 205b 5d0a 0a0a 2020 2020 2020 2020 2320   []...        # 
+00007f40: 6164 6420 6465 7465 6374 6f72 2f63 6861  add detector/cha
+00007f50: 6e6e 656c 206c 6973 7420 6672 6f6d 2061  nnel list from a
+00007f60: 6463 206d 6574 6164 6174 612c 206e 6565  dc metadata, nee
+00007f70: 6473 2074 6f20 6d61 7463 680a 2020 2020  ds to match.    
+00007f80: 2020 2020 2320 6465 7465 6374 6f72 2073      # detector s
+00007f90: 6574 7469 6e67 7320 6172 7261 7920 6f72  ettings array or
+00007fa0: 6465 720a 2020 2020 2020 2020 7465 735f  der.        tes_
+00007fb0: 6368 616e 7320 3d20 6c69 7374 2829 0a20  chans = list(). 
+00007fc0: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
+00007fd0: 6368 616e 7320 3d20 6c69 7374 2829 0a20  chans = list(). 
+00007fe0: 2020 2020 2020 2063 6f6e 7472 6f6c 6c65         controlle
+00007ff0: 725f 6368 616e 7320 3d20 6c69 7374 2829  r_chans = list()
+00008000: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+00008010: 696f 6e5f 6469 6374 203d 2073 656c 662e  ion_dict = self.
+00008020: 6765 745f 636f 6e6e 6563 7469 6f6e 5f64  get_connection_d
+00008030: 6963 7428 6164 635f 6e61 6d65 3d61 6463  ict(adc_name=adc
+00008040: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00008080: 7461 3d6d 6574 6164 6174 6129 0a0a 2020  ta=metadata)..  
+00008090: 2020 2020 2020 6966 2063 6f6e 6e65 6374        if connect
+000080a0: 696f 6e5f 6469 6374 3a0a 2020 2020 2020  ion_dict:.      
+000080b0: 2020 2020 2020 6368 616e 5f6c 6973 7420        chan_list 
+000080c0: 3d20 6465 7465 6374 6f72 5f63 6f6e 6669  = detector_confi
+000080d0: 675f 6469 6374 5b27 6368 616e 6e65 6c5f  g_dict['channel_
+000080e0: 6c69 7374 275d 0a20 2020 2020 2020 2020  list'].         
+000080f0: 2020 2069 6620 286e 6f74 2069 7369 6e73     if (not isins
+00008100: 7461 6e63 6528 6368 616e 5f6c 6973 742c  tance(chan_list,
+00008110: 206e 702e 6e64 6172 7261 7929 0a20 2020   np.ndarray).   
+00008120: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00008130: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00008140: 6368 616e 5f6c 6973 742c 206c 6973 7429  chan_list, list)
+00008150: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00008160: 2020 2063 6861 6e5f 6c69 7374 2020 3d20     chan_list  = 
+00008170: 5b63 6861 6e5f 6c69 7374 5d0a 2020 2020  [chan_list].    
+00008180: 2020 2020 2020 2020 666f 7220 6368 616e          for chan
+00008190: 2069 6e20 6368 616e 5f6c 6973 743a 0a20   in chan_list:. 
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000081b0: 6620 6368 616e 2069 6e20 636f 6e6e 6563  f chan in connec
+000081c0: 7469 6f6e 5f64 6963 745b 2761 6463 5f63  tion_dict['adc_c
+000081d0: 6861 6e73 275d 3a0a 2020 2020 2020 2020  hans']:.        
+000081e0: 2020 2020 2020 2020 2020 2020 696e 6420              ind 
+000081f0: 3d20 636f 6e6e 6563 7469 6f6e 5f64 6963  = connection_dic
+00008200: 745b 2761 6463 5f63 6861 6e73 275d 2e69  t['adc_chans'].i
+00008210: 6e64 6578 2869 6e74 2863 6861 6e29 290a  ndex(int(chan)).
+00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008230: 2020 2020 6966 2063 6f6e 6e65 6374 696f      if connectio
+00008240: 6e5f 6469 6374 5b27 636f 6e74 726f 6c6c  n_dict['controll
+00008250: 6572 5f63 6861 6e73 275d 3a0a 2020 2020  er_chans']:.    
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 2020 636f 6e74 726f 6c6c 6572 5f63      controller_c
+00008280: 6861 6e73 2e61 7070 656e 6428 636f 6e6e  hans.append(conn
+00008290: 6563 7469 6f6e 5f64 6963 745b 2763 6f6e  ection_dict['con
+000082a0: 7472 6f6c 6c65 725f 6368 616e 7327 5d5b  troller_chans'][
+000082b0: 696e 645d 290a 2020 2020 2020 2020 2020  ind]).          
+000082c0: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
+000082d0: 6e65 6374 696f 6e5f 6469 6374 5b27 7465  nection_dict['te
+000082e0: 735f 6368 616e 7327 5d3a 0a20 2020 2020  s_chans']:.     
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2074 6573 5f63 6861 6e73 2e61 7070     tes_chans.app
+00008310: 656e 6428 636f 6e6e 6563 7469 6f6e 5f64  end(connection_d
+00008320: 6963 745b 2774 6573 5f63 6861 6e73 275d  ict['tes_chans']
+00008330: 5b69 6e64 5d29 0a20 2020 2020 2020 2020  [ind]).         
+00008340: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00008350: 6e6e 6563 7469 6f6e 5f64 6963 745b 2764  nnection_dict['d
+00008360: 6574 6563 746f 725f 6368 616e 7327 5d3a  etector_chans']:
+00008370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008380: 2020 2020 2020 2020 2064 6574 6563 746f           detecto
+00008390: 725f 6368 616e 732e 6170 7065 6e64 2863  r_chans.append(c
+000083a0: 6f6e 6e65 6374 696f 6e5f 6469 6374 5b27  onnection_dict['
+000083b0: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
+000083c0: 5b69 6e64 5d29 0a20 2020 2020 2020 2020  [ind]).         
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008400: 200a 2020 2020 2020 2020 6465 7465 6374   .        detect
+00008410: 6f72 5f63 6f6e 6669 675f 6469 6374 5b27  or_config_dict['
+00008420: 7465 735f 6368 616e 7327 5d20 3d20 2074  tes_chans'] =  t
+00008430: 6573 5f63 6861 6e73 0a20 2020 2020 2020  es_chans.       
+00008440: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
+00008450: 5f64 6963 745b 2764 6574 6563 746f 725f  _dict['detector_
+00008460: 6368 616e 7327 5d20 3d20 2064 6574 6563  chans'] =  detec
+00008470: 746f 725f 6368 616e 730a 2020 2020 2020  tor_chans.      
+00008480: 2020 6465 7465 6374 6f72 5f63 6f6e 6669    detector_confi
+00008490: 675f 6469 6374 5b27 636f 6e74 726f 6c6c  g_dict['controll
+000084a0: 6572 5f63 6861 6e73 275d 203d 2020 636f  er_chans'] =  co
+000084b0: 6e74 726f 6c6c 6572 5f63 6861 6e73 2020  ntroller_chans  
+000084c0: 200a 0a20 2020 2020 2020 2023 2063 6f6e   ..        # con
+000084d0: 7665 7274 2074 6f20 6c69 7374 2069 6620  vert to list if 
+000084e0: 6e65 6564 6564 2028 7369 7a65 206f 6620  needed (size of 
+000084f0: 6e62 2063 6861 6e6e 656c 7329 0a20 2020  nb channels).   
+00008500: 2020 2020 206e 625f 6368 616e 203d 206c       nb_chan = l
+00008510: 656e 2864 6574 6563 746f 725f 636f 6e66  en(detector_conf
+00008520: 6967 5f64 6963 745b 2764 6574 6563 746f  ig_dict['detecto
+00008530: 725f 6368 616e 7327 5d29 0a20 2020 2020  r_chans']).     
+00008540: 2020 2066 6f72 2063 6f6e 6669 6720 696e     for config in
+00008550: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
+00008560: 5f64 6963 742e 6b65 7973 2829 3a0a 2020  _dict.keys():.  
+00008570: 2020 2020 2020 2020 2020 7061 7261 6d20            param 
+00008580: 3d20 6465 7465 6374 6f72 5f63 6f6e 6669  = detector_confi
+00008590: 675f 6469 6374 5b63 6f6e 6669 675d 0a20  g_dict[config]. 
+000085a0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000085b0: 7420 6973 696e 7374 616e 6365 2870 6172  t isinstance(par
+000085c0: 616d 2c20 6c69 7374 2920 616e 6420 6e6f  am, list) and no
+000085d0: 7420 6973 696e 7374 616e 6365 2870 6172  t isinstance(par
+000085e0: 616d 2c20 6e70 2e6e 6461 7272 6179 293a  am, np.ndarray):
+000085f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008600: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
+00008610: 5f64 6963 745b 636f 6e66 6967 5d20 3d20  _dict[config] = 
+00008620: 5b64 6574 6563 746f 725f 636f 6e66 6967  [detector_config
+00008630: 5f64 6963 745b 636f 6e66 6967 5d5d 2a6e  _dict[config]]*n
+00008640: 625f 6368 616e 0a20 2020 200a 2020 2020  b_chan.    .    
+00008650: 2020 2020 2320 636f 6e76 6572 7420 746f      # convert to
+00008660: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
+00008670: 2020 2020 6465 7465 6374 6f72 5f63 6f6e      detector_con
+00008680: 6669 6720 3d20 6469 6374 2829 0a20 2020  fig = dict().   
+00008690: 2020 2020 2069 6620 7573 655f 6368 616e       if use_chan
+000086a0: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
+000086b0: 2020 2063 6861 6e5f 6c69 7374 203d 2064     chan_list = d
+000086c0: 6574 6563 746f 725f 636f 6e66 6967 5f64  etector_config_d
+000086d0: 6963 745b 2764 6574 6563 746f 725f 6368  ict['detector_ch
+000086e0: 616e 7327 5d0a 2020 2020 2020 2020 2020  ans'].          
+000086f0: 2020 666f 7220 6368 616e 2069 6e20 6368    for chan in ch
+00008700: 616e 5f6c 6973 743a 0a20 2020 2020 2020  an_list:.       
+00008710: 2020 2020 2020 2020 2063 6861 6e5f 696e           chan_in
+00008720: 6465 7820 3d20 6465 7465 6374 6f72 5f63  dex = detector_c
+00008730: 6f6e 6669 675f 6469 6374 5b27 6465 7465  onfig_dict['dete
+00008740: 6374 6f72 5f63 6861 6e73 275d 2e69 6e64  ctor_chans'].ind
+00008750: 6578 2863 6861 6e29 0a20 2020 2020 2020  ex(chan).       
+00008760: 2020 2020 2020 2020 2064 6574 6563 746f           detecto
+00008770: 725f 636f 6e66 6967 5b63 6861 6e5d 203d  r_config[chan] =
+00008780: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00008790: 2020 2020 2020 2020 666f 7220 636f 6e66          for conf
+000087a0: 6967 2069 6e20 6465 7465 6374 6f72 5f63  ig in detector_c
+000087b0: 6f6e 6669 675f 6469 6374 3a0a 2020 2020  onfig_dict:.    
+000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087d0: 6966 206c 656e 2864 6574 6563 746f 725f  if len(detector_
+000087e0: 636f 6e66 6967 5f64 6963 745b 636f 6e66  config_dict[conf
+000087f0: 6967 5d29 3d3d 6e62 5f63 6861 6e3a 0a20  ig])==nb_chan:. 
+00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008810: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
+00008820: 636f 6e66 6967 5b63 6861 6e5d 5b63 6f6e  config[chan][con
+00008830: 6669 675d 203d 2064 6574 6563 746f 725f  fig] = detector_
+00008840: 636f 6e66 6967 5f64 6963 745b 636f 6e66  config_dict[conf
+00008850: 6967 5d5b 6368 616e 5f69 6e64 6578 5d0a  ig][chan_index].
+00008860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008870: 2020 2020 2020 2020 2020 6465 7465 6374            detect
+00008880: 6f72 5f63 6f6e 6669 6720 3d20 6465 7465  or_config = dete
+00008890: 6374 6f72 5f63 6f6e 6669 675f 6469 6374  ctor_config_dict
+000088a0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000088b0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
+000088e0: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
+000088f0: 0a0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008910: 2020 2020 2020 200a 2020 2020 6465 6620         .    def 
+00008920: 6765 745f 636f 6e6e 6563 7469 6f6e 5f64  get_connection_d
+00008930: 6963 7428 7365 6c66 2c20 6669 6c65 5f6e  ict(self, file_n
+00008940: 616d 653d 4e6f 6e65 2c20 6164 635f 6e61  ame=None, adc_na
+00008950: 6d65 3d27 6164 6331 272c 206d 6574 6164  me='adc1', metad
+00008960: 6174 613d 4e6f 6e65 293a 0a20 2020 2020  ata=None):.     
+00008970: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00008980: 6574 2063 6f6e 6e65 6374 696f 6e20 6469  et connection di
+00008990: 6374 696f 6e61 7279 2066 6f72 2073 7065  ctionary for spe
+000089a0: 6369 6669 6420 6164 6320 6e61 6d65 0a20  cifid adc name. 
+000089b0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000089c0: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
+000089d0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+000089e0: 696f 6e5f 6469 6374 3d64 6963 7428 290a  ion_dict=dict().
+000089f0: 0a20 2020 2020 2020 2023 206d 6574 6164  .        # metad
+00008a00: 6174 610a 2020 2020 2020 2020 6164 635f  ata.        adc_
+00008a10: 6d65 7461 6461 7461 203d 204e 6f6e 650a  metadata = None.
+00008a20: 2020 2020 2020 2020 6966 206d 6574 6164          if metad
+00008a30: 6174 6120 6973 204e 6f6e 6520 6f72 2027  ata is None or '
+00008a40: 6772 6f75 705f 6c69 7374 2720 6e6f 7420  group_list' not 
+00008a50: 696e 206d 6574 6164 6174 613a 0a20 2020  in metadata:.   
+00008a60: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00008a70: 6120 3d20 7365 6c66 2e67 6574 5f6d 6574  a = self.get_met
+00008a80: 6164 6174 6128 6669 6c65 5f6e 616d 653d  adata(file_name=
+00008a90: 6669 6c65 5f6e 616d 6529 0a0a 2020 2020  file_name)..    
+00008aa0: 2020 2020 6966 2027 6772 6f75 705f 6c69      if 'group_li
+00008ab0: 7374 2720 696e 206d 6574 6164 6174 6120  st' in metadata 
+00008ac0: 616e 6420 6164 635f 6e61 6d65 2069 6e20  and adc_name in 
+00008ad0: 6d65 7461 6461 7461 5b27 6772 6f75 705f  metadata['group_
+00008ae0: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
+00008af0: 2020 2020 6164 635f 6d65 7461 6461 7461      adc_metadata
+00008b00: 2020 3d20 6d65 7461 6461 7461 5b27 6772    = metadata['gr
+00008b10: 6f75 7073 275d 5b61 6463 5f6e 616d 655d  oups'][adc_name]
+00008b20: 0a0a 2020 2020 2020 2020 6966 2061 6463  ..        if adc
+00008b30: 5f6d 6574 6164 6174 6120 6973 204e 6f6e  _metadata is Non
+00008b40: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+00008b50: 7272 6f72 5f6d 7367 203d 2027 4144 4320  rror_msg = 'ADC 
+00008b60: 6d65 7461 6461 7461 206e 6f74 2066 6f75  metadata not fou
+00008b70: 6e64 2127 0a20 2020 2020 2020 2020 2020  nd!'.           
+00008b80: 2069 6620 7365 6c66 2e5f 7261 6973 655f   if self._raise_
+00008b90: 6572 726f 7273 3a0a 2020 2020 2020 2020  errors:.        
+00008ba0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00008bb0: 6520 5661 6c75 6545 7272 6f72 2865 7272  e ValueError(err
+00008bc0: 6f72 5f6d 7367 290a 2020 2020 2020 2020  or_msg).        
+00008bd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008be0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00008bf0: 2757 4152 4e49 4e47 3a20 2720 2b20 6572  'WARNING: ' + er
+00008c00: 726f 725f 6d73 6729 0a20 2020 2020 2020  ror_msg).       
+00008c10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008c20: 636f 6e65 6374 696f 6e5f 6469 6374 0a0a  conection_dict..
+00008c30: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+00008c40: 696f 6e5f 6469 6374 5b27 6164 635f 6368  ion_dict['adc_ch
+00008c50: 616e 7327 5d20 3d20 6c69 7374 2829 0a20  ans'] = list(). 
+00008c60: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+00008c70: 6e5f 6469 6374 5b27 636f 6e74 726f 6c6c  n_dict['controll
+00008c80: 6572 5f63 6861 6e73 275d 203d 206c 6973  er_chans'] = lis
+00008c90: 7428 290a 2020 2020 2020 2020 636f 6e6e  t().        conn
+00008ca0: 6563 7469 6f6e 5f64 6963 745b 2774 6573  ection_dict['tes
+00008cb0: 5f63 6861 6e73 275d 203d 206c 6973 7428  _chans'] = list(
+00008cc0: 290a 2020 2020 2020 2020 636f 6e6e 6563  ).        connec
+00008cd0: 7469 6f6e 5f64 6963 745b 2764 6574 6563  tion_dict['detec
+00008ce0: 746f 725f 6368 616e 7327 5d20 3d20 6c69  tor_chans'] = li
+00008cf0: 7374 2829 0a20 2020 2020 2020 200a 2020  st().        .  
+00008d00: 2020 2020 2020 2320 6c6f 6f70 206d 6574        # loop met
+00008d10: 6164 6174 6120 746f 2066 696e 6420 636f  adata to find co
+00008d20: 6e6e 6563 7469 6f6e 730a 2020 2020 2020  nnections.      
+00008d30: 2020 666f 7220 6b65 792c 7661 6c75 6520    for key,value 
+00008d40: 696e 2061 6463 5f6d 6574 6164 6174 612e  in adc_metadata.
+00008d50: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00008d60: 2020 2020 2069 6620 6b65 792e 6669 6e64       if key.find
+00008d70: 2827 636f 6e6e 6563 7469 6f6e 2729 213d  ('connection')!=
+00008d80: 2d31 3a0a 2020 2020 2020 2020 2020 2020  -1:.            
+00008d90: 2020 2020 636f 6e6e 6563 7469 6f6e 5f64      connection_d
+00008da0: 6963 745b 2761 6463 5f63 6861 6e73 275d  ict['adc_chans']
+00008db0: 2e61 7070 656e 6428 696e 7428 6b65 795b  .append(int(key[
+00008dc0: 3130 3a5d 2929 0a20 2020 2020 2020 2020  10:])).         
+00008dd0: 2020 2020 2020 2066 6f72 2063 6f6e 6e65         for conne
+00008de0: 6374 696f 6e5f 7479 7065 2069 6e20 7661  ction_type in va
+00008df0: 6c75 653a 0a20 2020 2020 2020 2020 2020  lue:.           
+00008e00: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+00008e10: 5f6e 616d 6520 3d20 636f 6e6e 6563 7469  _name = connecti
+00008e20: 6f6e 5f74 7970 655b 636f 6e6e 6563 7469  on_type[connecti
+00008e30: 6f6e 5f74 7970 652e 6669 6e64 2827 3a27  on_type.find(':'
+00008e40: 292b 313a 5d0a 2020 2020 2020 2020 2020  )+1:].          
+00008e50: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
+00008e60: 6e65 6374 696f 6e5f 7479 7065 2e66 696e  nection_type.fin
+00008e70: 6428 2774 6573 3a27 2921 3d2d 313a 0a20  d('tes:')!=-1:. 
+00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e90: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+00008ea0: 6e5f 6469 6374 5b27 7465 735f 6368 616e  n_dict['tes_chan
+00008eb0: 7327 5d2e 6170 7065 6e64 2863 6861 6e6e  s'].append(chann
+00008ec0: 656c 5f6e 616d 6529 0a20 2020 2020 2020  el_name).       
+00008ed0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00008ee0: 636f 6e6e 6563 7469 6f6e 5f74 7970 652e  connection_type.
+00008ef0: 6669 6e64 2827 6465 7465 6374 6f72 3a27  find('detector:'
+00008f00: 2921 3d2d 313a 0a20 2020 2020 2020 2020  )!=-1:.         
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008f20: 6f6e 6e65 6374 696f 6e5f 6469 6374 5b27  onnection_dict['
+00008f30: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
+00008f40: 2e61 7070 656e 6428 6368 616e 6e65 6c5f  .append(channel_
+00008f50: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+00008f60: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
+00008f70: 6e65 6374 696f 6e5f 7479 7065 2e66 696e  nection_type.fin
+00008f80: 6428 2763 6f6e 7472 6f6c 6c65 723a 2729  d('controller:')
+00008f90: 213d 2d31 3a0a 2020 2020 2020 2020 2020  !=-1:.          
+00008fa0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00008fb0: 6e6e 6563 7469 6f6e 5f64 6963 745b 2763  nnection_dict['c
+00008fc0: 6f6e 7472 6f6c 6c65 725f 6368 616e 7327  ontroller_chans'
+00008fd0: 5d2e 6170 7065 6e64 2863 6861 6e6e 656c  ].append(channel
+00008fe0: 5f6e 616d 6529 0a0a 2020 2020 2020 2020  _name)..        
+00008ff0: 7265 7475 726e 2063 6f6e 6e65 6374 696f  return connectio
+00009000: 6e5f 6469 6374 2020 2020 2020 2020 2020  n_dict          
+00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009020: 2020 2020 0a0a 0a20 2020 200a 0a20 2020      ...    ..   
+00009030: 2064 6566 2067 6574 5f63 6f6e 6e65 6374   def get_connect
+00009040: 696f 6e5f 7461 626c 6528 7365 6c66 2c20  ion_table(self, 
+00009050: 6669 6c65 5f6e 616d 653d 4e6f 6e65 2c20  file_name=None, 
+00009060: 6d65 7461 6461 7461 3d4e 6f6e 6529 3a0a  metadata=None):.
+00009070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009080: 2020 2020 4765 7420 636f 6e6e 6563 7469      Get connecti
+00009090: 6f6e 2074 6162 6c65 0a20 2020 2020 2020  on table.       
+000090a0: 2022 2222 0a20 2020 2020 2020 200a 2020   """.        .  
+000090b0: 2020 2020 2020 6966 206d 6574 6164 6174        if metadat
+000090c0: 6120 6973 204e 6f6e 653a 0a20 2020 2020  a is None:.     
+000090d0: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
+000090e0: 3d20 7365 6c66 2e67 6574 5f6d 6574 6164  = self.get_metad
+000090f0: 6174 6128 6669 6c65 5f6e 616d 653d 6669  ata(file_name=fi
+00009100: 6c65 5f6e 616d 6529 0a20 2020 2020 2020  le_name).       
+00009110: 200a 2020 2020 2020 2020 2320 6368 6563   .        # chec
+00009120: 6b20 6164 6320 6c69 7374 2065 7869 7374  k adc list exist
+00009130: 200a 2020 2020 2020 2020 6966 2027 6164   .        if 'ad
+00009140: 635f 6c69 7374 2720 6e6f 7420 696e 206d  c_list' not in m
+00009150: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
+00009160: 2020 2020 2070 7269 6e74 2827 4552 524f       print('ERRO
+00009170: 523a 204e 6f20 4144 4320 6d65 7461 6461  R: No ADC metada
+00009180: 7461 2066 6f75 6e64 2069 6e20 7468 6520  ta found in the 
+00009190: 6669 6c65 2127 290a 2020 2020 2020 2020  file!').        
+000091a0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+000091b0: 2020 2020 0a20 2020 2020 2020 2023 206c      .        # l
+000091c0: 6f6f 7020 6164 6320 616e 6420 6669 6e64  oop adc and find
+000091d0: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+000091e0: 2020 2020 636f 6e6e 6563 7469 6f6e 5f6c      connection_l
+000091f0: 6973 7420 3d20 6c69 7374 2829 0a20 2020  ist = list().   
+00009200: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
+00009210: 6e61 6d65 5f6c 6973 7420 3d20 6c69 7374  name_list = list
+00009220: 2829 0a20 2020 2020 2020 2066 6f72 2061  ().        for a
+00009230: 6463 5f69 6420 696e 206d 6574 6164 6174  dc_id in metadat
+00009240: 615b 2761 6463 5f6c 6973 7427 5d3a 0a20  a['adc_list']:. 
+00009250: 2020 2020 2020 2020 2020 2061 6463 5f6d             adc_m
+00009260: 6574 6164 6174 6120 3d20 6d65 7461 6461  etadata = metada
+00009270: 7461 5b27 6772 6f75 7073 275d 5b61 6463  ta['groups'][adc
+00009280: 5f69 645d 0a20 2020 2020 2020 2020 2020  _id].           
+00009290: 2066 6f72 206b 6579 2c76 616c 2069 6e20   for key,val in 
+000092a0: 6164 635f 6d65 7461 6461 7461 2e69 7465  adc_metadata.ite
+000092b0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+000092c0: 2020 2020 2020 6966 206b 6579 5b30 3a31        if key[0:1
+000092d0: 305d 3d3d 2763 6f6e 6e65 6374 696f 6e27  0]=='connection'
+000092e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000092f0: 2020 2020 2020 6164 635f 6368 616e 203d        adc_chan =
+00009300: 2072 652e 7375 6228 7227 5c73 2b27 2c27   re.sub(r'\s+','
+00009310: 272c 2073 7472 286b 6579 2929 5b31 303a  ', str(key))[10:
+00009320: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00009330: 2020 2020 2020 6e61 6d65 5f76 616c 5f6c        name_val_l
+00009340: 6973 742c 206e 616d 655f 6c69 7374 2c20  ist, name_list, 
+00009350: 7661 6c5f 6c69 7374 203d 2028 0a20 2020  val_list = (.   
+00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009370: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
+00009380: 7574 696c 732e 6578 7472 6163 745f 6164  utils.extract_ad
+00009390: 635f 636f 6e6e 6563 7469 6f6e 286c 6973  c_connection(lis
+000093a0: 7428 7661 6c29 2929 0a20 2020 2020 2020  t(val))).       
+000093b0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+000093c0: 5f6c 6973 7420 203d 205b 6164 635f 6964  _list  = [adc_id
+000093d0: 2c61 6463 5f63 6861 6e5d 202b 2076 616c  ,adc_chan] + val
+000093e0: 5f6c 6973 740a 2020 2020 2020 2020 2020  _list.          
+000093f0: 2020 2020 2020 2020 2020 6e61 6d65 5f6c            name_l
+00009400: 6973 7420 3d20 5b27 6164 635f 6964 272c  ist = ['adc_id',
+00009410: 2761 6463 5f63 6861 6e6e 656c 275d 202b  'adc_channel'] +
+00009420: 206e 616d 655f 6c69 7374 0a20 2020 2020   name_list.     
+00009430: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009440: 6f6e 6e65 6374 696f 6e5f 6c69 7374 2e61  onnection_list.a
+00009450: 7070 656e 6428 7661 6c5f 6c69 7374 290a  ppend(val_list).
+00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009470: 2020 2020 6966 206e 6f74 2063 6f6e 6e65      if not conne
+00009480: 6374 696f 6e5f 6e61 6d65 5f6c 6973 743a  ction_name_list:
+00009490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094a0: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+000094b0: 696f 6e5f 6e61 6d65 5f6c 6973 7420 3d20  ion_name_list = 
+000094c0: 6e61 6d65 5f6c 6973 740a 2020 2020 2020  name_list.      
+000094d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000094e0: 6966 2063 6f6e 6e65 6374 696f 6e5f 6e61  if connection_na
+000094f0: 6d65 5f6c 6973 7421 3d6e 616d 655f 6c69  me_list!=name_li
+00009500: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00009510: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00009520: 7428 2745 5252 4f52 3a20 6d69 7373 696e  t('ERROR: missin
+00009530: 6720 6164 6320 636f 6e6e 6563 7469 6f6e  g adc connection
+00009540: 2076 616c 7565 7321 2729 0a20 2020 2020   values!').     
+00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009560: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+00009570: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00009580: 2063 6f6e 6e65 6374 696f 6e5f 7461 626c   connection_tabl
+00009590: 6520 3d20 7064 2e44 6174 6146 7261 6d65  e = pd.DataFrame
+000095a0: 2863 6f6e 6e65 6374 696f 6e5f 6c69 7374  (connection_list
+000095b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095d0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+000095e0: 733d 636f 6e6e 6563 7469 6f6e 5f6e 616d  s=connection_nam
+000095f0: 655f 6c69 7374 2029 0a20 2020 2020 2020  e_list ).       
+00009600: 2072 6574 7572 6e20 636f 6e6e 6563 7469   return connecti
+00009610: 6f6e 5f74 6162 6c65 0a0a 0a20 2020 200a  on_table...    .
+00009620: 2020 0a0a 2020 2020 6465 6620 5f6f 7065    ..    def _ope
+00009630: 6e5f 6669 6c65 2873 656c 662c 2066 696c  n_file(self, fil
+00009640: 655f 6e61 6d65 2c20 7277 5f73 7472 696e  e_name, rw_strin
+00009650: 673d 2772 272c 206c 6f61 645f 6d65 7461  g='r', load_meta
+00009660: 6461 7461 3d54 7275 6529 3a0a 2020 2020  data=True):.    
+00009670: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00009680: 6f70 656e 2066 696c 6520 0a20 2020 2020  open file .     
+00009690: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000096a0: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
+000096b0: 6669 6c65 2069 7320 6e6f 7420 4e6f 6e65  file is not None
+000096c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000096d0: 6c66 2e5f 636c 6f73 655f 6669 6c65 2829  lf._close_file()
+000096e0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000096f0: 2020 2020 2020 6669 6c65 203d 204e 6f6e        file = Non
+00009700: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
+00009710: 2020 2020 2020 2020 2020 2066 696c 6520             file 
+00009720: 3d20 6835 7079 2e46 696c 6528 6669 6c65  = h5py.File(file
+00009730: 5f6e 616d 652c 7277 5f73 7472 696e 6729  _name,rw_string)
+00009740: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
+00009750: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00009760: 6e74 2827 4552 524f 523a 2075 6e61 626c  nt('ERROR: unabl
+00009770: 6520 746f 206f 7065 6e20 6669 6c65 2027  e to open file '
+00009780: 202b 2066 696c 655f 6e61 6d65 290a 2020   + file_name).  
+00009790: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000097a0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000097b0: 6375 7272 656e 745f 6669 6c65 203d 2066  current_file = f
+000097c0: 696c 650a 2020 2020 2020 2020 7365 6c66  ile.        self
+000097d0: 2e5f 6375 7272 656e 745f 6669 6c65 5f6e  ._current_file_n
+000097e0: 616d 6520 3d20 6669 6c65 5f6e 616d 650a  ame = file_name.
+000097f0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+00009800: 7272 656e 745f 6669 6c65 5f6e 625f 6576  rrent_file_nb_ev
+00009810: 656e 7473 203d 2030 0a20 2020 2020 2020  ents = 0.       
+00009820: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+00009830: 696c 655f 6576 656e 745f 636f 756e 7465  ile_event_counte
+00009840: 7220 3d20 300a 2020 2020 2020 2020 0a20  r = 0.        . 
+00009850: 2020 2020 2020 2023 206c 6f61 6420 6d65         # load me
+00009860: 7461 6461 7461 0a20 2020 2020 2020 2069  tadata.        i
+00009870: 6620 6c6f 6164 5f6d 6574 6164 6174 613a  f load_metadata:
+00009880: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00009890: 6c66 2e5f 6c6f 6164 5f6d 6574 6164 6174  lf._load_metadat
+000098a0: 6128 290a 2020 2020 2020 2020 2020 2020  a().            
+000098b0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+000098c0: 6865 636b 2065 7665 6e74 730a 2020 2020  heck events.    
+000098d0: 2020 2020 2020 2020 6966 2027 6164 635f          if 'adc_
+000098e0: 6c69 7374 2720 6e6f 7420 696e 2073 656c  list' not in sel
+000098f0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+00009900: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
+00009910: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00009920: 2757 4152 4e49 4e47 3a20 4e6f 2041 4443  'WARNING: No ADC
+00009930: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f75   information fou
+00009940: 6e64 2069 6e20 7468 6520 6669 6c65 2729  nd in the file')
+00009950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009960: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
+00009970: 2020 2020 2066 6f72 2061 6463 5f6e 616d       for adc_nam
+00009980: 6520 696e 2073 656c 662e 5f63 7572 7265  e in self._curre
+00009990: 6e74 5f66 696c 655f 6d65 7461 6461 7461  nt_file_metadata
+000099a0: 5b27 6164 635f 6c69 7374 275d 3a0a 2020  ['adc_list']:.  
+000099b0: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+000099c0: 5f65 7665 6e74 735f 6164 6320 3d20 7365  _events_adc = se
+000099d0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+000099e0: 5f6d 6574 6164 6174 615b 2767 726f 7570  _metadata['group
+000099f0: 7327 5d5b 6164 635f 6e61 6d65 5d5b 276e  s'][adc_name]['n
+00009a00: 625f 6461 7461 7365 7473 275d 0a20 2020  b_datasets'].   
+00009a10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009a20: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00009a30: 6c65 5f6e 625f 6576 656e 7473 3d3d 303a  le_nb_events==0:
+00009a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a50: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+00009a60: 6e74 5f66 696c 655f 6e62 5f65 7665 6e74  nt_file_nb_event
+00009a70: 7320 3d20 6e62 5f65 7665 6e74 735f 6164  s = nb_events_ad
+00009a80: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
+00009a90: 2020 656c 6966 2073 656c 662e 5f63 7572    elif self._cur
+00009aa0: 7265 6e74 5f66 696c 655f 6e62 5f65 7665  rent_file_nb_eve
+00009ab0: 6e74 7320 213d 206e 625f 6576 656e 7473  nts != nb_events
+00009ac0: 5f61 6463 3a0a 2020 2020 2020 2020 2020  _adc:.          
+00009ad0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00009ae0: 2745 5252 4f52 3a20 496e 636f 6e73 6973  'ERROR: Inconsis
+00009af0: 7465 6e74 206e 756d 6265 7220 6f66 2065  tent number of e
+00009b00: 7665 6e74 7320 6265 7477 6565 6e20 4144  vents between AD
+00009b10: 4320 6465 7669 6365 7321 2729 0a20 2020  C devices!').   
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2073 656c 662e 5f63 6c6f 7365 5f66 696c   self._close_fil
+00009b40: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00009b50: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00009b60: 616c 7365 0a0a 2020 2020 2020 2020 7365  alse..        se
+00009b70: 6c66 2e5f 6669 6c65 5f63 6f75 6e74 6572  lf._file_counter
+00009b80: 202b 3d20 3120 0a20 2020 2020 2020 2072   += 1 .        r
+00009b90: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00009ba0: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+00009bb0: 2020 2020 2020 2020 200a 2020 2020 0a0a           .    ..
+00009bc0: 2020 2020 6465 6620 5f63 6c6f 7365 5f66      def _close_f
+00009bd0: 696c 6528 7365 6c66 293a 0a20 2020 2020  ile(self):.     
+00009be0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00009bf0: 6c6f 7365 2063 7572 7265 6e74 2066 696c  lose current fil
+00009c00: 6520 616e 6420 7265 7365 740a 2020 2020  e and reset.    
+00009c10: 2020 2020 6375 7272 656e 7420 6669 6c65      current file
+00009c20: 2070 6172 616d 6574 6572 730a 0a20 2020   parameters..   
+00009c30: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00009c40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00009c50: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00009c60: 0a20 2020 2020 2020 2052 6574 7572 6e0a  .        Return.
+00009c70: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
+00009c80: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
+00009c90: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00009ca0: 2020 6966 2073 656c 662e 5f63 7572 7265    if self._curre
+00009cb0: 6e74 5f66 696c 6520 6973 206e 6f74 204e  nt_file is not N
+00009cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009cd0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+00009ce0: 696c 652e 636c 6f73 6528 290a 2020 0a20  ile.close().  . 
+00009cf0: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
+00009d00: 697a 650a 2020 2020 2020 2020 7365 6c66  ize.        self
+00009d10: 2e5f 6375 7272 656e 745f 6669 6c65 203d  ._current_file =
+00009d20: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00009d30: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00009d40: 5f6e 616d 6520 3d20 4e6f 6e65 0a20 2020  _name = None.   
+00009d50: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+00009d60: 6e74 5f66 696c 655f 6d65 7461 6461 7461  nt_file_metadata
+00009d70: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00009d80: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00009d90: 6c65 5f6e 625f 6576 656e 7473 203d 2030  le_nb_events = 0
+00009da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009db0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00009dc0: 2020 2020 2020 0a0a 0a20 2020 2064 6566        ...    def
+00009dd0: 205f 6c6f 6164 5f6d 6574 6164 6174 6128   _load_metadata(
+00009de0: 7365 6c66 2c20 696e 636c 7564 655f 6461  self, include_da
+00009df0: 7461 7365 745f 6d65 7461 6461 7461 3d46  taset_metadata=F
+00009e00: 616c 7365 293a 0a0a 2020 2020 2020 2020  alse):..        
+00009e10: 2222 220a 2020 2020 2020 2020 4675 6e63  """.        Func
+00009e20: 7469 6f6e 2074 6f20 6c6f 6164 2061 6c6c  tion to load all
+00009e30: 206d 6574 6164 6174 6120 6672 6f6d 2063   metadata from c
+00009e40: 7572 7265 6e74 2066 696c 652e 2053 746f  urrent file. Sto
+00009e50: 7265 2069 6e20 0a20 2020 2020 2020 2061  re in .        a
+00009e60: 6e20 696e 7465 726e 616c 2064 6963 7469  n internal dicti
+00009e70: 6f6e 6172 790a 0a20 2020 2020 2020 2050  onary..        P
+00009e80: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00009e90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020    ----------..  
+00009ea0: 2020 2020 2020 696e 636c 7564 655f 6461        include_da
+00009eb0: 7461 7365 745f 6d65 7461 6461 7461 203a  taset_metadata :
+00009ec0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+00009ed0: 2020 2020 2020 2020 2020 2069 6620 5472             if Tr
+00009ee0: 7565 2c20 7265 6164 2064 6174 6173 6574  ue, read dataset
+00009ef0: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
+00009f00: 2020 2020 2044 6566 6175 6c74 3a20 4661       Default: Fa
+00009f10: 6c73 650a 0a0a 2020 2020 2020 2020 5265  lse...        Re
+00009f20: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
+00009f30: 2d2d 2d0a 2020 2020 2020 2020 0a20 2020  ---.        .   
+00009f40: 2020 2020 206d 6574 6164 6174 615f 6469       metadata_di
+00009f50: 6374 203a 2064 6963 740a 2020 2020 2020  ct : dict.      
+00009f60: 2020 2020 6469 6374 696f 6e61 7279 2077      dictionary w
+00009f70: 6974 6820 6d65 7461 6461 7461 0a20 2020  ith metadata.   
+00009f80: 2020 2020 200a 0a20 2020 2020 2020 2022       ..        "
+00009f90: 2222 0a0a 2020 2020 2020 2020 2320 6368  ""..        # ch
+00009fa0: 6563 6b20 6966 2066 696c 6520 6578 6973  eck if file exis
+00009fb0: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
+00009fc0: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
+00009fd0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00009fe0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00009ff0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000a000: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
+0000a010: 2063 6f6e 7461 696e 6e65 720a 2020 2020   containner.    
+0000a020: 2020 2020 6d65 7461 6461 7461 5f64 6963      metadata_dic
+0000a030: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0000a040: 200a 0a20 2020 2020 2020 2023 2066 696c   ..        # fil
+0000a050: 6520 6d61 7461 6461 7461 0a20 2020 2020  e matadata.     
+0000a060: 2020 206d 6574 6164 6174 615f 6469 6374     metadata_dict
+0000a070: 203d 2073 656c 662e 5f65 7874 7261 6374   = self._extract
+0000a080: 5f6d 6574 6164 6174 6128 7365 6c66 2e5f  _metadata(self._
+0000a090: 6375 7272 656e 745f 6669 6c65 2e61 7474  current_file.att
+0000a0a0: 7273 290a 2020 2020 2020 0a20 2020 200a  rs).      .    .
+0000a0b0: 2020 2020 2020 2020 2320 6772 6f75 702f          # group/
+0000a0c0: 6461 7461 7365 7420 6d65 7461 6461 7461  dataset metadata
+0000a0d0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+0000a0e0: 615f 6469 6374 5b27 6772 6f75 705f 6c69  a_dict['group_li
+0000a0f0: 7374 275d 203d 206c 6973 7428 290a 2020  st'] = list().  
+0000a100: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
+0000a110: 6963 745b 2761 6463 5f6c 6973 7427 5d20  ict['adc_list'] 
+0000a120: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
+0000a130: 206d 6574 6164 6174 615f 6469 6374 5b27   metadata_dict['
+0000a140: 6772 6f75 7073 275d 203d 2064 6963 7428  groups'] = dict(
+0000a150: 290a 2020 2020 2020 2020 2020 200a 2020  ).           .  
+0000a160: 2020 2020 2020 2320 4c6f 6f70 2067 726f        # Loop gro
+0000a170: 7570 730a 2020 2020 2020 2020 666f 7220  ups.        for 
+0000a180: 6b65 792c 2067 726f 7570 2069 6e20 7365  key, group in se
+0000a190: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+0000a1a0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0000a1b0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
+0000a1c0: 7570 6461 7465 206c 6973 740a 2020 2020  update list.    
+0000a1d0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0000a1e0: 5f64 6963 745b 2767 726f 7570 5f6c 6973  _dict['group_lis
+0000a1f0: 7427 5d2e 6170 7065 6e64 286b 6579 290a  t'].append(key).
+0000a200: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+0000a210: 6579 5b30 3a33 5d3d 3d27 6164 6327 3a0a  ey[0:3]=='adc':.
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a230: 6d65 7461 6461 7461 5f64 6963 745b 2761  metadata_dict['a
+0000a240: 6463 5f6c 6973 7427 5d2e 6170 7065 6e64  dc_list'].append
+0000a250: 286b 6579 290a 2020 2020 2020 2020 2020  (key).          
+0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a270: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+0000a280: 2020 2023 2073 6176 6520 6d65 7461 6461     # save metada
+0000a290: 7461 0a20 2020 2020 2020 2020 2020 206d  ta.            m
+0000a2a0: 6574 6164 6174 615f 6469 6374 5b27 6772  etadata_dict['gr
+0000a2b0: 6f75 7073 275d 5b6b 6579 5d20 3d20 6469  oups'][key] = di
+0000a2c0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+0000a2d0: 206d 6574 6164 6174 615f 6469 6374 5b27   metadata_dict['
+0000a2e0: 6772 6f75 7073 275d 5b6b 6579 5d20 3d20  groups'][key] = 
+0000a2f0: 2073 656c 662e 5f65 7874 7261 6374 5f6d   self._extract_m
+0000a300: 6574 6164 6174 6128 6772 6f75 702e 6174  etadata(group.at
+0000a310: 7472 7329 0a20 2020 2020 2020 200a 2020  trs).        .  
+0000a320: 2020 2020 2020 2020 2020 2320 6461 7461            # data
+0000a330: 7365 7473 0a20 2020 2020 2020 2020 2020  sets.           
+0000a340: 2064 6174 6173 6574 5f6c 6973 7420 3d20   dataset_list = 
+0000a350: 6c69 7374 2867 726f 7570 2e6b 6579 7328  list(group.keys(
+0000a360: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
+0000a370: 6574 6164 6174 615f 6469 6374 5b27 6772  etadata_dict['gr
+0000a380: 6f75 7073 275d 5b6b 6579 5d5b 2764 6174  oups'][key]['dat
+0000a390: 6173 6574 5f6c 6973 7427 5d20 3d20 6461  aset_list'] = da
+0000a3a0: 7461 7365 745f 6c69 7374 0a20 2020 2020  taset_list.     
+0000a3b0: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
+0000a3c0: 6469 6374 5b27 6772 6f75 7073 275d 5b6b  dict['groups'][k
+0000a3d0: 6579 5d5b 276e 625f 6461 7461 7365 7473  ey]['nb_datasets
+0000a3e0: 275d 203d 206c 656e 2864 6174 6173 6574  '] = len(dataset
+0000a3f0: 5f6c 6973 7429 0a20 2020 2020 2020 2020  _list).         
+0000a400: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+0000a410: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
+0000a420: 6461 7461 7365 745f 6d65 7461 6461 7461  dataset_metadata
+0000a430: 2061 6e64 206c 656e 2864 6174 6173 6574   and len(dataset
+0000a440: 5f6c 6973 7429 3e30 3a0a 2020 2020 2020  _list)>0:.      
+0000a450: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+0000a460: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000a470: 204c 6f6f 7020 6461 7461 7365 7473 2061   Loop datasets a
+0000a480: 6e64 2061 6464 206d 6574 6164 6174 610a  nd add metadata.
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 6d65 7461 6461 7461 5f64 6963 745b 2767  metadata_dict['g
+0000a4b0: 726f 7570 7327 5d5b 6b65 795d 5b27 6461  roups'][key]['da
+0000a4c0: 7461 7365 7473 275d 203d 2064 6963 7428  tasets'] = dict(
+0000a4d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a4e0: 2020 666f 7220 6461 7461 7365 745f 6b65    for dataset_ke
+0000a4f0: 792c 2064 6174 6173 6574 2069 6e20 6772  y, dataset in gr
+0000a500: 6f75 702e 6974 656d 7328 293a 0a20 2020  oup.items():.   
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 206d 6574 6164 6174 615f 6469 6374 5b27   metadata_dict['
+0000a530: 6772 6f75 7073 275d 5b6b 6579 5d5b 2764  groups'][key]['d
+0000a540: 6174 6173 6574 7327 5d5b 6461 7461 7365  atasets'][datase
+0000a550: 745f 6b65 795d 203d 2028 0a20 2020 2020  t_key] = (.     
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2073 656c 662e 5f65 7874 7261 6374     self._extract
+0000a580: 5f6d 6574 6164 6174 6128 6461 7461 7365  _metadata(datase
+0000a590: 742e 6174 7472 7329 0a20 2020 2020 2020  t.attrs).       
+0000a5a0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
+0000a5d0: 2020 2320 7361 7665 0a20 2020 2020 2020    # save.       
+0000a5e0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+0000a5f0: 696c 655f 6d65 7461 6461 7461 203d 206d  ile_metadata = m
+0000a600: 6574 6164 6174 615f 6469 6374 0a20 2020  etadata_dict.   
+0000a610: 2020 0a0a 0a0a 0a0a 0a20 2020 2064 6566    .......    def
+0000a620: 205f 6578 7472 6163 745f 6d65 7461 6461   _extract_metada
+0000a630: 7461 2873 656c 662c 2061 7474 7269 6275  ta(self, attribu
+0000a640: 7465 7329 3a0a 2020 2020 2020 2020 2222  tes):.        ""
+0000a650: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
+0000a660: 7420 6d65 7461 6461 7461 2066 726f 6d20  t metadata from 
+0000a670: 6174 7472 6962 7574 6520 6469 6374 696f  attribute dictio
+0000a680: 6e61 7279 0a20 2020 2020 2020 2022 2222  nary.        """
+0000a690: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a6a0: 2020 6d65 7461 6461 7461 5f64 6963 7420    metadata_dict 
+0000a6b0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0000a6c0: 2066 6f72 206b 6579 2c76 616c 7565 2069   for key,value i
+0000a6d0: 6e20 6174 7472 6962 7574 6573 2e69 7465  n attributes.ite
+0000a6e0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000a6f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000a700: 7661 6c75 652c 2062 7974 6573 293a 0a20  value, bytes):. 
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000a720: 616c 7565 203d 2076 616c 7565 2e64 6563  alue = value.dec
+0000a730: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+0000a740: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+0000a750: 6528 7661 6c75 652c 206e 702e 6e64 6172  e(value, np.ndar
+0000a760: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
+0000a770: 2020 2020 2020 6966 2076 616c 7565 2e64        if value.d
+0000a780: 7479 7065 203d 3d20 6e70 2e6f 626a 6563  type == np.objec
+0000a790: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000a7a0: 2020 2020 2020 2076 616c 7565 203d 2076         value = v
+0000a7b0: 616c 7565 2e61 7374 7970 6528 7374 7229  alue.astype(str)
+0000a7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a7d0: 2023 2061 2066 6577 2070 6172 7469 6375   # a few particu
+0000a7e0: 6c61 7220 6361 7365 730a 2020 2020 2020  lar cases.      
+0000a7f0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+0000a800: 203d 3d20 2772 756e 5f70 7572 706f 7365   == 'run_purpose
+0000a810: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+0000a820: 2020 2020 2020 2076 616c 7565 203d 2027         value = '
+0000a830: 2027 2e6a 6f69 6e28 6c69 7374 2876 616c   '.join(list(val
+0000a840: 7565 2929 2020 2020 2020 2020 2020 2020  ue))            
+0000a850: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000a860: 2020 2020 206d 6574 6164 6174 615f 6469       metadata_di
+0000a870: 6374 5b6b 6579 5d20 3d20 7661 6c75 650a  ct[key] = value.
+0000a880: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+0000a890: 6574 6164 6174 615f 6469 6374 0a20 2020  etadata_dict.   
+0000a8a0: 2020 2020 200a 0a20 2020 200a 2020 2020       ..    .    
+0000a8b0: 6465 6620 5f6c 6f61 645f 6576 656e 7428  def _load_event(
+0000a8c0: 7365 6c66 2c20 6576 656e 745f 696e 6465  self, event_inde
+0000a8d0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+0000a8e0: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
+0000a8f0: 6368 616e 733d 4e6f 6e65 2c0a 2020 2020  chans=None,.    
+0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a910: 6164 6374 6f76 6f6c 743d 4661 6c73 652c  adctovolt=False,
+0000a920: 2061 6463 746f 616d 703d 4661 6c73 652c   adctoamp=False,
+0000a930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a940: 2020 2020 2062 6173 656c 696e 6573 7562       baselinesub
+0000a950: 3d46 616c 7365 2c20 6261 7365 6c69 6e65  =False, baseline
+0000a960: 696e 6473 3d4e 6f6e 652c 0a20 2020 2020  inds=None,.     
+0000a970: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000a980: 6463 5f6e 616d 653d 2761 6463 3127 293a  dc_name='adc1'):
+0000a990: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a9a0: 2020 2222 220a 2020 2020 2020 2020 4c6f    """.        Lo
+0000a9b0: 6164 2074 7261 6365 7320 616e 6420 6d65  ad traces and me
+0000a9c0: 7461 6461 7461 2066 726f 6d20 6375 7272  tadata from curr
+0000a9d0: 656e 7420 6669 6c65 2020 6261 7365 6420  ent file  based 
+0000a9e0: 6f6e 0a20 2020 2020 2020 2065 7665 6e74  on.        event
+0000a9f0: 2069 6e64 6578 0a20 0a20 2020 2020 2020   index. .       
+0000aa00: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0000aa10: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000aa20: 2020 2020 2020 2065 7665 6e74 5f69 6e64         event_ind
+0000aa30: 6578 203a 2069 6e74 0a20 2020 2020 2020  ex : int.       
+0000aa40: 2020 2065 7665 6e74 2028 6864 6635 2022     event (hdf5 "
+0000aa50: 6461 7461 7365 7422 2920 206e 756d 6265  dataset")  numbe
+0000aa60: 7220 0a20 2020 2020 2020 200a 2020 2020  r .        .    
+0000aa70: 2020 2020 6465 7465 6374 6f72 5f63 6861      detector_cha
+0000aa80: 6e73 203a 2073 7472 206f 7220 6c69 7374  ns : str or list
+0000aa90: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000aaa0: 2020 2020 2064 6574 6563 746f 722f 6368       detector/ch
+0000aab0: 616e 6e65 6c20 6e61 6d65 206f 7220 6c69  annel name or li
+0000aac0: 7374 206f 6620 6465 7465 6374 6f72 732f  st of detectors/
+0000aad0: 6368 616e 6e65 6c73 0a20 2020 2020 2020  channels.       
+0000aae0: 2020 2069 6620 4e6f 6e65 2c20 6765 7420     if None, get 
+0000aaf0: 616c 6c20 6368 616e 6e65 6c73 2028 6465  all channels (de
+0000ab00: 6661 756c 7429 0a0a 2020 2020 2020 2020  fault)..        
+0000ab10: 6164 6374 6f76 6f6c 7420 3a20 626f 6f6c  adctovolt : bool
+0000ab20: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000ab30: 2020 2020 2063 6f6e 7665 7274 2066 726f       convert fro
+0000ab40: 6d20 4144 4320 746f 2076 6f6c 7473 0a20  m ADC to volts. 
+0000ab50: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+0000ab60: 3a20 4661 6c73 650a 0a20 2020 2020 2020  : False..       
+0000ab70: 2061 6463 746f 616d 7020 3a20 626f 6f6c   adctoamp : bool
+0000ab80: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000ab90: 2020 2020 2063 6f6e 7665 7274 2066 726f       convert fro
+0000aba0: 6d20 4144 4320 746f 2063 7572 7265 6e74  m ADC to current
+0000abb0: 2061 6d70 730a 2020 2020 2020 2020 2020   amps.          
+0000abc0: 6465 6661 756c 743a 2046 616c 7365 0a20  default: False. 
+0000abd0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000abe0: 2020 2020 2020 0a20 2020 2020 2020 2062        .        b
+0000abf0: 6173 656c 696e 6573 7562 3a20 626f 6f6c  aselinesub: bool
+0000ac00: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000ac10: 2020 2020 2069 6620 5472 7565 2c20 7375       if True, su
+0000ac20: 6274 7261 6374 2070 7265 2d70 756c 7365  btract pre-pulse
+0000ac30: 2062 6173 656c 696e 650a 2020 2020 2020   baseline.      
+0000ac40: 2020 2020 6465 6661 756c 743a 2046 616c      default: Fal
+0000ac50: 7365 0a0a 2020 2020 2020 2020 6261 7365  se..        base
+0000ac60: 6c69 6e65 696e 6473 3a20 7475 706c 6520  lineinds: tuple 
+0000ac70: 2869 6e74 2c20 696e 7429 206f 7220 6c69  (int, int) or li
+0000ac80: 7374 205b 696e 742c 2069 6e74 5d0a 2020  st [int, int].  
+0000ac90: 2020 2020 2020 2020 6d69 6e2f 6d61 7820          min/max 
+0000aca0: 696e 6465 7820 666f 7220 2062 6173 656c  index for  basel
+0000acb0: 696e 6520 6361 6c63 756c 6174 696f 6e20  ine calculation 
+0000acc0: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
+0000acd0: 6c74 3a20 2831 302c 2030 2e38 2a70 7265  lt: (10, 0.8*pre
+0000ace0: 7472 6967 6765 7220 6c65 6e67 7468 2929  trigger length))
+0000acf0: 0a20 2020 2020 2020 2020 200a 2020 2020  .          .    
+0000ad00: 2020 2020 6164 635f 6e61 6d65 203a 2073      adc_name : s
+0000ad10: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
+0000ad20: 2020 2020 2020 206e 616d 652f 4944 206f         name/ID o
+0000ad30: 6620 7468 6520 6164 630a 2020 2020 2020  f the adc.      
+0000ad40: 2020 2020 6465 6661 756c 743a 2022 6164      default: "ad
+0000ad50: 6331 220a 0a20 2020 2020 2020 2052 6574  c1"..        Ret
+0000ad60: 7572 6e0a 2020 2020 2020 2020 2d2d 2d2d  urn.        ----
+0000ad70: 2d2d 0a20 2020 2020 2020 200a 2020 2020  --.        .    
+0000ad80: 2020 2020 6172 7261 7920 3a20 3244 206e      array : 2D n
+0000ad90: 756d 7079 2061 7272 6179 0a20 2020 2020  umpy array.     
+0000ada0: 2020 2020 2020 7472 6163 6573 2066 6f72        traces for
+0000adb0: 2065 6163 6820 6368 616e 6e65 6c20 5b6e   each channel [n
+0000adc0: 6220 6368 616e 6e65 6c2c 206e 6220 7361  b channel, nb sa
+0000add0: 6d70 6c65 735d 0a0a 2020 2020 2020 2020  mples]..        
+0000ade0: 696e 666f 203a 2064 6963 740a 2020 2020  info : dict.    
+0000adf0: 2020 2020 2020 2066 696c 652f 6576 656e         file/even
+0000ae00: 742f 6465 7465 6374 6f72 206d 6574 6164  t/detector metad
+0000ae10: 6174 6120 2869 6620 2269 6e63 6c75 6465  ata (if "include
+0000ae20: 5f6d 6574 6164 6174 6122 203d 2054 7275  _metadata" = Tru
+0000ae30: 6529 0a0a 0a20 2020 2020 2020 200a 2020  e)...        .  
+0000ae40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+0000ae60: 2020 2020 2020 2023 2063 6865 636b 2066         # check f
+0000ae70: 696c 6520 6f70 656e 0a20 2020 2020 2020  ile open.       
+0000ae80: 2069 6620 7365 6c66 2e5f 6375 7272 656e   if self._curren
+0000ae90: 745f 6669 6c65 2069 7320 4e6f 6e65 3a0a  t_file is None:.
+0000aea0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000aeb0: 6520 5661 6c75 6545 7272 6f72 2827 4e6f  e ValueError('No
+0000aec0: 2066 696c 6520 6f70 656e 2127 290a 2020   file open!').  
+0000aed0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000aee0: 2067 6574 2064 6174 6173 6574 0a20 2020   get dataset.   
+0000aef0: 2020 2020 2064 6174 6173 6574 5f6e 616d       dataset_nam
+0000af00: 6520 3d20 2765 7665 6e74 5f27 202b 2073  e = 'event_' + s
+0000af10: 7472 2865 7665 6e74 5f69 6e64 6578 290a  tr(event_index).
+0000af20: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
+0000af30: 3d20 7365 6c66 2e5f 6375 7272 656e 745f  = self._current_
+0000af40: 6669 6c65 5b61 6463 5f6e 616d 655d 5b64  file[adc_name][d
+0000af50: 6174 6173 6574 5f6e 616d 655d 0a20 2020  ataset_name].   
+0000af60: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+0000af70: 7265 6164 2064 6174 6173 6574 0a20 2020  read dataset.   
+0000af80: 2020 2020 2064 696d 7320 3d20 6461 7461       dims = data
+0000af90: 7365 742e 7368 6170 650a 2020 2020 2020  set.shape.      
+0000afa0: 2020 7472 6163 6573 5f69 6e74 203d 206e    traces_int = n
+0000afb0: 702e 7a65 726f 7328 2864 696d 735b 305d  p.zeros((dims[0]
+0000afc0: 2c64 696d 735b 315d 292c 2064 7479 7065  ,dims[1]), dtype
+0000afd0: 3d6e 702e 696e 7431 3629 0a20 2020 2020  =np.int16).     
+0000afe0: 2020 2064 6174 6173 6574 2e72 6561 645f     dataset.read_
+0000aff0: 6469 7265 6374 2874 7261 6365 735f 696e  direct(traces_in
+0000b000: 7429 0a20 2020 2020 200a 2020 2020 2020  t).      .      
+0000b010: 2020 2320 6765 7420 6d65 7461 6461 7461    # get metadata
+0000b020: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
+0000b030: 7365 6c66 2e5f 6578 7472 6163 745f 6d65  self._extract_me
+0000b040: 7461 6461 7461 2864 6174 6173 6574 2e61  tadata(dataset.a
+0000b050: 7474 7273 290a 2020 2020 2020 2020 696e  ttrs).        in
+0000b060: 666f 2e75 7064 6174 6528 7365 6c66 2e5f  fo.update(self._
+0000b070: 6578 7472 6163 745f 6d65 7461 6461 7461  extract_metadata
+0000b080: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
+0000b090: 696c 652e 6174 7472 7329 290a 2020 2020  ile.attrs)).    
+0000b0a0: 2020 2020 696e 666f 2e75 7064 6174 6528      info.update(
+0000b0b0: 7365 6c66 2e5f 6578 7472 6163 745f 6d65  self._extract_me
+0000b0c0: 7461 6461 7461 2873 656c 662e 5f63 7572  tadata(self._cur
+0000b0d0: 7265 6e74 5f66 696c 655b 6164 635f 6e61  rent_file[adc_na
+0000b0e0: 6d65 5d2e 6174 7472 7329 290a 2020 2020  me].attrs)).    
+0000b0f0: 2020 2020 696e 666f 5b27 7265 6164 5f73      info['read_s
+0000b100: 7461 7475 7327 5d20 3d20 300a 2020 2020  tatus'] = 0.    
+0000b110: 2020 2020 696e 666f 5b27 6572 726f 725f      info['error_
+0000b120: 6d73 6727 5d20 3d20 2727 0a0a 0a20 2020  msg'] = ''...   
+0000b130: 2020 2020 2023 2065 7874 7261 6374 206c       # extract l
+0000b140: 6973 7420 6f66 2061 6463 2063 6861 6e6e  ist of adc chann
+0000b150: 656c 732c 2069 6e64 6578 2063 6f72 7265  els, index corre
+0000b160: 7370 6f6e 6420 746f 2061 7272 6179 2069  spond to array i
+0000b170: 6e64 6578 210a 2020 2020 2020 2020 6164  ndex!.        ad
+0000b180: 635f 6e75 6d73 5f66 696c 6520 3d20 696e  c_nums_file = in
+0000b190: 666f 5b27 6164 635f 6368 616e 6e65 6c5f  fo['adc_channel_
+0000b1a0: 696e 6469 6365 7327 5d0a 2020 2020 2020  indices'].      
+0000b1b0: 2020 6966 2028 6e6f 7420 6973 696e 7374    if (not isinst
+0000b1c0: 616e 6365 2861 6463 5f6e 756d 735f 6669  ance(adc_nums_fi
+0000b1d0: 6c65 2c20 6c69 7374 290a 2020 2020 2020  le, list).      
+0000b1e0: 2020 2020 2020 616e 6420 6e6f 7420 6973        and not is
+0000b1f0: 696e 7374 616e 6365 2861 6463 5f6e 756d  instance(adc_num
+0000b200: 735f 6669 6c65 2c20 6e70 2e6e 6461 7272  s_file, np.ndarr
+0000b210: 6179 2929 3a0a 2020 2020 2020 2020 2020  ay)):.          
+0000b220: 2020 6164 635f 6e75 6d73 5f66 696c 6520    adc_nums_file 
+0000b230: 3d20 6e70 2e61 7272 6179 285b 6164 635f  = np.array([adc_
+0000b240: 6e75 6d73 5f66 696c 655d 290a 2020 2020  nums_file]).    
+0000b250: 2020 2020 6e62 5f63 6861 6e6e 656c 735f      nb_channels_
+0000b260: 6669 6c65 203d 206c 656e 2861 6463 5f6e  file = len(adc_n
+0000b270: 756d 735f 6669 6c65 290a 0a0a 2020 2020  ums_file)...    
+0000b280: 2020 2020 2320 6765 7420 636f 6e6e 6563      # get connec
+0000b290: 7469 6f6e 206d 6170 2061 6e64 2063 6f6e  tion map and con
+0000b2a0: 7665 7274 2074 6f20 6e75 6d70 7920 6172  vert to numpy ar
+0000b2b0: 7261 790a 2020 2020 2020 2020 636f 6e6e  ray.        conn
+0000b2c0: 6563 7469 6f6e 7320 3d20 7365 6c66 2e67  ections = self.g
+0000b2d0: 6574 5f63 6f6e 6e65 6374 696f 6e5f 6469  et_connection_di
+0000b2e0: 6374 2861 6463 5f6e 616d 653d 6164 635f  ct(adc_name=adc_
+0000b2f0: 6e61 6d65 2c20 6d65 7461 6461 7461 3d69  name, metadata=i
+0000b300: 6e66 6f29 0a20 2020 2020 2020 2020 2020  nfo).           
+0000b310: 2020 200a 2020 2020 2020 2020 2320 4669     .        # Fi
+0000b320: 6c74 6572 2062 6173 6564 206f 6e20 6465  lter based on de
+0000b330: 7465 6374 6f72 5f63 6861 6e73 2061 7267  tector_chans arg
+0000b340: 756d 656e 740a 2020 2020 2020 2020 7365  ument.        se
+0000b350: 6c65 6374 6564 5f61 7272 6179 5f69 6e64  lected_array_ind
+0000b360: 6963 6573 203d 206c 6973 7428 290a 2020  ices = list().  
+0000b370: 2020 2020 2020 7365 6c65 6374 6564 5f61        selected_a
+0000b380: 6463 5f6e 756d 7320 3d20 6c69 7374 2829  dc_nums = list()
+0000b390: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
+0000b3a0: 645f 6465 7465 6374 6f72 5f63 6861 6e73  d_detector_chans
+0000b3b0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+0000b3c0: 2020 7365 6c65 6374 6564 5f74 6573 5f63    selected_tes_c
+0000b3d0: 6861 6e73 203d 206c 6973 7428 290a 2020  hans = list().  
+0000b3e0: 2020 2020 2020 7365 6c65 6374 6564 5f63        selected_c
+0000b3f0: 6f6e 7472 6f6c 6c65 725f 6368 616e 7320  ontroller_chans 
+0000b400: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
+0000b410: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
+0000b420: 2020 2069 6620 6465 7465 6374 6f72 5f63     if detector_c
+0000b430: 6861 6e73 2069 7320 6e6f 7420 4e6f 6e65  hans is not None
+0000b440: 3a0a 2020 2020 2020 2020 2020 2020 0a20  :.            . 
+0000b450: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
+0000b460: 7665 7274 2064 6574 6563 746f 725f 6368  vert detector_ch
+0000b470: 616e 7320 746f 206c 6973 7420 6966 206e  ans to list if n
+0000b480: 6565 6465 640a 2020 2020 2020 2020 2020  eeded.          
+0000b490: 2020 6966 2028 6e6f 7420 6973 696e 7374    if (not isinst
+0000b4a0: 616e 6365 2864 6574 6563 746f 725f 6368  ance(detector_ch
+0000b4b0: 616e 732c 206c 6973 7429 0a20 2020 2020  ans, list).     
+0000b4c0: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
+0000b4d0: 6f74 2069 7369 6e73 7461 6e63 6528 6465  ot isinstance(de
+0000b4e0: 7465 6374 6f72 5f63 6861 6e73 2c20 6e70  tector_chans, np
+0000b4f0: 2e6e 6461 7272 6179 2929 3a0a 2020 2020  .ndarray)):.    
+0000b500: 2020 2020 2020 2020 2020 2020 6465 7465              dete
+0000b510: 6374 6f72 5f63 6861 6e73 203d 205b 6465  ctor_chans = [de
+0000b520: 7465 6374 6f72 5f63 6861 6e73 5d0a 2020  tector_chans].  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2020 2020 2020 2020 0a0a 2020 2020            ..    
+0000b550: 2020 2020 2020 2020 2320 6c6f 6f70 2073          # loop s
+0000b560: 656c 6563 7465 6420 6368 616e 6e65 6c73  elected channels
+0000b570: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000b580: 2063 6861 6e20 696e 2064 6574 6563 746f   chan in detecto
+0000b590: 725f 6368 616e 733a 0a0a 2020 2020 2020  r_chans:..      
+0000b5a0: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
+0000b5b0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+0000b5c0: 2020 6966 2063 6861 6e20 6e6f 7420 696e    if chan not in
+0000b5d0: 2063 6f6e 6e65 6374 696f 6e73 5b27 6465   connections['de
+0000b5e0: 7465 6374 6f72 5f63 6861 6e73 275d 3a0a  tector_chans']:.
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000b610: 7272 6f72 2827 4465 7465 6374 6f72 2063  rror('Detector c
+0000b620: 6861 6e6e 656c 2027 202b 2063 6861 6e0a  hannel ' + chan.
+0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b650: 2020 2020 202b 2027 206e 6f74 2061 7661       + ' not ava
+0000b660: 696c 6162 6c65 2069 6e20 7261 7720 6461  ilable in raw da
+0000b670: 7461 2e27 0a20 2020 2020 2020 2020 2020  ta.'.           
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2020 2020 2020 2020 2b20 2720 4368            + ' Ch
+0000b6a0: 6563 6b20 636f 6e6e 6563 7469 6f6e 206d  eck connection m
+0000b6b0: 6170 2127 290a 2020 2020 2020 2020 2020  ap!').          
+0000b6c0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+0000b6d0: 2020 2020 2020 2023 2066 696e 6420 6368         # find ch
+0000b6e0: 616e 6e65 6c20 696e 6465 7820 696e 2063  annel index in c
+0000b6f0: 6f6e 6e65 6374 696f 6e20 6d61 700a 2020  onnection map.  
+0000b700: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000b710: 6420 3d20 636f 6e6e 6563 7469 6f6e 735b  d = connections[
+0000b720: 2764 6574 6563 746f 725f 6368 616e 7327  'detector_chans'
+0000b730: 5d2e 696e 6465 7828 6368 616e 290a 0a20  ].index(chan).. 
+0000b740: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000b750: 2065 7874 7261 6374 2073 656c 6563 7465   extract selecte
+0000b760: 6420 4144 4320 6e75 6d62 6572 0a20 2020  d ADC number.   
+0000b770: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b780: 6563 7465 645f 6164 6320 3d20 696e 7428  ected_adc = int(
+0000b790: 636f 6e6e 6563 7469 6f6e 735b 2761 6463  connections['adc
+0000b7a0: 5f63 6861 6e73 275d 5b69 6e64 5d29 0a20  _chans'][ind]). 
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b7c0: 6620 7365 6c65 6374 6564 5f61 6463 206e  f selected_adc n
+0000b7d0: 6f74 2069 6e20 6164 635f 6e75 6d73 5f66  ot in adc_nums_f
+0000b7e0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
+0000b7f0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000b800: 616c 7565 4572 726f 7228 2750 726f 626c  alueError('Probl
+0000b810: 656d 2077 6974 6820 7261 7720 6461 7461  em with raw data
+0000b820: 2e20 556e 6162 6c65 2074 6f20 6669 6e64  . Unable to find
+0000b830: 2041 4443 2063 6861 6e6e 656c 2729 0a20   ADC channel'). 
+0000b840: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2320 7361 7665 2063 6f6e 6e65 6374 696f  # save connectio
+0000b870: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
+0000b880: 2020 2073 656c 6563 7465 645f 6164 635f     selected_adc_
+0000b890: 6e75 6d73 2e61 7070 656e 6428 7365 6c65  nums.append(sele
+0000b8a0: 6374 6564 5f61 6463 290a 2020 2020 2020  cted_adc).      
+0000b8b0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000b8c0: 6564 5f64 6574 6563 746f 725f 6368 616e  ed_detector_chan
+0000b8d0: 732e 6170 7065 6e64 2863 6f6e 6e65 6374  s.append(connect
+0000b8e0: 696f 6e73 5b27 6465 7465 6374 6f72 5f63  ions['detector_c
+0000b8f0: 6861 6e73 275d 5b69 6e64 5d29 0a20 2020  hans'][ind]).   
+0000b900: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000b910: 2774 6573 5f63 6861 6e73 2720 696e 2063  'tes_chans' in c
+0000b920: 6f6e 6e65 6374 696f 6e73 3a0a 2020 2020  onnections:.    
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 7365 6c65 6374 6564 5f74 6573 5f63 6861  selected_tes_cha
+0000b950: 6e73 2e61 7070 656e 6428 636f 6e6e 6563  ns.append(connec
+0000b960: 7469 6f6e 735b 2774 6573 5f63 6861 6e73  tions['tes_chans
+0000b970: 275d 5b69 6e64 5d29 0a20 2020 2020 2020  '][ind]).       
+0000b980: 2020 2020 2020 2020 2069 6620 2763 6f6e           if 'con
+0000b990: 7472 6f6c 6c65 725f 6368 616e 7327 2069  troller_chans' i
+0000b9a0: 6e20 636f 6e6e 6563 7469 6f6e 733a 0a20  n connections:. 
+0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9c0: 2020 2073 656c 6563 7465 645f 636f 6e74     selected_cont
+0000b9d0: 726f 6c6c 6572 5f63 6861 6e73 2e61 7070  roller_chans.app
+0000b9e0: 656e 6428 636f 6e6e 6563 7469 6f6e 735b  end(connections[
+0000b9f0: 2763 6f6e 7472 6f6c 6c65 725f 6368 616e  'controller_chan
+0000ba00: 7327 5d5b 696e 645d 290a 0a20 2020 2020  s'][ind])..     
+0000ba10: 2020 2020 2020 2020 2020 2023 2073 6176             # sav
+0000ba20: 6520 6172 7261 7920 696e 6465 780a 2020  e array index.  
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000ba40: 645f 6164 6320 3d20 696e 7428 6e70 2e77  d_adc = int(np.w
+0000ba50: 6865 7265 2861 6463 5f6e 756d 735f 6669  here(adc_nums_fi
+0000ba60: 6c65 3d3d 7365 6c65 6374 6564 5f61 6463  le==selected_adc
+0000ba70: 295b 305d 290a 2020 2020 2020 2020 2020  )[0]).          
+0000ba80: 2020 2020 2020 7365 6c65 6374 6564 5f61        selected_a
+0000ba90: 7272 6179 5f69 6e64 6963 6573 2e61 7070  rray_indices.app
+0000baa0: 656e 6428 696e 645f 6164 6329 2020 2020  end(ind_adc)    
+0000bab0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000bac0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+0000bad0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000bae0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+0000baf0: 5f61 7272 6179 5f69 6e64 6963 6573 203d  _array_indices =
+0000bb00: 206c 6973 7428 7261 6e67 6528 6e62 5f63   list(range(nb_c
+0000bb10: 6861 6e6e 656c 735f 6669 6c65 2929 0a20  hannels_file)). 
+0000bb20: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+0000bb30: 7465 645f 6164 635f 6e75 6d73 203d 206c  ted_adc_nums = l
+0000bb40: 6973 7428 6164 635f 6e75 6d73 5f66 696c  ist(adc_nums_fil
+0000bb50: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
+0000bb60: 6f72 2061 6463 5f63 6861 6e20 696e 2073  or adc_chan in s
+0000bb70: 656c 6563 7465 645f 6164 635f 6e75 6d73  elected_adc_nums
+0000bb80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bb90: 2020 696e 6420 3d20 636f 6e6e 6563 7469    ind = connecti
+0000bba0: 6f6e 735b 2761 6463 5f63 6861 6e73 275d  ons['adc_chans']
+0000bbb0: 2e69 6e64 6578 2861 6463 5f63 6861 6e29  .index(adc_chan)
+0000bbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bbd0: 2073 656c 6563 7465 645f 6465 7465 6374   selected_detect
+0000bbe0: 6f72 5f63 6861 6e73 2e61 7070 656e 6428  or_chans.append(
+0000bbf0: 636f 6e6e 6563 7469 6f6e 735b 2764 6574  connections['det
+0000bc00: 6563 746f 725f 6368 616e 7327 5d5b 696e  ector_chans'][in
+0000bc10: 645d 290a 2020 2020 2020 2020 2020 2020  d]).            
+0000bc20: 2020 2020 6966 2027 7465 735f 6368 616e      if 'tes_chan
+0000bc30: 7327 2069 6e20 636f 6e6e 6563 7469 6f6e  s' in connection
+0000bc40: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000bc50: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+0000bc60: 7465 735f 6368 616e 732e 6170 7065 6e64  tes_chans.append
+0000bc70: 2863 6f6e 6e65 6374 696f 6e73 5b27 7465  (connections['te
+0000bc80: 735f 6368 616e 7327 5d5b 696e 645d 290a  s_chans'][ind]).
 0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000bcb0: 2827 5072 6f62 6c65 6d20 7769 7468 2072  ('Problem with r
-0000bcc0: 6177 2064 6174 612e 2055 6e61 626c 6520  aw data. Unable 
-0000bcd0: 746f 2066 696e 6420 4144 4320 6368 616e  to find ADC chan
-0000bce0: 6e65 6c27 290a 2020 2020 2020 2020 2020  nel').          
-0000bcf0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0000bd00: 2020 2020 2020 2023 2073 6176 6520 636f         # save co
-0000bd10: 6e6e 6563 7469 6f6e 730a 2020 2020 2020  nnections.      
-0000bd20: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-0000bd30: 6564 5f61 6463 5f6e 756d 732e 6170 7065  ed_adc_nums.appe
-0000bd40: 6e64 2873 656c 6563 7465 645f 6164 6329  nd(selected_adc)
-0000bd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bd60: 2073 656c 6563 7465 645f 6465 7465 6374   selected_detect
-0000bd70: 6f72 5f63 6861 6e73 2e61 7070 656e 6428  or_chans.append(
-0000bd80: 636f 6e6e 6563 7469 6f6e 735b 2764 6574  connections['det
-0000bd90: 6563 746f 725f 6368 616e 7327 5d5b 696e  ector_chans'][in
-0000bda0: 645d 290a 2020 2020 2020 2020 2020 2020  d]).            
-0000bdb0: 2020 2020 6966 2027 7465 735f 6368 616e      if 'tes_chan
-0000bdc0: 7327 2069 6e20 636f 6e6e 6563 7469 6f6e  s' in connection
-0000bdd0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000bde0: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-0000bdf0: 7465 735f 6368 616e 732e 6170 7065 6e64  tes_chans.append
-0000be00: 2863 6f6e 6e65 6374 696f 6e73 5b27 7465  (connections['te
-0000be10: 735f 6368 616e 7327 5d5b 696e 645d 290a  s_chans'][ind]).
-0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be30: 6966 2027 636f 6e74 726f 6c6c 6572 5f63  if 'controller_c
-0000be40: 6861 6e73 2720 696e 2063 6f6e 6e65 6374  hans' in connect
-0000be50: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-0000be60: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-0000be70: 6564 5f63 6f6e 7472 6f6c 6c65 725f 6368  ed_controller_ch
-0000be80: 616e 732e 6170 7065 6e64 2863 6f6e 6e65  ans.append(conne
-0000be90: 6374 696f 6e73 5b27 636f 6e74 726f 6c6c  ctions['controll
-0000bea0: 6572 5f63 6861 6e73 275d 5b69 6e64 5d29  er_chans'][ind])
-0000beb0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bec0: 2020 2320 7361 7665 2061 7272 6179 2069    # save array i
-0000bed0: 6e64 6578 0a20 2020 2020 2020 2020 2020  ndex.           
-0000bee0: 2020 2020 2069 6e64 5f61 6463 203d 2069       ind_adc = i
-0000bef0: 6e74 286e 702e 7768 6572 6528 6164 635f  nt(np.where(adc_
-0000bf00: 6e75 6d73 5f66 696c 653d 3d73 656c 6563  nums_file==selec
-0000bf10: 7465 645f 6164 6329 5b30 5d29 0a20 2020  ted_adc)[0]).   
-0000bf20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000bf30: 6563 7465 645f 6172 7261 795f 696e 6469  ected_array_indi
-0000bf40: 6365 732e 6170 7065 6e64 2869 6e64 5f61  ces.append(ind_a
-0000bf50: 6463 2920 2020 2020 2020 2020 2020 2020  dc)             
-0000bf60: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-0000bf70: 2020 2020 0a20 2020 2020 2020 2065 6c73      .        els
-0000bf80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000bf90: 656c 6563 7465 645f 6172 7261 795f 696e  elected_array_in
-0000bfa0: 6469 6365 7320 3d20 6c69 7374 2872 616e  dices = list(ran
-0000bfb0: 6765 286e 625f 6368 616e 6e65 6c73 5f66  ge(nb_channels_f
-0000bfc0: 696c 6529 290a 2020 2020 2020 2020 2020  ile)).          
-0000bfd0: 2020 7365 6c65 6374 6564 5f61 6463 5f6e    selected_adc_n
-0000bfe0: 756d 7320 3d20 6c69 7374 2861 6463 5f6e  ums = list(adc_n
-0000bff0: 756d 735f 6669 6c65 290a 2020 2020 2020  ums_file).      
-0000c000: 2020 2020 2020 666f 7220 6164 635f 6368        for adc_ch
-0000c010: 616e 2069 6e20 7365 6c65 6374 6564 5f61  an in selected_a
-0000c020: 6463 5f6e 756d 733a 0a20 2020 2020 2020  dc_nums:.       
-0000c030: 2020 2020 2020 2020 2069 6e64 203d 2063           ind = c
-0000c040: 6f6e 6e65 6374 696f 6e73 5b27 6164 635f  onnections['adc_
-0000c050: 6368 616e 7327 5d2e 696e 6465 7828 6164  chans'].index(ad
-0000c060: 635f 6368 616e 290a 2020 2020 2020 2020  c_chan).        
-0000c070: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-0000c080: 5f64 6574 6563 746f 725f 6368 616e 732e  _detector_chans.
-0000c090: 6170 7065 6e64 2863 6f6e 6e65 6374 696f  append(connectio
-0000c0a0: 6e73 5b27 6465 7465 6374 6f72 5f63 6861  ns['detector_cha
-0000c0b0: 6e73 275d 5b69 6e64 5d29 0a20 2020 2020  ns'][ind]).     
-0000c0c0: 2020 2020 2020 2020 2020 2069 6620 2774             if 't
-0000c0d0: 6573 5f63 6861 6e73 2720 696e 2063 6f6e  es_chans' in con
-0000c0e0: 6e65 6374 696f 6e73 3a0a 2020 2020 2020  nections:.      
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c100: 6c65 6374 6564 5f74 6573 5f63 6861 6e73  lected_tes_chans
-0000c110: 2e61 7070 656e 6428 636f 6e6e 6563 7469  .append(connecti
-0000c120: 6f6e 735b 2774 6573 5f63 6861 6e73 275d  ons['tes_chans']
-0000c130: 5b69 6e64 5d29 0a20 2020 2020 2020 2020  [ind]).         
-0000c140: 2020 2020 2020 2069 6620 2763 6f6e 7472         if 'contr
-0000c150: 6f6c 6c65 725f 6368 616e 7327 2069 6e20  oller_chans' in 
-0000c160: 636f 6e6e 6563 7469 6f6e 733a 0a20 2020  connections:.   
-0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c180: 2073 656c 6563 7465 645f 636f 6e74 726f   selected_contro
-0000c190: 6c6c 6572 5f63 6861 6e73 2e61 7070 656e  ller_chans.appen
-0000c1a0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-0000c1b0: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-0000c1c0: 6374 696f 6e73 5b27 636f 6e74 726f 6c6c  ctions['controll
-0000c1d0: 6572 5f63 6861 6e73 275d 5b69 6e64 5d0a  er_chans'][ind].
-0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1f0: 2020 2020 290a 0a0a 2020 2020 2020 2020      )...        
-0000c200: 2320 6368 6563 6b20 6e75 6d62 6572 2063  # check number c
-0000c210: 6861 6e6e 656c 730a 2020 2020 2020 2020  hannels.        
-0000c220: 6966 206e 6f74 2073 656c 6563 7465 645f  if not selected_
-0000c230: 6172 7261 795f 696e 6469 6365 7320 6f72  array_indices or
-0000c240: 206c 656e 2873 656c 6563 7465 645f 6172   len(selected_ar
-0000c250: 7261 795f 696e 6469 6365 7329 3d3d 303a  ray_indices)==0:
-0000c260: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000c270: 7365 2056 616c 7565 4572 726f 7228 2755  se ValueError('U
-0000c280: 6e61 626c 6520 746f 2066 696e 6420 7365  nable to find se
-0000c290: 6c65 6374 6564 2063 6861 6e6e 656c 2873  lected channel(s
-0000c2a0: 292e 2043 6865 636b 2063 6f6e 6e65 6374  ). Check connect
-0000c2b0: 696f 6e20 7461 626c 6521 2729 0a0a 2020  ion table!')..  
-0000c2c0: 2020 2020 2020 2320 6578 7472 6163 7420        # extract 
-0000c2d0: 6172 7261 7920 666f 7220 7365 6c65 6374  array for select
-0000c2e0: 6564 2063 6861 6e6e 656c 730a 2020 2020  ed channels.    
-0000c2f0: 2020 2020 7472 6163 6573 5f69 6e74 203d      traces_int =
-0000c300: 2074 7261 6365 735f 696e 745b 7365 6c65   traces_int[sele
-0000c310: 6374 6564 5f61 7272 6179 5f69 6e64 6963  cted_array_indic
-0000c320: 6573 2c3a 5d0a 2020 2020 2020 2020 696e  es,:].        in
-0000c330: 666f 5b27 6164 635f 6368 616e 6e65 6c5f  fo['adc_channel_
-0000c340: 696e 6469 6365 7327 5d20 3d20 7365 6c65  indices'] = sele
-0000c350: 6374 6564 5f61 6463 5f6e 756d 730a 2020  cted_adc_nums.  
-0000c360: 2020 2020 2020 696e 666f 5b27 6164 635f        info['adc_
-0000c370: 6368 616e 7327 5d20 3d20 7365 6c65 6374  chans'] = select
-0000c380: 6564 5f61 6463 5f6e 756d 730a 2020 2020  ed_adc_nums.    
-0000c390: 2020 2020 696e 666f 5b27 6465 7465 6374      info['detect
-0000c3a0: 6f72 5f63 6861 6e73 275d 203d 2073 656c  or_chans'] = sel
-0000c3b0: 6563 7465 645f 6465 7465 6374 6f72 5f63  ected_detector_c
-0000c3c0: 6861 6e73 0a20 2020 2020 2020 2069 6e66  hans.        inf
-0000c3d0: 6f5b 2774 6573 5f63 6861 6e73 275d 203d  o['tes_chans'] =
-0000c3e0: 2073 656c 6563 7465 645f 7465 735f 6368   selected_tes_ch
-0000c3f0: 616e 730a 2020 2020 2020 2020 696e 666f  ans.        info
-0000c400: 5b27 636f 6e74 726f 6c6c 6572 5f63 6861  ['controller_cha
-0000c410: 6e73 275d 203d 2073 656c 6563 7465 645f  ns'] = selected_
-0000c420: 636f 6e74 726f 6c6c 6572 5f63 6861 6e73  controller_chans
-0000c430: 0a20 2020 2020 2020 2069 6e66 6f5b 2761  .        info['a
-0000c440: 6463 5f63 6f6e 7665 7273 696f 6e5f 6661  dc_conversion_fa
-0000c450: 6374 6f72 275d 203d 2020 696e 666f 5b27  ctor'] =  info['
-0000c460: 6164 635f 636f 6e76 6572 7369 6f6e 5f66  adc_conversion_f
-0000c470: 6163 746f 7227 5d5b 7365 6c65 6374 6564  actor'][selected
-0000c480: 5f61 7272 6179 5f69 6e64 6963 6573 2c3a  _array_indices,:
-0000c490: 5d0a 2020 2020 2020 2020 696e 666f 5b27  ].        info['
-0000c4a0: 766f 6c74 6167 655f 7261 6e67 6527 5d20  voltage_range'] 
-0000c4b0: 3d20 696e 666f 5b27 766f 6c74 6167 655f  = info['voltage_
-0000c4c0: 7261 6e67 6527 5d5b 7365 6c65 6374 6564  range'][selected
-0000c4d0: 5f61 7272 6179 5f69 6e64 6963 6573 2c3a  _array_indices,:
-0000c4e0: 5d0a 0a0a 2020 2020 2020 2020 2320 6765  ]...        # ge
-0000c4f0: 7420 6465 7465 6374 6f72 2063 6f6e 6669  t detector confi
-0000c500: 670a 2020 2020 2020 2020 6465 7465 6374  g.        detect
-0000c510: 6f72 5f63 6f6e 6669 6720 3d20 7365 6c66  or_config = self
-0000c520: 2e67 6574 5f64 6574 6563 746f 725f 636f  .get_detector_co
-0000c530: 6e66 6967 2829 0a20 2020 2020 2020 2069  nfig().        i
-0000c540: 6e66 6f5b 2764 6574 6563 746f 725f 636f  nfo['detector_co
-0000c550: 6e66 6967 275d 203d 2064 6963 7428 290a  nfig'] = dict().
-0000c560: 2020 2020 2020 2020 666f 7220 6465 7420          for det 
-0000c570: 696e 2069 6e66 6f5b 2764 6574 6563 746f  in info['detecto
-0000c580: 725f 6368 616e 7327 5d3a 0a20 2020 2020  r_chans']:.     
-0000c590: 2020 2020 2020 2069 6e66 6f5b 2764 6574         info['det
-0000c5a0: 6563 746f 725f 636f 6e66 6967 275d 5b64  ector_config'][d
-0000c5b0: 6574 5d20 3d20 6465 7465 6374 6f72 5f63  et] = detector_c
-0000c5c0: 6f6e 6669 675b 6465 745d 0a20 2020 2020  onfig[det].     
-0000c5d0: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-0000c5e0: 2020 2020 2023 2063 6f6e 7665 7274 2074       # convert t
-0000c5f0: 6f20 766f 6c74 2f61 6d70 730a 2020 2020  o volt/amps.    
-0000c600: 2020 2020 7472 6163 6573 203d 205b 5d0a      traces = [].
-0000c610: 2020 2020 2020 2020 6966 2061 6463 746f          if adcto
-0000c620: 766f 6c74 206f 7220 6164 6374 6f61 6d70  volt or adctoamp
-0000c630: 3a0a 0a20 2020 2020 2020 2020 2020 2023  :..            #
-0000c640: 2069 6e69 7469 616c 697a 650a 2020 2020   initialize.    
-0000c650: 2020 2020 2020 2020 7472 6163 6573 203d          traces =
-0000c660: 206e 702e 7a65 726f 735f 6c69 6b65 2874   np.zeros_like(t
-0000c670: 7261 6365 735f 696e 742c 2064 7479 7065  races_int, dtype
-0000c680: 3d6e 702e 666c 6f61 7436 3429 0a0a 2020  =np.float64)..  
-0000c690: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
-0000c6a0: 6572 7420 746f 2076 6f6c 7473 0a20 2020  ert to volts.   
-0000c6b0: 2020 2020 2020 2020 2066 6f72 2069 6368           for ich
-0000c6c0: 616e 2069 6e20 7261 6e67 6528 7472 6163  an in range(trac
-0000c6d0: 6573 5f69 6e74 2e73 6861 7065 5b30 5d29  es_int.shape[0])
-0000c6e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c6f0: 2020 6361 6c5f 636f 6566 6620 3d20 696e    cal_coeff = in
-0000c700: 666f 5b27 6164 635f 636f 6e76 6572 7369  fo['adc_conversi
-0000c710: 6f6e 5f66 6163 746f 7227 5d5b 6963 6861  on_factor'][icha
-0000c720: 6e5d 5b3a 3a2d 315d 0a20 2020 2020 2020  n][::-1].       
-0000c730: 2020 2020 2020 2020 2070 6f6c 7920 3d20           poly = 
-0000c740: 6e70 2e70 6f6c 7931 6428 6361 6c5f 636f  np.poly1d(cal_co
-0000c750: 6566 6629 0a20 2020 2020 2020 2020 2020  eff).           
-0000c760: 2020 2020 2074 7261 6365 735b 6963 6861       traces[icha
-0000c770: 6e2c 3a5d 203d 2070 6f6c 7928 7472 6163  n,:] = poly(trac
-0000c780: 6573 5f69 6e74 5b69 6368 616e 2c3a 5d29  es_int[ichan,:])
-0000c790: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000c7a0: 636f 6e76 6572 7420 746f 2061 6d70 730a  convert to amps.
-0000c7b0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000c7c0: 6463 746f 616d 703a 0a20 2020 2020 2020  dctoamp:.       
-0000c7d0: 2020 2020 2020 2020 2069 6620 6465 7465           if dete
-0000c7e0: 6374 6f72 5f63 6f6e 6669 6720 6973 204e  ctor_config is N
-0000c7f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000c800: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0000c810: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
-0000c820: 3a20 556e 6162 6c65 2074 6f20 636f 6e76  : Unable to conv
-0000c830: 6572 7420 746f 2061 6d70 732e 2027 0a20  ert to amps. '. 
-0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c860: 2020 2020 2b20 274e 6f20 6465 7465 6374      + 'No detect
-0000c870: 6f72 2063 6f6e 6669 6720 6176 6169 6c61  or config availa
-0000c880: 626c 6521 2729 0a20 2020 2020 2020 2020  ble!').         
-0000c890: 2020 2020 2020 2066 6f72 2069 6368 616e         for ichan
-0000c8a0: 2069 6e20 7261 6e67 6528 7472 6163 6573   in range(traces
-0000c8b0: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
-0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8d0: 6465 7420 3d20 696e 666f 5b27 6465 7465  det = info['dete
-0000c8e0: 6374 6f72 5f63 6861 6e73 275d 5b69 6368  ctor_chans'][ich
-0000c8f0: 616e 5d0a 2020 2020 2020 2020 2020 2020  an].            
-0000c900: 2020 2020 2020 2020 6966 2027 636c 6f73          if 'clos
-0000c910: 655f 6c6f 6f70 5f6e 6f72 6d27 2069 6e20  e_loop_norm' in 
-0000c920: 6465 7465 6374 6f72 5f63 6f6e 6669 675b  detector_config[
-0000c930: 6465 745d 3a0a 2020 2020 2020 2020 2020  det]:.          
-0000c940: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000c950: 6163 6573 5b69 6368 616e 2c3a 5d20 3d20  aces[ichan,:] = 
-0000c960: 7472 6163 6573 5b69 6368 616e 2c3a 5d2f  traces[ichan,:]/
-0000c970: 6465 7465 6374 6f72 5f63 6f6e 6669 675b  detector_config[
-0000c980: 6465 745d 5b27 636c 6f73 655f 6c6f 6f70  det]['close_loop
-0000c990: 5f6e 6f72 6d27 5d0a 2020 2020 2020 2020  _norm'].        
-0000c9a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000c9b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c9c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000c9d0: 5661 6c75 6545 7272 6f72 2827 4552 524f  ValueError('ERRO
-0000c9e0: 523a 2055 6e61 626c 6520 746f 2063 6f6e  R: Unable to con
-0000c9f0: 7665 7274 2074 6f20 616d 7073 2e20 270a  vert to amps. '.
+0000bca0: 6966 2027 636f 6e74 726f 6c6c 6572 5f63  if 'controller_c
+0000bcb0: 6861 6e73 2720 696e 2063 6f6e 6e65 6374  hans' in connect
+0000bcc0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+0000bcd0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000bce0: 6564 5f63 6f6e 7472 6f6c 6c65 725f 6368  ed_controller_ch
+0000bcf0: 616e 732e 6170 7065 6e64 280a 2020 2020  ans.append(.    
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 2020 2020 636f 6e6e 6563 7469 6f6e 735b      connections[
+0000bd20: 2763 6f6e 7472 6f6c 6c65 725f 6368 616e  'controller_chan
+0000bd30: 7327 5d5b 696e 645d 0a20 2020 2020 2020  s'][ind].       
+0000bd40: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000bd50: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
+0000bd60: 206e 756d 6265 7220 6368 616e 6e65 6c73   number channels
+0000bd70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000bd80: 7365 6c65 6374 6564 5f61 7272 6179 5f69  selected_array_i
+0000bd90: 6e64 6963 6573 206f 7220 6c65 6e28 7365  ndices or len(se
+0000bda0: 6c65 6374 6564 5f61 7272 6179 5f69 6e64  lected_array_ind
+0000bdb0: 6963 6573 293d 3d30 3a0a 2020 2020 2020  ices)==0:.      
+0000bdc0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000bdd0: 6545 7272 6f72 2827 556e 6162 6c65 2074  eError('Unable t
+0000bde0: 6f20 6669 6e64 2073 656c 6563 7465 6420  o find selected 
+0000bdf0: 6368 616e 6e65 6c28 7329 2e20 4368 6563  channel(s). Chec
+0000be00: 6b20 636f 6e6e 6563 7469 6f6e 2074 6162  k connection tab
+0000be10: 6c65 2127 290a 0a20 2020 2020 2020 2023  le!')..        #
+0000be20: 2065 7874 7261 6374 2061 7272 6179 2066   extract array f
+0000be30: 6f72 2073 656c 6563 7465 6420 6368 616e  or selected chan
+0000be40: 6e65 6c73 0a20 2020 2020 2020 2074 7261  nels.        tra
+0000be50: 6365 735f 696e 7420 3d20 7472 6163 6573  ces_int = traces
+0000be60: 5f69 6e74 5b73 656c 6563 7465 645f 6172  _int[selected_ar
+0000be70: 7261 795f 696e 6469 6365 732c 3a5d 0a20  ray_indices,:]. 
+0000be80: 2020 2020 2020 2069 6e66 6f5b 2761 6463         info['adc
+0000be90: 5f63 6861 6e6e 656c 5f69 6e64 6963 6573  _channel_indices
+0000bea0: 275d 203d 2073 656c 6563 7465 645f 6164  '] = selected_ad
+0000beb0: 635f 6e75 6d73 0a20 2020 2020 2020 2069  c_nums.        i
+0000bec0: 6e66 6f5b 2761 6463 5f63 6861 6e73 275d  nfo['adc_chans']
+0000bed0: 203d 2073 656c 6563 7465 645f 6164 635f   = selected_adc_
+0000bee0: 6e75 6d73 0a20 2020 2020 2020 2069 6e66  nums.        inf
+0000bef0: 6f5b 2764 6574 6563 746f 725f 6368 616e  o['detector_chan
+0000bf00: 7327 5d20 3d20 7365 6c65 6374 6564 5f64  s'] = selected_d
+0000bf10: 6574 6563 746f 725f 6368 616e 730a 2020  etector_chans.  
+0000bf20: 2020 2020 2020 696e 666f 5b27 7465 735f        info['tes_
+0000bf30: 6368 616e 7327 5d20 3d20 7365 6c65 6374  chans'] = select
+0000bf40: 6564 5f74 6573 5f63 6861 6e73 0a20 2020  ed_tes_chans.   
+0000bf50: 2020 2020 2069 6e66 6f5b 2763 6f6e 7472       info['contr
+0000bf60: 6f6c 6c65 725f 6368 616e 7327 5d20 3d20  oller_chans'] = 
+0000bf70: 7365 6c65 6374 6564 5f63 6f6e 7472 6f6c  selected_control
+0000bf80: 6c65 725f 6368 616e 730a 2020 2020 2020  ler_chans.      
+0000bf90: 2020 696e 666f 5b27 6164 635f 636f 6e76    info['adc_conv
+0000bfa0: 6572 7369 6f6e 5f66 6163 746f 7227 5d20  ersion_factor'] 
+0000bfb0: 3d20 2069 6e66 6f5b 2761 6463 5f63 6f6e  =  info['adc_con
+0000bfc0: 7665 7273 696f 6e5f 6661 6374 6f72 275d  version_factor']
+0000bfd0: 5b73 656c 6563 7465 645f 6172 7261 795f  [selected_array_
+0000bfe0: 696e 6469 6365 732c 3a5d 0a20 2020 2020  indices,:].     
+0000bff0: 2020 2069 6e66 6f5b 2776 6f6c 7461 6765     info['voltage
+0000c000: 5f72 616e 6765 275d 203d 2069 6e66 6f5b  _range'] = info[
+0000c010: 2776 6f6c 7461 6765 5f72 616e 6765 275d  'voltage_range']
+0000c020: 5b73 656c 6563 7465 645f 6172 7261 795f  [selected_array_
+0000c030: 696e 6469 6365 732c 3a5d 0a0a 0a20 2020  indices,:]...   
+0000c040: 2020 2020 2023 2067 6574 2064 6574 6563       # get detec
+0000c050: 746f 7220 636f 6e66 6967 0a20 2020 2020  tor config.     
+0000c060: 2020 2064 6574 6563 746f 725f 636f 6e66     detector_conf
+0000c070: 6967 203d 2073 656c 662e 6765 745f 6465  ig = self.get_de
+0000c080: 7465 6374 6f72 5f63 6f6e 6669 6728 290a  tector_config().
+0000c090: 2020 2020 2020 2020 696e 666f 5b27 6465          info['de
+0000c0a0: 7465 6374 6f72 5f63 6f6e 6669 6727 5d20  tector_config'] 
+0000c0b0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0000c0c0: 2066 6f72 2064 6574 2069 6e20 696e 666f   for det in info
+0000c0d0: 5b27 6465 7465 6374 6f72 5f63 6861 6e73  ['detector_chans
+0000c0e0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+0000c0f0: 696e 666f 5b27 6465 7465 6374 6f72 5f63  info['detector_c
+0000c100: 6f6e 6669 6727 5d5b 6465 745d 203d 2064  onfig'][det] = d
+0000c110: 6574 6563 746f 725f 636f 6e66 6967 5b64  etector_config[d
+0000c120: 6574 5d0a 2020 2020 2020 2020 0a20 2020  et].        .   
+0000c130: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+0000c140: 636f 6e76 6572 7420 746f 2076 6f6c 742f  convert to volt/
+0000c150: 616d 7073 0a20 2020 2020 2020 2074 7261  amps.        tra
+0000c160: 6365 7320 3d20 5b5d 0a20 2020 2020 2020  ces = [].       
+0000c170: 2069 6620 6164 6374 6f76 6f6c 7420 6f72   if adctovolt or
+0000c180: 2061 6463 746f 616d 703a 0a0a 2020 2020   adctoamp:..    
+0000c190: 2020 2020 2020 2020 2320 696e 6974 6961          # initia
+0000c1a0: 6c69 7a65 0a20 2020 2020 2020 2020 2020  lize.           
+0000c1b0: 2074 7261 6365 7320 3d20 6e70 2e7a 6572   traces = np.zer
+0000c1c0: 6f73 5f6c 696b 6528 7472 6163 6573 5f69  os_like(traces_i
+0000c1d0: 6e74 2c20 6474 7970 653d 6e70 2e66 6c6f  nt, dtype=np.flo
+0000c1e0: 6174 3634 290a 0a20 2020 2020 2020 2020  at64)..         
+0000c1f0: 2020 2023 2063 6f6e 7665 7274 2074 6f20     # convert to 
+0000c200: 766f 6c74 730a 2020 2020 2020 2020 2020  volts.          
+0000c210: 2020 666f 7220 6963 6861 6e20 696e 2072    for ichan in r
+0000c220: 616e 6765 2874 7261 6365 735f 696e 742e  ange(traces_int.
+0000c230: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
+0000c240: 2020 2020 2020 2020 2020 2063 616c 5f63             cal_c
+0000c250: 6f65 6666 203d 2069 6e66 6f5b 2761 6463  oeff = info['adc
+0000c260: 5f63 6f6e 7665 7273 696f 6e5f 6661 6374  _conversion_fact
+0000c270: 6f72 275d 5b69 6368 616e 5d5b 3a3a 2d31  or'][ichan][::-1
+0000c280: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000c290: 2020 706f 6c79 203d 206e 702e 706f 6c79    poly = np.poly
+0000c2a0: 3164 2863 616c 5f63 6f65 6666 290a 2020  1d(cal_coeff).  
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000c2c0: 6163 6573 5b69 6368 616e 2c3a 5d20 3d20  aces[ichan,:] = 
+0000c2d0: 706f 6c79 2874 7261 6365 735f 696e 745b  poly(traces_int[
+0000c2e0: 6963 6861 6e2c 3a5d 290a 0a20 2020 2020  ichan,:])..     
+0000c2f0: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
+0000c300: 2074 6f20 616d 7073 0a20 2020 2020 2020   to amps.       
+0000c310: 2020 2020 2069 6620 6164 6374 6f61 6d70       if adctoamp
+0000c320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c330: 2020 6966 2064 6574 6563 746f 725f 636f    if detector_co
+0000c340: 6e66 6967 2069 7320 4e6f 6e65 3a0a 2020  nfig is None:.  
+0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c360: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000c370: 6f72 2827 4552 524f 523a 2055 6e61 626c  or('ERROR: Unabl
+0000c380: 6520 746f 2063 6f6e 7665 7274 2074 6f20  e to convert to 
+0000c390: 616d 7073 2e20 270a 2020 2020 2020 2020  amps. '.        
+0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3b0: 2020 2020 2020 2020 2020 2020 202b 2027               + '
+0000c3c0: 4e6f 2064 6574 6563 746f 7220 636f 6e66  No detector conf
+0000c3d0: 6967 2061 7661 696c 6162 6c65 2127 290a  ig available!').
+0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3f0: 666f 7220 6963 6861 6e20 696e 2072 616e  for ichan in ran
+0000c400: 6765 2874 7261 6365 732e 7368 6170 655b  ge(traces.shape[
+0000c410: 305d 293a 0a20 2020 2020 2020 2020 2020  0]):.           
+0000c420: 2020 2020 2020 2020 2064 6574 203d 2069           det = i
+0000c430: 6e66 6f5b 2764 6574 6563 746f 725f 6368  nfo['detector_ch
+0000c440: 616e 7327 5d5b 6963 6861 6e5d 0a20 2020  ans'][ichan].   
+0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 2069 6620 2763 6c6f 7365 5f6c 6f6f 705f   if 'close_loop_
+0000c470: 6e6f 726d 2720 696e 2064 6574 6563 746f  norm' in detecto
+0000c480: 725f 636f 6e66 6967 5b64 6574 5d3a 0a20  r_config[det]:. 
+0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4a0: 2020 2020 2020 2074 7261 6365 735b 6963         traces[ic
+0000c4b0: 6861 6e2c 3a5d 203d 2074 7261 6365 735b  han,:] = traces[
+0000c4c0: 6963 6861 6e2c 3a5d 2f64 6574 6563 746f  ichan,:]/detecto
+0000c4d0: 725f 636f 6e66 6967 5b64 6574 5d5b 2763  r_config[det]['c
+0000c4e0: 6c6f 7365 5f6c 6f6f 705f 6e6f 726d 275d  lose_loop_norm']
+0000c4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c500: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c520: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000c530: 726f 7228 2745 5252 4f52 3a20 556e 6162  ror('ERROR: Unab
+0000c540: 6c65 2074 6f20 636f 6e76 6572 7420 746f  le to convert to
+0000c550: 2061 6d70 732e 2027 0a20 2020 2020 2020   amps. '.       
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c580: 2020 2b20 274e 6f20 6e6f 726d 616c 697a    + 'No normaliz
+0000c590: 6174 696f 6e20 6176 6169 6c61 626c 6520  ation available 
+0000c5a0: 666f 7220 2720 2b20 6465 7429 2020 2020  for ' + det)    
+0000c5b0: 2020 0a20 2020 2020 2020 2065 6c73 653a    .        else:
+0000c5c0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+0000c5d0: 6365 7320 3d20 7472 6163 6573 5f69 6e74  ces = traces_int
+0000c5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c5f0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+0000c600: 2020 0a20 2020 2020 2020 2023 2062 6173    .        # bas
+0000c610: 656c 696e 6520 7375 6274 7261 6374 0a20  eline subtract. 
+0000c620: 2020 2020 2020 2069 6620 6261 7365 6c69         if baseli
+0000c630: 6e65 7375 623a 0a20 2020 2020 2020 2020  nesub:.         
+0000c640: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+0000c650: 2320 6669 6e64 2062 6173 656c 696e 6520  # find baseline 
+0000c660: 7374 6172 742f 7374 6f70 0a20 2020 2020  start/stop.     
+0000c670: 2020 2020 2020 2062 6173 656c 696e 655f         baseline_
+0000c680: 7374 6172 7420 3d20 4e6f 6e65 0a20 2020  start = None.   
+0000c690: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
+0000c6a0: 655f 7374 6f70 203d 204e 6f6e 650a 2020  e_stop = None.  
+0000c6b0: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
+0000c6c0: 656c 696e 6569 6e64 7320 6973 206e 6f74  elineinds is not
+0000c6d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000c6e0: 2020 2020 2020 2069 6620 6c65 6e28 6261         if len(ba
+0000c6f0: 7365 6c69 6e65 696e 6473 2921 3d32 3a0a  selineinds)!=2:.
+0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c710: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000c720: 7272 6f72 2827 4552 524f 523a 2062 6173  rror('ERROR: bas
+0000c730: 656c 696e 6569 6e64 7320 7368 6f75 6c64  elineinds should
+0000c740: 2062 6520 6c69 7374 2f74 7570 6c65 206f   be list/tuple o
+0000c750: 6620 6c65 6e67 7468 2032 2729 0a20 2020  f length 2').   
+0000c760: 2020 2020 2020 2020 2020 2020 2062 6173               bas
+0000c770: 656c 696e 655f 7374 6172 7420 3d20 6261  eline_start = ba
+0000c780: 7365 6c69 6e65 696e 6473 5b30 5d0a 2020  selineinds[0].  
+0000c790: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+0000c7a0: 7365 6c69 6e65 5f73 746f 7020 3d20 2062  seline_stop =  b
+0000c7b0: 6173 656c 696e 6569 6e64 735b 315d 0a20  aselineinds[1]. 
+0000c7c0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+0000c7d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000c7e0: 2027 6e62 5f73 616d 706c 6573 5f70 7265   'nb_samples_pre
+0000c7f0: 7472 6967 6765 7227 2069 6e20 696e 666f  trigger' in info
+0000c800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c810: 2020 6261 7365 6c69 6e65 5f73 7461 7274    baseline_start
+0000c820: 203d 2031 300a 2020 2020 2020 2020 2020   = 10.          
+0000c830: 2020 2020 2020 6261 7365 6c69 6e65 5f73        baseline_s
+0000c840: 746f 7020 3d20 696e 7428 726f 756e 6428  top = int(round(
+0000c850: 696e 666f 5b27 6e62 5f73 616d 706c 6573  info['nb_samples
+0000c860: 5f70 7265 7472 6967 6765 7227 5d2a 302e  _pretrigger']*0.
+0000c870: 3829 290a 0a20 2020 2020 2020 2020 2020  8))..           
+0000c880: 2069 6620 2862 6173 656c 696e 655f 7374   if (baseline_st
+0000c890: 6172 7420 6973 204e 6f6e 6520 6f72 2062  art is None or b
+0000c8a0: 6173 656c 696e 655f 7374 6f70 2069 7320  aseline_stop is 
+0000c8b0: 4e6f 6e65 206f 720a 2020 2020 2020 2020  None or.        
+0000c8c0: 2020 2020 2020 2020 6261 7365 6c69 6e65          baseline
+0000c8d0: 5f73 746f 703c 3d62 6173 656c 696e 655f  _stop<=baseline_
+0000c8e0: 7374 6172 7420 6f72 2062 6173 656c 696e  start or baselin
+0000c8f0: 655f 7374 6f70 3e3d 7472 6163 6573 2e73  e_stop>=traces.s
+0000c900: 6861 7065 5b31 5d29 3a0a 2020 2020 2020  hape[1]):.      
+0000c910: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000c920: 5661 6c75 6545 7272 6f72 2827 4552 524f  ValueError('ERRO
+0000c930: 523a 2055 6e61 626c 6520 746f 2066 696e  R: Unable to fin
+0000c940: 6420 6261 7365 6c69 6e65 2073 7461 7274  d baseline start
+0000c950: 2f73 746f 702e 2027 0a20 2020 2020 2020  /stop. '.       
+0000c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c970: 2020 2020 2020 2020 2020 2b20 2741 6464            + 'Add
+0000c980: 2061 7267 756d 656e 7420 2262 6173 656c   argument "basel
+0000c990: 696e 6569 6e64 7322 2729 0a0a 2020 2020  ineinds"')..    
+0000c9a0: 2020 2020 2020 2020 7472 6163 6573 203d          traces =
+0000c9b0: 2074 7261 6365 7320 2d20 6e70 2e6d 6561   traces - np.mea
+0000c9c0: 6e28 7472 6163 6573 5b3a 2c62 6173 656c  n(traces[:,basel
+0000c9d0: 696e 655f 7374 6172 743a 6261 7365 6c69  ine_start:baseli
+0000c9e0: 6e65 5f73 746f 705d 2c0a 2020 2020 2020  ne_stop],.      
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca20: 2020 2020 2020 2020 202b 2027 4e6f 206e           + 'No n
-0000ca30: 6f72 6d61 6c69 7a61 7469 6f6e 2061 7661  ormalization ava
-0000ca40: 696c 6162 6c65 2066 6f72 2027 202b 2064  ilable for ' + d
-0000ca50: 6574 2920 2020 2020 200a 2020 2020 2020  et)      .      
-0000ca60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ca70: 2020 2020 7472 6163 6573 203d 2074 7261      traces = tra
-0000ca80: 6365 735f 696e 740a 2020 2020 2020 2020  ces_int.        
-0000ca90: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000caa0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0000cab0: 2020 2320 6261 7365 6c69 6e65 2073 7562    # baseline sub
-0000cac0: 7472 6163 740a 2020 2020 2020 2020 6966  tract.        if
-0000cad0: 2062 6173 656c 696e 6573 7562 3a0a 2020   baselinesub:.  
-0000cae0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-0000caf0: 2020 2020 2020 2023 2066 696e 6420 6261         # find ba
-0000cb00: 7365 6c69 6e65 2073 7461 7274 2f73 746f  seline start/sto
-0000cb10: 700a 2020 2020 2020 2020 2020 2020 6261  p.            ba
-0000cb20: 7365 6c69 6e65 5f73 7461 7274 203d 204e  seline_start = N
-0000cb30: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000cb40: 6261 7365 6c69 6e65 5f73 746f 7020 3d20  baseline_stop = 
-0000cb50: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000cb60: 2069 6620 6261 7365 6c69 6e65 696e 6473   if baselineinds
-0000cb70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000cb80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000cb90: 206c 656e 2862 6173 656c 696e 6569 6e64   len(baselineind
-0000cba0: 7329 213d 323a 0a20 2020 2020 2020 2020  s)!=2:.         
-0000cbb0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000cbc0: 2056 616c 7565 4572 726f 7228 2745 5252   ValueError('ERR
-0000cbd0: 4f52 3a20 6261 7365 6c69 6e65 696e 6473  OR: baselineinds
-0000cbe0: 2073 686f 756c 6420 6265 206c 6973 742f   should be list/
-0000cbf0: 7475 706c 6520 6f66 206c 656e 6774 6820  tuple of length 
-0000cc00: 3227 290a 2020 2020 2020 2020 2020 2020  2').            
-0000cc10: 2020 2020 6261 7365 6c69 6e65 5f73 7461      baseline_sta
-0000cc20: 7274 203d 2062 6173 656c 696e 6569 6e64  rt = baselineind
-0000cc30: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
-0000cc40: 2020 2020 2062 6173 656c 696e 655f 7374       baseline_st
-0000cc50: 6f70 203d 2020 6261 7365 6c69 6e65 696e  op =  baselinein
-0000cc60: 6473 5b31 5d0a 2020 2020 2020 2020 2020  ds[1].          
-0000cc70: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0000cc80: 2020 2065 6c69 6620 276e 625f 7361 6d70     elif 'nb_samp
-0000cc90: 6c65 735f 7072 6574 7269 6767 6572 2720  les_pretrigger' 
-0000cca0: 696e 2069 6e66 6f3a 0a20 2020 2020 2020  in info:.       
-0000ccb0: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
-0000ccc0: 655f 7374 6172 7420 3d20 3130 0a20 2020  e_start = 10.   
-0000ccd0: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-0000cce0: 656c 696e 655f 7374 6f70 203d 2069 6e74  eline_stop = int
-0000ccf0: 2872 6f75 6e64 2869 6e66 6f5b 276e 625f  (round(info['nb_
-0000cd00: 7361 6d70 6c65 735f 7072 6574 7269 6767  samples_pretrigg
-0000cd10: 6572 275d 2a30 2e38 2929 0a0a 2020 2020  er']*0.8))..    
-0000cd20: 2020 2020 2020 2020 6966 2028 6261 7365          if (base
-0000cd30: 6c69 6e65 5f73 7461 7274 2069 7320 4e6f  line_start is No
-0000cd40: 6e65 206f 7220 6261 7365 6c69 6e65 5f73  ne or baseline_s
-0000cd50: 746f 7020 6973 204e 6f6e 6520 6f72 0a20  top is None or. 
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000cd70: 6173 656c 696e 655f 7374 6f70 3c3d 6261  aseline_stop<=ba
-0000cd80: 7365 6c69 6e65 5f73 7461 7274 206f 7220  seline_start or 
-0000cd90: 6261 7365 6c69 6e65 5f73 746f 703e 3d74  baseline_stop>=t
-0000cda0: 7261 6365 732e 7368 6170 655b 315d 293a  races.shape[1]):
-0000cdb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cdc0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000cdd0: 7228 2745 5252 4f52 3a20 556e 6162 6c65  r('ERROR: Unable
-0000cde0: 2074 6f20 6669 6e64 2062 6173 656c 696e   to find baselin
-0000cdf0: 6520 7374 6172 742f 7374 6f70 2e20 270a  e start/stop. '.
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce20: 202b 2027 4164 6420 6172 6775 6d65 6e74   + 'Add argument
-0000ce30: 2022 6261 7365 6c69 6e65 696e 6473 2227   "baselineinds"'
-0000ce40: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
-0000ce50: 7261 6365 7320 3d20 7472 6163 6573 202d  races = traces -
-0000ce60: 206e 702e 6d65 616e 2874 7261 6365 735b   np.mean(traces[
-0000ce70: 3a2c 6261 7365 6c69 6e65 5f73 7461 7274  :,baseline_start
-0000ce80: 3a62 6173 656c 696e 655f 7374 6f70 5d2c  :baseline_stop],
-0000ce90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ceb0: 2020 2020 2020 2061 7869 733d 2d31 2c20         axis=-1, 
-0000cec0: 6b65 6570 6469 6d73 3d54 7275 6529 0a20  keepdims=True). 
-0000ced0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000cee0: 2020 2020 0a20 2020 2020 2020 2072 6574      .        ret
-0000cef0: 7572 6e20 7472 6163 6573 2c20 696e 666f  urn traces, info
-0000cf00: 0a20 2020 2020 2020 200a 0a0a 2020 2020  .        ...    
-0000cf10: 2020 2020 0a20 2020 200a 2020 2020 2020      .    .      
-0000cf20: 2020 0a0a 0a0a 0a0a 0a0a 2020 2020 2020    ........      
-0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 2020 2020 2020 2020 0a0a 0a20 2020 200a          ...    .
-0000cf50: 636c 6173 7320 4835 5772 6974 6572 3a0a  class H5Writer:.
-0000cf60: 2020 2020 0a20 2020 2064 6566 205f 5f69      .    def __i
-0000cf70: 6e69 745f 5f28 7365 6c66 2c20 7261 6973  nit__(self, rais
-0000cf80: 655f 6572 726f 7273 3d54 7275 652c 2076  e_errors=True, v
-0000cf90: 6572 626f 7365 3d54 7275 6529 3a0a 0a0a  erbose=True):...
-0000cfa0: 2020 2020 2020 2020 7365 6c66 2e5f 7261          self._ra
-0000cfb0: 6973 655f 6572 726f 7273 203d 2072 6169  ise_errors = rai
-0000cfc0: 7365 5f65 7272 6f72 730a 2020 2020 2020  se_errors.      
-0000cfd0: 2020 7365 6c66 2e5f 7665 7262 6f73 6520    self._verbose 
-0000cfe0: 3d20 7665 7262 6f73 650a 2020 2020 2020  = verbose.      
-0000cff0: 2020 0a20 2020 2020 2020 2023 2066 696c    .        # fil
-0000d000: 6520 7061 7468 0a20 2020 2020 2020 2073  e path.        s
-0000d010: 656c 662e 5f73 6572 6965 735f 7061 7468  elf._series_path
-0000d020: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-0000d030: 2023 2073 6572 6965 730a 2020 2020 2020   # series.      
-0000d040: 2020 7365 6c66 2e5f 7365 7269 6573 5f6e    self._series_n
-0000d050: 616d 6520 3d20 4e6f 6e65 0a20 2020 2020  ame = None.     
-0000d060: 2020 2073 656c 662e 5f73 6572 6965 735f     self._series_
-0000d070: 6e75 6d20 3d20 4e6f 6e65 0a20 2020 2020  num = None.     
-0000d080: 2020 200a 2020 2020 2020 2020 2320 6375     .        # cu
-0000d090: 7272 656e 7420 6669 6c65 2069 6e66 6f0a  rrent file info.
-0000d0a0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-0000d0b0: 7272 656e 745f 6669 6c65 203d 204e 6f6e  rrent_file = Non
-0000d0c0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000d0d0: 6375 7272 656e 745f 6669 6c65 5f6e 616d  current_file_nam
-0000d0e0: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
-0000d0f0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000d100: 696c 655f 6e62 5f65 7665 6e74 7320 3d20  ile_nb_events = 
-0000d110: 300a 2020 2020 2020 2020 7365 6c66 2e5f  0.        self._
-0000d120: 6375 7272 656e 745f 6669 6c65 5f65 7665  current_file_eve
-0000d130: 6e74 5f63 6f75 6e74 6572 203d 2030 0a20  nt_counter = 0. 
-0000d140: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
-0000d150: 7265 6e74 5f66 696c 655f 6164 635f 6772  rent_file_adc_gr
-0000d160: 6f75 7020 3d20 4e6f 6e65 0a20 2020 2020  oup = None.     
-0000d170: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000d180: 5f66 696c 655f 6465 7463 6f6e 6669 675f  _file_detconfig_
-0000d190: 6772 6f75 7020 3d20 4e6f 6e65 0a20 2020  group = None.   
-0000d1a0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-0000d1b0: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
-0000d1c0: 2073 656c 662e 5f66 696c 655f 6d65 7461   self._file_meta
-0000d1d0: 6461 7461 203d 204e 6f6e 650a 2020 2020  data = None.    
-0000d1e0: 2020 2020 7365 6c66 2e5f 6465 7465 6374      self._detect
-0000d1f0: 6f72 5f63 6f6e 6669 6720 3d20 4e6f 6e65  or_config = None
-0000d200: 0a20 2020 2020 2020 2073 656c 662e 5f61  .        self._a
-0000d210: 6463 5f63 6f6e 6669 6720 203d 204e 6f6e  dc_config  = Non
-0000d220: 650a 0a20 2020 2020 2020 200a 2020 2020  e..        .    
-0000d230: 2020 2020 2320 6576 656e 7420 636f 756e      # event coun
-0000d240: 7465 720a 2020 2020 2020 2020 7365 6c66  ter.        self
-0000d250: 2e5f 676c 6f62 616c 5f65 7665 6e74 5f63  ._global_event_c
-0000d260: 6f75 6e74 6572 203d 2030 0a20 2020 2020  ounter = 0.     
-0000d270: 2020 2020 0a20 2020 2020 2020 2023 2066      .        # f
-0000d280: 696c 6520 636f 756e 7465 720a 2020 2020  ile counter.    
-0000d290: 2020 2020 7365 6c66 2e5f 6669 6c65 5f63      self._file_c
-0000d2a0: 6f75 6e74 6572 203d 2030 0a0a 2020 2020  ounter = 0..    
-0000d2b0: 2020 2020 2320 6d61 7820 6576 656e 7420      # max event 
-0000d2c0: 7065 7220 6475 6d70 0a20 2020 2020 2020  per dump.       
-0000d2d0: 2073 656c 662e 5f6e 625f 6576 656e 7473   self._nb_events
-0000d2e0: 5f70 6572 5f64 756d 705f 6d61 7820 3d20  _per_dump_max = 
-0000d2f0: 3130 3030 0a20 2020 2020 2020 2073 656c  1000.        sel
-0000d300: 662e 5f61 6463 5f6e 616d 6520 3d20 2761  f._adc_name = 'a
-0000d310: 6463 3127 0a0a 0a20 2020 2064 6566 2069  dc1'...    def i
-0000d320: 6e69 7469 616c 697a 6528 7365 6c66 2c20  nitialize(self, 
-0000d330: 7365 7269 6573 5f6e 616d 652c 2064 6174  series_name, dat
-0000d340: 615f 7061 7468 3d27 2e2f 2729 3a0a 2020  a_path='./'):.  
-0000d350: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d360: 2020 496e 6974 6961 6c69 7a65 206e 6577    Initialize new
-0000d370: 2077 7269 7469 6e67 0a20 2020 2020 2020   writing.       
-0000d380: 2022 2222 0a20 2020 2020 2020 200a 2020   """.        .  
-0000d390: 2020 2020 2020 2320 636c 6561 7220 6576        # clear ev
-0000d3a0: 6572 7974 6869 6e67 0a20 2020 2020 2020  erything.       
-0000d3b0: 2073 656c 662e 636c 6561 7228 290a 2020   self.clear().  
-0000d3c0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-0000d3d0: 2073 6572 6965 7320 6e61 6d65 200a 2020   series name .  
-0000d3e0: 2020 2020 2020 7365 6c66 2e5f 7365 7269        self._seri
-0000d3f0: 6573 5f6e 616d 6520 3d20 7365 7269 6573  es_name = series
-0000d400: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-0000d410: 6c66 2e5f 7365 7269 6573 5f6e 756d 203d  lf._series_num =
-0000d420: 2065 7874 7261 6374 5f73 6572 6965 735f   extract_series_
-0000d430: 6e75 6d28 7365 7269 6573 5f6e 616d 6529  num(series_name)
-0000d440: 0a20 2020 2020 2020 200a 0a0a 2020 2020  .        ...    
-0000d450: 2020 2020 2320 6372 6561 7465 206e 6577      # create new
-0000d460: 2064 6972 6563 746f 7279 0a20 2020 2020   directory.     
-0000d470: 2020 2023 7365 6c66 2e5f 7365 7269 6573     #self._series
-0000d480: 5f70 6174 6820 3d20 6461 7461 5f70 6174  _path = data_pat
-0000d490: 6820 2b20 272f 2720 2b20 7365 7269 6573  h + '/' + series
-0000d4a0: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-0000d4b0: 6c66 2e5f 7365 7269 6573 5f70 6174 6820  lf._series_path 
-0000d4c0: 3d20 6461 7461 5f70 6174 680a 2020 2020  = data_path.    
-0000d4d0: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
-0000d4e0: 6e6f 7420 6f73 2e70 6174 682e 6973 6469  not os.path.isdi
-0000d4f0: 7228 7365 6c66 2e5f 7365 7269 6573 5f70  r(self._series_p
-0000d500: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
-0000d510: 2020 6f73 2e6d 6b64 6972 2873 656c 662e    os.mkdir(self.
-0000d520: 5f73 6572 6965 735f 7061 7468 290a 2020  _series_path).  
-0000d530: 2020 2020 2020 2020 2020 6f73 2e63 686d            os.chm
-0000d540: 6f64 2873 656c 662e 5f73 6572 6965 735f  od(self._series_
-0000d550: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
-0000d560: 2020 2020 2020 2020 2020 2073 7461 742e             stat.
-0000d570: 535f 4952 5758 4720 7c20 7374 6174 2e53  S_IRWXG | stat.S
-0000d580: 5f49 5257 5855 207c 2073 7461 742e 535f  _IRWXU | stat.S_
-0000d590: 4952 4f54 4820 7c20 7374 6174 2e53 5f49  IROTH | stat.S_I
-0000d5a0: 584f 5448 290a 0a0a 2020 2020 6465 6620  XOTH)...    def 
-0000d5b0: 7365 745f 6d65 7461 6461 7461 2873 656c  set_metadata(sel
-0000d5c0: 662c 2066 696c 655f 6d65 7461 6461 7461  f, file_metadata
-0000d5d0: 3d4e 6f6e 652c 2061 6463 5f63 6f6e 6669  =None, adc_confi
-0000d5e0: 673d 4e6f 6e65 2c20 6465 7465 6374 6f72  g=None, detector
-0000d5f0: 5f63 6f6e 6669 673d 4e6f 6e65 293a 0a20  _config=None):. 
-0000d600: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d610: 2020 2053 6574 206d 6574 6164 6174 6120     Set metadata 
-0000d620: 7768 6963 6820 7769 6c6c 2062 6520 7772  which will be wr
-0000d630: 6974 7465 6e20 2069 6e20 6561 6368 2066  itten  in each f
-0000d640: 696c 6573 0a20 2020 2020 2020 2066 696c  iles.        fil
-0000d650: 655f 6d65 7461 6461 7461 203d 2067 656e  e_metadata = gen
-0000d660: 6572 616c 2064 6174 6120 7461 6b69 6e67  eral data taking
-0000d670: 2069 6e66 6f72 6d61 7469 6f6e 2028 6669   information (fi
-0000d680: 6c65 206c 6576 656c 206d 6574 6164 6174  le level metadat
-0000d690: 6129 0a20 2020 2020 2020 2061 6463 5f63  a).        adc_c
-0000d6a0: 6f6e 6669 6720 3d20 6164 6320 636f 6e66  onfig = adc conf
-0000d6b0: 6967 7572 6174 696f 6e20 2867 726f 7570  iguration (group
-0000d6c0: 206c 6576 656c 206d 6574 6164 6174 6129   level metadata)
-0000d6d0: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
-0000d6e0: 725f 636f 6e66 6967 203d 2064 6574 6563  r_config = detec
-0000d6f0: 746f 7220 7365 7474 696e 6773 2028 6772  tor settings (gr
-0000d700: 6f75 7020 6c65 7665 6c20 6d65 7461 6461  oup level metada
-0000d710: 7461 290a 2020 2020 2020 2020 2222 220a  ta).        """.
-0000d720: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
-0000d730: 5f6d 6574 6164 6174 6120 6973 206e 6f74  _metadata is not
-0000d740: 204e 6f6e 653a 0a20 2020 2020 2020 200a   None:.        .
-0000d750: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000d760: 7369 6e73 7461 6e63 6528 6669 6c65 5f6d  sinstance(file_m
-0000d770: 6574 6164 6174 612c 2064 6963 7429 3a0a  etadata, dict):.
-0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d790: 7365 6c66 2e5f 6669 6c65 5f6d 6574 6164  self._file_metad
-0000d7a0: 6174 6120 3d20 6669 6c65 5f6d 6574 6164  ata = file_metad
-0000d7b0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-0000d7c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000d7d0: 2020 2020 2020 7072 696e 7428 2757 4152        print('WAR
-0000d7e0: 4e49 4e47 3a20 6d65 7461 6461 7461 206e  NING: metadata n
-0000d7f0: 6565 6473 2074 6f20 6265 2061 2064 6963  eeds to be a dic
-0000d800: 7469 6f6e 6172 7927 290a 0a20 2020 2020  tionary')..     
-0000d810: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000d820: 2020 2020 6966 2061 6463 5f63 6f6e 6669      if adc_confi
-0000d830: 6720 6973 206e 6f74 204e 6f6e 653a 0a20  g is not None:. 
-0000d840: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000d850: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000d860: 7461 6e63 6528 6164 635f 636f 6e66 6967  tance(adc_config
-0000d870: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-0000d880: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-0000d890: 6463 5f63 6f6e 6669 6720 3d20 6164 635f  dc_config = adc_
-0000d8a0: 636f 6e66 6967 0a20 2020 2020 2020 2020  config.         
-0000d8b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000d8c0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-0000d8d0: 5741 524e 494e 473a 2061 6463 5f63 6f6e  WARNING: adc_con
-0000d8e0: 6669 6720 6e65 6564 7320 746f 2062 6520  fig needs to be 
-0000d8f0: 6120 6469 6374 696f 6e61 7279 2729 0a0a  a dictionary')..
-0000d900: 0a20 2020 2020 2020 2069 6620 6465 7465  .        if dete
-0000d910: 6374 6f72 5f63 6f6e 6669 6720 6973 206e  ctor_config is n
-0000d920: 6f74 204e 6f6e 653a 0a0a 2020 2020 2020  ot None:..      
-0000d930: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000d940: 6e63 6528 6465 7465 6374 6f72 5f63 6f6e  nce(detector_con
-0000d950: 6669 672c 2064 6963 7429 3a0a 2020 2020  fig, dict):.    
-0000d960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d970: 2e5f 6465 7465 6374 6f72 5f63 6f6e 6669  ._detector_confi
-0000d980: 6720 3d20 6465 7465 6374 6f72 5f63 6f6e  g = detector_con
-0000d990: 6669 670a 2020 2020 2020 2020 2020 2020  fig.            
-0000d9a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000d9b0: 2020 2020 2020 7072 696e 7428 2757 4152        print('WAR
-0000d9c0: 4e49 4e47 3a20 6465 7465 6374 6f72 2063  NING: detector c
-0000d9d0: 6f6e 6669 6720 6e65 6564 7320 746f 2062  onfig needs to b
-0000d9e0: 6520 6120 6469 6374 696f 6e61 7279 2729  e a dictionary')
-0000d9f0: 0a0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000da00: 2020 200a 0a20 2020 2020 2020 2020 2020     ..           
-0000da10: 200a 0a20 2020 2064 6566 2063 6c6f 7365   ..    def close
-0000da20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000da30: 2222 220a 2020 2020 2020 2020 636c 6f73  """.        clos
-0000da40: 6520 6375 7272 656e 7420 6669 6c65 0a20  e current file. 
-0000da50: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-0000da60: 2020 2020 7365 6c66 2e5f 636c 6f73 655f      self._close_
-0000da70: 6669 6c65 2829 0a20 2020 2020 2020 2020  file().         
-0000da80: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-0000da90: 2064 6566 2063 6c65 6172 2873 656c 6629   def clear(self)
-0000daa0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-0000dab0: 636c 6f73 655f 6669 6c65 2829 0a20 2020  close_file().   
-0000dac0: 2020 2020 2073 656c 662e 5f66 696c 655f       self._file_
-0000dad0: 636f 756e 7465 7220 3d20 300a 2020 2020  counter = 0.    
-0000dae0: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
-0000daf0: 745f 6669 6c65 203d 204e 6f6e 650a 2020  t_file = None.  
-0000db00: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
-0000db10: 656e 745f 6669 6c65 5f6e 616d 6520 3d20  ent_file_name = 
-0000db20: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000db30: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-0000db40: 6164 635f 6772 6f75 7020 3d20 4e6f 6e65  adc_group = None
-0000db50: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-0000db60: 7572 7265 6e74 5f66 696c 655f 6465 7463  urrent_file_detc
-0000db70: 6f6e 6669 675f 6772 6f75 7020 3d20 4e6f  onfig_group = No
-0000db80: 6e65 2020 2020 0a20 2020 2020 2020 2073  ne    .        s
-0000db90: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
-0000dba0: 655f 6576 656e 745f 636f 756e 7465 7220  e_event_counter 
-0000dbb0: 3d20 300a 2020 2020 2020 2020 7365 6c66  = 0.        self
-0000dbc0: 2e5f 676c 6f62 616c 5f65 7665 6e74 5f63  ._global_event_c
-0000dbd0: 6f75 6e74 6572 203d 2030 0a20 2020 2020  ounter = 0.     
-0000dbe0: 2020 2073 656c 662e 5f66 696c 655f 6d65     self._file_me
-0000dbf0: 7461 6461 7461 203d 204e 6f6e 650a 2020  tadata = None.  
-0000dc00: 2020 2020 2020 7365 6c66 2e5f 6465 7465        self._dete
-0000dc10: 6374 6f72 5f63 6f6e 6669 6720 3d20 4e6f  ctor_config = No
-0000dc20: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0000dc30: 5f61 6463 5f63 6f6e 6669 6720 3d20 4e6f  _adc_config = No
-0000dc40: 6e65 0a20 2020 2020 0a20 2020 2020 2020  ne.     .       
-0000dc50: 200a 2020 2020 6465 6620 7772 6974 655f   .    def write_
-0000dc60: 6576 656e 7428 7365 6c66 2c20 6461 7461  event(self, data
-0000dc70: 5f61 7272 6179 2c20 7072 6566 6978 3d4e  _array, prefix=N
-0000dc80: 6f6e 652c 2064 6174 6173 6574 5f6d 6574  one, dataset_met
-0000dc90: 6164 6174 613d 4e6f 6e65 2c0a 2020 2020  adata=None,.    
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcb0: 6461 7461 5f6d 6f64 653d 4e6f 6e65 2c20  data_mode=None, 
-0000dcc0: 6164 635f 6e61 6d65 3d27 6164 6331 2729  adc_name='adc1')
-0000dcd0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000dce0: 2020 2020 2020 7772 6974 6520 7075 6c73        write puls
-0000dcf0: 6520 6461 7461 2069 6e20 6669 6c65 730a  e data in files.
-0000dd00: 2020 2020 2020 2020 2222 220a 0a0a 2020          """...  
-0000dd10: 2020 2020 2020 2320 6f70 656e 2066 696c        # open fil
-0000dd20: 6520 6966 206e 6565 6465 640a 2020 2020  e if needed.    
-0000dd30: 2020 2020 6966 2028 7365 6c66 2e5f 6375      if (self._cu
-0000dd40: 7272 656e 745f 6669 6c65 2069 7320 4e6f  rrent_file is No
-0000dd50: 6e65 206f 720a 2020 2020 2020 2020 2020  ne or.          
-0000dd60: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-0000dd70: 6669 6c65 5f65 7665 6e74 5f63 6f75 6e74  file_event_count
-0000dd80: 6572 203e 3d20 7365 6c66 2e5f 6e62 5f65  er >= self._nb_e
-0000dd90: 7665 6e74 735f 7065 725f 6475 6d70 5f6d  vents_per_dump_m
-0000dda0: 6178 293a 0a20 2020 2020 2020 2020 2020  ax):.           
-0000ddb0: 2073 656c 662e 5f6f 7065 6e5f 6669 6c65   self._open_file
-0000ddc0: 2870 7265 6669 783d 7072 6566 6978 290a  (prefix=prefix).
-0000ddd0: 0a0a 2020 2020 2020 2020 2320 6576 656e  ..        # even
-0000dde0: 7420 636f 756e 7465 720a 2020 2020 2020  t counter.      
-0000ddf0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-0000de00: 6669 6c65 5f65 7665 6e74 5f63 6f75 6e74  file_event_count
-0000de10: 6572 202b 3d20 310a 2020 2020 2020 2020  er += 1.        
-0000de20: 7365 6c66 2e5f 676c 6f62 616c 5f65 7665  self._global_eve
-0000de30: 6e74 5f63 6f75 6e74 6572 202b 3d20 310a  nt_counter += 1.
-0000de40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000de50: 2023 2063 7265 6174 6520 6461 7461 7365   # create datase
-0000de60: 740a 2020 2020 2020 2020 6461 7461 7365  t.        datase
-0000de70: 745f 6e61 6d65 203d 2027 6576 656e 745f  t_name = 'event_
-0000de80: 2720 2b20 7374 7228 7365 6c66 2e5f 6375  ' + str(self._cu
-0000de90: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
-0000dea0: 5f63 6f75 6e74 6572 290a 2020 2020 2020  _counter).      
-0000deb0: 2020 6461 7461 7365 7420 3d20 7365 6c66    dataset = self
-0000dec0: 2e5f 6375 7272 656e 745f 6669 6c65 5f61  ._current_file_a
-0000ded0: 6463 5f67 726f 7570 2e63 7265 6174 655f  dc_group.create_
-0000dee0: 6461 7461 7365 7428 6461 7461 7365 745f  dataset(dataset_
-0000def0: 6e61 6d65 2c20 6461 7461 3d64 6174 615f  name, data=data_
-0000df00: 6172 7261 7929 0a20 2020 2020 200a 2020  array).      .  
-0000df10: 2020 2020 2020 2320 6164 6420 6d65 7461        # add meta
-0000df20: 6461 7461 0a20 2020 2020 2020 2069 6620  data.        if 
-0000df30: 6461 7461 7365 745f 6d65 7461 6461 7461  dataset_metadata
-0000df40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000df50: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
-0000df60: 792c 7661 6c20 696e 2064 6174 6173 6574  y,val in dataset
-0000df70: 5f6d 6574 6164 6174 612e 6974 656d 7328  _metadata.items(
-0000df80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000df90: 2020 2069 6620 2869 7369 6e73 7461 6e63     if (isinstanc
-0000dfa0: 6528 7661 6c2c 206e 702e 6e64 6172 7261  e(val, np.ndarra
-0000dfb0: 7929 2061 6e64 2076 616c 2e64 7479 7065  y) and val.dtype
-0000dfc0: 2e74 7970 6520 6973 206e 702e 7374 725f  .type is np.str_
-0000dfd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000dfe0: 2020 2020 2020 2064 7420 3d20 6835 7079         dt = h5py
-0000dff0: 2e73 7472 696e 675f 6474 7970 6528 290a  .string_dtype().
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e010: 2020 2020 7661 6c20 3d20 7661 6c2e 6173      val = val.as
-0000e020: 7479 7065 2864 7429 0a20 2020 2020 2020  type(dt).       
-0000e030: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-0000e040: 2e61 7474 7273 5b6b 6579 5d20 3d20 7661  .attrs[key] = va
-0000e050: 6c0a 0a20 2020 2020 2020 2064 6174 6173  l..        datas
-0000e060: 6574 2e61 7474 7273 5b27 6576 656e 745f  et.attrs['event_
-0000e070: 6964 275d 203d 2073 656c 662e 5f67 6c6f  id'] = self._glo
-0000e080: 6261 6c5f 6576 656e 745f 636f 756e 7465  bal_event_counte
-0000e090: 7220 0a20 2020 2020 2020 2064 6174 6173  r .        datas
-0000e0a0: 6574 2e61 7474 7273 5b27 6576 656e 745f  et.attrs['event_
-0000e0b0: 696e 6465 7827 5d20 3d20 7365 6c66 2e5f  index'] = self._
-0000e0c0: 6375 7272 656e 745f 6669 6c65 5f65 7665  current_file_eve
-0000e0d0: 6e74 5f63 6f75 6e74 6572 0a20 2020 2020  nt_counter.     
-0000e0e0: 2020 2064 6174 6173 6574 2e61 7474 7273     dataset.attrs
-0000e0f0: 5b27 6576 656e 745f 6e75 6d27 5d20 3d20  ['event_num'] = 
-0000e100: 7365 6c66 2e5f 6669 6c65 5f63 6f75 6e74  self._file_count
-0000e110: 6572 202a 3130 3030 3030 202b 2073 656c  er *100000 + sel
-0000e120: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-0000e130: 6576 656e 745f 636f 756e 7465 720a 2020  event_counter.  
-0000e140: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-0000e150: 2020 2020 2020 2023 2075 7064 6174 6520         # update 
-0000e160: 6e75 6d62 6572 206f 6620 6576 656e 7473  number of events
-0000e170: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-0000e180: 7572 7265 6e74 5f66 696c 655f 6164 635f  urrent_file_adc_
-0000e190: 6772 6f75 702e 6174 7472 735b 276e 625f  group.attrs['nb_
-0000e1a0: 6576 656e 7473 275d 203d 2073 656c 662e  events'] = self.
-0000e1b0: 5f63 7572 7265 6e74 5f66 696c 655f 6576  _current_file_ev
-0000e1c0: 656e 745f 636f 756e 7465 720a 2020 2020  ent_counter.    
-0000e1d0: 2020 2020 6966 2064 6174 615f 6d6f 6465      if data_mode
-0000e1e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e1f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e200: 6375 7272 656e 745f 6669 6c65 5f61 6463  current_file_adc
-0000e210: 5f67 726f 7570 2e61 7474 7273 5b27 6461  _group.attrs['da
-0000e220: 7461 5f6d 6f64 6527 5d20 3d20 7374 7228  ta_mode'] = str(
-0000e230: 6461 7461 5f6d 6f64 6529 0a0a 0a20 2020  data_mode)...   
-0000e240: 2020 2020 2023 2066 6c75 7368 0a20 2020       # flush.   
-0000e250: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000e260: 6e74 5f66 696c 652e 666c 7573 6828 290a  nt_file.flush().
-0000e270: 2020 2020 2020 2020 0a0a 0a0a 0a0a 2020          ......  
-0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e290: 2020 0a20 2020 2064 6566 205f 6f70 656e    .    def _open
-0000e2a0: 5f66 696c 6528 7365 6c66 2c20 7072 6566  _file(self, pref
-0000e2b0: 6978 3d4e 6f6e 6529 3a0a 2020 2020 2020  ix=None):.      
-0000e2c0: 2020 2222 220a 2020 2020 2020 2020 6f70    """.        op
-0000e2d0: 656e 2066 696c 6520 0a20 2020 2020 2020  en file .       
-0000e2e0: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
-0000e2f0: 636c 6f73 6520 6669 6c65 2069 6620 6e65  close file if ne
-0000e300: 6564 6564 0a20 2020 2020 2020 2069 6620  eded.        if 
-0000e310: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
-0000e320: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
-0000e330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e340: 2e5f 636c 6f73 655f 6669 6c65 2829 0a0a  ._close_file()..
-0000e350: 0a20 2020 2020 2020 2023 2064 756d 700a  .        # dump.
-0000e360: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
-0000e370: 6c65 5f63 6f75 6e74 6572 202b 3d31 0a20  le_counter +=1. 
-0000e380: 2020 2020 2020 2064 756d 7020 3d20 7374         dump = st
-0000e390: 7228 7365 6c66 2e5f 6669 6c65 5f63 6f75  r(self._file_cou
-0000e3a0: 6e74 6572 290a 2020 2020 2020 2020 666f  nter).        fo
-0000e3b0: 7220 7820 696e 2072 616e 6765 2831 2c35  r x in range(1,5
-0000e3c0: 2d6c 656e 2864 756d 7029 293a 0a20 2020  -len(dump)):.   
-0000e3d0: 2020 2020 2020 2020 2069 6620 783e 3d31           if x>=1
-0000e3e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e3f0: 2020 6475 6d70 203d 2027 3027 2b64 756d    dump = '0'+dum
-0000e400: 700a 0a0a 2020 2020 2020 2020 2320 6675  p...        # fu
-0000e410: 6c6c 2066 696c 6520 6e61 6d65 0a20 2020  ll file name.   
-0000e420: 2020 2020 2066 696c 655f 6e61 6d65 203d       file_name =
-0000e430: 2073 656c 662e 5f73 6572 6965 735f 7061   self._series_pa
-0000e440: 7468 202b 2027 2f27 0a20 2020 2020 2020  th + '/'.       
-0000e450: 2069 6620 7072 6566 6978 2069 7320 6e6f   if prefix is no
-0000e460: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e470: 2020 2020 6669 6c65 5f6e 616d 6520 2b3d      file_name +=
-0000e480: 2070 7265 6669 7820 2b20 275f 270a 2020   prefix + '_'.  
-0000e490: 2020 2020 2020 6669 6c65 5f6e 616d 6520        file_name 
-0000e4a0: 2b3d 2073 656c 662e 5f73 6572 6965 735f  += self._series_
-0000e4b0: 6e61 6d65 202b 2027 5f46 2720 2b20 6475  name + '_F' + du
-0000e4c0: 6d70 202b 2027 2e68 6466 3527 0a20 2020  mp + '.hdf5'.   
-0000e4d0: 2020 2020 2070 7269 6e74 2827 494e 464f       print('INFO
-0000e4e0: 3a20 4f70 656e 696e 6720 6669 6c65 206e  : Opening file n
-0000e4f0: 616d 6520 2227 202b 2066 696c 655f 6e61  ame "' + file_na
-0000e500: 6d65 202b 2027 2227 290a 2020 2020 2020  me + '"').      
-0000e510: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
-0000e520: 2020 2020 6669 6c65 203d 204e 6f6e 650a      file = None.
-0000e530: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000e540: 2020 2020 2020 2020 2066 696c 6520 3d20           file = 
-0000e550: 6835 7079 2e46 696c 6528 6669 6c65 5f6e  h5py.File(file_n
-0000e560: 616d 652c 2027 7727 290a 2020 2020 2020  ame, 'w').      
-0000e570: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-0000e580: 2020 2020 2020 7072 696e 7428 2745 5252        print('ERR
-0000e590: 4f52 3a20 556e 6162 6c65 2074 6f20 6f70  OR: Unable to op
-0000e5a0: 656e 2066 696c 6520 2720 2b20 6669 6c65  en file ' + file
-0000e5b0: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
-0000e5c0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
-0000e5d0: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000e5e0: 5f66 696c 6520 3d20 6669 6c65 0a20 2020  _file = file.   
-0000e5f0: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000e600: 6e74 5f66 696c 655f 6e61 6d65 203d 2066  nt_file_name = f
-0000e610: 696c 655f 6e61 6d65 0a20 2020 2020 2020  ile_name.       
-0000e620: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000e630: 696c 655f 6e62 5f65 7665 6e74 7320 3d20  ile_nb_events = 
-0000e640: 300a 2020 2020 2020 2020 7365 6c66 2e5f  0.        self._
-0000e650: 6375 7272 656e 745f 6669 6c65 5f65 7665  current_file_eve
-0000e660: 6e74 5f63 6f75 6e74 6572 203d 2030 0a0a  nt_counter = 0..
-0000e670: 0a20 2020 2020 2020 2023 2066 696c 6520  .        # file 
-0000e680: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
-0000e690: 2069 6620 7365 6c66 2e5f 6669 6c65 5f6d   if self._file_m
-0000e6a0: 6574 6164 6174 6120 6973 206e 6f74 204e  etadata is not N
-0000e6b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000e6c0: 2066 6f72 206b 6579 2c76 616c 2069 6e20   for key,val in 
-0000e6d0: 7365 6c66 2e5f 6669 6c65 5f6d 6574 6164  self._file_metad
-0000e6e0: 6174 612e 6974 656d 7328 293a 0a20 2020  ata.items():.   
-0000e6f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e700: 2869 7369 6e73 7461 6e63 6528 7661 6c2c  (isinstance(val,
-0000e710: 206e 702e 6e64 6172 7261 7929 2061 6e64   np.ndarray) and
-0000e720: 2076 616c 2e64 7479 7065 2e74 7970 6520   val.dtype.type 
-0000e730: 6973 206e 702e 7374 725f 293a 0a20 2020  is np.str_):.   
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2064 7420 3d20 6835 7079 2e73 7472 696e   dt = h5py.strin
-0000e760: 675f 6474 7970 6528 290a 2020 2020 2020  g_dtype().      
-0000e770: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000e780: 6c20 3d20 7661 6c2e 6173 7479 7065 2864  l = val.astype(d
-0000e790: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-0000e7a0: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000e7b0: 5f66 696c 652e 6174 7472 735b 6b65 795d  _file.attrs[key]
-0000e7c0: 203d 2076 616c 0a20 2020 2020 2020 2073   = val.        s
-0000e7d0: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
-0000e7e0: 652e 6174 7472 735b 2770 7265 6669 7827  e.attrs['prefix'
-0000e7f0: 5d20 3d20 7072 6566 6978 0a20 2020 2020  ] = prefix.     
-0000e800: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000e810: 5f66 696c 652e 6174 7472 735b 2773 6572  _file.attrs['ser
-0000e820: 6965 735f 6e75 6d27 5d20 3d20 7365 6c66  ies_num'] = self
-0000e830: 2e5f 7365 7269 6573 5f6e 756d 0a20 2020  ._series_num.   
-0000e840: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000e850: 6e74 5f66 696c 652e 6174 7472 735b 2764  nt_file.attrs['d
-0000e860: 756d 705f 6e75 6d27 5d20 3d20 696e 7428  ump_num'] = int(
-0000e870: 6475 6d70 290a 2020 2020 2020 2020 0a20  dump).        . 
-0000e880: 2020 2020 2020 2023 2064 6574 6563 746f         # detecto
-0000e890: 7220 636f 6e66 6967 0a20 2020 2020 2020  r config.       
-0000e8a0: 2069 6620 7365 6c66 2e5f 6465 7465 6374   if self._detect
-0000e8b0: 6f72 5f63 6f6e 6669 6720 6973 206e 6f74  or_config is not
-0000e8c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000e8d0: 2020 2066 6f72 2063 6f6e 6669 675f 6b65     for config_ke
-0000e8e0: 792c 636f 6e66 6967 5f76 616c 2069 6e20  y,config_val in 
-0000e8f0: 7365 6c66 2e5f 6465 7465 6374 6f72 5f63  self._detector_c
-0000e900: 6f6e 6669 672e 6974 656d 7328 293a 0a20  onfig.items():. 
-0000e910: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e920: 6620 6973 696e 7374 616e 6365 2863 6f6e  f isinstance(con
-0000e930: 6669 675f 7661 6c2c 6469 6374 293a 0a20  fig_val,dict):. 
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000e960: 5f66 696c 655f 6465 7463 6f6e 6669 675f  _file_detconfig_
-0000e970: 6772 6f75 7020 3d20 7365 6c66 2e5f 6375  group = self._cu
-0000e980: 7272 656e 745f 6669 6c65 2e63 7265 6174  rrent_file.creat
-0000e990: 655f 6772 6f75 7028 636f 6e66 6967 5f6b  e_group(config_k
-0000e9a0: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
-0000e9b0: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-0000e9c0: 7661 6c20 696e 2063 6f6e 6669 675f 7661  val in config_va
-0000e9d0: 6c2e 6974 656d 7328 293a 0a20 2020 2020  l.items():.     
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 2069 6620 2869 7369 6e73 7461 6e63     if (isinstanc
-0000ea00: 6528 7661 6c2c 206e 702e 6e64 6172 7261  e(val, np.ndarra
-0000ea10: 7929 2061 6e64 2076 616c 2e64 7479 7065  y) and val.dtype
-0000ea20: 2e74 7970 6520 6973 206e 702e 7374 725f  .type is np.str_
-0000ea30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000ea50: 7420 3d20 6835 7079 2e73 7472 696e 675f  t = h5py.string_
-0000ea60: 6474 7970 6528 290a 2020 2020 2020 2020  dtype().        
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea80: 2020 2020 7661 6c20 3d20 7661 6c2e 6173      val = val.as
-0000ea90: 7479 7065 2864 7429 0a20 2020 2020 2020  type(dt).       
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000eac0: 696c 655f 6465 7463 6f6e 6669 675f 6772  ile_detconfig_gr
-0000ead0: 6f75 702e 6174 7472 735b 6b65 795d 203d  oup.attrs[key] =
-0000eae0: 2076 616c 0a20 2020 2020 2020 200a 2020   val.        .  
-0000eaf0: 2020 2020 2020 2320 6372 6561 7465 2061        # create a
-0000eb00: 6463 2067 726f 7570 0a20 2020 2020 2020  dc group.       
-0000eb10: 2069 6620 7365 6c66 2e5f 6164 635f 636f   if self._adc_co
-0000eb20: 6e66 6967 2069 7320 6e6f 7420 4e6f 6e65  nfig is not None
-0000eb30: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000eb40: 7220 636f 6e66 6967 5f6b 6579 2c63 6f6e  r config_key,con
-0000eb50: 6669 675f 7661 6c20 696e 2073 656c 662e  fig_val in self.
-0000eb60: 5f61 6463 5f63 6f6e 6669 672e 6974 656d  _adc_config.item
-0000eb70: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-0000eb80: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000eb90: 6365 2863 6f6e 6669 675f 7661 6c2c 6469  ce(config_val,di
-0000eba0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-0000ebb0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-0000ebc0: 7572 7265 6e74 5f66 696c 655f 6164 635f  urrent_file_adc_
-0000ebd0: 6772 6f75 7020 203d 2073 656c 662e 5f63  group  = self._c
-0000ebe0: 7572 7265 6e74 5f66 696c 652e 6372 6561  urrent_file.crea
-0000ebf0: 7465 5f67 726f 7570 2863 6f6e 6669 675f  te_group(config_
-0000ec00: 6b65 7929 0a20 2020 2020 2020 2020 2020  key).           
-0000ec10: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
-0000ec20: 2c76 616c 2069 6e20 636f 6e66 6967 5f76  ,val in config_v
-0000ec30: 616c 2e69 7465 6d73 2829 3a0a 2020 2020  al.items():.    
-0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec50: 2020 2020 6966 2028 6973 696e 7374 616e      if (isinstan
-0000ec60: 6365 2876 616c 2c20 6e70 2e6e 6461 7272  ce(val, np.ndarr
-0000ec70: 6179 2920 616e 6420 7661 6c2e 6474 7970  ay) and val.dtyp
-0000ec80: 652e 7479 7065 2069 7320 6e70 2e73 7472  e.type is np.str
-0000ec90: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecb0: 6474 203d 2068 3570 792e 7374 7269 6e67  dt = h5py.string
-0000ecc0: 5f64 7479 7065 2829 0a20 2020 2020 2020  _dtype().       
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2020 2020 2076 616c 203d 2076 616c 2e61       val = val.a
-0000ecf0: 7374 7970 6528 6474 290a 2020 2020 2020  stype(dt).      
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed10: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-0000ed20: 6669 6c65 5f61 6463 5f67 726f 7570 2e61  file_adc_group.a
-0000ed30: 7474 7273 5b6b 6579 5d20 3d20 7661 6c0a  ttrs[key] = val.
-0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed60: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000ed70: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-0000ed80: 2020 6465 6620 5f63 6c6f 7365 5f66 696c    def _close_fil
-0000ed90: 6528 7365 6c66 293a 0a0a 2020 2020 2020  e(self):..      
-0000eda0: 2020 6966 2073 656c 662e 5f63 7572 7265    if self._curre
-0000edb0: 6e74 5f66 696c 6520 6973 206e 6f74 204e  nt_file is not N
-0000edc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000edd0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000ede0: 696c 652e 636c 6f73 6528 290a 2020 0a20  ile.close().  . 
-0000edf0: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
-0000ee00: 697a 650a 2020 2020 2020 2020 7365 6c66  ize.        self
-0000ee10: 2e5f 6375 7272 656e 745f 6669 6c65 203d  ._current_file =
-0000ee20: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-0000ee30: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000ee40: 5f6e 616d 6520 3d20 4e6f 6e65 0a20 2020  _name = None.   
-0000ee50: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000ee60: 6e74 5f66 696c 655f 6e62 5f65 7665 6e74  nt_file_nb_event
-0000ee70: 7320 3d20 300a 2020 2020 2020 2020 7365  s = 0.        se
-0000ee80: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000ee90: 5f61 6463 5f67 726f 7570 203d 204e 6f6e  _adc_group = Non
-0000eea0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000eeb0: 6375 7272 656e 745f 6669 6c65 5f64 6574  current_file_det
-0000eec0: 636f 6e66 6967 5f67 726f 7570 203d 204e  config_group = N
-0000eed0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000eee0: 2e5f 6375 7272 656e 745f 6669 6c65 5f65  ._current_file_e
-0000eef0: 7665 6e74 5f63 6f75 6e74 6572 203d 2030  vent_counter = 0
-0000ef00: 0a0a 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-0000ef10: 2020 2020 2020 2020 200a 0a64 6566 2067           ..def g
-0000ef20: 6574 7261 6e64 6576 656e 7473 2862 6173  etrandevents(bas
-0000ef30: 6570 6174 682c 2065 7674 6e75 6d73 2c20  epath, evtnums, 
-0000ef40: 7365 7269 6573 6e75 6d73 2c20 6375 743d  seriesnums, cut=
-0000ef50: 4e6f 6e65 2c20 6368 616e 6e65 6c73 3d4e  None, channels=N
-0000ef60: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000ef70: 2020 2020 2020 2073 756d 6368 616e 733d         sumchans=
-0000ef80: 4661 6c73 652c 206c 6763 706c 6f74 3d46  False, lgcplot=F
-0000ef90: 616c 7365 2c20 6e74 7261 6365 733d 312c  alse, ntraces=1,
-0000efa0: 206e 706c 6f74 3d32 302c 0a20 2020 2020   nplot=20,.     
-0000efb0: 2020 2020 2020 2020 2020 2020 2073 6565               see
-0000efc0: 643d 4e6f 6e65 2c20 696e 6462 6173 6570  d=None, indbasep
-0000efd0: 7265 3d4e 6f6e 6529 3a0a 2020 2020 2222  re=None):.    ""
-0000efe0: 220a 2020 2020 4675 6e63 7469 6f6e 2066  ".    Function f
-0000eff0: 6f72 206c 6f61 6469 6e67 2028 616e 6420  or loading (and 
-0000f000: 706c 6f74 7469 6e67 2920 7261 6e64 6f6d  plotting) random
-0000f010: 2065 7665 6e74 7320 6672 6f6d 2061 2064   events from a d
-0000f020: 6174 6173 6574 732e 0a20 2020 2048 6173  atasets..    Has
-0000f030: 2066 756e 6374 696f 6e61 6c69 7479 2074   functionality t
-0000f040: 6f20 7075 6c6c 2072 616e 646f 6d6c 7920  o pull randomly 
-0000f050: 6672 6f6d 2061 2073 7065 6369 6669 6564  from a specified
-0000f060: 2063 7574 2e0a 0a20 2020 2050 6172 616d   cut...    Param
-0000f070: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0000f080: 2d2d 2d2d 0a20 2020 2062 6173 6570 6174  ----.    basepat
-0000f090: 6820 3a20 7374 720a 2020 2020 2020 2020  h : str.        
-0000f0a0: 5468 6520 6261 7365 2070 6174 6820 746f  The base path to
-0000f0b0: 2074 6865 2064 6972 6563 746f 7279 2074   the directory t
-0000f0c0: 6861 7420 636f 6e74 6169 6e73 2074 6865  hat contains the
-0000f0d0: 2066 6f6c 6465 7273 2074 6861 740a 2020   folders that.  
-0000f0e0: 2020 2020 2020 7468 6520 6576 656e 7420        the event 
-0000f0f0: 6475 6d70 7320 6172 6520 696e 2e20 5468  dumps are in. Th
-0000f100: 6520 666f 6c64 6572 7320 696e 2074 6869  e folders in thi
-0000f110: 7320 6469 7265 6374 6f72 7920 7368 6f75  s directory shou
-0000f120: 6c64 2062 650a 2020 2020 2020 2020 7468  ld be.        th
-0000f130: 6520 7365 7269 6573 206e 756d 6265 7273  e series numbers
-0000f140: 2e0a 2020 2020 6576 746e 756d 7320 3a20  ..    evtnums : 
-0000f150: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
-0000f160: 2020 2041 6e20 6172 7261 7920 6f66 2061     An array of a
-0000f170: 6c6c 2065 7665 6e74 206e 756d 6265 7273  ll event numbers
-0000f180: 2066 6f72 2074 6865 2065 7665 6e74 7320   for the events 
-0000f190: 696e 2061 6c6c 2064 6174 6173 6574 732e  in all datasets.
-0000f1a0: 0a20 2020 2073 6572 6965 736e 756d 7320  .    seriesnums 
-0000f1b0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-0000f1c0: 2020 2020 2041 6e20 6172 7261 7920 6f66       An array of
-0000f1d0: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
-0000f1e0: 6e67 2073 6572 6965 7320 6e75 6d62 6572  ng series number
-0000f1f0: 7320 666f 7220 6561 6368 2065 7665 6e74  s for each event
-0000f200: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
-0000f210: 696e 2065 7674 6e75 6d73 2e0a 2020 2020  in evtnums..    
-0000f220: 6375 7420 3a20 6172 7261 795f 6c69 6b65  cut : array_like
-0000f230: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000f240: 2020 2041 2062 6f6f 6c65 616e 2061 7272     A boolean arr
-0000f250: 6179 206f 6620 7468 6520 6375 7420 7468  ay of the cut th
-0000f260: 6174 2073 686f 756c 6420 6265 2061 7070  at should be app
-0000f270: 6c69 6564 2074 6f20 7468 6520 6461 7461  lied to the data
-0000f280: 2e0a 2020 2020 2020 2020 4966 206c 6566  ..        If lef
-0000f290: 7420 6173 204e 6f6e 652c 2074 6865 6e20  t as None, then 
-0000f2a0: 6e6f 2063 7574 2069 7320 6170 706c 6965  no cut is applie
-0000f2b0: 642e 0a20 2020 2063 6861 6e6e 656c 7320  d..    channels 
-0000f2c0: 3a20 6c69 7374 2c20 6f70 7469 6f6e 616c  : list, optional
-0000f2d0: 0a20 2020 2020 2020 2041 206c 6973 7420  .        A list 
-0000f2e0: 6f66 2073 7472 696e 6773 2074 6861 7420  of strings that 
-0000f2f0: 636f 6e74 6169 6e73 2061 6c6c 206f 6620  contains all of 
-0000f300: 7468 6520 6368 616e 6e65 6c73 2074 6861  the channels tha
-0000f310: 7420 7368 6f75 6c64 0a20 2020 2020 2020  t should.       
-0000f320: 2062 6520 6c6f 6164 6564 2e20 4966 206c   be loaded. If l
-0000f330: 6566 7420 6173 204e 6f6e 652c 2061 6c6c  eft as None, all
-0000f340: 2063 6861 6e6e 656c 7320 6172 6520 6c6f   channels are lo
-0000f350: 6164 6564 2e0a 2020 2020 7375 6d63 6861  aded..    sumcha
-0000f360: 6e73 203a 2062 6f6f 6c2c 206f 7074 696f  ns : bool, optio
-0000f370: 6e61 6c0a 2020 2020 2020 2020 4120 626f  nal.        A bo
-0000f380: 6f6c 6561 6e20 666c 6167 2066 6f72 2077  olean flag for w
-0000f390: 6865 7468 6572 206f 7220 6e6f 7420 746f  hether or not to
-0000f3a0: 2073 756d 2074 6865 2063 6861 6e6e 656c   sum the channel
-0000f3b0: 7320 7768 656e 0a20 2020 2020 2020 2070  s when.        p
-0000f3c0: 6c6f 7474 696e 672e 2049 6620 4661 6c73  lotting. If Fals
-0000f3d0: 652c 2065 6163 6820 6368 616e 6e65 6c20  e, each channel 
-0000f3e0: 6973 2070 6c6f 7474 6564 2069 6e64 6976  is plotted indiv
-0000f3f0: 6964 7561 6c6c 792e 0a20 2020 2020 2020  idually..       
-0000f400: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
-0000f410: 652e 0a20 2020 206e 7472 6163 6573 203a  e..    ntraces :
-0000f420: 2069 6e74 2c20 7374 722c 206f 7074 696f   int, str, optio
-0000f430: 6e61 6c0a 2020 2020 2020 2020 5468 6520  nal.        The 
-0000f440: 6e75 6d62 6572 206f 6620 7472 6163 6573  number of traces
-0000f450: 2074 6f20 7261 6e64 6f6d 6c79 206c 6f61   to randomly loa
-0000f460: 6420 6672 6f6d 2074 6865 2064 6174 6120  d from the data 
-0000f470: 2877 6974 6820 7468 650a 2020 2020 2020  (with the.      
-0000f480: 2020 6375 742c 2069 6620 7370 6563 6966    cut, if specif
-0000f490: 6965 6429 2e20 4966 2061 6c6c 2074 7261  ied). If all tra
-0000f4a0: 6365 7320 6672 6f6d 2061 2073 7065 6366  ces from a specf
-0000f4b0: 6965 6420 6375 7420 6172 650a 2020 2020  ied cut are.    
-0000f4c0: 2020 2020 6465 7369 7265 642c 2070 6173      desired, pas
-0000f4d0: 7320 7468 6520 7374 7269 6e67 2022 616c  s the string "al
-0000f4e0: 6c22 2e20 4465 6661 756c 7420 6973 2031  l". Default is 1
-0000f4f0: 2e0a 2020 2020 6c67 6370 6c6f 7420 3a20  ..    lgcplot : 
-0000f500: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
-0000f510: 2020 2020 2020 204c 6f67 6963 616c 2066         Logical f
-0000f520: 6c61 6720 6f6e 2077 6865 7468 6572 206f  lag on whether o
-0000f530: 7220 6e6f 7420 746f 2070 6c6f 7420 7468  r not to plot th
-0000f540: 6520 7075 6c6c 6564 2074 7261 6365 732e  e pulled traces.
-0000f550: 0a20 2020 206e 706c 6f74 203a 2069 6e74  .    nplot : int
-0000f560: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000f570: 2020 2049 6620 6c67 6370 6c6f 7420 6973     If lgcplot is
-0000f580: 2054 7275 652c 2074 6865 206e 756d 6265   True, the numbe
-0000f590: 7220 6f66 2074 7261 6365 7320 746f 2070  r of traces to p
-0000f5a0: 6c6f 742e 0a20 2020 2073 6565 6420 3a20  lot..    seed : 
-0000f5b0: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-0000f5c0: 2020 2020 2020 4120 7661 6c75 6520 746f        A value to
-0000f5d0: 2070 6173 7320 746f 206e 702e 7261 6e64   pass to np.rand
-0000f5e0: 6f6d 2e73 6565 6420 6966 2074 6865 2075  om.seed if the u
-0000f5f0: 7365 7220 7769 7368 6573 2074 6f20 7573  ser wishes to us
-0000f600: 650a 2020 2020 2020 2020 7468 6520 7361  e.        the sa
-0000f610: 6d65 2072 616e 646f 6d20 7365 6564 2065  me random seed e
-0000f620: 6163 6820 7469 6d65 2067 6574 7261 6e64  ach time getrand
-0000f630: 6576 656e 7473 2069 7320 6361 6c6c 6564  events is called
-0000f640: 2e0a 2020 2020 696e 6462 6173 6570 7265  ..    indbasepre
-0000f650: 203a 204e 6f6e 6554 7970 652c 2069 6e74   : NoneType, int
-0000f660: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000f670: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
-0000f680: 2069 6e64 6963 6573 2075 7020 746f 2077   indices up to w
-0000f690: 6869 6368 2061 2074 7261 6365 2073 686f  hich a trace sho
-0000f6a0: 756c 6420 6265 2061 7665 7261 6765 6420  uld be averaged 
-0000f6b0: 746f 0a20 2020 2020 2020 2064 6574 6572  to.        deter
-0000f6c0: 6d69 6e65 2074 6865 2062 6173 656c 696e  mine the baselin
-0000f6d0: 652e 2054 6869 7320 6261 7365 6c69 6e65  e. This baseline
-0000f6e0: 2077 696c 6c20 7468 656e 2062 6520 7375   will then be su
-0000f6f0: 6274 7261 6374 6564 0a20 2020 2020 2020  btracted.       
-0000f700: 2066 726f 6d20 7468 6520 7472 6163 6573   from the traces
-0000f710: 2077 6865 6e20 706c 6f74 7469 6e67 2e20   when plotting. 
-0000f720: 4966 206c 6566 7420 6173 204e 6f6e 652c  If left as None,
-0000f730: 206e 6f20 6261 7365 6c69 6e65 0a20 2020   no baseline.   
-0000f740: 2020 2020 2073 7562 7472 6163 7469 6f6e       subtraction
-0000f750: 2077 696c 6c20 6265 2064 6f6e 652e 0a0a   will be done...
-0000f760: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000f770: 2d2d 2d2d 2d2d 2d0a 2020 2020 7420 3a20  -------.    t : 
-0000f780: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
-0000f790: 5468 6520 7469 6d65 2076 616c 7565 7320  The time values 
-0000f7a0: 666f 7220 706c 6f74 7469 6e67 2074 6865  for plotting the
-0000f7b0: 2065 7665 6e74 732e 0a20 2020 2078 203a   events..    x :
-0000f7c0: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
-0000f7d0: 2041 7272 6179 2063 6f6e 7461 696e 696e   Array containin
-0000f7e0: 6720 616c 6c20 6f66 2074 6865 2065 7665  g all of the eve
-0000f7f0: 6e74 7320 7468 6174 2077 6572 6520 7075  nts that were pu
-0000f800: 6c6c 6564 2e0a 2020 2020 6372 616e 6420  lled..    crand 
-0000f810: 3a20 6e64 6172 7261 790a 2020 2020 2020  : ndarray.      
-0000f820: 2020 426f 6f6c 6561 6e20 6172 7261 7920    Boolean array 
-0000f830: 7468 6174 2063 6f6e 7461 696e 7320 7468  that contains th
-0000f840: 6520 6375 7420 6f6e 2074 6865 206c 6f61  e cut on the loa
-0000f850: 6465 6420 6461 7461 2e0a 0a20 2020 2022  ded data...    "
-0000f860: 2222 0a0a 2020 2020 6966 2073 6565 6420  ""..    if seed 
-0000f870: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000f880: 2020 2020 206e 702e 7261 6e64 6f6d 2e73       np.random.s
-0000f890: 6565 6428 7365 6564 290a 0a20 2020 2069  eed(seed)..    i
-0000f8a0: 6620 6973 696e 7374 616e 6365 2863 6861  f isinstance(cha
-0000f8b0: 6e6e 656c 732c 2073 7472 293a 0a20 2020  nnels, str):.   
-0000f8c0: 2020 2020 2063 6861 6e6e 656c 7320 3d20       channels = 
-0000f8d0: 5b63 6861 6e6e 656c 735d 0a0a 2020 2020  [channels]..    
-0000f8e0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-0000f8f0: 6528 6576 746e 756d 732c 2070 642e 5365  e(evtnums, pd.Se
-0000f900: 7269 6573 293a 0a20 2020 2020 2020 2065  ries):.        e
-0000f910: 7674 6e75 6d73 203d 2070 642e 5365 7269  vtnums = pd.Seri
-0000f920: 6573 2864 6174 613d 6576 746e 756d 7329  es(data=evtnums)
-0000f930: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
-0000f940: 7374 616e 6365 2873 6572 6965 736e 756d  stance(seriesnum
-0000f950: 732c 2070 642e 5365 7269 6573 293a 0a20  s, pd.Series):. 
-0000f960: 2020 2020 2020 2073 6572 6965 736e 756d         seriesnum
-0000f970: 7320 3d20 7064 2e53 6572 6965 7328 6461  s = pd.Series(da
-0000f980: 7461 3d73 6572 6965 736e 756d 7329 0a0a  ta=seriesnums)..
-0000f990: 2020 2020 6966 2063 7574 2069 7320 4e6f      if cut is No
-0000f9a0: 6e65 3a0a 2020 2020 2020 2020 6375 7420  ne:.        cut 
-0000f9b0: 3d20 6e70 2e6f 6e65 7328 6c65 6e28 6576  = np.ones(len(ev
-0000f9c0: 746e 756d 7329 2c20 6474 7970 653d 626f  tnums), dtype=bo
-0000f9d0: 6f6c 290a 0a20 2020 2069 6620 6e70 2e73  ol)..    if np.s
-0000f9e0: 756d 2863 7574 2920 3d3d 2030 3a0a 2020  um(cut) == 0:.  
-0000f9f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000fa00: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-0000fa10: 2020 2020 2254 6865 2069 6e70 7574 7465      "The inputte
-0000fa20: 6420 6375 7420 6861 7320 6e6f 2065 7665  d cut has no eve
-0000fa30: 6e74 732c 2063 616e 6e6f 7420 6c6f 6164  nts, cannot load
-0000fa40: 2061 6e79 2074 7261 6365 732e 220a 2020   any traces.".  
-0000fa50: 2020 2020 2020 290a 0a20 2020 2069 6620        )..    if 
-0000fa60: 6e74 7261 6365 7320 3d3d 2027 616c 6c27  ntraces == 'all'
-0000fa70: 206f 7220 6e74 7261 6365 7320 3e20 6e70   or ntraces > np
-0000fa80: 2e73 756d 2863 7574 293a 0a20 2020 2020  .sum(cut):.     
-0000fa90: 2020 206e 7472 6163 6573 203d 206e 702e     ntraces = np.
-0000faa0: 7375 6d28 6375 7429 0a20 2020 2020 2020  sum(cut).       
-0000fab0: 2069 6620 6e74 7261 6365 7320 3e20 3130   if ntraces > 10
-0000fac0: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
-0000fad0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-0000fae0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000faf0: 596f 7520 6172 6520 6c6f 6164 696e 6720  You are loading 
-0000fb00: 6120 6c61 7267 6520 6e75 6d62 6572 206f  a large number o
-0000fb10: 6620 7472 6163 6573 2022 0a20 2020 2020  f traces ".     
-0000fb20: 2020 2020 2020 2020 2020 2066 2228 7b6e             f"({n
-0000fb30: 7472 6163 6573 7d29 2e20 4265 2063 6172  traces}). Be car
-0000fb40: 6566 756c 2077 6974 6820 796f 7572 2052  eful with your R
-0000fb50: 414d 2075 7361 6765 2e22 0a20 2020 2020  AM usage.".     
-0000fb60: 2020 2020 2020 2029 0a0a 2020 2020 696e         )..    in
-0000fb70: 6473 203d 206e 702e 7261 6e64 6f6d 2e63  ds = np.random.c
-0000fb80: 686f 6963 6528 0a20 2020 2020 2020 206e  hoice(.        n
-0000fb90: 702e 666c 6174 6e6f 6e7a 6572 6f28 6375  p.flatnonzero(cu
-0000fba0: 7429 2c0a 2020 2020 2020 2020 7369 7a65  t),.        size
-0000fbb0: 3d6e 7472 6163 6573 2c0a 2020 2020 2020  =ntraces,.      
-0000fbc0: 2020 7265 706c 6163 653d 4661 6c73 652c    replace=False,
-0000fbd0: 0a20 2020 2029 0a0a 2020 2020 6372 616e  .    )..    cran
-0000fbe0: 6420 3d20 6e70 2e7a 6572 6f73 286c 656e  d = np.zeros(len
-0000fbf0: 2865 7674 6e75 6d73 292c 2064 7479 7065  (evtnums), dtype
-0000fc00: 3d62 6f6f 6c29 0a20 2020 2063 7261 6e64  =bool).    crand
-0000fc10: 5b69 6e64 735d 203d 2054 7275 650a 0a20  [inds] = True.. 
-0000fc20: 2020 2068 355f 7265 6164 6572 203d 2048     h5_reader = H
-0000fc30: 3552 6561 6465 7228 290a 0a20 2020 2066  5Reader()..    f
-0000fc40: 6972 7374 5f66 696c 6520 3d20 736f 7274  irst_file = sort
-0000fc50: 6564 2867 6c6f 6228 6627 7b62 6173 6570  ed(glob(f'{basep
-0000fc60: 6174 687d 2f2a 2a2f 2a2e 6864 6635 272c  ath}/**/*.hdf5',
-0000fc70: 2072 6563 7572 7369 7665 3d54 7275 6529   recursive=True)
-0000fc80: 295b 305d 0a0a 2020 2020 6966 2063 6861  )[0]..    if cha
-0000fc90: 6e6e 656c 7320 6973 204e 6f6e 653a 0a20  nnels is None:. 
-0000fca0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-0000fcb0: 6e5f 6469 6374 203d 2068 355f 7265 6164  n_dict = h5_read
-0000fcc0: 6572 2e67 6574 5f63 6f6e 6e65 6374 696f  er.get_connectio
-0000fcd0: 6e5f 6469 6374 280a 2020 2020 2020 2020  n_dict(.        
-0000fce0: 2020 2020 6669 6c65 5f6e 616d 653d 6669      file_name=fi
-0000fcf0: 7273 745f 6669 6c65 2c0a 2020 2020 2020  rst_file,.      
-0000fd00: 2020 290a 2020 2020 2020 2020 6368 616e    ).        chan
-0000fd10: 6e65 6c73 203d 2063 6f6e 6e65 6374 696f  nels = connectio
-0000fd20: 6e5f 6469 6374 5b27 6465 7465 6374 6f72  n_dict['detector
-0000fd30: 5f63 6861 6e73 275d 0a0a 2020 2020 6673  _chans']..    fs
-0000fd40: 5f6c 6973 7420 3d20 5b5d 0a20 2020 206d  _list = [].    m
-0000fd50: 6574 6164 6174 6120 3d20 6835 5f72 6561  etadata = h5_rea
-0000fd60: 6465 722e 6765 745f 6d65 7461 6461 7461  der.get_metadata
-0000fd70: 2866 696c 655f 6e61 6d65 3d66 6972 7374  (file_name=first
-0000fd80: 5f66 696c 6529 0a20 2020 2066 6f72 206c  _file).    for l
-0000fd90: 6162 656c 2069 6e20 6d65 7461 6461 7461  abel in metadata
-0000fda0: 5b27 6772 6f75 705f 6c69 7374 275d 3a0a  ['group_list']:.
-0000fdb0: 2020 2020 2020 2020 6673 5f6c 6973 742e          fs_list.
-0000fdc0: 6170 7065 6e64 286d 6574 6164 6174 615b  append(metadata[
-0000fdd0: 2767 726f 7570 7327 5d5b 6c61 6265 6c5d  'groups'][label]
-0000fde0: 2e67 6574 2827 7361 6d70 6c65 5f72 6174  .get('sample_rat
-0000fdf0: 6527 2929 0a0a 2020 2020 6673 203d 206e  e'))..    fs = n
-0000fe00: 702e 756e 6971 7565 286c 6973 7428 6669  p.unique(list(fi
-0000fe10: 6c74 6572 284e 6f6e 652c 2066 735f 6c69  lter(None, fs_li
-0000fe20: 7374 2929 295b 305d 0a0a 2020 2020 6172  st)))[0]..    ar
-0000fe30: 722c 206d 6574 6164 6174 6120 3d20 6835  r, metadata = h5
-0000fe40: 5f72 6561 6465 722e 7265 6164 5f6d 616e  _reader.read_man
-0000fe50: 795f 6576 656e 7473 280a 2020 2020 2020  y_events(.      
-0000fe60: 2020 6669 6c65 7061 7468 3d67 6c6f 6228    filepath=glob(
-0000fe70: 6627 7b62 6173 6570 6174 687d 2f2a 2729  f'{basepath}/*')
-0000fe80: 2c0a 2020 2020 2020 2020 6576 656e 745f  ,.        event_
-0000fe90: 6e75 6d73 3d6e 702e 6173 6172 7261 7928  nums=np.asarray(
-0000fea0: 6576 746e 756d 735b 6375 7420 2620 6372  evtnums[cut & cr
-0000feb0: 616e 645d 292c 0a20 2020 2020 2020 2073  and]),.        s
-0000fec0: 6572 6965 735f 6e75 6d73 3d6e 702e 6173  eries_nums=np.as
-0000fed0: 6172 7261 7928 7365 7269 6573 6e75 6d73  array(seriesnums
-0000fee0: 5b63 7574 2026 2063 7261 6e64 5d29 2c0a  [cut & crand]),.
-0000fef0: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
-0000ff00: 6f72 6d61 743d 322c 0a20 2020 2020 2020  ormat=2,.       
-0000ff10: 2069 6e63 6c75 6465 5f6d 6574 6164 6174   include_metadat
-0000ff20: 613d 5472 7565 2c0a 2020 2020 2020 2020  a=True,.        
-0000ff30: 6465 7465 6374 6f72 5f63 6861 6e73 3d63  detector_chans=c
-0000ff40: 6861 6e6e 656c 732c 0a20 2020 2020 2020  hannels,.       
-0000ff50: 2061 6463 746f 616d 703d 5472 7565 2c0a   adctoamp=True,.
-0000ff60: 2020 2020 290a 0a20 2020 2069 6620 6368      )..    if ch
-0000ff70: 616e 6e65 6c73 2021 3d20 6d65 7461 6461  annels != metada
-0000ff80: 7461 5b30 5d5b 2764 6574 6563 746f 725f  ta[0]['detector_
-0000ff90: 6368 616e 7327 5d3a 0a20 2020 2020 2020  chans']:.       
-0000ffa0: 2063 6861 6e73 203d 205b 6d65 7461 6461   chans = [metada
-0000ffb0: 7461 5b30 5d5b 2764 6574 6563 746f 725f  ta[0]['detector_
-0000ffc0: 6368 616e 7327 5d2e 696e 6465 7828 6368  chans'].index(ch
-0000ffd0: 2920 666f 7220 6368 2069 6e20 6368 616e  ) for ch in chan
-0000ffe0: 6e65 6c73 5d0a 2020 2020 2020 2020 7820  nels].        x 
-0000fff0: 3d20 6172 725b 3a2c 2063 6861 6e73 5d2e  = arr[:, chans].
-00010000: 6173 7479 7065 2866 6c6f 6174 290a 2020  astype(float).  
-00010010: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00010020: 7820 3d20 6172 722e 6173 7479 7065 2866  x = arr.astype(f
-00010030: 6c6f 6174 290a 0a20 2020 2074 203d 206e  loat)..    t = n
-00010040: 702e 6172 616e 6765 2878 2e73 6861 7065  p.arange(x.shape
-00010050: 5b2d 315d 292f 6673 0a0a 2020 2020 6966  [-1])/fs..    if
-00010060: 206c 6763 706c 6f74 3a0a 2020 2020 2020   lgcplot:.      
-00010070: 2020 6966 206e 706c 6f74 3e6e 7472 6163    if nplot>ntrac
-00010080: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00010090: 6e70 6c6f 7420 3d20 6e74 7261 6365 730a  nplot = ntraces.
-000100a0: 0a20 2020 2020 2020 2066 6f72 2069 6920  .        for ii 
-000100b0: 696e 2072 616e 6765 286e 706c 6f74 293a  in range(nplot):
-000100c0: 0a0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-000100d0: 672c 2061 7820 3d20 706c 742e 7375 6270  g, ax = plt.subp
-000100e0: 6c6f 7473 2866 6967 7369 7a65 3d28 3130  lots(figsize=(10
-000100f0: 2c20 3629 290a 2020 2020 2020 2020 2020  , 6)).          
-00010100: 2020 6966 2073 756d 6368 616e 733a 0a20    if sumchans:. 
-00010110: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010120: 7261 6365 5f73 756d 203d 2078 5b69 695d  race_sum = x[ii]
-00010130: 2e73 756d 2861 7869 733d 3029 0a0a 2020  .sum(axis=0)..  
-00010140: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010150: 2069 6e64 6261 7365 7072 6520 6973 206e   indbasepre is n
-00010160: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00010170: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-00010180: 656c 696e 6520 3d20 6e70 2e6d 6561 6e28  eline = np.mean(
-00010190: 7472 6163 655f 7375 6d5b 2e2e 2e2c 203a  trace_sum[..., :
-000101a0: 696e 6462 6173 6570 7265 5d29 0a20 2020  indbasepre]).   
-000101b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000101c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000101d0: 2020 2020 2020 2062 6173 656c 696e 6520         baseline 
-000101e0: 3d20 300a 0a20 2020 2020 2020 2020 2020  = 0..           
-000101f0: 2020 2020 2061 782e 706c 6f74 2874 202a       ax.plot(t *
-00010200: 2031 6536 2c20 7472 6163 655f 7375 6d20   1e6, trace_sum 
-00010210: 2a20 3165 362c 206c 6162 656c 3d22 5375  * 1e6, label="Su
-00010220: 6d6d 6564 2043 6861 6e6e 656c 7322 290a  mmed Channels").
-00010230: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00010240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010250: 2020 636f 6c6f 7273 203d 2070 6c74 2e63    colors = plt.c
-00010260: 6d2e 7669 7269 6469 7328 0a20 2020 2020  m.viridis(.     
-00010270: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00010280: 702e 6c69 6e73 7061 6365 2830 2c20 312c  p.linspace(0, 1,
-00010290: 206e 756d 3d78 2e73 6861 7065 5b31 5d29   num=x.shape[1])
-000102a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000102b0: 2020 2020 2020 616c 7068 613d 302e 352c        alpha=0.5,
-000102c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102d0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000102e0: 2020 2066 6f72 206a 6a2c 2063 6861 6e20     for jj, chan 
-000102f0: 696e 2065 6e75 6d65 7261 7465 2863 6861  in enumerate(cha
-00010300: 6e6e 656c 7329 3a0a 2020 2020 2020 2020  nnels):.        
-00010310: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00010320: 6c20 3d20 6622 4368 616e 6e65 6c20 7b63  l = f"Channel {c
-00010330: 6861 6e7d 220a 0a20 2020 2020 2020 2020  han}"..         
-00010340: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00010350: 6462 6173 6570 7265 2069 7320 6e6f 7420  dbasepre is not 
-00010360: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010370: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00010380: 7365 6c69 6e65 203d 206e 702e 6d65 616e  seline = np.mean
-00010390: 2878 5b69 692c 206a 6a2c 203a 696e 6462  (x[ii, jj, :indb
-000103a0: 6173 6570 7265 5d29 0a20 2020 2020 2020  asepre]).       
-000103b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000103c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000103d0: 2020 2020 2020 2020 2020 2062 6173 656c             basel
-000103e0: 696e 6520 3d20 300a 0a20 2020 2020 2020  ine = 0..       
-000103f0: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
-00010400: 706c 6f74 280a 2020 2020 2020 2020 2020  plot(.          
-00010410: 2020 2020 2020 2020 2020 2020 2020 7420                t 
-00010420: 2a20 3165 362c 0a20 2020 2020 2020 2020  * 1e6,.         
-00010430: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00010440: 5b69 692c 206a 6a5d 202a 2031 6536 202d  [ii, jj] * 1e6 -
-00010450: 2062 6173 656c 696e 6520 2a20 3165 362c   baseline * 1e6,
-00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010470: 2020 2020 2020 2020 2063 6f6c 6f72 3d63           color=c
-00010480: 6f6c 6f72 735b 6a6a 5d2c 0a20 2020 2020  olors[jj],.     
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 206c 6162 656c 3d6c 6162 656c 2c0a     label=label,.
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000104d0: 2020 6178 2e67 7269 6428 290a 2020 2020    ax.grid().    
-000104e0: 2020 2020 2020 2020 6178 2e73 6574 5f79          ax.set_y
-000104f0: 6c61 6265 6c28 2243 7572 7265 6e74 205b  label("Current [
-00010500: cebc 415d 2229 0a20 2020 2020 2020 2020  ..A]").         
-00010510: 2020 2061 782e 7365 745f 786c 6162 656c     ax.set_xlabel
-00010520: 2822 5469 6d65 205b cebc 735d 2229 0a20  ("Time [..s]"). 
-00010530: 2020 2020 2020 2020 2020 2061 782e 7365             ax.se
-00010540: 745f 7469 746c 6528 0a20 2020 2020 2020  t_title(.       
-00010550: 2020 2020 2020 2020 2066 2250 756c 7365           f"Pulse
-00010560: 732c 2045 7674 204e 756d 207b 6576 746e  s, Evt Num {evtn
-00010570: 756d 735b 6372 616e 645d 2e69 6c6f 635b  ums[crand].iloc[
-00010580: 6969 5d7d 2c20 220a 2020 2020 2020 2020  ii]}, ".        
-00010590: 2020 2020 2020 2020 6622 5365 7269 6573          f"Series
-000105a0: 204e 756d 207b 7365 7269 6573 6e75 6d73   Num {seriesnums
-000105b0: 5b63 7261 6e64 5d2e 696c 6f63 5b69 695d  [crand].iloc[ii]
-000105c0: 7d22 0a20 2020 2020 2020 2020 2020 2029  }".            )
-000105d0: 0a20 2020 2020 2020 2020 2020 2061 782e  .            ax.
-000105e0: 6c65 6765 6e64 2829 0a0a 2020 2020 7265  legend()..    re
-000105f0: 7475 726e 2074 2c20 782c 2063 7261 6e64  turn t, x, crand
-00010600: 0a20 200a                                .  .
+0000ca10: 6178 6973 3d2d 312c 206b 6565 7064 696d  axis=-1, keepdim
+0000ca20: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
+0000ca30: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
+0000ca40: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
+0000ca50: 6365 732c 2069 6e66 6f0a 2020 2020 2020  ces, info.      
+0000ca60: 2020 0a0a 0a20 2020 2020 2020 200a 2020    ...        .  
+0000ca70: 2020 0a20 2020 2020 2020 200a 0a0a 0a0a    .        .....
+0000ca80: 0a0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 200a 0a0a 2020 2020 0a63 6c61 7373 2048   ...    .class H
+0000cab0: 3557 7269 7465 723a 0a20 2020 200a 2020  5Writer:.    .  
+0000cac0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000cad0: 656c 662c 2072 6169 7365 5f65 7272 6f72  elf, raise_error
+0000cae0: 733d 5472 7565 2c20 7665 7262 6f73 653d  s=True, verbose=
+0000caf0: 5472 7565 293a 0a0a 0a20 2020 2020 2020  True):...       
+0000cb00: 2073 656c 662e 5f72 6169 7365 5f65 7272   self._raise_err
+0000cb10: 6f72 7320 3d20 7261 6973 655f 6572 726f  ors = raise_erro
+0000cb20: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+0000cb30: 5f76 6572 626f 7365 203d 2076 6572 626f  _verbose = verbo
+0000cb40: 7365 0a20 2020 2020 2020 200a 2020 2020  se.        .    
+0000cb50: 2020 2020 2320 6669 6c65 2070 6174 680a      # file path.
+0000cb60: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+0000cb70: 7269 6573 5f70 6174 6820 3d20 4e6f 6e65  ries_path = None
+0000cb80: 0a0a 2020 2020 2020 2020 2320 7365 7269  ..        # seri
+0000cb90: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+0000cba0: 5f73 6572 6965 735f 6e61 6d65 203d 204e  _series_name = N
+0000cbb0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000cbc0: 2e5f 7365 7269 6573 5f6e 756d 203d 204e  ._series_num = N
+0000cbd0: 6f6e 650a 2020 2020 2020 2020 0a20 2020  one.        .   
+0000cbe0: 2020 2020 2023 2063 7572 7265 6e74 2066       # current f
+0000cbf0: 696c 6520 696e 666f 0a20 2020 2020 2020  ile info.       
+0000cc00: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+0000cc10: 696c 6520 3d20 4e6f 6e65 0a20 2020 2020  ile = None.     
+0000cc20: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+0000cc30: 5f66 696c 655f 6e61 6d65 203d 204e 6f6e  _file_name = Non
+0000cc40: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000cc50: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
+0000cc60: 6576 656e 7473 203d 2030 0a20 2020 2020  events = 0.     
+0000cc70: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+0000cc80: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+0000cc90: 7465 7220 3d20 300a 2020 2020 2020 2020  ter = 0.        
+0000cca0: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+0000ccb0: 6c65 5f61 6463 5f67 726f 7570 203d 204e  le_adc_group = N
+0000ccc0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ccd0: 2e5f 6375 7272 656e 745f 6669 6c65 5f64  ._current_file_d
+0000cce0: 6574 636f 6e66 6967 5f67 726f 7570 203d  etconfig_group =
+0000ccf0: 204e 6f6e 650a 2020 2020 2020 2020 0a20   None.        . 
+0000cd00: 2020 2020 2020 2023 206d 6574 6164 6174         # metadat
+0000cd10: 610a 2020 2020 2020 2020 7365 6c66 2e5f  a.        self._
+0000cd20: 6669 6c65 5f6d 6574 6164 6174 6120 3d20  file_metadata = 
+0000cd30: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000cd40: 662e 5f64 6574 6563 746f 725f 636f 6e66  f._detector_conf
+0000cd50: 6967 203d 204e 6f6e 650a 2020 2020 2020  ig = None.      
+0000cd60: 2020 7365 6c66 2e5f 6164 635f 636f 6e66    self._adc_conf
+0000cd70: 6967 2020 3d20 4e6f 6e65 0a0a 2020 2020  ig  = None..    
+0000cd80: 2020 2020 0a20 2020 2020 2020 2023 2065      .        # e
+0000cd90: 7665 6e74 2063 6f75 6e74 6572 0a20 2020  vent counter.   
+0000cda0: 2020 2020 2073 656c 662e 5f67 6c6f 6261       self._globa
+0000cdb0: 6c5f 6576 656e 745f 636f 756e 7465 7220  l_event_counter 
+0000cdc0: 3d20 300a 2020 2020 2020 2020 200a 2020  = 0.         .  
+0000cdd0: 2020 2020 2020 2320 6669 6c65 2063 6f75        # file cou
+0000cde0: 6e74 6572 0a20 2020 2020 2020 2073 656c  nter.        sel
+0000cdf0: 662e 5f66 696c 655f 636f 756e 7465 7220  f._file_counter 
+0000ce00: 3d20 300a 0a20 2020 2020 2020 2023 206d  = 0..        # m
+0000ce10: 6178 2065 7665 6e74 2070 6572 2064 756d  ax event per dum
+0000ce20: 700a 2020 2020 2020 2020 7365 6c66 2e5f  p.        self._
+0000ce30: 6e62 5f65 7665 6e74 735f 7065 725f 6475  nb_events_per_du
+0000ce40: 6d70 5f6d 6178 203d 2031 3030 300a 2020  mp_max = 1000.  
+0000ce50: 2020 2020 2020 7365 6c66 2e5f 6164 635f        self._adc_
+0000ce60: 6e61 6d65 203d 2027 6164 6331 270a 0a0a  name = 'adc1'...
+0000ce70: 2020 2020 6465 6620 696e 6974 6961 6c69      def initiali
+0000ce80: 7a65 2873 656c 662c 2073 6572 6965 735f  ze(self, series_
+0000ce90: 6e61 6d65 2c20 6461 7461 5f70 6174 683d  name, data_path=
+0000cea0: 272e 2f27 293a 0a20 2020 2020 2020 2022  './'):.        "
+0000ceb0: 2222 0a20 2020 2020 2020 2049 6e69 7469  "".        Initi
+0000cec0: 616c 697a 6520 6e65 7720 7772 6974 696e  alize new writin
+0000ced0: 670a 2020 2020 2020 2020 2222 220a 2020  g.        """.  
+0000cee0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000cef0: 2063 6c65 6172 2065 7665 7279 7468 696e   clear everythin
+0000cf00: 670a 2020 2020 2020 2020 7365 6c66 2e63  g.        self.c
+0000cf10: 6c65 6172 2829 0a20 2020 2020 2020 200a  lear().        .
+0000cf20: 2020 2020 2020 2020 2320 7365 7269 6573          # series
+0000cf30: 206e 616d 6520 0a20 2020 2020 2020 2073   name .        s
+0000cf40: 656c 662e 5f73 6572 6965 735f 6e61 6d65  elf._series_name
+0000cf50: 203d 2073 6572 6965 735f 6e61 6d65 0a20   = series_name. 
+0000cf60: 2020 2020 2020 2073 656c 662e 5f73 6572         self._ser
+0000cf70: 6965 735f 6e75 6d20 3d20 6578 7472 6163  ies_num = extrac
+0000cf80: 745f 7365 7269 6573 5f6e 756d 2873 6572  t_series_num(ser
+0000cf90: 6965 735f 6e61 6d65 290a 2020 2020 2020  ies_name).      
+0000cfa0: 2020 0a0a 0a20 2020 2020 2020 2023 2063    ...        # c
+0000cfb0: 7265 6174 6520 6e65 7720 6469 7265 6374  reate new direct
+0000cfc0: 6f72 790a 2020 2020 2020 2020 2373 656c  ory.        #sel
+0000cfd0: 662e 5f73 6572 6965 735f 7061 7468 203d  f._series_path =
+0000cfe0: 2064 6174 615f 7061 7468 202b 2027 2f27   data_path + '/'
+0000cff0: 202b 2073 6572 6965 735f 6e61 6d65 0a20   + series_name. 
+0000d000: 2020 2020 2020 2073 656c 662e 5f73 6572         self._ser
+0000d010: 6965 735f 7061 7468 203d 2064 6174 615f  ies_path = data_
+0000d020: 7061 7468 0a20 2020 2020 2020 200a 2020  path.        .  
+0000d030: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
+0000d040: 7061 7468 2e69 7364 6972 2873 656c 662e  path.isdir(self.
+0000d050: 5f73 6572 6965 735f 7061 7468 293a 0a20  _series_path):. 
+0000d060: 2020 2020 2020 2020 2020 206f 732e 6d6b             os.mk
+0000d070: 6469 7228 7365 6c66 2e5f 7365 7269 6573  dir(self._series
+0000d080: 5f70 6174 6829 0a20 2020 2020 2020 2020  _path).         
+0000d090: 2020 206f 732e 6368 6d6f 6428 7365 6c66     os.chmod(self
+0000d0a0: 2e5f 7365 7269 6573 5f70 6174 682c 0a20  ._series_path,. 
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2020 7374 6174 2e53 5f49 5257 5847      stat.S_IRWXG
+0000d0d0: 207c 2073 7461 742e 535f 4952 5758 5520   | stat.S_IRWXU 
+0000d0e0: 7c20 7374 6174 2e53 5f49 524f 5448 207c  | stat.S_IROTH |
+0000d0f0: 2073 7461 742e 535f 4958 4f54 4829 0a0a   stat.S_IXOTH)..
+0000d100: 0a20 2020 2064 6566 2073 6574 5f6d 6574  .    def set_met
+0000d110: 6164 6174 6128 7365 6c66 2c20 6669 6c65  adata(self, file
+0000d120: 5f6d 6574 6164 6174 613d 4e6f 6e65 2c20  _metadata=None, 
+0000d130: 6164 635f 636f 6e66 6967 3d4e 6f6e 652c  adc_config=None,
+0000d140: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
+0000d150: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000d160: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
+0000d170: 6d65 7461 6461 7461 2077 6869 6368 2077  metadata which w
+0000d180: 696c 6c20 6265 2077 7269 7474 656e 2020  ill be written  
+0000d190: 696e 2065 6163 6820 6669 6c65 730a 2020  in each files.  
+0000d1a0: 2020 2020 2020 6669 6c65 5f6d 6574 6164        file_metad
+0000d1b0: 6174 6120 3d20 6765 6e65 7261 6c20 6461  ata = general da
+0000d1c0: 7461 2074 616b 696e 6720 696e 666f 726d  ta taking inform
+0000d1d0: 6174 696f 6e20 2866 696c 6520 6c65 7665  ation (file leve
+0000d1e0: 6c20 6d65 7461 6461 7461 290a 2020 2020  l metadata).    
+0000d1f0: 2020 2020 6164 635f 636f 6e66 6967 203d      adc_config =
+0000d200: 2061 6463 2063 6f6e 6669 6775 7261 7469   adc configurati
+0000d210: 6f6e 2028 6772 6f75 7020 6c65 7665 6c20  on (group level 
+0000d220: 6d65 7461 6461 7461 290a 2020 2020 2020  metadata).      
+0000d230: 2020 6465 7465 6374 6f72 5f63 6f6e 6669    detector_confi
+0000d240: 6720 3d20 6465 7465 6374 6f72 2073 6574  g = detector set
+0000d250: 7469 6e67 7320 2867 726f 7570 206c 6576  tings (group lev
+0000d260: 656c 206d 6574 6164 6174 6129 0a20 2020  el metadata).   
+0000d270: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0000d280: 2020 6966 2066 696c 655f 6d65 7461 6461    if file_metada
+0000d290: 7461 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ta is not None:.
+0000d2a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000d2b0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0000d2c0: 6365 2866 696c 655f 6d65 7461 6461 7461  ce(file_metadata
+0000d2d0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
+0000d2e0: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
+0000d2f0: 696c 655f 6d65 7461 6461 7461 203d 2066  ile_metadata = f
+0000d300: 696c 655f 6d65 7461 6461 7461 0a20 2020  ile_metadata.   
+0000d310: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d330: 7269 6e74 2827 5741 524e 494e 473a 206d  rint('WARNING: m
+0000d340: 6574 6164 6174 6120 6e65 6564 7320 746f  etadata needs to
+0000d350: 2062 6520 6120 6469 6374 696f 6e61 7279   be a dictionary
+0000d360: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
+0000d370: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
+0000d380: 6164 635f 636f 6e66 6967 2069 7320 6e6f  adc_config is no
+0000d390: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000d3a0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+0000d3b0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
+0000d3c0: 6463 5f63 6f6e 6669 672c 2064 6963 7429  dc_config, dict)
+0000d3d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d3e0: 2020 7365 6c66 2e5f 6164 635f 636f 6e66    self._adc_conf
+0000d3f0: 6967 203d 2061 6463 5f63 6f6e 6669 670a  ig = adc_config.
+0000d400: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000d410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d420: 2020 7072 696e 7428 2757 4152 4e49 4e47    print('WARNING
+0000d430: 3a20 6164 635f 636f 6e66 6967 206e 6565  : adc_config nee
+0000d440: 6473 2074 6f20 6265 2061 2064 6963 7469  ds to be a dicti
+0000d450: 6f6e 6172 7927 290a 0a0a 2020 2020 2020  onary')...      
+0000d460: 2020 6966 2064 6574 6563 746f 725f 636f    if detector_co
+0000d470: 6e66 6967 2069 7320 6e6f 7420 4e6f 6e65  nfig is not None
+0000d480: 3a0a 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000d490: 6620 6973 696e 7374 616e 6365 2864 6574  f isinstance(det
+0000d4a0: 6563 746f 725f 636f 6e66 6967 2c20 6469  ector_config, di
+0000d4b0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+0000d4c0: 2020 2020 2073 656c 662e 5f64 6574 6563       self._detec
+0000d4d0: 746f 725f 636f 6e66 6967 203d 2064 6574  tor_config = det
+0000d4e0: 6563 746f 725f 636f 6e66 6967 0a20 2020  ector_config.   
+0000d4f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d510: 7269 6e74 2827 5741 524e 494e 473a 2064  rint('WARNING: d
+0000d520: 6574 6563 746f 7220 636f 6e66 6967 206e  etector config n
+0000d530: 6565 6473 2074 6f20 6265 2061 2064 6963  eeds to be a dic
+0000d540: 7469 6f6e 6172 7927 290a 0a0a 2020 2020  tionary')...    
+0000d550: 2020 2020 2020 2020 2020 2020 0a0a 2020              ..  
+0000d560: 2020 2020 2020 2020 2020 0a0a 2020 2020            ..    
+0000d570: 6465 6620 636c 6f73 6528 7365 6c66 293a  def close(self):
+0000d580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d590: 2020 2020 2063 6c6f 7365 2063 7572 7265       close curre
+0000d5a0: 6e74 2066 696c 650a 2020 2020 2020 2020  nt file.        
+0000d5b0: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+0000d5c0: 662e 5f63 6c6f 7365 5f66 696c 6528 290a  f._close_file().
+0000d5d0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000d5e0: 2020 2020 200a 2020 2020 6465 6620 636c       .    def cl
+0000d5f0: 6561 7228 7365 6c66 293a 0a20 2020 2020  ear(self):.     
+0000d600: 2020 2073 656c 662e 5f63 6c6f 7365 5f66     self._close_f
+0000d610: 696c 6528 290a 2020 2020 2020 2020 7365  ile().        se
+0000d620: 6c66 2e5f 6669 6c65 5f63 6f75 6e74 6572  lf._file_counter
+0000d630: 203d 2030 0a20 2020 2020 2020 2073 656c   = 0.        sel
+0000d640: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
+0000d650: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000d660: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+0000d670: 655f 6e61 6d65 203d 204e 6f6e 650a 2020  e_name = None.  
+0000d680: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+0000d690: 656e 745f 6669 6c65 5f61 6463 5f67 726f  ent_file_adc_gro
+0000d6a0: 7570 203d 204e 6f6e 650a 2020 2020 2020  up = None.      
+0000d6b0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
+0000d6c0: 6669 6c65 5f64 6574 636f 6e66 6967 5f67  file_detconfig_g
+0000d6d0: 726f 7570 203d 204e 6f6e 6520 2020 200a  roup = None    .
+0000d6e0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+0000d6f0: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
+0000d700: 5f63 6f75 6e74 6572 203d 2030 0a20 2020  _counter = 0.   
+0000d710: 2020 2020 2073 656c 662e 5f67 6c6f 6261       self._globa
+0000d720: 6c5f 6576 656e 745f 636f 756e 7465 7220  l_event_counter 
+0000d730: 3d20 300a 2020 2020 2020 2020 7365 6c66  = 0.        self
+0000d740: 2e5f 6669 6c65 5f6d 6574 6164 6174 6120  ._file_metadata 
+0000d750: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000d760: 656c 662e 5f64 6574 6563 746f 725f 636f  elf._detector_co
+0000d770: 6e66 6967 203d 204e 6f6e 650a 2020 2020  nfig = None.    
+0000d780: 2020 2020 7365 6c66 2e5f 6164 635f 636f      self._adc_co
+0000d790: 6e66 6967 203d 204e 6f6e 650a 2020 2020  nfig = None.    
+0000d7a0: 200a 2020 2020 2020 2020 0a20 2020 2064   .        .    d
+0000d7b0: 6566 2077 7269 7465 5f65 7665 6e74 2873  ef write_event(s
+0000d7c0: 656c 662c 2064 6174 615f 6172 7261 792c  elf, data_array,
+0000d7d0: 2070 7265 6669 783d 4e6f 6e65 2c20 6461   prefix=None, da
+0000d7e0: 7461 7365 745f 6d65 7461 6461 7461 3d4e  taset_metadata=N
+0000d7f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000d800: 2020 2020 2020 2020 2064 6174 615f 6d6f           data_mo
+0000d810: 6465 3d4e 6f6e 652c 2061 6463 5f6e 616d  de=None, adc_nam
+0000d820: 653d 2761 6463 3127 293a 0a20 2020 2020  e='adc1'):.     
+0000d830: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
+0000d840: 7269 7465 2070 756c 7365 2064 6174 6120  rite pulse data 
+0000d850: 696e 2066 696c 6573 0a20 2020 2020 2020  in files.       
+0000d860: 2022 2222 0a0a 0a20 2020 2020 2020 2023   """...        #
+0000d870: 206f 7065 6e20 6669 6c65 2069 6620 6e65   open file if ne
+0000d880: 6564 6564 0a20 2020 2020 2020 2069 6620  eded.        if 
+0000d890: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
+0000d8a0: 696c 6520 6973 204e 6f6e 6520 6f72 0a20  ile is None or. 
+0000d8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d8c0: 5f63 7572 7265 6e74 5f66 696c 655f 6576  _current_file_ev
+0000d8d0: 656e 745f 636f 756e 7465 7220 3e3d 2073  ent_counter >= s
+0000d8e0: 656c 662e 5f6e 625f 6576 656e 7473 5f70  elf._nb_events_p
+0000d8f0: 6572 5f64 756d 705f 6d61 7829 3a0a 2020  er_dump_max):.  
+0000d900: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000d910: 6f70 656e 5f66 696c 6528 7072 6566 6978  open_file(prefix
+0000d920: 3d70 7265 6669 7829 0a0a 0a20 2020 2020  =prefix)...     
+0000d930: 2020 2023 2065 7665 6e74 2063 6f75 6e74     # event count
+0000d940: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+0000d950: 5f63 7572 7265 6e74 5f66 696c 655f 6576  _current_file_ev
+0000d960: 656e 745f 636f 756e 7465 7220 2b3d 2031  ent_counter += 1
+0000d970: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
+0000d980: 6c6f 6261 6c5f 6576 656e 745f 636f 756e  lobal_event_coun
+0000d990: 7465 7220 2b3d 2031 0a20 2020 2020 2020  ter += 1.       
+0000d9a0: 200a 2020 2020 2020 2020 2320 6372 6561   .        # crea
+0000d9b0: 7465 2064 6174 6173 6574 0a20 2020 2020  te dataset.     
+0000d9c0: 2020 2064 6174 6173 6574 5f6e 616d 6520     dataset_name 
+0000d9d0: 3d20 2765 7665 6e74 5f27 202b 2073 7472  = 'event_' + str
+0000d9e0: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
+0000d9f0: 696c 655f 6576 656e 745f 636f 756e 7465  ile_event_counte
+0000da00: 7229 0a20 2020 2020 2020 2064 6174 6173  r).        datas
+0000da10: 6574 203d 2073 656c 662e 5f63 7572 7265  et = self._curre
+0000da20: 6e74 5f66 696c 655f 6164 635f 6772 6f75  nt_file_adc_grou
+0000da30: 702e 6372 6561 7465 5f64 6174 6173 6574  p.create_dataset
+0000da40: 2864 6174 6173 6574 5f6e 616d 652c 2064  (dataset_name, d
+0000da50: 6174 613d 6461 7461 5f61 7272 6179 290a  ata=data_array).
+0000da60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000da70: 2061 6464 206d 6574 6164 6174 610a 2020   add metadata.  
+0000da80: 2020 2020 2020 6966 2064 6174 6173 6574        if dataset
+0000da90: 5f6d 6574 6164 6174 6120 6973 206e 6f74  _metadata is not
+0000daa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000dab0: 2020 2066 6f72 206b 6579 2c76 616c 2069     for key,val i
+0000dac0: 6e20 6461 7461 7365 745f 6d65 7461 6461  n dataset_metada
+0000dad0: 7461 2e69 7465 6d73 2829 3a0a 2020 2020  ta.items():.    
+0000dae0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0000daf0: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+0000db00: 6e70 2e6e 6461 7272 6179 2920 616e 6420  np.ndarray) and 
+0000db10: 7661 6c2e 6474 7970 652e 7479 7065 2069  val.dtype.type i
+0000db20: 7320 6e70 2e73 7472 5f29 3a0a 2020 2020  s np.str_):.    
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db40: 6474 203d 2068 3570 792e 7374 7269 6e67  dt = h5py.string
+0000db50: 5f64 7479 7065 2829 0a20 2020 2020 2020  _dtype().       
+0000db60: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0000db70: 203d 2076 616c 2e61 7374 7970 6528 6474   = val.astype(dt
+0000db80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000db90: 2020 6461 7461 7365 742e 6174 7472 735b    dataset.attrs[
+0000dba0: 6b65 795d 203d 2076 616c 0a0a 2020 2020  key] = val..    
+0000dbb0: 2020 2020 6461 7461 7365 742e 6174 7472      dataset.attr
+0000dbc0: 735b 2765 7665 6e74 5f69 6427 5d20 3d20  s['event_id'] = 
+0000dbd0: 7365 6c66 2e5f 676c 6f62 616c 5f65 7665  self._global_eve
+0000dbe0: 6e74 5f63 6f75 6e74 6572 200a 2020 2020  nt_counter .    
+0000dbf0: 2020 2020 6461 7461 7365 742e 6174 7472      dataset.attr
+0000dc00: 735b 2765 7665 6e74 5f69 6e64 6578 275d  s['event_index']
+0000dc10: 203d 2073 656c 662e 5f63 7572 7265 6e74   = self._current
+0000dc20: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+0000dc30: 7465 720a 2020 2020 2020 2020 6461 7461  ter.        data
+0000dc40: 7365 742e 6174 7472 735b 2765 7665 6e74  set.attrs['event
+0000dc50: 5f6e 756d 275d 203d 2073 656c 662e 5f66  _num'] = self._f
+0000dc60: 696c 655f 636f 756e 7465 7220 2a31 3030  ile_counter *100
+0000dc70: 3030 3020 2b20 7365 6c66 2e5f 6375 7272  000 + self._curr
+0000dc80: 656e 745f 6669 6c65 5f65 7665 6e74 5f63  ent_file_event_c
+0000dc90: 6f75 6e74 6572 0a20 2020 2020 2020 2020  ounter.         
+0000dca0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000dcb0: 2320 7570 6461 7465 206e 756d 6265 7220  # update number 
+0000dcc0: 6f66 2065 7665 6e74 730a 2020 2020 2020  of events.      
+0000dcd0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
+0000dce0: 6669 6c65 5f61 6463 5f67 726f 7570 2e61  file_adc_group.a
+0000dcf0: 7474 7273 5b27 6e62 5f65 7665 6e74 7327  ttrs['nb_events'
+0000dd00: 5d20 3d20 7365 6c66 2e5f 6375 7272 656e  ] = self._curren
+0000dd10: 745f 6669 6c65 5f65 7665 6e74 5f63 6f75  t_file_event_cou
+0000dd20: 6e74 6572 0a20 2020 2020 2020 2069 6620  nter.        if 
+0000dd30: 6461 7461 5f6d 6f64 6520 6973 206e 6f74  data_mode is not
+0000dd40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000dd50: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+0000dd60: 5f66 696c 655f 6164 635f 6772 6f75 702e  _file_adc_group.
+0000dd70: 6174 7472 735b 2764 6174 615f 6d6f 6465  attrs['data_mode
+0000dd80: 275d 203d 2073 7472 2864 6174 615f 6d6f  '] = str(data_mo
+0000dd90: 6465 290a 0a0a 2020 2020 2020 2020 2320  de)...        # 
+0000dda0: 666c 7573 680a 2020 2020 2020 2020 7365  flush.        se
+0000ddb0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+0000ddc0: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
+0000ddd0: 200a 0a0a 0a0a 0a20 2020 2020 2020 2020   ......         
+0000dde0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000ddf0: 6465 6620 5f6f 7065 6e5f 6669 6c65 2873  def _open_file(s
+0000de00: 656c 662c 2070 7265 6669 783d 4e6f 6e65  elf, prefix=None
+0000de10: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000de20: 2020 2020 2020 206f 7065 6e20 6669 6c65         open file
+0000de30: 200a 2020 2020 2020 2020 2222 220a 0a20   .        """.. 
+0000de40: 2020 2020 2020 2023 2063 6c6f 7365 2066         # close f
+0000de50: 696c 6520 6966 206e 6565 6465 640a 2020  ile if needed.  
+0000de60: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
+0000de70: 7572 7265 6e74 5f66 696c 6520 6973 206e  urrent_file is n
+0000de80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000de90: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
+0000dea0: 5f66 696c 6528 290a 0a0a 2020 2020 2020  _file()...      
+0000deb0: 2020 2320 6475 6d70 0a20 2020 2020 2020    # dump.       
+0000dec0: 2073 656c 662e 5f66 696c 655f 636f 756e   self._file_coun
+0000ded0: 7465 7220 2b3d 310a 2020 2020 2020 2020  ter +=1.        
+0000dee0: 6475 6d70 203d 2073 7472 2873 656c 662e  dump = str(self.
+0000def0: 5f66 696c 655f 636f 756e 7465 7229 0a20  _file_counter). 
+0000df00: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
+0000df10: 7261 6e67 6528 312c 352d 6c65 6e28 6475  range(1,5-len(du
+0000df20: 6d70 2929 3a0a 2020 2020 2020 2020 2020  mp)):.          
+0000df30: 2020 6966 2078 3e3d 313a 0a20 2020 2020    if x>=1:.     
+0000df40: 2020 2020 2020 2020 2020 2064 756d 7020             dump 
+0000df50: 3d20 2730 272b 6475 6d70 0a0a 0a20 2020  = '0'+dump...   
+0000df60: 2020 2020 2023 2066 756c 6c20 6669 6c65       # full file
+0000df70: 206e 616d 650a 2020 2020 2020 2020 6669   name.        fi
+0000df80: 6c65 5f6e 616d 6520 3d20 7365 6c66 2e5f  le_name = self._
+0000df90: 7365 7269 6573 5f70 6174 6820 2b20 272f  series_path + '/
+0000dfa0: 270a 2020 2020 2020 2020 6966 2070 7265  '.        if pre
+0000dfb0: 6669 7820 6973 206e 6f74 204e 6f6e 653a  fix is not None:
+0000dfc0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+0000dfd0: 655f 6e61 6d65 202b 3d20 7072 6566 6978  e_name += prefix
+0000dfe0: 202b 2027 5f27 0a20 2020 2020 2020 2066   + '_'.        f
+0000dff0: 696c 655f 6e61 6d65 202b 3d20 7365 6c66  ile_name += self
+0000e000: 2e5f 7365 7269 6573 5f6e 616d 6520 2b20  ._series_name + 
+0000e010: 275f 4627 202b 2064 756d 7020 2b20 272e  '_F' + dump + '.
+0000e020: 6864 6635 270a 2020 2020 2020 2020 7072  hdf5'.        pr
+0000e030: 696e 7428 2749 4e46 4f3a 204f 7065 6e69  int('INFO: Openi
+0000e040: 6e67 2066 696c 6520 6e61 6d65 2022 2720  ng file name "' 
+0000e050: 2b20 6669 6c65 5f6e 616d 6520 2b20 2722  + file_name + '"
+0000e060: 2729 0a20 2020 2020 2020 200a 2020 2020  ').        .    
+0000e070: 2020 2020 0a20 2020 2020 2020 2066 696c      .        fil
+0000e080: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
+0000e090: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000e0a0: 2020 6669 6c65 203d 2068 3570 792e 4669    file = h5py.Fi
+0000e0b0: 6c65 2866 696c 655f 6e61 6d65 2c20 2777  le(file_name, 'w
+0000e0c0: 2729 0a20 2020 2020 2020 2065 7863 6570  ').        excep
+0000e0d0: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
+0000e0e0: 7269 6e74 2827 4552 524f 523a 2055 6e61  rint('ERROR: Una
+0000e0f0: 626c 6520 746f 206f 7065 6e20 6669 6c65  ble to open file
+0000e100: 2027 202b 2066 696c 655f 6e61 6d65 290a   ' + file_name).
+0000e110: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000e120: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
+0000e130: 2e5f 6375 7272 656e 745f 6669 6c65 203d  ._current_file =
+0000e140: 2066 696c 650a 2020 2020 2020 2020 7365   file.        se
+0000e150: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+0000e160: 5f6e 616d 6520 3d20 6669 6c65 5f6e 616d  _name = file_nam
+0000e170: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000e180: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
+0000e190: 6576 656e 7473 203d 2030 0a20 2020 2020  events = 0.     
+0000e1a0: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+0000e1b0: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+0000e1c0: 7465 7220 3d20 300a 0a0a 2020 2020 2020  ter = 0...      
+0000e1d0: 2020 2320 6669 6c65 206d 6574 6164 6174    # file metadat
+0000e1e0: 610a 2020 2020 2020 2020 6966 2073 656c  a.        if sel
+0000e1f0: 662e 5f66 696c 655f 6d65 7461 6461 7461  f._file_metadata
+0000e200: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000e210: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+0000e220: 792c 7661 6c20 696e 2073 656c 662e 5f66  y,val in self._f
+0000e230: 696c 655f 6d65 7461 6461 7461 2e69 7465  ile_metadata.ite
+0000e240: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000e250: 2020 2020 2020 6966 2028 6973 696e 7374        if (isinst
+0000e260: 616e 6365 2876 616c 2c20 6e70 2e6e 6461  ance(val, np.nda
+0000e270: 7272 6179 2920 616e 6420 7661 6c2e 6474  rray) and val.dt
+0000e280: 7970 652e 7479 7065 2069 7320 6e70 2e73  ype.type is np.s
+0000e290: 7472 5f29 3a0a 2020 2020 2020 2020 2020  tr_):.          
+0000e2a0: 2020 2020 2020 2020 2020 6474 203d 2068            dt = h
+0000e2b0: 3570 792e 7374 7269 6e67 5f64 7479 7065  5py.string_dtype
+0000e2c0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000e2d0: 2020 2020 2020 2076 616c 203d 2076 616c         val = val
+0000e2e0: 2e61 7374 7970 6528 6474 290a 2020 2020  .astype(dt).    
+0000e2f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e300: 2e5f 6375 7272 656e 745f 6669 6c65 2e61  ._current_file.a
+0000e310: 7474 7273 5b6b 6579 5d20 3d20 7661 6c0a  ttrs[key] = val.
+0000e320: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+0000e330: 7272 656e 745f 6669 6c65 2e61 7474 7273  rrent_file.attrs
+0000e340: 5b27 7072 6566 6978 275d 203d 2070 7265  ['prefix'] = pre
+0000e350: 6669 780a 2020 2020 2020 2020 7365 6c66  fix.        self
+0000e360: 2e5f 6375 7272 656e 745f 6669 6c65 2e61  ._current_file.a
+0000e370: 7474 7273 5b27 7365 7269 6573 5f6e 756d  ttrs['series_num
+0000e380: 275d 203d 2073 656c 662e 5f73 6572 6965  '] = self._serie
+0000e390: 735f 6e75 6d0a 2020 2020 2020 2020 7365  s_num.        se
+0000e3a0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+0000e3b0: 2e61 7474 7273 5b27 6475 6d70 5f6e 756d  .attrs['dump_num
+0000e3c0: 275d 203d 2069 6e74 2864 756d 7029 0a20  '] = int(dump). 
+0000e3d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000e3e0: 2320 6465 7465 6374 6f72 2063 6f6e 6669  # detector confi
+0000e3f0: 670a 2020 2020 2020 2020 6966 2073 656c  g.        if sel
+0000e400: 662e 5f64 6574 6563 746f 725f 636f 6e66  f._detector_conf
+0000e410: 6967 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ig is not None:.
+0000e420: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e430: 636f 6e66 6967 5f6b 6579 2c63 6f6e 6669  config_key,confi
+0000e440: 675f 7661 6c20 696e 2073 656c 662e 5f64  g_val in self._d
+0000e450: 6574 6563 746f 725f 636f 6e66 6967 2e69  etector_config.i
+0000e460: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+0000e470: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000e480: 7461 6e63 6528 636f 6e66 6967 5f76 616c  tance(config_val
+0000e490: 2c64 6963 7429 3a0a 2020 2020 2020 2020  ,dict):.        
+0000e4a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e4b0: 2e5f 6375 7272 656e 745f 6669 6c65 5f64  ._current_file_d
+0000e4c0: 6574 636f 6e66 6967 5f67 726f 7570 203d  etconfig_group =
+0000e4d0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+0000e4e0: 696c 652e 6372 6561 7465 5f67 726f 7570  ile.create_group
+0000e4f0: 2863 6f6e 6669 675f 6b65 7929 0a20 2020  (config_key).   
+0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e510: 2066 6f72 206b 6579 2c76 616c 2069 6e20   for key,val in 
+0000e520: 636f 6e66 6967 5f76 616c 2e69 7465 6d73  config_val.items
+0000e530: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000e540: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0000e550: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+0000e560: 6e70 2e6e 6461 7272 6179 2920 616e 6420  np.ndarray) and 
+0000e570: 7661 6c2e 6474 7970 652e 7479 7065 2069  val.dtype.type i
+0000e580: 7320 6e70 2e73 7472 5f29 3a0a 2020 2020  s np.str_):.    
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 2020 2020 2020 2020 6474 203d 2068 3570          dt = h5p
+0000e5b0: 792e 7374 7269 6e67 5f64 7479 7065 2829  y.string_dtype()
+0000e5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e5d0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0000e5e0: 203d 2076 616c 2e61 7374 7970 6528 6474   = val.astype(dt
+0000e5f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e600: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000e610: 6375 7272 656e 745f 6669 6c65 5f64 6574  current_file_det
+0000e620: 636f 6e66 6967 5f67 726f 7570 2e61 7474  config_group.att
+0000e630: 7273 5b6b 6579 5d20 3d20 7661 6c0a 2020  rs[key] = val.  
+0000e640: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000e650: 2063 7265 6174 6520 6164 6320 6772 6f75   create adc grou
+0000e660: 700a 2020 2020 2020 2020 6966 2073 656c  p.        if sel
+0000e670: 662e 5f61 6463 5f63 6f6e 6669 6720 6973  f._adc_config is
+0000e680: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e690: 2020 2020 2020 2066 6f72 2063 6f6e 6669         for confi
+0000e6a0: 675f 6b65 792c 636f 6e66 6967 5f76 616c  g_key,config_val
+0000e6b0: 2069 6e20 7365 6c66 2e5f 6164 635f 636f   in self._adc_co
+0000e6c0: 6e66 6967 2e69 7465 6d73 2829 3a0a 2020  nfig.items():.  
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000e6e0: 2069 7369 6e73 7461 6e63 6528 636f 6e66   isinstance(conf
+0000e6f0: 6967 5f76 616c 2c64 6963 7429 3a0a 2020  ig_val,dict):.  
+0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e710: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
+0000e720: 6669 6c65 5f61 6463 5f67 726f 7570 2020  file_adc_group  
+0000e730: 3d20 7365 6c66 2e5f 6375 7272 656e 745f  = self._current_
+0000e740: 6669 6c65 2e63 7265 6174 655f 6772 6f75  file.create_grou
+0000e750: 7028 636f 6e66 6967 5f6b 6579 290a 2020  p(config_key).  
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 666f 7220 6b65 792c 7661 6c20 696e    for key,val in
+0000e780: 2063 6f6e 6669 675f 7661 6c2e 6974 656d   config_val.item
+0000e790: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+0000e7a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e7b0: 2869 7369 6e73 7461 6e63 6528 7661 6c2c  (isinstance(val,
+0000e7c0: 206e 702e 6e64 6172 7261 7929 2061 6e64   np.ndarray) and
+0000e7d0: 2076 616c 2e64 7479 7065 2e74 7970 6520   val.dtype.type 
+0000e7e0: 6973 206e 702e 7374 725f 293a 0a20 2020  is np.str_):.   
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 2020 2020 2020 2020 2064 7420 3d20 6835           dt = h5
+0000e810: 7079 2e73 7472 696e 675f 6474 7970 6528  py.string_dtype(
+0000e820: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e830: 2020 2020 2020 2020 2020 2020 2020 7661                va
+0000e840: 6c20 3d20 7661 6c2e 6173 7479 7065 2864  l = val.astype(d
+0000e850: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+0000e860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e870: 5f63 7572 7265 6e74 5f66 696c 655f 6164  _current_file_ad
+0000e880: 635f 6772 6f75 702e 6174 7472 735b 6b65  c_group.attrs[ke
+0000e890: 795d 203d 2076 616c 0a20 2020 2020 2020  y] = val.       
+0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8b0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+0000e8c0: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
+0000e8d0: 2020 2020 2020 0a20 2020 2064 6566 205f        .    def _
+0000e8e0: 636c 6f73 655f 6669 6c65 2873 656c 6629  close_file(self)
+0000e8f0: 3a0a 0a20 2020 2020 2020 2069 6620 7365  :..        if se
+0000e900: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+0000e910: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000e920: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000e930: 6375 7272 656e 745f 6669 6c65 2e63 6c6f  current_file.clo
+0000e940: 7365 2829 0a20 200a 2020 2020 2020 2020  se().  .        
+0000e950: 2320 696e 6974 6961 6c69 7a65 0a20 2020  # initialize.   
+0000e960: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+0000e970: 6e74 5f66 696c 6520 3d20 4e6f 6e65 0a20  nt_file = None. 
+0000e980: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
+0000e990: 7265 6e74 5f66 696c 655f 6e61 6d65 203d  rent_file_name =
+0000e9a0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0000e9b0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+0000e9c0: 5f6e 625f 6576 656e 7473 203d 2030 0a20  _nb_events = 0. 
+0000e9d0: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
+0000e9e0: 7265 6e74 5f66 696c 655f 6164 635f 6772  rent_file_adc_gr
+0000e9f0: 6f75 7020 3d20 4e6f 6e65 0a20 2020 2020  oup = None.     
+0000ea00: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+0000ea10: 5f66 696c 655f 6465 7463 6f6e 6669 675f  _file_detconfig_
+0000ea20: 6772 6f75 7020 3d20 4e6f 6e65 0a20 2020  group = None.   
+0000ea30: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+0000ea40: 6e74 5f66 696c 655f 6576 656e 745f 636f  nt_file_event_co
+0000ea50: 756e 7465 7220 3d20 300a 0a0a 2020 2020  unter = 0...    
+0000ea60: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+0000ea70: 2020 0a0a 6465 6620 6765 7472 616e 6465    ..def getrande
+0000ea80: 7665 6e74 7328 6261 7365 7061 7468 2c20  vents(basepath, 
+0000ea90: 6576 746e 756d 732c 2073 6572 6965 736e  evtnums, seriesn
+0000eaa0: 756d 732c 2063 7574 3d4e 6f6e 652c 2063  ums, cut=None, c
+0000eab0: 6861 6e6e 656c 733d 4e6f 6e65 2c0a 2020  hannels=None,.  
+0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ead0: 7375 6d63 6861 6e73 3d46 616c 7365 2c20  sumchans=False, 
+0000eae0: 6c67 6370 6c6f 743d 4661 6c73 652c 206e  lgcplot=False, n
+0000eaf0: 7472 6163 6573 3d31 2c20 6e70 6c6f 743d  traces=1, nplot=
+0000eb00: 3230 2c0a 2020 2020 2020 2020 2020 2020  20,.            
+0000eb10: 2020 2020 2020 7365 6564 3d4e 6f6e 652c        seed=None,
+0000eb20: 2069 6e64 6261 7365 7072 653d 4e6f 6e65   indbasepre=None
+0000eb30: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
+0000eb40: 756e 6374 696f 6e20 666f 7220 6c6f 6164  unction for load
+0000eb50: 696e 6720 2861 6e64 2070 6c6f 7474 696e  ing (and plottin
+0000eb60: 6729 2072 616e 646f 6d20 6576 656e 7473  g) random events
+0000eb70: 2066 726f 6d20 6120 6461 7461 7365 7473   from a datasets
+0000eb80: 2e0a 2020 2020 4861 7320 6675 6e63 7469  ..    Has functi
+0000eb90: 6f6e 616c 6974 7920 746f 2070 756c 6c20  onality to pull 
+0000eba0: 7261 6e64 6f6d 6c79 2066 726f 6d20 6120  randomly from a 
+0000ebb0: 7370 6563 6966 6965 6420 6375 742e 0a0a  specified cut...
+0000ebc0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000ebd0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000ebe0: 2020 6261 7365 7061 7468 203a 2073 7472    basepath : str
+0000ebf0: 0a20 2020 2020 2020 2054 6865 2062 6173  .        The bas
+0000ec00: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
+0000ec10: 7265 6374 6f72 7920 7468 6174 2063 6f6e  rectory that con
+0000ec20: 7461 696e 7320 7468 6520 666f 6c64 6572  tains the folder
+0000ec30: 7320 7468 6174 0a20 2020 2020 2020 2074  s that.        t
+0000ec40: 6865 2065 7665 6e74 2064 756d 7073 2061  he event dumps a
+0000ec50: 7265 2069 6e2e 2054 6865 2066 6f6c 6465  re in. The folde
+0000ec60: 7273 2069 6e20 7468 6973 2064 6972 6563  rs in this direc
+0000ec70: 746f 7279 2073 686f 756c 6420 6265 0a20  tory should be. 
+0000ec80: 2020 2020 2020 2074 6865 2073 6572 6965         the serie
+0000ec90: 7320 6e75 6d62 6572 732e 0a20 2020 2065  s numbers..    e
+0000eca0: 7674 6e75 6d73 203a 2061 7272 6179 5f6c  vtnums : array_l
+0000ecb0: 696b 650a 2020 2020 2020 2020 416e 2061  ike.        An a
+0000ecc0: 7272 6179 206f 6620 616c 6c20 6576 656e  rray of all even
+0000ecd0: 7420 6e75 6d62 6572 7320 666f 7220 7468  t numbers for th
+0000ece0: 6520 6576 656e 7473 2069 6e20 616c 6c20  e events in all 
+0000ecf0: 6461 7461 7365 7473 2e0a 2020 2020 7365  datasets..    se
+0000ed00: 7269 6573 6e75 6d73 203a 2061 7272 6179  riesnums : array
+0000ed10: 5f6c 696b 650a 2020 2020 2020 2020 416e  _like.        An
+0000ed20: 2061 7272 6179 206f 6620 7468 6520 636f   array of the co
+0000ed30: 7272 6573 706f 6e64 696e 6720 7365 7269  rresponding seri
+0000ed40: 6573 206e 756d 6265 7273 2066 6f72 2065  es numbers for e
+0000ed50: 6163 6820 6576 656e 740a 2020 2020 2020  ach event.      
+0000ed60: 2020 6e75 6d62 6572 2069 6e20 6576 746e    number in evtn
+0000ed70: 756d 732e 0a20 2020 2063 7574 203a 2061  ums..    cut : a
+0000ed80: 7272 6179 5f6c 696b 652c 206f 7074 696f  rray_like, optio
+0000ed90: 6e61 6c0a 2020 2020 2020 2020 4120 626f  nal.        A bo
+0000eda0: 6f6c 6561 6e20 6172 7261 7920 6f66 2074  olean array of t
+0000edb0: 6865 2063 7574 2074 6861 7420 7368 6f75  he cut that shou
+0000edc0: 6c64 2062 6520 6170 706c 6965 6420 746f  ld be applied to
+0000edd0: 2074 6865 2064 6174 612e 0a20 2020 2020   the data..     
+0000ede0: 2020 2049 6620 6c65 6674 2061 7320 4e6f     If left as No
+0000edf0: 6e65 2c20 7468 656e 206e 6f20 6375 7420  ne, then no cut 
+0000ee00: 6973 2061 7070 6c69 6564 2e0a 2020 2020  is applied..    
+0000ee10: 6368 616e 6e65 6c73 203a 206c 6973 742c  channels : list,
+0000ee20: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000ee30: 2020 4120 6c69 7374 206f 6620 7374 7269    A list of stri
+0000ee40: 6e67 7320 7468 6174 2063 6f6e 7461 696e  ngs that contain
+0000ee50: 7320 616c 6c20 6f66 2074 6865 2063 6861  s all of the cha
+0000ee60: 6e6e 656c 7320 7468 6174 2073 686f 756c  nnels that shoul
+0000ee70: 640a 2020 2020 2020 2020 6265 206c 6f61  d.        be loa
+0000ee80: 6465 642e 2049 6620 6c65 6674 2061 7320  ded. If left as 
+0000ee90: 4e6f 6e65 2c20 616c 6c20 6368 616e 6e65  None, all channe
+0000eea0: 6c73 2061 7265 206c 6f61 6465 642e 0a20  ls are loaded.. 
+0000eeb0: 2020 2073 756d 6368 616e 7320 3a20 626f     sumchans : bo
+0000eec0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
+0000eed0: 2020 2020 2041 2062 6f6f 6c65 616e 2066       A boolean f
+0000eee0: 6c61 6720 666f 7220 7768 6574 6865 7220  lag for whether 
+0000eef0: 6f72 206e 6f74 2074 6f20 7375 6d20 7468  or not to sum th
+0000ef00: 6520 6368 616e 6e65 6c73 2077 6865 6e0a  e channels when.
+0000ef10: 2020 2020 2020 2020 706c 6f74 7469 6e67          plotting
+0000ef20: 2e20 4966 2046 616c 7365 2c20 6561 6368  . If False, each
+0000ef30: 2063 6861 6e6e 656c 2069 7320 706c 6f74   channel is plot
+0000ef40: 7465 6420 696e 6469 7669 6475 616c 6c79  ted individually
+0000ef50: 2e0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
+0000ef60: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
+0000ef70: 6e74 7261 6365 7320 3a20 696e 742c 2073  ntraces : int, s
+0000ef80: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
+0000ef90: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
+0000efa0: 6f66 2074 7261 6365 7320 746f 2072 616e  of traces to ran
+0000efb0: 646f 6d6c 7920 6c6f 6164 2066 726f 6d20  domly load from 
+0000efc0: 7468 6520 6461 7461 2028 7769 7468 2074  the data (with t
+0000efd0: 6865 0a20 2020 2020 2020 2063 7574 2c20  he.        cut, 
+0000efe0: 6966 2073 7065 6369 6669 6564 292e 2049  if specified). I
+0000eff0: 6620 616c 6c20 7472 6163 6573 2066 726f  f all traces fro
+0000f000: 6d20 6120 7370 6563 6669 6564 2063 7574  m a specfied cut
+0000f010: 2061 7265 0a20 2020 2020 2020 2064 6573   are.        des
+0000f020: 6972 6564 2c20 7061 7373 2074 6865 2073  ired, pass the s
+0000f030: 7472 696e 6720 2261 6c6c 222e 2044 6566  tring "all". Def
+0000f040: 6175 6c74 2069 7320 312e 0a20 2020 206c  ault is 1..    l
+0000f050: 6763 706c 6f74 203a 2062 6f6f 6c2c 206f  gcplot : bool, o
+0000f060: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000f070: 4c6f 6769 6361 6c20 666c 6167 206f 6e20  Logical flag on 
+0000f080: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
+0000f090: 6f20 706c 6f74 2074 6865 2070 756c 6c65  o plot the pulle
+0000f0a0: 6420 7472 6163 6573 2e0a 2020 2020 6e70  d traces..    np
+0000f0b0: 6c6f 7420 3a20 696e 742c 206f 7074 696f  lot : int, optio
+0000f0c0: 6e61 6c0a 2020 2020 2020 2020 4966 206c  nal.        If l
+0000f0d0: 6763 706c 6f74 2069 7320 5472 7565 2c20  gcplot is True, 
+0000f0e0: 7468 6520 6e75 6d62 6572 206f 6620 7472  the number of tr
+0000f0f0: 6163 6573 2074 6f20 706c 6f74 2e0a 2020  aces to plot..  
+0000f100: 2020 7365 6564 203a 2069 6e74 2c20 6f70    seed : int, op
+0000f110: 7469 6f6e 616c 0a20 2020 2020 2020 2041  tional.        A
+0000f120: 2076 616c 7565 2074 6f20 7061 7373 2074   value to pass t
+0000f130: 6f20 6e70 2e72 616e 646f 6d2e 7365 6564  o np.random.seed
+0000f140: 2069 6620 7468 6520 7573 6572 2077 6973   if the user wis
+0000f150: 6865 7320 746f 2075 7365 0a20 2020 2020  hes to use.     
+0000f160: 2020 2074 6865 2073 616d 6520 7261 6e64     the same rand
+0000f170: 6f6d 2073 6565 6420 6561 6368 2074 696d  om seed each tim
+0000f180: 6520 6765 7472 616e 6465 7665 6e74 7320  e getrandevents 
+0000f190: 6973 2063 616c 6c65 642e 0a20 2020 2069  is called..    i
+0000f1a0: 6e64 6261 7365 7072 6520 3a20 4e6f 6e65  ndbasepre : None
+0000f1b0: 5479 7065 2c20 696e 742c 206f 7074 696f  Type, int, optio
+0000f1c0: 6e61 6c0a 2020 2020 2020 2020 5468 6520  nal.        The 
+0000f1d0: 6e75 6d62 6572 206f 6620 696e 6469 6365  number of indice
+0000f1e0: 7320 7570 2074 6f20 7768 6963 6820 6120  s up to which a 
+0000f1f0: 7472 6163 6520 7368 6f75 6c64 2062 6520  trace should be 
+0000f200: 6176 6572 6167 6564 2074 6f0a 2020 2020  averaged to.    
+0000f210: 2020 2020 6465 7465 726d 696e 6520 7468      determine th
+0000f220: 6520 6261 7365 6c69 6e65 2e20 5468 6973  e baseline. This
+0000f230: 2062 6173 656c 696e 6520 7769 6c6c 2074   baseline will t
+0000f240: 6865 6e20 6265 2073 7562 7472 6163 7465  hen be subtracte
+0000f250: 640a 2020 2020 2020 2020 6672 6f6d 2074  d.        from t
+0000f260: 6865 2074 7261 6365 7320 7768 656e 2070  he traces when p
+0000f270: 6c6f 7474 696e 672e 2049 6620 6c65 6674  lotting. If left
+0000f280: 2061 7320 4e6f 6e65 2c20 6e6f 2062 6173   as None, no bas
+0000f290: 656c 696e 650a 2020 2020 2020 2020 7375  eline.        su
+0000f2a0: 6274 7261 6374 696f 6e20 7769 6c6c 2062  btraction will b
+0000f2b0: 6520 646f 6e65 2e0a 0a20 2020 2052 6574  e done...    Ret
+0000f2c0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+0000f2d0: 0a20 2020 2074 203a 206e 6461 7272 6179  .    t : ndarray
+0000f2e0: 0a20 2020 2020 2020 2054 6865 2074 696d  .        The tim
+0000f2f0: 6520 7661 6c75 6573 2066 6f72 2070 6c6f  e values for plo
+0000f300: 7474 696e 6720 7468 6520 6576 656e 7473  tting the events
+0000f310: 2e0a 2020 2020 7820 3a20 6e64 6172 7261  ..    x : ndarra
+0000f320: 790a 2020 2020 2020 2020 4172 7261 7920  y.        Array 
+0000f330: 636f 6e74 6169 6e69 6e67 2061 6c6c 206f  containing all o
+0000f340: 6620 7468 6520 6576 656e 7473 2074 6861  f the events tha
+0000f350: 7420 7765 7265 2070 756c 6c65 642e 0a20  t were pulled.. 
+0000f360: 2020 2063 7261 6e64 203a 206e 6461 7272     crand : ndarr
+0000f370: 6179 0a20 2020 2020 2020 2042 6f6f 6c65  ay.        Boole
+0000f380: 616e 2061 7272 6179 2074 6861 7420 636f  an array that co
+0000f390: 6e74 6169 6e73 2074 6865 2063 7574 206f  ntains the cut o
+0000f3a0: 6e20 7468 6520 6c6f 6164 6564 2064 6174  n the loaded dat
+0000f3b0: 612e 0a0a 2020 2020 2222 220a 0a20 2020  a...    """..   
+0000f3c0: 2069 6620 7365 6564 2069 7320 6e6f 7420   if seed is not 
+0000f3d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6e70  None:.        np
+0000f3e0: 2e72 616e 646f 6d2e 7365 6564 2873 6565  .random.seed(see
+0000f3f0: 6429 0a0a 2020 2020 6966 2069 7369 6e73  d)..    if isins
+0000f400: 7461 6e63 6528 6368 616e 6e65 6c73 2c20  tance(channels, 
+0000f410: 7374 7229 3a0a 2020 2020 2020 2020 6368  str):.        ch
+0000f420: 616e 6e65 6c73 203d 205b 6368 616e 6e65  annels = [channe
+0000f430: 6c73 5d0a 0a20 2020 2069 6620 6e6f 7420  ls]..    if not 
+0000f440: 6973 696e 7374 616e 6365 2865 7674 6e75  isinstance(evtnu
+0000f450: 6d73 2c20 7064 2e53 6572 6965 7329 3a0a  ms, pd.Series):.
+0000f460: 2020 2020 2020 2020 6576 746e 756d 7320          evtnums 
+0000f470: 3d20 7064 2e53 6572 6965 7328 6461 7461  = pd.Series(data
+0000f480: 3d65 7674 6e75 6d73 290a 2020 2020 6966  =evtnums).    if
+0000f490: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0000f4a0: 7365 7269 6573 6e75 6d73 2c20 7064 2e53  seriesnums, pd.S
+0000f4b0: 6572 6965 7329 3a0a 2020 2020 2020 2020  eries):.        
+0000f4c0: 7365 7269 6573 6e75 6d73 203d 2070 642e  seriesnums = pd.
+0000f4d0: 5365 7269 6573 2864 6174 613d 7365 7269  Series(data=seri
+0000f4e0: 6573 6e75 6d73 290a 0a20 2020 2069 6620  esnums)..    if 
+0000f4f0: 6375 7420 6973 204e 6f6e 653a 0a20 2020  cut is None:.   
+0000f500: 2020 2020 2063 7574 203d 206e 702e 6f6e       cut = np.on
+0000f510: 6573 286c 656e 2865 7674 6e75 6d73 292c  es(len(evtnums),
+0000f520: 2064 7479 7065 3d62 6f6f 6c29 0a0a 2020   dtype=bool)..  
+0000f530: 2020 6966 206e 702e 7375 6d28 6375 7429    if np.sum(cut)
+0000f540: 203d 3d20 303a 0a20 2020 2020 2020 2072   == 0:.        r
+0000f550: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000f560: 0a20 2020 2020 2020 2020 2020 2022 5468  .            "Th
+0000f570: 6520 696e 7075 7474 6564 2063 7574 2068  e inputted cut h
+0000f580: 6173 206e 6f20 6576 656e 7473 2c20 6361  as no events, ca
+0000f590: 6e6e 6f74 206c 6f61 6420 616e 7920 7472  nnot load any tr
+0000f5a0: 6163 6573 2e22 0a20 2020 2020 2020 2029  aces.".        )
+0000f5b0: 0a0a 2020 2020 6966 206e 7472 6163 6573  ..    if ntraces
+0000f5c0: 203d 3d20 2761 6c6c 2720 6f72 206e 7472   == 'all' or ntr
+0000f5d0: 6163 6573 203e 206e 702e 7375 6d28 6375  aces > np.sum(cu
+0000f5e0: 7429 3a0a 2020 2020 2020 2020 6e74 7261  t):.        ntra
+0000f5f0: 6365 7320 3d20 6e70 2e73 756d 2863 7574  ces = np.sum(cut
+0000f600: 290a 2020 2020 2020 2020 6966 206e 7472  ).        if ntr
+0000f610: 6163 6573 203e 2031 3030 303a 0a20 2020  aces > 1000:.   
+0000f620: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000f630: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+0000f640: 2020 2020 2020 2020 2259 6f75 2061 7265          "You are
+0000f650: 206c 6f61 6469 6e67 2061 206c 6172 6765   loading a large
+0000f660: 206e 756d 6265 7220 6f66 2074 7261 6365   number of trace
+0000f670: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+0000f680: 2020 2020 6622 287b 6e74 7261 6365 737d      f"({ntraces}
+0000f690: 292e 2042 6520 6361 7265 6675 6c20 7769  ). Be careful wi
+0000f6a0: 7468 2079 6f75 7220 5241 4d20 7573 6167  th your RAM usag
+0000f6b0: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
+0000f6c0: 290a 0a20 2020 2069 6e64 7320 3d20 6e70  )..    inds = np
+0000f6d0: 2e72 616e 646f 6d2e 6368 6f69 6365 280a  .random.choice(.
+0000f6e0: 2020 2020 2020 2020 6e70 2e66 6c61 746e          np.flatn
+0000f6f0: 6f6e 7a65 726f 2863 7574 292c 0a20 2020  onzero(cut),.   
+0000f700: 2020 2020 2073 697a 653d 6e74 7261 6365       size=ntrace
+0000f710: 732c 0a20 2020 2020 2020 2072 6570 6c61  s,.        repla
+0000f720: 6365 3d46 616c 7365 2c0a 2020 2020 290a  ce=False,.    ).
+0000f730: 0a20 2020 2063 7261 6e64 203d 206e 702e  .    crand = np.
+0000f740: 7a65 726f 7328 6c65 6e28 6576 746e 756d  zeros(len(evtnum
+0000f750: 7329 2c20 6474 7970 653d 626f 6f6c 290a  s), dtype=bool).
+0000f760: 2020 2020 6372 616e 645b 696e 6473 5d20      crand[inds] 
+0000f770: 3d20 5472 7565 0a0a 2020 2020 6835 5f72  = True..    h5_r
+0000f780: 6561 6465 7220 3d20 4835 5265 6164 6572  eader = H5Reader
+0000f790: 2829 0a0a 2020 2020 6669 7273 745f 6669  ()..    first_fi
+0000f7a0: 6c65 203d 2073 6f72 7465 6428 676c 6f62  le = sorted(glob
+0000f7b0: 2866 277b 6261 7365 7061 7468 7d2f 2a2a  (f'{basepath}/**
+0000f7c0: 2f2a 2e68 6466 3527 2c20 7265 6375 7273  /*.hdf5', recurs
+0000f7d0: 6976 653d 5472 7565 2929 5b30 5d0a 0a20  ive=True))[0].. 
+0000f7e0: 2020 2069 6620 6368 616e 6e65 6c73 2069     if channels i
+0000f7f0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000f800: 636f 6e6e 6563 7469 6f6e 5f64 6963 7420  connection_dict 
+0000f810: 3d20 6835 5f72 6561 6465 722e 6765 745f  = h5_reader.get_
+0000f820: 636f 6e6e 6563 7469 6f6e 5f64 6963 7428  connection_dict(
+0000f830: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+0000f840: 655f 6e61 6d65 3d66 6972 7374 5f66 696c  e_name=first_fil
+0000f850: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+0000f860: 2020 2020 2063 6861 6e6e 656c 7320 3d20       channels = 
+0000f870: 636f 6e6e 6563 7469 6f6e 5f64 6963 745b  connection_dict[
+0000f880: 2764 6574 6563 746f 725f 6368 616e 7327  'detector_chans'
+0000f890: 5d0a 0a20 2020 2066 735f 6c69 7374 203d  ]..    fs_list =
+0000f8a0: 205b 5d0a 2020 2020 6d65 7461 6461 7461   [].    metadata
+0000f8b0: 203d 2068 355f 7265 6164 6572 2e67 6574   = h5_reader.get
+0000f8c0: 5f6d 6574 6164 6174 6128 6669 6c65 5f6e  _metadata(file_n
+0000f8d0: 616d 653d 6669 7273 745f 6669 6c65 290a  ame=first_file).
+0000f8e0: 2020 2020 666f 7220 6c61 6265 6c20 696e      for label in
+0000f8f0: 206d 6574 6164 6174 615b 2767 726f 7570   metadata['group
+0000f900: 5f6c 6973 7427 5d3a 0a20 2020 2020 2020  _list']:.       
+0000f910: 2066 735f 6c69 7374 2e61 7070 656e 6428   fs_list.append(
+0000f920: 6d65 7461 6461 7461 5b27 6772 6f75 7073  metadata['groups
+0000f930: 275d 5b6c 6162 656c 5d2e 6765 7428 2773  '][label].get('s
+0000f940: 616d 706c 655f 7261 7465 2729 290a 0a20  ample_rate')).. 
+0000f950: 2020 2066 7320 3d20 6e70 2e75 6e69 7175     fs = np.uniqu
+0000f960: 6528 6c69 7374 2866 696c 7465 7228 4e6f  e(list(filter(No
+0000f970: 6e65 2c20 6673 5f6c 6973 7429 2929 5b30  ne, fs_list)))[0
+0000f980: 5d0a 0a20 2020 2061 7272 2c20 6d65 7461  ]..    arr, meta
+0000f990: 6461 7461 203d 2068 355f 7265 6164 6572  data = h5_reader
+0000f9a0: 2e72 6561 645f 6d61 6e79 5f65 7665 6e74  .read_many_event
+0000f9b0: 7328 0a20 2020 2020 2020 2066 696c 6570  s(.        filep
+0000f9c0: 6174 683d 676c 6f62 2866 277b 6261 7365  ath=glob(f'{base
+0000f9d0: 7061 7468 7d2f 2a27 292c 0a20 2020 2020  path}/*'),.     
+0000f9e0: 2020 2065 7665 6e74 5f6e 756d 733d 6e70     event_nums=np
+0000f9f0: 2e61 7361 7272 6179 2865 7674 6e75 6d73  .asarray(evtnums
+0000fa00: 5b63 7574 2026 2063 7261 6e64 5d29 2c0a  [cut & crand]),.
+0000fa10: 2020 2020 2020 2020 7365 7269 6573 5f6e          series_n
+0000fa20: 756d 733d 6e70 2e61 7361 7272 6179 2873  ums=np.asarray(s
+0000fa30: 6572 6965 736e 756d 735b 6375 7420 2620  eriesnums[cut & 
+0000fa40: 6372 616e 645d 292c 0a20 2020 2020 2020  crand]),.       
+0000fa50: 206f 7574 7075 745f 666f 726d 6174 3d32   output_format=2
+0000fa60: 2c0a 2020 2020 2020 2020 696e 636c 7564  ,.        includ
+0000fa70: 655f 6d65 7461 6461 7461 3d54 7275 652c  e_metadata=True,
+0000fa80: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
+0000fa90: 725f 6368 616e 733d 6368 616e 6e65 6c73  r_chans=channels
+0000faa0: 2c0a 2020 2020 2020 2020 6164 6374 6f61  ,.        adctoa
+0000fab0: 6d70 3d54 7275 652c 0a20 2020 2029 0a0a  mp=True,.    )..
+0000fac0: 2020 2020 6966 2063 6861 6e6e 656c 7320      if channels 
+0000fad0: 213d 206d 6574 6164 6174 615b 305d 5b27  != metadata[0]['
+0000fae0: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
+0000faf0: 3a0a 2020 2020 2020 2020 6368 616e 7320  :.        chans 
+0000fb00: 3d20 5b6d 6574 6164 6174 615b 305d 5b27  = [metadata[0]['
+0000fb10: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
+0000fb20: 2e69 6e64 6578 2863 6829 2066 6f72 2063  .index(ch) for c
+0000fb30: 6820 696e 2063 6861 6e6e 656c 735d 0a20  h in channels]. 
+0000fb40: 2020 2020 2020 2078 203d 2061 7272 5b3a         x = arr[:
+0000fb50: 2c20 6368 616e 735d 2e61 7374 7970 6528  , chans].astype(
+0000fb60: 666c 6f61 7429 0a20 2020 2065 6c73 653a  float).    else:
+0000fb70: 0a20 2020 2020 2020 2078 203d 2061 7272  .        x = arr
+0000fb80: 2e61 7374 7970 6528 666c 6f61 7429 0a0a  .astype(float)..
+0000fb90: 2020 2020 7420 3d20 6e70 2e61 7261 6e67      t = np.arang
+0000fba0: 6528 782e 7368 6170 655b 2d31 5d29 2f66  e(x.shape[-1])/f
+0000fbb0: 730a 0a20 2020 2069 6620 6c67 6370 6c6f  s..    if lgcplo
+0000fbc0: 743a 0a20 2020 2020 2020 2069 6620 6e70  t:.        if np
+0000fbd0: 6c6f 743e 6e74 7261 6365 733a 0a20 2020  lot>ntraces:.   
+0000fbe0: 2020 2020 2020 2020 206e 706c 6f74 203d           nplot =
+0000fbf0: 206e 7472 6163 6573 0a0a 2020 2020 2020   ntraces..      
+0000fc00: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
+0000fc10: 6528 6e70 6c6f 7429 3a0a 0a20 2020 2020  e(nplot):..     
+0000fc20: 2020 2020 2020 2066 6967 2c20 6178 203d         fig, ax =
+0000fc30: 2070 6c74 2e73 7562 706c 6f74 7328 6669   plt.subplots(fi
+0000fc40: 6773 697a 653d 2831 302c 2036 2929 0a20  gsize=(10, 6)). 
+0000fc50: 2020 2020 2020 2020 2020 2069 6620 7375             if su
+0000fc60: 6d63 6861 6e73 3a0a 2020 2020 2020 2020  mchans:.        
+0000fc70: 2020 2020 2020 2020 7472 6163 655f 7375          trace_su
+0000fc80: 6d20 3d20 785b 6969 5d2e 7375 6d28 6178  m = x[ii].sum(ax
+0000fc90: 6973 3d30 290a 0a20 2020 2020 2020 2020  is=0)..         
+0000fca0: 2020 2020 2020 2069 6620 696e 6462 6173         if indbas
+0000fcb0: 6570 7265 2069 7320 6e6f 7420 4e6f 6e65  epre is not None
+0000fcc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fcd0: 2020 2020 2020 6261 7365 6c69 6e65 203d        baseline =
+0000fce0: 206e 702e 6d65 616e 2874 7261 6365 5f73   np.mean(trace_s
+0000fcf0: 756d 5b2e 2e2e 2c20 3a69 6e64 6261 7365  um[..., :indbase
+0000fd00: 7072 655d 290a 2020 2020 2020 2020 2020  pre]).          
+0000fd10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 6261 7365 6c69 6e65 203d 2030 0a0a 2020  baseline = 0..  
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+0000fd50: 2e70 6c6f 7428 7420 2a20 3165 362c 2074  .plot(t * 1e6, t
+0000fd60: 7261 6365 5f73 756d 202a 2031 6536 2c20  race_sum * 1e6, 
+0000fd70: 6c61 6265 6c3d 2253 756d 6d65 6420 4368  label="Summed Ch
+0000fd80: 616e 6e65 6c73 2229 0a20 2020 2020 2020  annels").       
+0000fd90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000fda0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+0000fdb0: 7320 3d20 706c 742e 636d 2e76 6972 6964  s = plt.cm.virid
+0000fdc0: 6973 280a 2020 2020 2020 2020 2020 2020  is(.            
+0000fdd0: 2020 2020 2020 2020 6e70 2e6c 696e 7370          np.linsp
+0000fde0: 6163 6528 302c 2031 2c20 6e75 6d3d 782e  ace(0, 1, num=x.
+0000fdf0: 7368 6170 655b 315d 292c 0a20 2020 2020  shape[1]),.     
+0000fe00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000fe10: 6c70 6861 3d30 2e35 2c0a 2020 2020 2020  lpha=0.5,.      
+0000fe20: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000fe30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000fe40: 6a6a 2c20 6368 616e 2069 6e20 656e 756d  jj, chan in enum
+0000fe50: 6572 6174 6528 6368 616e 6e65 6c73 293a  erate(channels):
+0000fe60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fe70: 2020 2020 206c 6162 656c 203d 2066 2243       label = f"C
+0000fe80: 6861 6e6e 656c 207b 6368 616e 7d22 0a0a  hannel {chan}"..
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 2020 2020 6966 2069 6e64 6261 7365 7072      if indbasepr
+0000feb0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fed0: 2020 2020 2020 2062 6173 656c 696e 6520         baseline 
+0000fee0: 3d20 6e70 2e6d 6561 6e28 785b 6969 2c20  = np.mean(x[ii, 
+0000fef0: 6a6a 2c20 3a69 6e64 6261 7365 7072 655d  jj, :indbasepre]
+0000ff00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ff10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff30: 2020 2020 6261 7365 6c69 6e65 203d 2030      baseline = 0
+0000ff40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ff50: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff70: 2020 2020 2020 2074 202a 2031 6536 2c0a         t * 1e6,.
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2020 2020 2020 2020 785b 6969 2c20 6a6a          x[ii, jj
+0000ffa0: 5d20 2a20 3165 3620 2d20 6261 7365 6c69  ] * 1e6 - baseli
+0000ffb0: 6e65 202a 2031 6536 2c0a 2020 2020 2020  ne * 1e6,.      
+0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffd0: 2020 636f 6c6f 723d 636f 6c6f 7273 5b6a    color=colors[j
+0000ffe0: 6a5d 2c0a 2020 2020 2020 2020 2020 2020  j],.            
+0000fff0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00010000: 6c3d 6c61 6265 6c2c 0a20 2020 2020 2020  l=label,.       
+00010010: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00010020: 2020 2020 2020 2020 2020 2061 782e 6772             ax.gr
+00010030: 6964 2829 0a20 2020 2020 2020 2020 2020  id().           
+00010040: 2061 782e 7365 745f 796c 6162 656c 2822   ax.set_ylabel("
+00010050: 4375 7272 656e 7420 5bce bc41 5d22 290a  Current [..A]").
+00010060: 2020 2020 2020 2020 2020 2020 6178 2e73              ax.s
+00010070: 6574 5f78 6c61 6265 6c28 2254 696d 6520  et_xlabel("Time 
+00010080: 5bce bc73 5d22 290a 2020 2020 2020 2020  [..s]").        
+00010090: 2020 2020 6178 2e73 6574 5f74 6974 6c65      ax.set_title
+000100a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000100b0: 2020 6622 5075 6c73 6573 2c20 4576 7420    f"Pulses, Evt 
+000100c0: 4e75 6d20 7b65 7674 6e75 6d73 5b63 7261  Num {evtnums[cra
+000100d0: 6e64 5d2e 696c 6f63 5b69 695d 7d2c 2022  nd].iloc[ii]}, "
+000100e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000100f0: 2066 2253 6572 6965 7320 4e75 6d20 7b73   f"Series Num {s
+00010100: 6572 6965 736e 756d 735b 6372 616e 645d  eriesnums[crand]
+00010110: 2e69 6c6f 635b 6969 5d7d 220a 2020 2020  .iloc[ii]}".    
+00010120: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00010130: 2020 2020 2020 6178 2e6c 6567 656e 6428        ax.legend(
+00010140: 290a 0a20 2020 2072 6574 7572 6e20 742c  )..    return t,
+00010150: 2078 2c20 6372 616e 640a 2020 0a          x, crand.  .
```

### Comparing `pytesdaq-0.2.9/pytesdaq/io/redis.py` & `pytesdaq-0.3.0/pytesdaq/io/redis.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/processing/_iv_didv_tools.py` & `pytesdaq-0.3.0/pytesdaq/processing/_iv_didv_tools.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/processing/_iv_didv_tools_plotting.py` & `pytesdaq-0.3.0/pytesdaq/processing/_iv_didv_tools_plotting.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/processing/_process_iv_didv.py` & `pytesdaq-0.3.0/pytesdaq/processing/_process_iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/processing/trigger.py` & `pytesdaq-0.3.0/pytesdaq/processing/trigger.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/scope/readout.py` & `pytesdaq-0.3.0/pytesdaq/scope/readout.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/scope/scope.py` & `pytesdaq-0.3.0/pytesdaq/scope/scope.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/sequencer/iv_didv.py` & `pytesdaq-0.3.0/pytesdaq/sequencer/iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/sequencer/sequencer.py` & `pytesdaq-0.3.0/pytesdaq/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/sequencer/tc.py` & `pytesdaq-0.3.0/pytesdaq/sequencer/tc.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/utils/arg_utils.py` & `pytesdaq-0.3.0/pytesdaq/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/utils/connection_utils.py` & `pytesdaq-0.3.0/pytesdaq/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq/utils/remote.py` & `pytesdaq-0.3.0/pytesdaq/utils/remote.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/pytesdaq.egg-info/PKG-INFO` & `pytesdaq-0.3.0/pytesdaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.2.9
+Version: 0.3.0
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.2.9/pytesdaq.egg-info/SOURCES.txt` & `pytesdaq-0.3.0/pytesdaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.2.9/setup.py` & `pytesdaq-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
       long_description = f.read()
 
 
 setup(name='pytesdaq',
-      version='0.2.9',
+      version='0.3.0',
       description='DAQ and Intruments control for TES development',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Bruno Serfass',
       author_email='serfass@berkeley.edu',
       url="https://github.com/spice-herald/pytesdaq",
       zip_safe = False,
```

