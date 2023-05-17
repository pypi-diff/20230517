# Comparing `tmp/solox-2.6.2.tar.gz` & `tmp/solox-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-od_7kf29/solox-2.6.2.tar", last modified: Fri May  5 03:08:10 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-rb7jp8we/solox-2.6.3.tar", last modified: Wed May 17 01:23:16 2023, max compression
```

## Comparing `solox-2.6.2.tar` & `solox-2.6.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-05 03:08:00.000000 solox-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 03:08:00.000000 solox-2.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-05 03:08:10.000000 solox-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-05 03:08:00.000000 solox-2.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-05 03:08:10.000000 solox-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 03:08:00.000000 solox-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 03:08:00.000000 solox-2.6.2/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 03:08:00.000000 solox-2.6.2/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-05 03:08:00.000000 solox-2.6.2/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/analysis_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)   100609 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 03:08:00.000000 solox-2.6.2/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-05-05 03:08:00.000000 solox-2.6.2/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-05 03:08:00.000000 solox-2.6.2/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-05 03:08:00.000000 solox-2.6.2/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-17 01:23:07.000000 solox-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-17 01:23:07.000000 solox-2.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-17 01:23:16.000000 solox-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-17 01:23:07.000000 solox-2.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-17 01:23:16.000000 solox-2.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-17 01:23:07.000000 solox-2.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 01:23:07.000000 solox-2.6.3/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-17 01:23:07.000000 solox-2.6.3/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-17 01:23:07.000000 solox-2.6.3/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-17 01:23:07.000000 solox-2.6.3/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-17 01:23:07.000000 solox-2.6.3/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33714 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   101070 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-17 01:23:07.000000 solox-2.6.3/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 01:23:07.000000 solox-2.6.3/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-05-17 01:23:07.000000 solox-2.6.3/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-17 01:23:07.000000 solox-2.6.3/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-17 01:23:07.000000 solox-2.6.3/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 01:23:16.000000 solox-2.6.3/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.2/LICENSE` & `solox-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/PKG-INFO` & `solox-2.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.2
+Version: 2.6.3
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -40,24 +40,24 @@
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
-💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
+💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4. 
 
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox 
+pip install -U solox  (pip install solox==2.6.2)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
@@ -138,14 +138,16 @@
 * **Data Integrality:** We provide the data about CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
 * **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
 * **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
 * **PK Model:** Supports simultaneous comparative testing of two mobile devices.
   - 🌱2-devices: test the same app on two different phones.
   - 🌱2-apps: test two different apps on two phones with the same configuration.
 
+* **Collect in python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
+
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
```

### Comparing `solox-2.6.2/README.md` & `solox-2.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
-💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
+💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4. 
 
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox 
+pip install -U solox  (pip install solox==2.6.2)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
@@ -123,14 +123,16 @@
 * **Data Integrality:** We provide the data about CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
 * **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
 * **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
 * **PK Model:** Supports simultaneous comparative testing of two mobile devices.
   - 🌱2-devices: test the same app on two different phones.
   - 🌱2-apps: test two different apps on two phones with the same configuration.
 
+* **Collect in python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
+
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
```

### Comparing `solox-2.6.2/setup.py` & `solox-2.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/__main__.py` & `solox-2.6.3/solox/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from __future__ import absolute_import
 from logzero import logger
 import platform
 import fire as fire
 
 def checkPyVer():
     versions = platform.python_version().split('.')
-    if int(versions[0]) < 3:
-        logger.error('python version must be 3.10+ ,your python version is {}'.format(platform.python_version()))
-        logger.info('https://github.com/smart-test-ti/SoloX/blob/master/README.md#requirements')
-        return False
-    elif int(versions[1]) < 10:
+    if int(versions[0]) < 3 or int(versions[1]) < 10:
         logger.error('python version must be 3.10+ ,your python version is {}'.format(platform.python_version()))
         logger.info('https://github.com/smart-test-ti/SoloX/blob/master/README.md#requirements')
         return False
     return True    
 
 if __name__ == '__main__':
     check = checkPyVer()
