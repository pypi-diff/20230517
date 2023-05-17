# Comparing `tmp/Glances-3.4.0.tar.gz` & `tmp/Glances-3.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Glances-3.4.0.tar", last modified: Tue May 16 07:39:11 2023, max compression
+gzip compressed data, was "Glances-3.4.0.1.tar", last modified: Wed May 17 09:30:02 2023, max compression
```

## Comparing `Glances-3.4.0.tar` & `Glances-3.4.0.1.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.096802 Glances-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-16 07:39:02.000000 Glances-3.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-16 07:39:02.000000 Glances-3.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-05-16 07:39:02.000000 Glances-3.4.0/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.024801 Glances-3.4.0/Glances.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-05-16 07:39:10.000000 Glances-3.4.0/Glances.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-16 07:39:11.000000 Glances-3.4.0/Glances.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:39:10.000000 Glances-3.4.0/Glances.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 07:39:10.000000 Glances-3.4.0/Glances.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-16 07:39:10.000000 Glances-3.4.0/Glances.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 07:39:11.000000 Glances-3.4.0/Glances.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 07:39:02.000000 Glances-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    70446 2023-05-16 07:39:02.000000 Glances-3.4.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-05-16 07:39:11.096802 Glances-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-16 07:39:02.000000 Glances-3.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.024801 Glances-3.4.0/conf/
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-16 07:39:02.000000 Glances-3.4.0/conf/glances.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.028801 Glances-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.048801 Glances-3.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/amp-dropbox.png
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/amp-python-warning.png
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/amp-python.png
--rw-r--r--   0 runner    (1001) docker     (123)    80498 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/amps.png
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/aws.png
--rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/browser.png
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/cloud.png
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/connected.png
--rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/connections.png
--rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/containers.png
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/cpu-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/cpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/disconnected.png
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/diskio.png
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/events.png
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/folders.png
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/fs.png
--rw-r--r--   0 runner    (1001) docker     (123)    56273 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-architecture.excalidraw
--rw-r--r--   0 runner    (1001) docker     (123)   123499 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)   215750 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-flame.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-influxdb.png
--rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-memory-profiling-with-history.png
--rw-r--r--   0 runner    (1001) docker     (123)    31797 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-memory-profiling-without-history.png
--rw-r--r--   0 runner    (1001) docker     (123)   293649 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-responsive-webdesign.png
--rw-r--r--   0 runner    (1001) docker     (123)   357638 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/glances-summary.png
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/gpu.png
--rw-r--r--   0 runner    (1001) docker     (123)   141657 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/grafana.png
--rw-r--r--   0 runner    (1001) docker     (123)   187140 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/graph-load.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/hddtemp.png
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/header.png
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/ip.png
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/irq.png
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/load.png
--rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/loadpercent.png
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/mem-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/mem.png
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/monitored.png
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/network.png
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/per-cpu.png
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/pergpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/ports.png
--rw-r--r--   0 runner    (1001) docker     (123)    63154 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/processlist-extended.png
--rw-r--r--   0 runner    (1001) docker     (123)   160408 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/processlist-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)    53684 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/processlist-top.png
--rw-r--r--   0 runner    (1001) docker     (123)   227401 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/processlist-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)   151590 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/processlist.png
--rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/prometheus_exporter.png
--rw-r--r--   0 runner    (1001) docker     (123)    91914 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/prometheus_server.png
--rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/quicklook-percpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/quicklook.png
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/raid.png
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/reddit.png
--rw-r--r--   0 runner    (1001) docker     (123)  1089975 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/screencast.gif
--rw-r--r--   0 runner    (1001) docker     (123)   265567 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/screenshot-web.png
--rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/screenshot-web2.png
--rw-r--r--   0 runner    (1001) docker     (123)  1098062 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/screenshot-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)   508044 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/sensors.png
--rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/smart.png
--rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/sparkline.png
--rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/trend.png
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/twitter-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_static/wifi.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.048801 Glances-3.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/_templates/links.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.052801 Glances-3.4.0/docs/aoa/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/actions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/amps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/cloud.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/connections.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/cpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/diskio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/folders.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/fs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/gpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/hddtemp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/header.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/irq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/load.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/memory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/network.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/ports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/ps.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/quicklook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/raid.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/smart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/aoa/wifi.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44238 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/cmds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.056801 Glances-3.4.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/dev/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   328258 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/dev/glances-cprofile.png
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/glances.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.060801 Glances-3.4.0/docs/gw/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/couchdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/csv.rst
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/elastic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/graph.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/graphite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/influxdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/json.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/mongodb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/mqtt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/opentsdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/rabbitmq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/restful.rst
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/riemann.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/gw/zeromq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.060801 Glances-3.4.0/docs/man/
--rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/man/glances.1
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 07:39:02.000000 Glances-3.4.0/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.068801 Glances-3.4.0/glances/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.068801 Glances-3.4.0/glances/amps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps/glances_amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps/glances_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps/glances_nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps/glances_systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps/glances_systemv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/amps_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/autodiscover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/cpu_percent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.072801 Glances-3.4.0/glances/exports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_couchdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_restful.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_riemann.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/exports/glances_zeromq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/folder_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outdated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.076802 Glances-3.4.0/glances/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_curses_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_sparklines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_stdout_apidoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_stdout_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_stdout_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_stdout_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/glances_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.080802 Glances-3.4.0/glances/outputs/static/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.080802 Glances-3.4.0/glances/outputs/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/css/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/css/style.scss
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/css/variables.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.080802 Glances-3.4.0/glances/outputs/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/images/glances.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.080802 Glances-3.4.0/glances/outputs/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/App.vue
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.088802 Glances-3.4.0/glances/outputs/static/js/components/
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/help.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-alert.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-amps.vue
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-cloud.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-connections.vue
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-containers.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-cpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-diskio.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-folders.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-fs.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-gpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-ip.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-irq.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-load.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-mem-more.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-mem.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-memswap.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-network.vue
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-now.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-percpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-ports.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-process.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-processcount.vue
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-processlist.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-quicklook.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-raid.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-sensors.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-system.vue
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-uptime.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/components/plugin-wifi.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/filters.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/services.js
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/js/store.js
--rw-r--r--   0 runner    (1001) docker     (123)   445972 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.088802 Glances-3.4.0/glances/outputs/static/public/
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/public/87708faeed9a66b0fcdb.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   444157 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/public/glances.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.088802 Glances-3.4.0/glances/outputs/static/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/templates/index.html.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/outputs/static/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/password_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.096802 Glances-3.4.0/glances/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.096802 Glances-3.4.0/glances/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/containers/glances_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/containers/glances_podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/containers/stats_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_amps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_diskio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_irq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_mem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_memswap.py
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_percpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_processcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    34269 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_processlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_psutilversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_quicklook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_raid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_smart.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/glances_wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:11.096802 Glances-3.4.0/glances/plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/sensors/glances_batpercent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/plugins/sensors/glances_hddtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/ports_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/programs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/static_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/stats_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/stats_client_snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/stats_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/web_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-16 07:39:02.000000 Glances-3.4.0/glances/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 07:39:02.000000 Glances-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:39:11.096802 Glances-3.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4992 2023-05-16 07:39:02.000000 Glances-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-17 09:29:53.000000 Glances-3.4.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-17 09:29:53.000000 Glances-3.4.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-05-17 09:29:53.000000 Glances-3.4.0.1/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.333919 Glances-3.4.0.1/Glances.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 09:30:02.000000 Glances-3.4.0.1/Glances.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-17 09:29:53.000000 Glances-3.4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    70564 2023-05-17 09:29:53.000000 Glances-3.4.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-17 09:30:02.385920 Glances-3.4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-17 09:29:53.000000 Glances-3.4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.333919 Glances-3.4.0.1/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-17 09:29:53.000000 Glances-3.4.0.1/conf/glances.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.337919 Glances-3.4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.353919 Glances-3.4.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amp-dropbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amp-python-warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amp-python.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80498 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/amps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/aws.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/cloud.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/connected.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/connections.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/containers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/cpu-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/cpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/disconnected.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/diskio.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/events.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/folders.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/fs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56273 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-architecture.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (123)   123499 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)   215750 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-flame.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-influxdb.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-memory-profiling-with-history.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31797 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-memory-profiling-without-history.png
+-rw-r--r--   0 runner    (1001) docker     (123)   293649 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-responsive-webdesign.png
+-rw-r--r--   0 runner    (1001) docker     (123)   357638 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/glances-summary.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/gpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)   141657 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/grafana.png
+-rw-r--r--   0 runner    (1001) docker     (123)   187140 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/graph-load.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/hddtemp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/ip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/irq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/load.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/loadpercent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/mem-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/mem.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/monitored.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/per-cpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/pergpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/ports.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63154 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-extended.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160408 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53684 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-top.png
+-rw-r--r--   0 runner    (1001) docker     (123)   227401 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)   151590 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/processlist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/prometheus_exporter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91914 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/prometheus_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/quicklook-percpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/quicklook.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/raid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1089975 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screencast.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   265567 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot-web.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot-web2.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1098062 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)   508044 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/sensors.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/smart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/sparkline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/trend.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/twitter-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_static/wifi.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.353919 Glances-3.4.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/_templates/links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.357920 Glances-3.4.0.1/docs/aoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/amps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/cloud.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/cpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/diskio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/folders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/fs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/hddtemp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/irq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/load.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/memory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/network.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/ports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/ps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/quicklook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/raid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/smart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/aoa/wifi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44115 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/cmds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.357920 Glances-3.4.0.1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/dev/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   328258 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/dev/glances-cprofile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/glances.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.361919 Glances-3.4.0.1/docs/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/couchdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/elastic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/graphite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/influxdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/mongodb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/mqtt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/opentsdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/rabbitmq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/restful.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/riemann.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/gw/zeromq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.361919 Glances-3.4.0.1/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/man/glances.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 09:29:53.000000 Glances-3.4.0.1/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.365920 Glances-3.4.0.1/glances/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.365920 Glances-3.4.0.1/glances/amps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps/glances_systemv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/amps_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/autodiscover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/cpu_percent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.369920 Glances-3.4.0.1/glances/exports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_couchdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_riemann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/exports/glances_zeromq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/folder_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outdated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.369920 Glances-3.4.0.1/glances/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_curses_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_sparklines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_stdout_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/glances_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/css/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/css/style.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/css/variables.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/images/glances.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.373920 Glances-3.4.0.1/glances/outputs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/App.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.377920 Glances-3.4.0.1/glances/outputs/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/help.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-alert.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-amps.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cloud.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-connections.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-containers.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-diskio.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-folders.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-fs.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-gpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ip.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-irq.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-load.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem-more.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-memswap.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-network.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-now.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-percpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ports.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-process.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processcount.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processlist.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-quicklook.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-raid.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-sensors.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-system.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-uptime.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/components/plugin-wifi.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/filters.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/services.js
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/js/store.js
+-rw-r--r--   0 runner    (1001) docker     (123)   445972 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.377920 Glances-3.4.0.1/glances/outputs/static/public/
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/public/87708faeed9a66b0fcdb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   444157 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/public/glances.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.377920 Glances-3.4.0.1/glances/outputs/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/templates/index.html.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/outputs/static/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/password_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/glances/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/glances/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/glances_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/glances_podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/containers/stats_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_amps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_diskio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_irq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_mem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_memswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_percpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_processcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34269 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_processlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_psutilversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_quicklook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_raid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/glances_wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:30:02.385920 Glances-3.4.0.1/glances/plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/sensors/glances_batpercent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/plugins/sensors/glances_hddtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/ports_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/static_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats_client_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/stats_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/web_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-17 09:29:53.000000 Glances-3.4.0.1/glances/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-17 09:29:53.000000 Glances-3.4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:30:02.385920 Glances-3.4.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4992 2023-05-17 09:29:53.000000 Glances-3.4.0.1/setup.py
```

### Comparing `Glances-3.4.0/AUTHORS` & `Glances-3.4.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/CONTRIBUTING.md` & `Glances-3.4.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/COPYING` & `Glances-3.4.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/Glances.egg-info/PKG-INFO` & `Glances-3.4.0.1/Glances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 3.4.0
+Version: 3.4.0.1
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Glances-3.4.0/Glances.egg-info/SOURCES.txt` & `Glances-3.4.0.1/Glances.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/Glances.egg-info/requires.txt` & `Glances-3.4.0.1/Glances.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/NEWS.rst` & `Glances-3.4.0.1/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 ==============================================================================
                                 Glances changelog
 ==============================================================================
 
 ===============