```

### Comparing `solox-2.6.2/solox/debug.py` & `solox-2.6.3/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/_iosPerf.py` & `solox-2.6.3/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/adb/mac/adb` & `solox-2.6.3/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/adb.py` & `solox-2.6.3/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/apm.py` & `solox-2.6.3/solox/public/apm.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,77 +426,81 @@
             gpu = _gpu.getGPU(noLog=self.noLog)
             result = {'gpu': gpu}
             logger.info(f'gpu: {result}')
             if time.time() > self.end_time:
                 break
         return result
     
+    def setPerfs(self):
+        match(self.platform):
+            case Platform.Android:
+                adb.shell(cmd='dumpsys battery reset', deviceId=self.deviceId)
+                _flow = Flow(self.pkgName, self.deviceId, self.platform, pid=self.pid)
+                data = _flow.setAndroidNet()
+                f.record_net('end', data[0], data[1])
+                scene = f.make_report(app=self.pkgName, devices=self.deviceId,
+                                      platform=self.platform, model='normal')
+                summary = f._setAndroidPerfs(scene)
+                summary_dict = {}
+                summary_dict['cpu_app'] = summary['cpuAppRate']
+                summary_dict['cpu_sys'] = summary['cpuSystemRate']
+                summary_dict['mem_total'] = summary['totalPassAvg']
+                summary_dict['mem_native'] = summary['nativePassAvg']
+                summary_dict['mem_dalvik'] = summary['dalvikPassAvg']
+                summary_dict['fps'] = summary['fps']
+                summary_dict['jank'] = summary['jank']
+                summary_dict['level'] = summary['batteryLevel']
+                summary_dict['tem'] = summary['batteryTeml']
+                summary_dict['net_send'] = summary['flow_send']
+                summary_dict['net_recv'] = summary['flow_recv']
+                summary_dict['cpu_charts'] = f.getCpuLog(Platform.Android, scene)
+                summary_dict['mem_charts'] = f.getMemLog(Platform.Android, scene)
+                summary_dict['net_charts'] = f.getFlowLog(Platform.Android, scene)
+                summary_dict['battery_charts'] = f.getBatteryLog(Platform.Android, scene)
+                summary_dict['fps_charts'] = f.getFpsLog(Platform.Android, scene)['fps']
+                summary_dict['jank_charts'] = f.getFpsLog(Platform.Android, scene)['jank']
+                f.make_android_html(scene=scene, summary=summary_dict)
+            case Platform.iOS:
+                scene = f.make_report(app=self.pkgName, devices=self.deviceId, 
+                                      platform=self.platform, model='normal')
+                summary = f._setiOSPerfs(scene)
+                summary_dict = {}
+                summary_dict['cpu_app'] = summary['cpuAppRate']
+                summary_dict['cpu_sys'] = summary['cpuSystemRate']
+                summary_dict['mem_total'] = summary['totalPassAvg']
+                summary_dict['fps'] = summary['fps']
+                summary_dict['current'] = summary['batteryCurrent']
+                summary_dict['voltage'] = summary['batteryVoltage']
+                summary_dict['power'] = summary['batteryPower']
+                summary_dict['tem'] = summary['batteryTeml']
+                summary_dict['gpu'] = summary['gpu']
+                summary_dict['net_send'] = summary['flow_send']
+                summary_dict['net_recv'] = summary['flow_recv']
+                summary_dict['cpu_charts'] = f.getCpuLog(Platform.iOS, scene)
+                summary_dict['mem_charts'] = f.getMemLog(Platform.iOS, scene)
+                summary_dict['net_charts'] = f.getFlowLog(Platform.iOS, scene)
+                summary_dict['battery_charts'] = f.getBatteryLog(Platform.iOS, scene)
+                summary_dict['fps_charts'] = f.getFpsLog(Platform.iOS, scene)
+                summary_dict['gpu_charts'] = f.getGpuLog(Platform.iOS, scene)
+                f.make_ios_html(scene=scene, summary=summary_dict)
+            case _:
+                raise Exception('platfrom is invalid') 
 
     def collectAll(self):
         try:
             f.clear_file()
             pool = multiprocessing.Pool(processes=6)
             pool.apply_async(self.collectCpu)
             pool.apply_async(self.collectMemory)
             pool.apply_async(self.collectBattery)
             pool.apply_async(self.collectFps)
             pool.apply_async(self.collectFlow)
             pool.apply_async(self.collectGpu)
             pool.close()
             pool.join()