+Version 3.4.0.1
+===============
+
+Bug corrected:
+
+    * 3.4.0 crash on startupwith minimal deps #2401
+
+===============
 Version 3.4.0
 ===============
 
 Enhancements:
 
     * Enhance process "extended stats" display (in Curses interface) #2225
       _You can now *pin* a specific process to the top of the process list_
```

### Comparing `Glances-3.4.0/PKG-INFO` & `Glances-3.4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 3.4.0
+Version: 3.4.0.1
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Glances-3.4.0/README.rst` & `Glances-3.4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/conf/glances.conf` & `Glances-3.4.0.1/conf/glances.conf`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/Makefile` & `Glances-3.4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/amp-dropbox.png` & `Glances-3.4.0.1/docs/_static/amp-dropbox.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/amp-python-warning.png` & `Glances-3.4.0.1/docs/_static/amp-python-warning.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/amp-python.png` & `Glances-3.4.0.1/docs/_static/amp-python.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/amps.png` & `Glances-3.4.0.1/docs/_static/amps.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/aws.png` & `Glances-3.4.0.1/docs/_static/aws.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/browser.png` & `Glances-3.4.0.1/docs/_static/browser.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/cloud.png` & `Glances-3.4.0.1/docs/_static/cloud.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/connected.png` & `Glances-3.4.0.1/docs/_static/connected.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/connections.png` & `Glances-3.4.0.1/docs/_static/connections.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/containers.png` & `Glances-3.4.0.1/docs/_static/containers.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/cpu-wide.png` & `Glances-3.4.0.1/docs/_static/cpu-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/cpu.png` & `Glances-3.4.0.1/docs/_static/cpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/disconnected.png` & `Glances-3.4.0.1/docs/_static/disconnected.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/diskio.png` & `Glances-3.4.0.1/docs/_static/diskio.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/events.png` & `Glances-3.4.0.1/docs/_static/events.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/folders.png` & `Glances-3.4.0.1/docs/_static/folders.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/fs.png` & `Glances-3.4.0.1/docs/_static/fs.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-architecture.excalidraw` & `Glances-3.4.0.1/docs/_static/glances-architecture.excalidraw`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-architecture.png` & `Glances-3.4.0.1/docs/_static/glances-architecture.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-flame.svg` & `Glances-3.4.0.1/docs/_static/glances-flame.svg`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-influxdb.png` & `Glances-3.4.0.1/docs/_static/glances-influxdb.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-memory-profiling-with-history.png` & `Glances-3.4.0.1/docs/_static/glances-memory-profiling-with-history.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-memory-profiling-without-history.png` & `Glances-3.4.0.1/docs/_static/glances-memory-profiling-without-history.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-responsive-webdesign.png` & `Glances-3.4.0.1/docs/_static/glances-responsive-webdesign.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/glances-summary.png` & `Glances-3.4.0.1/docs/_static/glances-summary.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/gpu.png` & `Glances-3.4.0.1/docs/_static/gpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/grafana.png` & `Glances-3.4.0.1/docs/_static/grafana.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/graph-load.svg` & `Glances-3.4.0.1/docs/_static/graph-load.svg`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/hddtemp.png` & `Glances-3.4.0.1/docs/_static/hddtemp.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/header.png` & `Glances-3.4.0.1/docs/_static/header.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/ip.png` & `Glances-3.4.0.1/docs/_static/ip.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/irq.png` & `Glances-3.4.0.1/docs/_static/irq.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/load.png` & `Glances-3.4.0.1/docs/_static/load.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/loadpercent.png` & `Glances-3.4.0.1/docs/_static/loadpercent.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/mem-wide.png` & `Glances-3.4.0.1/docs/_static/mem-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/mem.png` & `Glances-3.4.0.1/docs/_static/mem.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/monitored.png` & `Glances-3.4.0.1/docs/_static/monitored.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/network.png` & `Glances-3.4.0.1/docs/_static/network.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/per-cpu.png` & `Glances-3.4.0.1/docs/_static/per-cpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/pergpu.png` & `Glances-3.4.0.1/docs/_static/pergpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/ports.png` & `Glances-3.4.0.1/docs/_static/ports.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/processlist-extended.png` & `Glances-3.4.0.1/docs/_static/processlist-extended.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/processlist-filter.png` & `Glances-3.4.0.1/docs/_static/processlist-filter.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/processlist-top.png` & `Glances-3.4.0.1/docs/_static/processlist-top.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/processlist-wide.png` & `Glances-3.4.0.1/docs/_static/processlist-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/processlist.png` & `Glances-3.4.0.1/docs/_static/processlist.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/prometheus_exporter.png` & `Glances-3.4.0.1/docs/_static/prometheus_exporter.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/prometheus_server.png` & `Glances-3.4.0.1/docs/_static/prometheus_server.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/quicklook-percpu.png` & `Glances-3.4.0.1/docs/_static/quicklook-percpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/quicklook.png` & `Glances-3.4.0.1/docs/_static/quicklook.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/raid.png` & `Glances-3.4.0.1/docs/_static/raid.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/reddit.png` & `Glances-3.4.0.1/docs/_static/reddit.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/screencast.gif` & `Glances-3.4.0.1/docs/_static/screencast.gif`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/screenshot-web.png` & `Glances-3.4.0.1/docs/_static/screenshot-web.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/screenshot-web2.png` & `Glances-3.4.0.1/docs/_static/screenshot-web2.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/screenshot-wide.png` & `Glances-3.4.0.1/docs/_static/screenshot-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/screenshot.png` & `Glances-3.4.0.1/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/sensors.png` & `Glances-3.4.0.1/docs/_static/sensors.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/smart.png` & `Glances-3.4.0.1/docs/_static/smart.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/sparkline.png` & `Glances-3.4.0.1/docs/_static/sparkline.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/trend.png` & `Glances-3.4.0.1/docs/_static/trend.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/twitter-icon.png` & `Glances-3.4.0.1/docs/_static/twitter-icon.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/_static/wifi.png` & `Glances-3.4.0.1/docs/_static/wifi.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/actions.rst` & `Glances-3.4.0.1/docs/aoa/actions.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/amps.rst` & `Glances-3.4.0.1/docs/aoa/amps.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/connections.rst` & `Glances-3.4.0.1/docs/aoa/connections.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/containers.rst` & `Glances-3.4.0.1/docs/aoa/containers.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/cpu.rst` & `Glances-3.4.0.1/docs/aoa/cpu.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/diskio.rst` & `Glances-3.4.0.1/docs/aoa/diskio.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/events.rst` & `Glances-3.4.0.1/docs/aoa/events.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/folders.rst` & `Glances-3.4.0.1/docs/aoa/folders.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/fs.rst` & `Glances-3.4.0.1/docs/aoa/fs.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/gpu.rst` & `Glances-3.4.0.1/docs/aoa/gpu.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/hddtemp.rst` & `Glances-3.4.0.1/docs/aoa/hddtemp.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/header.rst` & `Glances-3.4.0.1/docs/aoa/header.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/index.rst` & `Glances-3.4.0.1/docs/aoa/index.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/irq.rst` & `Glances-3.4.0.1/docs/aoa/irq.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/load.rst` & `Glances-3.4.0.1/docs/aoa/load.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/memory.rst` & `Glances-3.4.0.1/docs/aoa/memory.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/network.rst` & `Glances-3.4.0.1/docs/aoa/network.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/ports.rst` & `Glances-3.4.0.1/docs/aoa/ports.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/ps.rst` & `Glances-3.4.0.1/docs/aoa/ps.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/quicklook.rst` & `Glances-3.4.0.1/docs/aoa/quicklook.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/sensors.rst` & `Glances-3.4.0.1/docs/aoa/sensors.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/smart.rst` & `Glances-3.4.0.1/docs/aoa/smart.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/aoa/wifi.rst` & `Glances-3.4.0.1/docs/aoa/wifi.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/api.rst` & `Glances-3.4.0.1/docs/api.rst`

 * *Files 8% similar despite different names*

```diff
@@ -70,26 +70,24 @@
       "countmax": None,
       "countmin": 1.0,
       "key": "name",
       "name": "Dropbox",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.3811793327331543},
-      "timer": 1.0034148693084717},
+      "timer": 1.0500612258911133},
      {"count": 0,
       "countmax": 20.0,
       "countmin": None,
       "key": "name",
       "name": "Python",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.3809046745300293}]
-      "timer": 1.003244400024414}]
+      "timer": 1.0497639179229736}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/amps/name
     {"name": ["Dropbox", "Python", "Conntrack", "Nginx", "Systemd", "SystemV"]}
 
 Get a specific item when field matchs the given value::
@@ -99,15 +97,15 @@
                   "countmax": None,
                   "countmin": 1.0,
                   "key": "name",
                   "name": "Dropbox",
                   "refresh": 3.0,
                   "regex": True,
                   "result": None,
-                  "timer": 1.0034148693084717}]}
+                  "timer": 1.0500612258911133}]}
 
 GET connections
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/connections
@@ -126,56 +124,56 @@
     # curl http://localhost:61208/api/3/containers
     {"containers": [{"Command": ["top"],
                      "Created": "2023-05-08T15:29:34.918692365+02:00",
                      "Id": "4b7f732d43e4bc5d92fe5298cba025b550e6a608754c1c38f9a90aaecd46b8f9",
                      "Image": "["docker.io/library/ubuntu:latest"]",
                      "Status": "running",
                      "Uptime": "1 weeks",
-                     "cpu": {"total": 7.811242562687869e-07},
-                     "cpu_percent": 7.811242562687869e-07,
+                     "cpu": {"total": 9.174878746049114e-07},
+                     "cpu_percent": 9.174878746049114e-07,
                      "engine": "podman",
                      "io": {"ior": 0.0, "iow": 0.0, "time_since_update": 1},
                      "io_r": 0.0,
                      "io_w": 0.0,
                      "key": "name",
-                     "memory": {"limit": 7836184576.0, "usage": 1576960.0},
-                     "memory_usage": 1576960.0,
+                     "memory": {"limit": 7836184576.0, "usage": 1548288.0},
+                     "memory_usage": 1548288.0,
                      "name": "frosty_bouman",
                      "network": {"rx": 0.0, "time_since_update": 1, "tx": 0.0},
                      "network_rx": 0.0,
                      "network_tx": 0.0,
                      "pod_id": "8d0f1c783def",
                      "pod_name": "frosty_bouman"},
                     {"Command": [],
                      "Created": "2022-10-22T14:23:03.120912374+02:00",
                      "Id": "9491515251edcd5bb5dc17205d7ee573c0be96fe0b08b0a12a7e2cea874565ea",
                      "Image": "["k8s.gcr.io/pause:3.5"]",
                      "Status": "running",
                      "Uptime": "1 weeks",
-                     "cpu": {"total": 2.630294095569028e-10},
-                     "cpu_percent": 2.630294095569028e-10,
+                     "cpu": {"total": 2.644991475256057e-10},
+                     "cpu_percent": 2.644991475256057e-10,
                      "engine": "podman",
                      "io": {"ior": 0.0, "iow": 0.0, "time_since_update": 1},
                      "io_r": 0.0,
                      "io_w": 0.0,
                      "key": "name",
-                     "memory": {"limit": 7836184576.0, "usage": 454656.0},
-                     "memory_usage": 454656.0,
+                     "memory": {"limit": 7836184576.0, "usage": 434176.0},
+                     "memory_usage": 434176.0,
                      "name": "8d0f1c783def-infra",
                      "network": {"rx": 0.0, "time_since_update": 1, "tx": 0.0},
                      "network_rx": 0.0,
                      "network_tx": 0.0,
                      "pod_id": "8d0f1c783def",
                      "pod_name": "8d0f1c783def-infra"},
                     {"Command": ["/portainer"],
                      "Created": "2022-10-29T14:59:10.266701439Z",
                      "Id": "3abd51c615968482d9ccff5afc629f267f6dda113ed68b75b432615fae3b49fb",
                      "Image": ["portainer/portainer-ce:2.9.3"],
                      "Status": "running",
-                     "Uptime": "3 days",
+                     "Uptime": "4 days",
                      "cpu": {"total": 0.0},
                      "cpu_percent": 0.0,
                      "engine": "docker",
                      "io": {},
                      "io_r": None,
                      "io_w": None,
                      "key": "name",
@@ -212,27 +210,27 @@
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/cpu
     {"cpucore": 4,
      "ctx_switches": 0,
      "guest": 0.0,
      "guest_nice": 0.0,
-     "idle": 73.0,
+     "idle": 66.1,
      "interrupts": 0,
      "iowait": 0.2,
      "irq": 0.0,
      "nice": 0.0,
      "soft_interrupts": 0,
-     "softirq": 0.4,
+     "softirq": 0.0,
      "steal": 0.0,
      "syscalls": 0,
-     "system": 4.1,
+     "system": 6.6,
      "time_since_update": 1,
-     "total": 27.4,
-     "user": 22.7}
+     "total": 35.5,
+     "user": 27.2}
 
 Fields descriptions:
 
 * **total**: Sum of all CPU percentages (except idle) (unit is *percent*)
 * **system**: percent time spent in kernel space. System CPU time is the time spent running code in the Operating System kernel (unit is *percent*)
 * **user**: CPU percent time spent in user space. User CPU time is the time spent on the processor running your program's code (or code in libraries) (unit is *percent*)
 * **iowait**: *(Linux)*: percent time spent by the CPU waiting for I/O operations to complete (unit is *percent*)
@@ -247,15 +245,15 @@
 * **syscalls**: number of system calls per second. Always 0 on Linux OS (unit is *number*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/cpu/total
-    {"total": 27.4}
+    {"total": 35.5}
 
 GET diskio
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/diskio
@@ -293,21 +291,21 @@
 GET fs
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/fs
     [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-      "free": 7953657856,
+      "free": 8354877440,
       "fs_type": "ext4",
       "key": "mnt_point",
       "mnt_point": "/",
-      "percent": 96.6,
+      "percent": 96.4,
       "size": 243334156288,
-      "used": 222993043456},
+      "used": 222591823872},
      {"device_name": "zsfpool",
       "free": 41811968,
       "fs_type": "zfs",
       "key": "mnt_point",
       "mnt_point": "/zsfpool",
       "percent": 0.3,
       "size": 41943040,
@@ -318,21 +316,21 @@
     # curl http://localhost:61208/api/3/fs/mnt_point
     {"mnt_point": ["/", "/zsfpool", "/var/snap/firefox/common/host-hunspell"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/fs/mnt_point//
     {"/": [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-            "free": 7953657856,
+            "free": 8354877440,
             "fs_type": "ext4",
             "key": "mnt_point",
             "mnt_point": "/",
-            "percent": 96.6,
+            "percent": 96.4,
             "size": 243334156288,
-            "used": 222993043456}]}
+            "used": 222591823872}]}
 
 GET ip
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/ip
@@ -351,46 +349,46 @@
 GET load
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/load
     {"cpucore": 4,
-     "min1": 0.55029296875,
-     "min15": 1.06982421875,
-     "min5": 0.85693359375}
+     "min1": 2.630859375,
+     "min15": 1.4560546875,
+     "min5": 1.42822265625}
 
 Fields descriptions:
 
 * **min1**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 1 minute (unit is *float*)
 * **min5**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 5 minutes (unit is *float*)
 * **min15**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 15 minutes (unit is *float*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/load/min1
-    {"min1": 0.55029296875}
+    {"min1": 2.630859375}
 
 GET mem
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/mem
-    {"active": 3109634048,
-     "available": 2829815808,
-     "buffers": 207228928,
-     "cached": 3178246144,
-     "free": 2829815808,
-     "inactive": 3462545408,
-     "percent": 63.9,
-     "shared": 451821568,
+    {"active": 3263430656,
+     "available": 2511720448,
+     "buffers": 743632896,
+     "cached": 2523037696,
+     "free": 2511720448,
+     "inactive": 3192811520,
+     "percent": 67.9,
+     "shared": 627544064,
      "total": 7836184576,
-     "used": 5006368768}
+     "used": 5324464128}
 
 Fields descriptions:
 
 * **total**: Total physical memory available (unit is *bytes*)
 * **available**: The actual amount of available memory that can be given instantly to processes that request more memory in bytes; this is calculated by summing different memory values depending on the platform (e.g. free + buffers + cached on Linux) and it is supposed to be used to monitor actual memory usage in a cross platform fashion (unit is *bytes*)
 * **percent**: The percentage usage calculated as (total - available) / total * 100 (unit is *percent*)
 * **used**: Memory used, calculated differently depending on the platform and designed for informational purposes only (unit is *bytes*)
@@ -409,21 +407,21 @@
 
 GET memswap
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/memswap
-    {"free": 5400473600,
-     "percent": 33.2,
-     "sin": 2319233024,
-     "sout": 4863959040,
+    {"free": 5526786048,
+     "percent": 31.6,
+     "sin": 2906378240,
+     "sout": 5210710016,
      "time_since_update": 1,
      "total": 8082419712,
-     "used": 2681946112}
+     "used": 2555633664}
 
 Fields descriptions:
 
 * **total**: Total swap memory (unit is *bytes*)
 * **used**: Used swap memory (unit is *bytes*)
 * **free**: Free swap memory (unit is *bytes*)
 * **percent**: Used swap memory in percentage (unit is *percent*)
@@ -439,37 +437,37 @@
 GET network
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/network
     [{"alias": None,
-      "cumulative_cx": 130574070,
-      "cumulative_rx": 65287035,
-      "cumulative_tx": 65287035,
-      "cx": 2414,
+      "cumulative_cx": 151835804,
+      "cumulative_rx": 75917902,
+      "cumulative_tx": 75917902,
+      "cx": 6340,
       "interface_name": "lo",
       "is_up": True,
       "key": "interface_name",
-      "rx": 1207,
+      "rx": 3170,
       "speed": 0,
       "time_since_update": 1,
-      "tx": 1207},
+      "tx": 3170},
      {"alias": None,
-      "cumulative_cx": 8162673663,
-      "cumulative_rx": 7914211852,
-      "cumulative_tx": 248461811,
-      "cx": 17399,
+      "cumulative_cx": 8971420885,
+      "cumulative_rx": 8692531338,
+      "cumulative_tx": 278889547,
+      "cx": 32318,
       "interface_name": "wlp2s0",
       "is_up": True,
       "key": "interface_name",
-      "rx": 13173,
+      "rx": 20465,
       "speed": 0,
       "time_since_update": 1,
-      "tx": 4226}]
+      "tx": 11853}]
 
 Fields descriptions:
 
 * **interface_name**: Interface name (unit is *string*)
 * **alias**: Interface alias name (optional) (unit is *string*)
 * **rx**: The received/input rate (in bit per second) (unit is *bps*)
 * **tx**: The sent/output rate (in bit per second) (unit is *bps*)
@@ -491,66 +489,66 @@
                         "mpqemubr0",
                         "vethcddb0e6"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/network/interface_name/lo
     {"lo": [{"alias": None,
-             "cumulative_cx": 130574070,
-             "cumulative_rx": 65287035,
-             "cumulative_tx": 65287035,
-             "cx": 2414,
+             "cumulative_cx": 151835804,
+             "cumulative_rx": 75917902,
+             "cumulative_tx": 75917902,
+             "cx": 6340,
              "interface_name": "lo",
              "is_up": True,
              "key": "interface_name",
-             "rx": 1207,
+             "rx": 3170,
              "speed": 0,
              "time_since_update": 1,
-             "tx": 1207}]}
+             "tx": 3170}]}
 
 GET now
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/now
-    "2023-05-16 09:31:49 CEST"
+    "2023-05-17 11:24:06 CEST"
 
 GET percpu
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/percpu
     [{"cpu_number": 0,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 19.8,
+      "idle": 20.2,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
-      "system": 3.4,
-      "total": 80.2,
-      "user": 76.7},
+      "system": 6.7,
+      "total": 79.8,
+      "user": 73.1},
      {"cpu_number": 1,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 91.2,
+      "idle": 70.6,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
-      "system": 2.7,
-      "total": 8.8,
-      "user": 6.2}]
+      "system": 6.7,
+      "total": 29.4,
+      "user": 22.7}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/percpu/cpu_number
     {"cpu_number": [0, 1, 2, 3]}
 
 GET ports
@@ -561,15 +559,15 @@
     # curl http://localhost:61208/api/3/ports
     [{"description": "DefaultGateway",
       "host": "192.168.1.1",
       "indice": "port_0",
       "port": 0,
       "refresh": 30,
       "rtt_warning": None,
-      "status": 0.005767,
+      "status": 0.005277,
       "timeout": 3}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/ports/host
     {"host": ["192.168.1.1"]}
 
@@ -578,47 +576,47 @@
     # curl http://localhost:61208/api/3/ports/host/192.168.1.1
     {"192.168.1.1": [{"description": "DefaultGateway",
                       "host": "192.168.1.1",
                       "indice": "port_0",
                       "port": 0,
                       "refresh": 30,
                       "rtt_warning": None,
-                      "status": 0.005767,
+                      "status": 0.005277,
                       "timeout": 3}]}
 
 GET processcount
 ----------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/processcount
-    {"pid_max": 0, "running": 1, "sleeping": 315, "thread": 1562, "total": 382}
+    {"pid_max": 0, "running": 1, "sleeping": 316, "thread": 1601, "total": 384}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/processcount/total
-    {"total": 382}
+    {"total": 384}
 
 GET processlist
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/processlist
     [{"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox"],
       "cpu_percent": 0.0,
-      "cpu_times": [5239.7, 1595.52, 4093.05, 570.73, 0.0],
+      "cpu_times": [6652.64, 2012.85, 5052.81, 704.23, 0.0],
       "gids": [1000, 1000, 1000],
-      "io_counters": [3503764480, 5856641024, 0, 0, 0],
+      "io_counters": [4205573120, 6936297472, 0, 0, 0],
       "key": "pid",
-      "memory_info": [468434944, 22123225088, 114802688, 618496, 0, 1282670592, 0],
-      "memory_percent": 5.977844695423366,
+      "memory_info": [507658240, 22263525376, 129363968, 618496, 0, 1405198336, 0],
+      "memory_percent": 6.478385432048301,
       "name": "firefox",
       "nice": 0,
-      "num_threads": 160,
+      "num_threads": 168,
       "pid": 10541,
       "status": "S",
       "time_since_update": 1,
       "username": "nicolargo"},
      {"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox",
                   "-contentproc",
                   "-childID",
@@ -635,239 +633,240 @@
                   "-appDir",
                   "/snap/firefox/2605/usr/lib/firefox/browser",
                   "{c94b5dea-52c6-4c75-a314-5de48bda9cdc}",
                   "10541",
                   "true",
                   "tab"],
       "cpu_percent": 0.0,
-      "cpu_times": [914.43, 104.03, 0.0, 0.0, 0.0],
+      "cpu_times": [1100.17, 125.28, 0.0, 0.0, 0.0],
       "gids": [1000, 1000, 1000],
-      "io_counters": [131410944, 0, 0, 0, 0],
+      "io_counters": [209806336, 0, 0, 0, 0],
       "key": "pid",
-      "memory_info": [438992896, 3601903616, 70893568, 618496, 0, 1002868736, 0],
-      "memory_percent": 5.602125520939235,
+      "memory_info": [406437888, 3516469248, 78082048, 618496, 0, 918466560, 0],
+      "memory_percent": 5.186680891167411,
       "name": "WebExtensions",
       "nice": 0,
       "num_threads": 20,
       "pid": 11043,
       "status": "S",
       "time_since_update": 1,
       "username": "nicolargo"}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/processlist/pid
     {"pid": [10541,
              11043,
+             59195,
              10770,
-             55857,
              10778,
-             181461,
-             59195,
-             3927,
              60503,
+             55857,
+             3927,
              10774,
              59454,
-             195248,
-             228679,
-             165661,
+             250191,
+             181461,
              10790,
+             195248,
              4288,
-             11646,
              10733,
-             59069,
-             229507,
-             229901,
-             229717,
+             60104,
+             11646,
              421,
-             59523,
+             165661,
+             59069,
+             257253,
+             257768,
+             257484,
+             257543,
              59161,
+             59523,
              60232,
-             60489,
-             230002,
              2398,
-             230013,
-             60104,
+             11380,
+             257817,
+             4339,
+             257829,
+             4385,
              3810,
-             60106,
-             195141,
-             59525,
              4243,
-             60134,
              11381,
-             10710,
-             11380,
-             4385,
-             1618,
+             59525,
              59663,
+             10710,
+             195141,
+             250777,
+             60106,
              143262,
+             257721,
+             60489,
              143263,
-             193297,
-             193376,
+             60134,
+             1618,
+             1771,
              59182,
              2636,
-             1771,
+             250733,
              4023,
-             3730,
              60191,
-             4666,
+             3730,
+             250835,
              60192,
-             1,
-             193364,
+             4666,
              1584,
-             227509,
              56140,
+             1,
              17997,
+             227509,
              4179,
              4091,
              4000,
+             250871,
              4090,
              4403,
              4075,
+             3991,
              3901,
+             4308,
+             1605,
              3115,
-             193411,
              2554,
-             1605,
              1794,
-             1630,
              2168,
-             4046,
+             1630,
+             1727,
              36919,
-             3991,
-             4308,
+             4046,
+             1631,
              3719,
-             4339,
              59126,
              20173,
+             3710,
              2607,
+             4009,
              1598,
-             3710,
              2341,
-             1631,
              3956,
-             1727,
              4105,
+             74953,
              59127,
              3908,
-             4009,
-             1379,
              1764,
+             1379,
+             256714,
              4086,
              4244,
              1818,
              1583,
-             197243,
-             4127,
              4169,
-             4126,
+             3745,
+             4127,
              14243,
              4442,
-             74953,
+             4126,
              14266,
-             4097,
              1627,
-             4078,
              2116,
+             4097,
+             4078,
+             3989,
              1628,
-             4080,
              1566,
-             3745,
-             3498,
+             4316,
              4145,
+             4080,
+             3498,
              4119,
-             3748,
              3925,
+             3748,
              2604,
-             3939,
-             4062,
              3970,
+             3939,
              1591,
              4033,
-             3952,
-             4099,
              4005,
-             1624,
+             4099,
+             4062,
+             3952,
              1612,
-             4316,
+             1624,
              4196,
              3825,
              3947,
-             1825,
-             4107,
              1606,
+             4107,
              3975,
              4098,
              4302,
-             2605,
              1579,
-             3743,
+             2605,
              4074,
-             60199,
-             3989,
+             3743,
              10848,
              3819,
              4157,
-             461,
-             1380,
              4079,
              3753,
+             1380,
+             1825,
              3499,
-             56119,
-             3727,
              1616,
+             3727,
              1575,
              3728,
+             461,
              3888,
              3934,
              1593,
+             56119,
              1377,
              1964,
-             229977,
+             257754,
              1582,
              12480,
              12489,
+             59145,
              18045,
              4332,
              3118,
              1634,
              1390,
              1391,
-             59145,
-             3573,
              2361,
-             20400,
+             3573,
              16182,
+             20400,
              1725,
              1726,
              12483,
              1567,
              20396,
              20180,
              12492,
              59130,
-             230001,
+             257816,
              4593,
-             3720,
              56100,
              56106,
              56087,
+             3720,
              3503,
              56081,
              4072,
              3794,
              2358,
-             225591,
+             247115,
              2382,
              2345,
              1637,
              2360,
              1392,
-             20185,
              1577,
+             20185,
              12486,
              2,
              3,
              4,
              5,
              6,
              8,
@@ -902,29 +901,27 @@
              42,
              43,
              44,
              45,
              92,
              93,
              94,
-             95,
              96,
              97,
              98,
              99,
              100,
              101,
              103,
              106,
              107,
              109,
              110,
              112,
              117,
-             117,
              118,
              119,
              129,
              132,
              138,
              181,
              183,
@@ -934,15 +931,15 @@
              226,
              228,
              231,
              232,
              233,
              234,
              249,
-             254,
+             250,
              255,
              256,
              313,
              361,
              362,
              439,
              440,
@@ -1007,64 +1004,65 @@
              2493,
              2506,
              2508,
              2510,
              2515,
              2525,
              3988,
-             190070,
-             190071,
-             190072,
-             193066,
-             193067,
              193069,
              193070,
              193072,
-             193122,
-             199564,
-             199838,
-             199918,
-             200002,
-             224417,
-             225391,
-             226425,
-             228320,
-             228350,
-             228656,
-             228870,
-             228902,
-             229080,
-             229081,
-             229082,
-             229233,
-             229447,
-             229542,
-             229866,
-             229894]}
+             249139,
+             249929,
+             250365,
+             250457,
+             250459,
+             250462,
+             250467,
+             250473,
+             250474,
+             250475,
+             250476,
+             250477,
+             250479,
+             250529,
+             255880,
+             256024,
+             256316,
+             256366,
+             256541,
+             256899,
+             256900,
+             256944,
+             256946,
+             257104,
+             257206,
+             257329,
+             257419]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/processlist/pid/10541
     {"10541": [{"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox"],
                 "cpu_percent": 0.0,
-                "cpu_times": [5239.7, 1595.52, 4093.05, 570.73, 0.0],
+                "cpu_times": [6652.64, 2012.85, 5052.81, 704.23, 0.0],
                 "gids": [1000, 1000, 1000],
-                "io_counters": [3503764480, 5856641024, 0, 0, 0],
+                "io_counters": [4205573120, 6936297472, 0, 0, 0],
                 "key": "pid",
-                "memory_info": [468434944,
-                                22123225088,
-                                114802688,
+                "memory_info": [507658240,
+                                22263525376,
+                                129363968,
                                 618496,
                                 0,
-                                1282670592,
+                                1405198336,
                                 0],
-                "memory_percent": 5.977844695423366,
+                "memory_percent": 6.478385432048301,
                 "name": "firefox",
                 "nice": 0,
-                "num_threads": 160,
+                "num_threads": 168,
                 "pid": 10541,
                 "status": "S",
                 "time_since_update": 1,
                 "username": "nicolargo"}]}
 
 GET psutilversion
 -----------------
@@ -1076,77 +1074,77 @@
 
 GET quicklook
 -------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/quicklook
-    {"cpu": 27.4,
+    {"cpu": 35.5,
      "cpu_hz": 2025000000.0,
-     "cpu_hz_current": 1273975000.0,
+     "cpu_hz_current": 1498956999.9999998,
      "cpu_name": "Intel(R) Core(TM) i7-4500U CPU @ 1.80GHz",
-     "mem": 63.9,
+     "mem": 67.9,
      "percpu": [{"cpu_number": 0,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 19.8,
+                 "idle": 20.2,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 3.4,
-                 "total": 80.2,
-                 "user": 76.7},
+                 "system": 6.7,
+                 "total": 79.8,
+                 "user": 73.1},
                 {"cpu_number": 1,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 91.2,
+                 "idle": 70.6,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 2.7,
-                 "total": 8.8,
-                 "user": 6.2},
+                 "system": 6.7,
+                 "total": 29.4,
+                 "user": 22.7},
                 {"cpu_number": 2,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 91.3,
+                 "idle": 85.7,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
-                 "softirq": 1.2,
+                 "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 2.6,
-                 "total": 8.7,
-                 "user": 6.1},
+                 "system": 3.4,
+                 "total": 14.3,
+                 "user": 10.9},
                 {"cpu_number": 3,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 88.6,
-                 "iowait": 0.9,
+                 "idle": 82.0,
+                 "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
-                 "softirq": 0.6,
+                 "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 2.6,
-                 "total": 11.4,
-                 "user": 7.9}],
-     "swap": 33.2}
+                 "system": 6.6,
+                 "total": 18.0,
+                 "user": 11.5}],
+     "swap": 31.6}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/quicklook/cpu
-    {"cpu": 27.4}
+    {"cpu": 35.5}
 
 GET sensors
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/sensors
@@ -1172,17 +1170,14 @@
                "acpitz 1",
                "Package id 0",
                "Core 0",
                "Core 1",
                "CPU",
                "Ambient",
                "SODIMM",
-               "CPU",
-               "Ambient",
-               "SODIMM",
                "BAT BAT0"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/sensors/label/acpitz 0
     {"acpitz 0": [{"critical": 105,
                    "key": "label",
@@ -1212,15 +1207,15 @@
 
 GET uptime
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/uptime
-    "7 days, 20:30:06"
+    "8 days, 22:22:23"
 
 GET all stats
 -------------
 
 Get all Glances stats::
 
     # curl http://localhost:61208/api/3/all
@@ -1228,41 +1223,41 @@
 
 GET stats history
 -----------------
 
 History of a plugin::
 
     # curl http://localhost:61208/api/3/cpu/history
-    {"system": [["2023-05-16T09:31:50.863038", 4.1],
-                ["2023-05-16T09:31:51.981409", 4.1],
-                ["2023-05-16T09:31:53.140895", 2.0]],
-     "user": [["2023-05-16T09:31:50.863029", 22.7],
-              ["2023-05-16T09:31:51.981402", 22.7],
-              ["2023-05-16T09:31:53.140888", 6.9]]}
+    {"system": [["2023-05-17T11:24:07.350522", 6.6],
+                ["2023-05-17T11:24:08.472521", 6.6],
+                ["2023-05-17T11:24:09.656447", 2.5]],
+     "user": [["2023-05-17T11:24:07.350513", 27.2],
+              ["2023-05-17T11:24:08.472515", 27.2],
+              ["2023-05-17T11:24:09.656439", 10.8]]}
 
 Limit history to last 2 values::
 
     # curl http://localhost:61208/api/3/cpu/history/2
-    {"system": [["2023-05-16T09:31:51.981409", 4.1],
-                ["2023-05-16T09:31:53.140895", 2.0]],
-     "user": [["2023-05-16T09:31:51.981402", 22.7],
-              ["2023-05-16T09:31:53.140888", 6.9]]}
+    {"system": [["2023-05-17T11:24:08.472521", 6.6],
+                ["2023-05-17T11:24:09.656447", 2.5]],
+     "user": [["2023-05-17T11:24:08.472515", 27.2],
+              ["2023-05-17T11:24:09.656439", 10.8]]}
 
 History for a specific field::
 
     # curl http://localhost:61208/api/3/cpu/system/history
-    {"system": [["2023-05-16T09:31:50.863038", 4.1],
-                ["2023-05-16T09:31:51.981409", 4.1],
-                ["2023-05-16T09:31:53.140895", 2.0]]}
+    {"system": [["2023-05-17T11:24:07.350522", 6.6],
+                ["2023-05-17T11:24:08.472521", 6.6],
+                ["2023-05-17T11:24:09.656447", 2.5]]}
 
 Limit history for a specific field to last 2 values::
 
     # curl http://localhost:61208/api/3/cpu/system/history
-    {"system": [["2023-05-16T09:31:51.981409", 4.1],
-                ["2023-05-16T09:31:53.140895", 2.0]]}
+    {"system": [["2023-05-17T11:24:08.472521", 6.6],
+                ["2023-05-17T11:24:09.656447", 2.5]]}
 
 GET limits (used for thresholds)
 --------------------------------
 
 All limits/thresholds::
 
     # curl http://localhost:61208/api/3/all/limits
```