-            match(self.platform):
-                case Platform.Android:
-                    adb.shell(cmd='dumpsys battery reset', deviceId=self.deviceId)
-                    _flow = Flow(self.pkgName, self.deviceId, self.platform, pid=self.pid)
-                    data = _flow.setAndroidNet()
-                    f.record_net('end', data[0], data[1])
-                    scene = f.make_report(app=self.pkgName, devices=self.deviceId, 
-                                          platform=self.platform, model='normal')
-                    summary = f._setAndroidPerfs(scene)
-                    summary_dict = {}
-                    summary_dict['cpu_app'] = summary['cpuAppRate']
-                    summary_dict['cpu_sys'] = summary['cpuSystemRate']
-                    summary_dict['mem_total'] = summary['totalPassAvg']
-                    summary_dict['mem_native'] = summary['nativePassAvg']
-                    summary_dict['mem_dalvik'] = summary['dalvikPassAvg']
-                    summary_dict['fps'] = summary['fps']
-                    summary_dict['jank'] = summary['jank']
-                    summary_dict['level'] = summary['batteryLevel']
-                    summary_dict['tem'] = summary['batteryTeml']
-                    summary_dict['net_send'] = summary['flow_send']
-                    summary_dict['net_recv'] = summary['flow_recv']
-                    summary_dict['cpu_charts'] = f.getCpuLog(Platform.Android, scene)
-                    summary_dict['mem_charts'] = f.getMemLog(Platform.Android, scene)
-                    summary_dict['net_charts'] = f.getFlowLog(Platform.Android, scene)
-                    summary_dict['battery_charts'] = f.getBatteryLog(Platform.Android, scene)
-                    summary_dict['fps_charts'] = f.getFpsLog(Platform.Android, scene)['fps']
-                    summary_dict['jank_charts'] = f.getFpsLog(Platform.Android, scene)['jank']
-                    f.make_android_html(scene=scene, summary=summary_dict)
-                case Platform.iOS:
-                    scene = f.make_report(app=self.pkgName, devices=self.deviceId, 
-                                          platform=self.platform, model='normal')
-                    summary = f._setiOSPerfs(scene)
-                    summary_dict = {}
-                    summary_dict['cpu_app'] = summary['cpuAppRate']
-                    summary_dict['cpu_sys'] = summary['cpuSystemRate']
-                    summary_dict['mem_total'] = summary['totalPassAvg']
-                    summary_dict['fps'] = summary['fps']
-                    summary_dict['current'] = summary['batteryCurrent']
-                    summary_dict['voltage'] = summary['batteryVoltage']
-                    summary_dict['power'] = summary['batteryPower']
-                    summary_dict['tem'] = summary['batteryTeml']
-                    summary_dict['gpu'] = summary['gpu']
-                    summary_dict['net_send'] = summary['flow_send']
-                    summary_dict['net_recv'] = summary['flow_recv']
-                    summary_dict['cpu_charts'] = f.getCpuLog(Platform.iOS, scene)
-                    summary_dict['mem_charts'] = f.getMemLog(Platform.iOS, scene)
-                    summary_dict['net_charts'] = f.getFlowLog(Platform.iOS, scene)
-                    summary_dict['battery_charts'] = f.getBatteryLog(Platform.iOS, scene)
-                    summary_dict['fps_charts'] = f.getFpsLog(Platform.iOS, scene)
-                    summary_dict['gpu_charts'] = f.getGpuLog(Platform.iOS, scene)
-                    f.make_ios_html(scene=scene, summary=summary_dict)
-                case _:
-                    raise Exception('platfrom is invalid')        
+            self.setPerfs()     
         except KeyboardInterrupt:
-            logger.info('End of testing')
+            self.setPerfs()
         except Exception:
-            traceback.print_exc()
+            traceback.print_exc()
+        finally:
+            logger.info('End of testing')
```

### Comparing `solox-2.6.2/solox/public/apm_pk.py` & `solox-2.6.3/solox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/common.py` & `solox-2.6.3/solox/public/common.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/fps.py` & `solox-2.6.3/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/__main__.py` & `solox-2.6.3/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_crash.py` & `solox-2.6.3/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_device.py` & `solox-2.6.3/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_hexdump.py` & `solox-2.6.3/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_imagemounter.py` & `solox-2.6.3/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_installation.py` & `solox-2.6.3/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_instruments.py` & `solox-2.6.3/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_ipautil.py` & `solox-2.6.3/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_perf.py` & `solox-2.6.3/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_proto.py` & `solox-2.6.3/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_relay.py` & `solox-2.6.3/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_safe_socket.py` & `solox-2.6.3/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_ssl.py` & `solox-2.6.3/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_sync.py` & `solox-2.6.3/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_types.py` & `solox-2.6.3/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_usbmux.py` & `solox-2.6.3/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_utils.py` & `solox-2.6.3/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.3/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/bplist.py` & `solox-2.6.3/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/exceptions.py` & `solox-2.6.3/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/plistlib2.py` & `solox-2.6.3/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.3/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/iosperf/struct2.py` & `solox-2.6.3/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/report_template/android.html` & `solox-2.6.3/solox/public/report_template/android.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/public/report_template/ios.html` & `solox-2.6.3/solox/public/report_template/ios.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/highlight.min.css` & `solox-2.6.3/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.3/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/select2.min.css` & `solox-2.6.3/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/sweetalert2.min.css` & `solox-2.6.3/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/tabler.demo.min.css` & `solox-2.6.3/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/css/tabler.min.css` & `solox-2.6.3/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/404.png` & `solox-2.6.3/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/500.png` & `solox-2.6.3/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/avatar.png` & `solox-2.6.3/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/coffee.png` & `solox-2.6.3/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/empty.png` & `solox-2.6.3/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/readme/home.png` & `solox-2.6.3/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/image/readme/pk.png` & `solox-2.6.3/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/apexcharts.js` & `solox-2.6.3/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/gray.js` & `solox-2.6.3/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/highlight.min.js` & `solox-2.6.3/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/highstock.js` & `solox-2.6.3/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/html2canvas.min.js` & `solox-2.6.3/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/jquery.min.js` & `solox-2.6.3/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/select2.min.js` & `solox-2.6.3/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/socket.io.js` & `solox-2.6.3/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/sweetalert2.min.js` & `solox-2.6.3/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/tabler.demo.min.js` & `solox-2.6.3/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/js/tabler.min.js` & `solox-2.6.3/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/static/logo/logo.png` & `solox-2.6.3/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/404.html` & `solox-2.6.3/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/500.html` & `solox-2.6.3/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/analysis.html` & `solox-2.6.3/solox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/analysis_compare.html` & `solox-2.6.3/solox/templates/analysis_compare.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/analysis_pk.html` & `solox-2.6.3/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/base.html` & `solox-2.6.3/solox/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 <div class="d-flex flex-column flex-md-row flex-fill align-items-stretch align-items-md-center">
                     {% block navbar_nav %}{% endblock %}
                 </div>
             </div>
             {% if model in ['2-app','2-devices'] %}
             <div class="nav-item dropdown d-none d-md-flex me-3">
                 <a  href="/?platform=Android&lan={{ lan }}" class="btn  btn-pill w-100" >