### Comparing `Glances-3.4.0/docs/cmds.rst` & `Glances-3.4.0.1/docs/cmds.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/conf.py` & `Glances-3.4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/config.rst` & `Glances-3.4.0.1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/dev/glances-cprofile.png` & `Glances-3.4.0.1/docs/dev/glances-cprofile.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/docker.rst` & `Glances-3.4.0.1/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/glances.rst` & `Glances-3.4.0.1/docs/glances.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/cassandra.rst` & `Glances-3.4.0.1/docs/gw/cassandra.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/couchdb.rst` & `Glances-3.4.0.1/docs/gw/couchdb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/csv.rst` & `Glances-3.4.0.1/docs/gw/csv.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/graph.rst` & `Glances-3.4.0.1/docs/gw/graph.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/graphite.rst` & `Glances-3.4.0.1/docs/gw/graphite.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/influxdb.rst` & `Glances-3.4.0.1/docs/gw/influxdb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/kafka.rst` & `Glances-3.4.0.1/docs/gw/kafka.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/mongodb.rst` & `Glances-3.4.0.1/docs/gw/mongodb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/mqtt.rst` & `Glances-3.4.0.1/docs/gw/mqtt.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/prometheus.rst` & `Glances-3.4.0.1/docs/gw/prometheus.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/restful.rst` & `Glances-3.4.0.1/docs/gw/restful.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/statsd.rst` & `Glances-3.4.0.1/docs/gw/statsd.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/gw/zeromq.rst` & `Glances-3.4.0.1/docs/gw/zeromq.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/index.rst` & `Glances-3.4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/install.rst` & `Glances-3.4.0.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/make.bat` & `Glances-3.4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/man/glances.1` & `Glances-3.4.0.1/docs/man/glances.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "GLANCES" "1" "May 16, 2023" "3.4.0" "Glances"
+.TH "GLANCES" "1" "May 17, 2023" "3.4.0.1" "Glances"
 .SH NAME
 glances \- An eye on your system
 .SH SYNOPSIS
 .sp
 \fBglances\fP [OPTIONS]
 .SH DESCRIPTION
 .sp
```

### Comparing `Glances-3.4.0/docs/objects.inv` & `Glances-3.4.0.1/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/docs/quickstart.rst` & `Glances-3.4.0.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/__init__.py` & `Glances-3.4.0.1/glances/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import platform
 import signal
 import sys
 
 # Global name
 # Version should start and end with a numerical char
 # See https://packaging.python.org/specifications/core-metadata/#version
-__version__ = '3.4.0'
+__version__ = '3.4.0.1'
 __author__ = 'Nicolas Hennion <nicolas@nicolargo.com>'
 __license__ = 'LGPLv3'
 
 # Import psutil
 try:
     from psutil import __version__ as psutil_version
 except ImportError:
```

### Comparing `Glances-3.4.0/glances/actions.py` & `Glances-3.4.0.1/glances/actions.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/amps/glances_amp.py` & `Glances-3.4.0.1/glances/amps/glances_amp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/amps/glances_default.py` & `Glances-3.4.0.1/glances/amps/glances_default.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/amps/glances_nginx.py` & `Glances-3.4.0.1/glances/amps/glances_nginx.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/amps/glances_systemd.py` & `Glances-3.4.0.1/glances/amps/glances_systemd.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/amps/glances_systemv.py` & `Glances-3.4.0.1/glances/amps/glances_systemv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/amps_list.py` & `Glances-3.4.0.1/glances/amps_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/attribute.py` & `Glances-3.4.0.1/glances/attribute.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/autodiscover.py` & `Glances-3.4.0.1/glances/autodiscover.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/client.py` & `Glances-3.4.0.1/glances/client.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/client_browser.py` & `Glances-3.4.0.1/glances/client_browser.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/compat.py` & `Glances-3.4.0.1/glances/compat.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/config.py` & `Glances-3.4.0.1/glances/config.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/cpu_percent.py` & `Glances-3.4.0.1/glances/cpu_percent.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/events.py` & `Glances-3.4.0.1/glances/events.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_cassandra.py` & `Glances-3.4.0.1/glances/exports/glances_cassandra.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_couchdb.py` & `Glances-3.4.0.1/glances/exports/glances_couchdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_csv.py` & `Glances-3.4.0.1/glances/exports/glances_csv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_elasticsearch.py` & `Glances-3.4.0.1/glances/exports/glances_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_export.py` & `Glances-3.4.0.1/glances/exports/glances_export.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_graph.py` & `Glances-3.4.0.1/glances/exports/glances_graph.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_graphite.py` & `Glances-3.4.0.1/glances/exports/glances_graphite.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_influxdb.py` & `Glances-3.4.0.1/glances/exports/glances_influxdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_influxdb2.py` & `Glances-3.4.0.1/glances/exports/glances_influxdb2.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_json.py` & `Glances-3.4.0.1/glances/exports/glances_json.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_kafka.py` & `Glances-3.4.0.1/glances/exports/glances_kafka.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_mongodb.py` & `Glances-3.4.0.1/glances/exports/glances_mongodb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_mqtt.py` & `Glances-3.4.0.1/glances/exports/glances_mqtt.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_opentsdb.py` & `Glances-3.4.0.1/glances/exports/glances_opentsdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_prometheus.py` & `Glances-3.4.0.1/glances/exports/glances_prometheus.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_rabbitmq.py` & `Glances-3.4.0.1/glances/exports/glances_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_restful.py` & `Glances-3.4.0.1/glances/exports/glances_restful.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_riemann.py` & `Glances-3.4.0.1/glances/exports/glances_riemann.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_statsd.py` & `Glances-3.4.0.1/glances/exports/glances_statsd.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/exports/glances_zeromq.py` & `Glances-3.4.0.1/glances/exports/glances_zeromq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/filter.py` & `Glances-3.4.0.1/glances/filter.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/folder_list.py` & `Glances-3.4.0.1/glances/folder_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/globals.py` & `Glances-3.4.0.1/glances/globals.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/history.py` & `Glances-3.4.0.1/glances/history.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/logger.py` & `Glances-3.4.0.1/glances/logger.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/main.py` & `Glances-3.4.0.1/glances/main.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outdated.py` & `Glances-3.4.0.1/glances/outdated.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_bars.py` & `Glances-3.4.0.1/glances/outputs/glances_bars.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_bottle.py` & `Glances-3.4.0.1/glances/outputs/glances_bottle.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_curses.py` & `Glances-3.4.0.1/glances/outputs/glances_curses.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_curses_browser.py` & `Glances-3.4.0.1/glances/outputs/glances_curses_browser.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_sparklines.py` & `Glances-3.4.0.1/glances/outputs/glances_sparklines.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_stdout.py` & `Glances-3.4.0.1/glances/outputs/glances_stdout.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_stdout_apidoc.py` & `Glances-3.4.0.1/glances/outputs/glances_stdout_apidoc.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_stdout_csv.py` & `Glances-3.4.0.1/glances/outputs/glances_stdout_csv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_stdout_issue.py` & `Glances-3.4.0.1/glances/outputs/glances_stdout_issue.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_stdout_json.py` & `Glances-3.4.0.1/glances/outputs/glances_stdout_json.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/glances_unicode.py` & `Glances-3.4.0.1/glances/outputs/glances_unicode.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/README.md` & `Glances-3.4.0.1/glances/outputs/static/README.md`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/css/bootstrap.less` & `Glances-3.4.0.1/glances/outputs/static/css/bootstrap.less`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/css/style.scss` & `Glances-3.4.0.1/glances/outputs/static/css/style.scss`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/images/favicon.ico` & `Glances-3.4.0.1/glances/outputs/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/images/glances.png` & `Glances-3.4.0.1/glances/outputs/static/images/glances.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/App.vue` & `Glances-3.4.0.1/glances/outputs/static/js/App.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/help.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/help.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-alert.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-alert.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-amps.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-amps.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-cloud.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cloud.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-connections.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-connections.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-containers.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-containers.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-cpu.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-cpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-diskio.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-diskio.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-folders.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-folders.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-fs.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-fs.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-gpu.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-gpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-ip.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ip.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-irq.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-irq.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-load.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-load.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-mem-more.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem-more.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-mem.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-mem.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-memswap.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-memswap.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-network.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-network.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-percpu.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-percpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-ports.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-ports.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-process.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-process.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-processcount.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processcount.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-processlist.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-processlist.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-quicklook.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-quicklook.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-raid.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-raid.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-sensors.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-sensors.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-system.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-system.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/components/plugin-wifi.vue` & `Glances-3.4.0.1/glances/outputs/static/js/components/plugin-wifi.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/filters.js` & `Glances-3.4.0.1/glances/outputs/static/js/filters.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/js/services.js` & `Glances-3.4.0.1/glances/outputs/static/js/services.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/package-lock.json` & `Glances-3.4.0.1/glances/outputs/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/package.json` & `Glances-3.4.0.1/glances/outputs/static/package.json`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/public/87708faeed9a66b0fcdb.png` & `Glances-3.4.0.1/glances/outputs/static/public/87708faeed9a66b0fcdb.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/public/favicon.ico` & `Glances-3.4.0.1/glances/outputs/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/public/glances.js` & `Glances-3.4.0.1/glances/outputs/static/public/glances.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/outputs/static/webpack.config.js` & `Glances-3.4.0.1/glances/outputs/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/password.py` & `Glances-3.4.0.1/glances/password.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/password_list.py` & `Glances-3.4.0.1/glances/password_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/containers/glances_docker.py` & `Glances-3.4.0.1/glances/plugins/containers/glances_docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 #
 # SPDX-License-Identifier: LGPL-3.0-only
 #
 
 """Docker Extension unit for Glances' Containers plugin."""
 import time
 