-                    <svg t="1682331413507" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="9942" width="50" height="50"><path d="M512.149985 512.049995m-511.950005 0a511.950005 511.950005 0 1 0 1023.90001 0 511.950005 511.950005 0 1 0-1023.90001 0Z" fill="#1BAF96" p-id="9943"></path><path d="M634.738014 267.273899l-122.288058 265.974026L440.956938 734.92823l-125.087785 37.796309L286.971975 782.923543l-13.998633 23.997656 314.16932 211.579338c247.175862-36.296455 436.957328-249.175666 436.957328-506.450542 0-39.596133-4.499561-78.192364-12.99873-115.288741L740.927644 208.979592l-106.18963 58.294307z" fill="#199E85" p-id="9944"></path><path d="M650.03652 582.14315l-59.3942-56.894444c-13.998633-13.398692 0-27.197344 0-27.197344l63.79377-60.994043c43.295772-41.395957 41.495948-101.79006 41.495948-101.79006V256.974905l-183.382092-15.298506L329.167855 256.974905v78.292354s-1.799824 60.294112 41.495947 101.79006l63.793771 60.994043s13.998633 13.798652 0 27.197344L374.963382 582.14315s-45.795528 43.495752-45.795527 112.888976v77.692413h366.664193v-77.692413c0-69.393223-45.795528-112.888976-45.795528-112.888976z" fill="#FFFFFF" p-id="9945"></path><path d="M497.25144 679.83361l0.499951-168.083586c0.19998-31.496924-14.598574-51.394981-20.298017-57.094424L412.959672 392.961625c-21.897862-20.897959-22.697783-55.494581-22.697784-55.794551h244.476126s-0.399961 34.496631-22.697784 55.794551l-63.79377 60.994043c-6.499365 6.399375-20.797969 26.297432-20.597988 57.794356v168.083586h-30.397032z" fill="#4F5D73" p-id="9946"></path><path d="M757.026072 236.676887c0 16.89835-13.698662 30.597012-30.597012 30.597012H298.570843c-16.89835 0-30.597012-13.698662-30.597012-30.597012s13.698662-30.597012 30.597012-30.597012h427.758226c16.99834 0.09999 30.697002 13.798652 30.697003 30.597012z m0 550.046285c0 16.89835-13.698662 30.597012-30.597012 30.597012H298.570843c-16.89835 0-30.597012-13.698662-30.597012-30.597012 0-16.89835 13.698662-30.597012 30.597012-30.597012h427.758226c16.99834 0.09999 30.697002 13.798652 30.697003 30.597012z" fill="#F2B955" p-id="9947"></path><path d="M650.03652 756.22615H374.963382L512.549946 633.938092l137.486574 122.288058z" fill="#4F5D73" p-id="9948"></path></svg>
+                    <svg t="1684145849174" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="12372" width="50" height="50"><path d="M512 64C264.576 64 64 264.576 64 512s200.576 448 448 448 448-200.576 448-448S759.424 64 512 64z" fill="#94BFFF" p-id="12373"></path><path d="M498.56 519.666a10.668 10.668 0 0 1 0-15.332c21.718-21.126 84.97-82.904 148.374-147.128 14.336-14.516 19.86-35.152 7.744-51.408-4.972-6.654-11.584-14.192-20.352-22.284-11.926-11.014-23.296-18.38-32.768-23.28-15.51-8.02-33.686-3.928-47.766 6.24-110.25 79.572-185.43 165.484-221.802 211.612-15.98 20.29-15.98 47.538 0 67.828 36.372 46.128 111.552 132.04 221.802 211.614 14.08 10.166 32.256 14.256 47.766 6.238 9.472-4.9 20.842-12.266 32.768-23.28 8.768-8.092 15.38-15.63 20.352-22.284 12.116-16.256 6.592-36.892-7.744-51.406-63.404-64.226-126.656-126.004-148.374-147.13z" fill="#1677FF" p-id="12374"></path></svg>
                     {% if lan == 'cn' %} 普通模式 {% else %} Normal Model {% endif %}
                 </a>
             </div>
             {% else %}
             <div class="nav-item dropdown d-none d-md-flex me-3">
                 <a href="/pk?model=2-devices&lan={{ lan }}" class="btn  btn-pill w-100" >
                     <svg t="1661854041585" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="10784" width="2000" height="2000"><path d="M17.408 862.208a450.56 129.024 0 1 0 901.12 0 450.56 129.024 0 1 0-901.12 0Z" fill="#EEF2FF" p-id="10785"></path><path d="M509.952 880.64H75.776c-17.408 0-30.72-13.312-30.72-30.72V293.888c0-64.512 52.224-116.736 116.736-116.736h522.24c35.84 0 64.512 28.672 64.512 64.512v400.384C748.544 774.144 642.048 880.64 509.952 880.64z" fill="#70D4FF" p-id="10786"></path><path d="M764.928 880.64H212.992c-17.408 0-30.72-13.312-30.72-30.72V60.416h755.712c35.84 0 64.512 28.672 64.512 64.512v517.12C1002.496 774.144 896 880.64 764.928 880.64z" fill="#4E8EFF" p-id="10787"></path><path d="M555.008 403.456c0 20.48-7.168 35.84-22.528 48.128-14.336 11.264-30.72 16.384-51.2 16.384h-28.672v48.128c0 9.216 2.048 15.36 6.144 19.456 4.096 4.096 11.264 5.12 21.504 5.12V563.2H373.76v-22.528c15.36 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-23.552-24.576v-22.528h109.568c19.456 0 35.84 5.12 49.152 15.36 14.336 12.288 22.528 27.648 22.528 46.08z m-59.392 2.048c0-26.624-11.264-39.936-34.816-39.936h-9.216v80.896h11.264c13.312 0 22.528-3.072 26.624-10.24 4.096-7.168 6.144-17.408 6.144-30.72zM800.768 563.2h-60.416c-8.192-7.168-15.36-15.36-21.504-22.528l-57.344-74.752v50.176c0 16.384 9.216 24.576 26.624 24.576V563.2H584.704v-22.528c16.384 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-24.576-24.576v-22.528h105.472v22.528c-17.408 0-26.624 8.192-26.624 24.576v50.176l39.936-37.888c13.312-12.288 19.456-21.504 19.456-27.648 0-5.12-5.12-8.192-15.36-8.192v-22.528h81.92v22.528c-9.216 0-15.36 1.024-20.48 4.096-3.072 2.048-8.192 6.144-15.36 13.312L705.536 430.08l70.656 94.208c7.168 9.216 15.36 15.36 25.6 16.384V563.2z" fill="#FFFFFF" p-id="10788"></path></svg>