-import requests
-
 from glances.compat import iterkeys, itervalues, nativestr, pretty_date
 from glances.logger import logger
 from glances.plugins.containers.stats_streamer import StatsStreamer
 
 # Docker-py library (optional and Linux-only)
 # https://github.com/docker/docker-py
 try:
+    import requests
     import docker
     from dateutil import parser, tz
 except Exception as e:
     import_docker_error_tag = True
     # Display debug message if import KeyError
-    logger.debug("Error loading Docker deps Lib. Docker plugin is disabled ({})".format(e))
+    logger.warning("Error loading Docker deps Lib. Docker plugin is disabled ({})".format(e))
 else:
     import_docker_error_tag = False
 
 
 class DockerStatsFetcher:
     MANDATORY_MEMORY_FIELDS = ["usage", 'limit']
```

### Comparing `Glances-3.4.0/glances/plugins/containers/glances_podman.py` & `Glances-3.4.0.1/glances/plugins/containers/glances_podman.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Podman library (optional and Linux-only)
 # https://pypi.org/project/podman/
 try:
     from podman import PodmanClient
 except Exception as e:
     import_podman_error_tag = True
     # Display debug message if import KeyError
-    logger.debug("Error loading Podman deps Lib. Podman feature in the Containers plugin is disabled ({})".format(e))
+    logger.warning("Error loading Podman deps Lib. Podman feature in the Containers plugin is disabled ({})".format(e))
 else:
     import_podman_error_tag = False
 
 
 class PodmanContainerStatsFetcher:
     MANDATORY_FIELDS = ["CPU", "MemUsage", "MemLimit", "NetInput", "NetOutput", "BlockInput", "BlockOutput"]
```

### Comparing `Glances-3.4.0/glances/plugins/containers/stats_streamer.py` & `Glances-3.4.0.1/glances/plugins/containers/stats_streamer.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_alert.py` & `Glances-3.4.0.1/glances/plugins/glances_alert.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_amps.py` & `Glances-3.4.0.1/glances/plugins/glances_amps.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_cloud.py` & `Glances-3.4.0.1/glances/plugins/glances_cloud.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_connections.py` & `Glances-3.4.0.1/glances/plugins/glances_connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,19 @@
             for s in [psutil.CONN_LISTEN, 'initiated', psutil.CONN_ESTABLISHED, 'terminated']:
                 ret.append(self.curse_new_line())
                 msg = '{:{width}}'.format(nativestr(s).capitalize(), width=len(s))
                 ret.append(self.curse_add_line(msg))
                 msg = '{:>{width}}'.format(self.stats[s], width=max_width - len(s) + 2)
                 ret.append(self.curse_add_line(msg))
         # Connections track
-        if self.stats['nf_conntrack_enabled']:
+        if (
+            self.stats['nf_conntrack_enabled']
+            and 'nf_conntrack_count' in self.stats
+            and 'nf_conntrack_max' in self.stats
+        ):
             s = 'Tracked'
             ret.append(self.curse_new_line())
             msg = '{:{width}}'.format(nativestr(s).capitalize(), width=len(s))
             ret.append(self.curse_add_line(msg))
             msg = '{:>{width}}'.format(
                 '{:0.0f}/{:0.0f}'.format(self.stats['nf_conntrack_count'], self.stats['nf_conntrack_max']),
                 width=max_width - len(s) + 2,
```

### Comparing `Glances-3.4.0/glances/plugins/glances_containers.py` & `Glances-3.4.0.1/glances/plugins/glances_containers.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_core.py` & `Glances-3.4.0.1/glances/plugins/glances_core.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_cpu.py` & `Glances-3.4.0.1/glances/plugins/glances_cpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_diskio.py` & `Glances-3.4.0.1/glances/plugins/glances_diskio.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_folders.py` & `Glances-3.4.0.1/glances/plugins/glances_folders.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_fs.py` & `Glances-3.4.0.1/glances/plugins/glances_fs.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_gpu.py` & `Glances-3.4.0.1/glances/plugins/glances_gpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_help.py` & `Glances-3.4.0.1/glances/plugins/glances_help.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_ip.py` & `Glances-3.4.0.1/glances/plugins/glances_ip.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_irq.py` & `Glances-3.4.0.1/glances/plugins/glances_irq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_load.py` & `Glances-3.4.0.1/glances/plugins/glances_load.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_mem.py` & `Glances-3.4.0.1/glances/plugins/glances_mem.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_memswap.py` & `Glances-3.4.0.1/glances/plugins/glances_memswap.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_network.py` & `Glances-3.4.0.1/glances/plugins/glances_network.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_now.py` & `Glances-3.4.0.1/glances/plugins/glances_now.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_percpu.py` & `Glances-3.4.0.1/glances/plugins/glances_percpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_plugin.py` & `Glances-3.4.0.1/glances/plugins/glances_plugin.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_ports.py` & `Glances-3.4.0.1/glances/plugins/glances_ports.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_processcount.py` & `Glances-3.4.0.1/glances/plugins/glances_processcount.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_processlist.py` & `Glances-3.4.0.1/glances/plugins/glances_processlist.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_psutilversion.py` & `Glances-3.4.0.1/glances/plugins/glances_psutilversion.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_quicklook.py` & `Glances-3.4.0.1/glances/plugins/glances_quicklook.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_raid.py` & `Glances-3.4.0.1/glances/plugins/glances_raid.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_sensors.py` & `Glances-3.4.0.1/glances/plugins/glances_sensors.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_smart.py` & `Glances-3.4.0.1/glances/plugins/glances_smart.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_system.py` & `Glances-3.4.0.1/glances/plugins/glances_system.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_uptime.py` & `Glances-3.4.0.1/glances/plugins/glances_uptime.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/glances_wifi.py` & `Glances-3.4.0.1/glances/plugins/glances_wifi.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/sensors/glances_batpercent.py` & `Glances-3.4.0.1/glances/plugins/sensors/glances_batpercent.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/plugins/sensors/glances_hddtemp.py` & `Glances-3.4.0.1/glances/plugins/sensors/glances_hddtemp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/ports_list.py` & `Glances-3.4.0.1/glances/ports_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/processes.py` & `Glances-3.4.0.1/glances/processes.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/programs.py` & `Glances-3.4.0.1/glances/programs.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/secure.py` & `Glances-3.4.0.1/glances/secure.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/server.py` & `Glances-3.4.0.1/glances/server.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/snmp.py` & `Glances-3.4.0.1/glances/snmp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/standalone.py` & `Glances-3.4.0.1/glances/standalone.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/static_list.py` & `Glances-3.4.0.1/glances/static_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/stats.py` & `Glances-3.4.0.1/glances/stats.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/stats_client.py` & `Glances-3.4.0.1/glances/stats_client.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/stats_client_snmp.py` & `Glances-3.4.0.1/glances/stats_client_snmp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/stats_server.py` & `Glances-3.4.0.1/glances/stats_server.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/thresholds.py` & `Glances-3.4.0.1/glances/thresholds.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/timer.py` & `Glances-3.4.0.1/glances/timer.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/web_list.py` & `Glances-3.4.0.1/glances/web_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/glances/webserver.py` & `Glances-3.4.0.1/glances/webserver.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/pyproject.toml` & `Glances-3.4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0/setup.py` & `Glances-3.4.0.1/setup.py`

 * *Files identical despite different names*