@@ -126,15 +126,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.2
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.3
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.2
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.3
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
```

### Comparing `solox-2.6.2/solox/templates/index.html` & `solox-2.6.3/solox/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -468,25 +468,29 @@
             }
         });
     }
 
     var timerQ = null;
 
     function getCpuRate(pkgname,device){
+        var process = '';
+        if(platform == 'Android'){
+            process = $('.select-pid').val()
+        }
         $.ajax({
             url: Host + "/apm/cpu",
             type: "GET",
             async: true,
             cache: false,
             data:{
                 model:'normal',
                 platform:platform,
                 pkgname:pkgname,
                 device:device,
-                process:$('.select-pid').val()
+                process:process
             },
             beforeSend: function () {
                window.clearTimeout(timerQ);
             },
             success: function (data) {
                 console.log(data)
                 if(stop == false){
@@ -601,25 +605,29 @@
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
         });
     }
 
     function getMemPss(pkgname,device)  {
+        var process = '';
+        if(platform == 'Android'){
+            process = $('.select-pid').val()
+        }
         $.ajax({
             url: Host + "/apm/mem",
             type: "GET",
             async: true,
             cache: false,
             data:{
                 model:'normal',
                 platform:platform,
                 pkgname:pkgname,
                 device:device,
-                process:$('.select-pid').val()
+                process:process
             },
             beforeSend: function () {
                window.clearTimeout(timerQ);
             },
             success: function (data) {
                 console.log(data)
                 if(stop == false){
@@ -654,52 +662,60 @@
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
         });
     }
 
     function setNetWork(type,device,pkgname,net_switch){
+        var process = '';
+        if(platform == 'Android'){
+            process = $('.select-pid').val()
+        }
         $.ajax({
             url: Host + "/apm/set/network",
             type: "GET",
             async: true,
             cache: false,
             data:{
                 platform:platform,
                 pkgname:pkgname,
                 device:device,
                 wifi_switch: net_switch,
                 type: type,
-                process:$('.select-pid').val()
+                process:process
             },
             success: function (data) {
                 if(data['status'] != 1){
                     SwalFire('error','something error',data['msg'],2000);
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
         });
     }
 
     function getNetWork(pkgname,device,net_switch)  {
+        var process = '';
+        if(platform == 'Android'){
+            process = $('.select-pid').val()
+        }
         $.ajax({
             url: Host + "/apm/network",
             type: "GET",
             async: true,
             cache: false,
             data:{
                 model:'normal',
                 platform:platform,
                 pkgname:pkgname,
                 device:device,
                 wifi_switch: net_switch,
-                process:$('.select-pid').val()
+                process:process
             },
             beforeSend: function () {
                window.clearTimeout(timerQ);
             },
             success: function (data) {
                 if(stop == false){
                     if(data['status'] == 1){
@@ -1390,15 +1406,17 @@
         $('#stop-apm').show();
         $('#run-apm').hide();
         initializeAPM();
         let device = $('.select-device').val();
         let pkgname = $('.select-app').val();
         if(device && pkgname){
             var net_switch = $('#net-switch').is(':checked');
-            setNetWork('pre',device,pkgname,net_switch)
+            if(platform == 'Android'){
+                setNetWork('pre',device,pkgname,net_switch)
+            }
             collectCpu(device,pkgname);
             collectMem(device,pkgname);
             collectNetwork(device,pkgname);
             collectFps(device,pkgname);
             collectBattery(device);
             if(platform == 'iOS'){
                 collectGpu(pkgname);
```

### Comparing `solox-2.6.2/solox/templates/pk.html` & `solox-2.6.3/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/templates/report.html` & `solox-2.6.3/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/view/apis.py` & `solox-2.6.3/solox/view/apis.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
 @api.route('/apm/cpu', methods=['post', 'get'])
 def getCpuRate():
     """get process cpu rate"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
-    process = method._request(request, 'process')
     try:
         match(model):
             case '2-devices':
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
@@ -186,14 +185,15 @@
                 pkgNameList = pkgname.split(',')
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 cpu = CPU_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = cpu.getAndroidCpuRate()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
+                process = method._request(request, 'process')
                 deviceId = d.getIdbyDevice(device, platform)
                 pid = process.split(':')[0] if platform == Platform.Android else None
                 cpu = CPU(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 appCpuRate, systemCpuRate = cpu.getCpuRate()
                 result = {'status': 1, 'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}        
     except Exception:
         logger.error('get cpu failed')
@@ -205,15 +205,14 @@
 @api.route('/apm/mem', methods=['post', 'get'])
 def getMEM():
     """get memery data"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
-    process = method._request(request, 'process')
     try:
         match(model):
             case '2-devices':
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
@@ -224,14 +223,15 @@
                 pkgNameList = pkgname.split(',')
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 mem = MEM_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = mem.getProcessMem()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
+                process = method._request(request, 'process')
                 deviceId = d.getIdbyDevice(device, platform)
                 pid = process.split(':')[0] if platform == Platform.Android else None
                 mem = MEM(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 totalPass, nativePass, dalvikPass = mem.getProcessMem()
                 result = {'status': 1, 'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}        
     except Exception:
         logger.error('get memory data failed')
@@ -265,15 +265,14 @@
 def getNetWorkData():
     """get network data"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
     wifi_switch = method._request(request, 'wifi_switch')
-    process = method._request(request, 'process')
     try:
         wifi = False if wifi_switch == 'false' else True
         match(model):
             case '2-devices':
                 pkgNameList = []
                 pkgNameList.append(pkgname)
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
@@ -285,14 +284,15 @@
                 pkgNameList = pkgname.split(',')
                 deviceId1 = d.getIdbyDevice(device.split(',')[0], 'Android')
                 deviceId2 = d.getIdbyDevice(device.split(',')[1], 'Android')
                 network = Flow_PK(pkgNameList=pkgNameList, deviceId1=deviceId1, deviceId2=deviceId2)
                 first, second = network.getNetWorkData()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
+                process = method._request(request, 'process')
                 deviceId = d.getIdbyDevice(device, platform)
                 pid = process.split(':')[0] if platform == Platform.Android else None
                 flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 data = flow.getNetWorkData(wifi=wifi,noLog=False)
                 result = {'status': 1, 'upflow': data[0], 'downflow': data[1]}    
     except Exception:
         logger.error('get network data failed')
```

### Comparing `solox-2.6.2/solox/view/pages.py` & `solox-2.6.3/solox/view/pages.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox/web.py` & `solox-2.6.3/solox/web.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.2/solox.egg-info/PKG-INFO` & `solox-2.6.3/solox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.2
+Version: 2.6.3
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -40,24 +40,24 @@
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## 📦Requirements
 
 - Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 - Install adb and configure environment variables (SoloX's  adb may not necessarily fit your computer) [**Download**](https://developer.android.com/studio/releases/platform-tools)
 
-💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
+💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4. 
 
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox 
+pip install -U solox  (pip install solox==2.6.2)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
@@ -138,14 +138,16 @@
 * **Data Integrality:** We provide the data about CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
 * **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
 * **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
 * **PK Model:** Supports simultaneous comparative testing of two mobile devices.
   - 🌱2-devices: test the same app on two different phones.
   - 🌱2-apps: test two different apps on two phones with the same configuration.
 
+* **Collect in python/API:** Support Python and API to collect performance data, helping users easily integrate into automated testing processes.
+
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
 
 - windows: PowerShell
```

### Comparing `solox-2.6.2/solox.egg-info/SOURCES.txt` & `solox-2.6.3/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

