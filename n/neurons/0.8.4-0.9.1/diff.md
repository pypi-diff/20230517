# Comparing `tmp/neurons-0.8.4.tar.gz` & `tmp/neurons-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neurons-0.8.4.tar", last modified: Mon Feb 18 15:08:41 2019, max compression
+gzip compressed data, was "dist/neurons-0.9.1.tar", last modified: Fri Jan 10 10:17:57 2020, max compression
```

## Comparing `neurons-0.8.4.tar` & `neurons-0.9.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/assets/
--rw-r--r--   0 plq       (1000) users      (100)      736 2019-02-18 13:15:27.000000 neurons-0.8.4/assets/Makefile
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/examples/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/examples/garage/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/examples/garage/garage/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/examples/garage/garage/const/
--rw-r--r--   0 plq       (1000) users      (100)     1858 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage/const/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)      129 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage/const/index.html
--rw-r--r--   0 plq       (1000) users      (100)     1712 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     2883 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage/application.py
--rw-r--r--   0 plq       (1000) users      (100)     2162 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage/main.py
--rw-r--r--   0 plq       (1000) users      (100)     2568 2019-02-18 13:15:41.000000 neurons-0.8.4/examples/garage/garage/model.py
--rw-r--r--   0 plq       (1000) users      (100)     2181 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage/service.py
--rwxr-xr-x   0 plq       (1000) users      (100)       94 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/garage.py
--rw-r--r--   0 plq       (1000) users      (100)      702 2019-02-18 13:15:27.000000 neurons-0.8.4/examples/garage/setup.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/base/
--rw-r--r--   0 plq       (1000) users      (100)     1750 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     1719 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/const.py
--rw-r--r--   0 plq       (1000) users      (100)     2231 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/error.py
--rw-r--r--   0 plq       (1000) users      (100)     2279 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/event.py
--rw-r--r--   0 plq       (1000) users      (100)     2235 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/model.py
--rw-r--r--   0 plq       (1000) users      (100)    13732 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/screen.py
--rw-r--r--   0 plq       (1000) users      (100)     2377 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/service.py
--rw-r--r--   0 plq       (1000) users      (100)     6507 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/base/session.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/daemon/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/daemon/config/
--rw-r--r--   0 plq       (1000) users      (100)     2912 2019-02-18 13:15:41.000000 neurons-0.8.4/neurons/daemon/config/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     2438 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/config/_base.py
--rw-r--r--   0 plq       (1000) users      (100)     2368 2019-02-18 13:15:41.000000 neurons-0.8.4/neurons/daemon/config/_wdict.py
--rw-r--r--   0 plq       (1000) users      (100)    33917 2019-02-18 13:15:41.000000 neurons-0.8.4/neurons/daemon/config/daemon.py
--rw-r--r--   0 plq       (1000) users      (100)    17665 2019-02-18 15:07:37.000000 neurons-0.8.4/neurons/daemon/config/endpoint.py
--rw-r--r--   0 plq       (1000) users      (100)     9476 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/config/limits.py
--rw-r--r--   0 plq       (1000) users      (100)    10569 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/config/logutils.py
--rw-r--r--   0 plq       (1000) users      (100)     2676 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/config/static_file.py
--rw-r--r--   0 plq       (1000) users      (100)     7049 2019-02-18 15:07:37.000000 neurons-0.8.4/neurons/daemon/config/store.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/daemon/dowser/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/daemon/dowser/const/
--rw-r--r--   0 plq       (1000) users      (100)     2366 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/const/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)      794 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/const/graphs.html
--rw-r--r--   0 plq       (1000) users      (100)      739 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/const/main.css
--rw-r--r--   0 plq       (1000) users      (100)      768 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/const/trace.html
--rw-r--r--   0 plq       (1000) users      (100)      612 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/const/tree.html
--rw-r--r--   0 plq       (1000) users      (100)     1870 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     3427 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/app.py
--rw-r--r--   0 plq       (1000) users      (100)     7576 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/reftree.py
--rw-r--r--   0 plq       (1000) users      (100)    15030 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/dowser/service.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/daemon/test/
--rw-r--r--   0 plq       (1000) users      (100)        0 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/test/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     1943 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/test/test_config.py
--rw-r--r--   0 plq       (1000) users      (100)     2770 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     6345 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/cli.py
--rw-r--r--   0 plq       (1000) users      (100)     9472 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/daemonize.py
--rw-r--r--   0 plq       (1000) users      (100)     3427 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/ipc.py
--rw-r--r--   0 plq       (1000) users      (100)    20366 2019-02-18 13:15:41.000000 neurons-0.8.4/neurons/daemon/main.py
--rw-r--r--   0 plq       (1000) users      (100)    10740 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/daemon/store.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/form/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/form/const/
--rw-r--r--   0 plq       (1000) users      (100)     1891 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/const/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     1282 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/const/test.html
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/form/test/
--rw-r--r--   0 plq       (1000) users      (100)     2507 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/test/__init__.py
--rwxr-xr-x   0 plq       (1000) users      (100)    17358 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/test/test_form.py
--rwxr-xr-x   0 plq       (1000) users      (100)     5306 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/test/test_form_table.py
--rw-r--r--   0 plq       (1000) users      (100)     2604 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)    36788 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/form.py
--rw-r--r--   0 plq       (1000) users      (100)    12273 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/table.py
--rw-r--r--   0 plq       (1000) users      (100)    52326 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/form/widget.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/geojson/
--rw-r--r--   0 plq       (1000) users      (100)     1969 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/geojson/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     4265 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/geojson/model.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/log/
--rw-r--r--   0 plq       (1000) users      (100)     1727 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/log/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     1751 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/log/method_call.py
--rw-r--r--   0 plq       (1000) users      (100)     4907 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/log/method_return.py
--rw-r--r--   0 plq       (1000) users      (100)     3643 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/log/model.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/const/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/const/comp/
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-array/
--rw-r--r--   0 plq       (1000) users      (100)     5977 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-array/neurons-array.html
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-complex-reference/
--rw-r--r--   0 plq       (1000) users      (100)     6527 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-dropdown.html
--rw-r--r--   0 plq       (1000) users      (100)     5530 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-href.html
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-date-time/
--rw-r--r--   0 plq       (1000) users      (100)     9293 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-date-time/neurons-datetime-picker.html
--rw-r--r--   0 plq       (1000) users      (100)      940 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/comp/neurons-date-time/neurons-moment-validator.html
--rw-r--r--   0 plq       (1000) users      (100)     1679 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/comp/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     2261 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     6596 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/defn.js
--rw-r--r--   0 plq       (1000) users      (100)     3306 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/dom_module.html
--rw-r--r--   0 plq       (1000) users      (100)     3024 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/preamble.js
--rw-r--r--   0 plq       (1000) users      (100)     3565 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/const/screen.html
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/protocol/
--rw-r--r--   0 plq       (1000) users      (100)     1820 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/protocol/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)    13337 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/protocol/form.py
--rw-r--r--   0 plq       (1000) users      (100)    14401 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/protocol/widget.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons/polymer/test/
--rw-r--r--   0 plq       (1000) users      (100)     1695 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/test/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     1983 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/test/test_jsutil.py
--rw-r--r--   0 plq       (1000) users      (100)     4322 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/test/test_widget.py
--rw-r--r--   0 plq       (1000) users      (100)     1874 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     4899 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/app.py
--rw-r--r--   0 plq       (1000) users      (100)     2842 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/jsutil.py
--rw-r--r--   0 plq       (1000) users      (100)     8404 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/model.py
--rw-r--r--   0 plq       (1000) users      (100)     8887 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/polymer/service.py
--rw-r--r--   0 plq       (1000) users      (100)     1999 2019-02-18 15:08:10.000000 neurons-0.8.4/neurons/__init__.py
--rw-r--r--   0 plq       (1000) users      (100)     1971 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/_base.py
--rw-r--r--   0 plq       (1000) users      (100)     2053 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/application.py
--rw-r--r--   0 plq       (1000) users      (100)     4310 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/context.py
--rw-r--r--   0 plq       (1000) users      (100)     3500 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/model.py
--rw-r--r--   0 plq       (1000) users      (100)     6398 2019-02-18 13:15:27.000000 neurons-0.8.4/neurons/version.py
-drwxr-xr-x   0 plq       (1000) users      (100)        0 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/
--rw-r--r--   0 plq       (1000) users      (100)     1208 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/PKG-INFO
--rw-r--r--   0 plq       (1000) users      (100)     3074 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/SOURCES.txt
--rw-r--r--   0 plq       (1000) users      (100)        1 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/dependency_links.txt
--rw-r--r--   0 plq       (1000) users      (100)       20 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/entry_points.txt
--rw-r--r--   0 plq       (1000) users      (100)        1 2019-02-18 13:17:48.000000 neurons-0.8.4/neurons.egg-info/not-zip-safe
--rw-r--r--   0 plq       (1000) users      (100)      141 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/requires.txt
--rw-r--r--   0 plq       (1000) users      (100)        8 2019-02-18 15:08:41.000000 neurons-0.8.4/neurons.egg-info/top_level.txt
--rw-r--r--   0 plq       (1000) users      (100)       27 2019-02-18 13:15:27.000000 neurons-0.8.4/.coveragerc
--rw-r--r--   0 plq       (1000) users      (100)      293 2019-02-18 13:15:27.000000 neurons-0.8.4/.editorconfig
--rw-r--r--   0 plq       (1000) users      (100)      590 2019-02-18 13:15:27.000000 neurons-0.8.4/.gitignore
--rw-r--r--   0 plq       (1000) users      (100)     1576 2019-02-18 13:15:27.000000 neurons-0.8.4/LICENSE
--rw-r--r--   0 plq       (1000) users      (100)      923 2019-02-18 13:15:27.000000 neurons-0.8.4/README.md
--rwxr-xr-x   0 plq       (1000) users      (100)     5589 2019-02-18 13:15:27.000000 neurons-0.8.4/run_tests.sh
--rwxr-xr-x   0 plq       (1000) users      (100)     3655 2019-02-18 13:15:41.000000 neurons-0.8.4/setup.py
--rw-r--r--   0 plq       (1000) users      (100)      464 2019-02-18 13:15:27.000000 neurons-0.8.4/tox.ini
--rw-r--r--   0 plq       (1000) users      (100)     1208 2019-02-18 15:08:41.000000 neurons-0.8.4/PKG-INFO
--rw-r--r--   0 plq       (1000) users      (100)       38 2019-02-18 15:08:41.000000 neurons-0.8.4/setup.cfg
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/assets/
+-rw-r--r--   0 plq       (1000) users      (100)      736 2018-11-22 08:52:55.000000 neurons-0.9.1/assets/Makefile
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/examples/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/examples/garage/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/examples/garage/garage/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/examples/garage/garage/const/
+-rw-r--r--   0 plq       (1000) users      (100)     1858 2018-11-22 08:52:55.000000 neurons-0.9.1/examples/garage/garage/const/__init__.py
+-rw-------   0 plq       (1000) users      (100)      129 2015-11-22 15:16:05.000000 neurons-0.9.1/examples/garage/garage/const/index.html
+-rw-r--r--   0 plq       (1000) users      (100)     1712 2018-11-22 08:52:55.000000 neurons-0.9.1/examples/garage/garage/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     2883 2020-01-10 10:11:44.000000 neurons-0.9.1/examples/garage/garage/application.py
+-rw-r--r--   0 plq       (1000) users      (100)     2161 2020-01-10 10:11:44.000000 neurons-0.9.1/examples/garage/garage/main.py
+-rw-r--r--   0 plq       (1000) users      (100)     2568 2020-01-10 10:11:44.000000 neurons-0.9.1/examples/garage/garage/model.py
+-rw-r--r--   0 plq       (1000) users      (100)     2181 2018-11-22 08:52:55.000000 neurons-0.9.1/examples/garage/garage/service.py
+-rwxr-xr-x   0 plq       (1000) users      (100)       94 2018-11-22 08:52:55.000000 neurons-0.9.1/examples/garage/garage.py
+-rw-------   0 plq       (1000) users      (100)      702 2015-11-22 15:16:05.000000 neurons-0.9.1/examples/garage/setup.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/base/
+-rw-r--r--   0 plq       (1000) users      (100)     1750 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     1719 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/const.py
+-rw-r--r--   0 plq       (1000) users      (100)     2231 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/error.py
+-rw-r--r--   0 plq       (1000) users      (100)     2279 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/event.py
+-rw-r--r--   0 plq       (1000) users      (100)     2235 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/model.py
+-rw-r--r--   0 plq       (1000) users      (100)    13751 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/base/screen.py
+-rw-r--r--   0 plq       (1000) users      (100)     2377 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/service.py
+-rw-r--r--   0 plq       (1000) users      (100)     6507 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/base/session.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/daemon/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/daemon/config/
+-rw-r--r--   0 plq       (1000) users      (100)     2912 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     2438 2018-11-22 08:52:59.000000 neurons-0.9.1/neurons/daemon/config/_base.py
+-rw-r--r--   0 plq       (1000) users      (100)     2368 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/_wdict.py
+-rw-r--r--   0 plq       (1000) users      (100)    35197 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/daemon.py
+-rw-r--r--   0 plq       (1000) users      (100)    17665 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/endpoint.py
+-rw-r--r--   0 plq       (1000) users      (100)     9476 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/limits.py
+-rw-r--r--   0 plq       (1000) users      (100)    11150 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/logutils.py
+-rw-r--r--   0 plq       (1000) users      (100)     2676 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/static_file.py
+-rw-r--r--   0 plq       (1000) users      (100)     7049 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/config/store.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/daemon/dowser/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/daemon/dowser/const/
+-rw-r--r--   0 plq       (1000) users      (100)     2366 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/daemon/dowser/const/__init__.py
+-rw-------   0 plq       (1000) users      (100)      794 2015-11-22 15:16:05.000000 neurons-0.9.1/neurons/daemon/dowser/const/graphs.html
+-rw-r--r--   0 plq       (1000) users      (100)      739 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/daemon/dowser/const/main.css
+-rw-------   0 plq       (1000) users      (100)      768 2015-11-22 15:16:05.000000 neurons-0.9.1/neurons/daemon/dowser/const/trace.html
+-rw-------   0 plq       (1000) users      (100)      612 2015-11-22 15:16:05.000000 neurons-0.9.1/neurons/daemon/dowser/const/tree.html
+-rw-r--r--   0 plq       (1000) users      (100)     1870 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/daemon/dowser/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     3427 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/dowser/app.py
+-rw-r--r--   0 plq       (1000) users      (100)     7511 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/dowser/reftree.py
+-rw-r--r--   0 plq       (1000) users      (100)    16582 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/dowser/service.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/daemon/test/
+-rw-r--r--   0 plq       (1000) users      (100)        0 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/daemon/test/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     1943 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/test/test_config.py
+-rw-r--r--   0 plq       (1000) users      (100)     2956 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     6345 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/cli.py
+-rw-r--r--   0 plq       (1000) users      (100)     9472 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/daemon/daemonize.py
+-rw-r--r--   0 plq       (1000) users      (100)     3427 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/daemon/ipc.py
+-rw-r--r--   0 plq       (1000) users      (100)    20377 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/main.py
+-rw-r--r--   0 plq       (1000) users      (100)    10726 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/daemon/store.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/form/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/form/const/
+-rw-r--r--   0 plq       (1000) users      (100)     1891 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/const/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     1282 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/const/test.html
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/form/test/
+-rw-r--r--   0 plq       (1000) users      (100)     2507 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/test/__init__.py
+-rwxr-xr-x   0 plq       (1000) users      (100)    17358 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/test/test_form.py
+-rwxr-xr-x   0 plq       (1000) users      (100)     5306 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/test/test_form_table.py
+-rw-r--r--   0 plq       (1000) users      (100)     2604 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)    38289 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/form/form.py
+-rw-r--r--   0 plq       (1000) users      (100)    12273 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/form/table.py
+-rw-r--r--   0 plq       (1000) users      (100)    52771 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/form/widget.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/geojson/
+-rw-r--r--   0 plq       (1000) users      (100)     1969 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/geojson/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     4265 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/geojson/model.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/log/
+-rw-r--r--   0 plq       (1000) users      (100)     1727 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/log/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     1751 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/log/method_call.py
+-rw-r--r--   0 plq       (1000) users      (100)     4907 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/log/method_return.py
+-rw-r--r--   0 plq       (1000) users      (100)     3643 2018-11-22 08:52:59.000000 neurons-0.9.1/neurons/log/model.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/const/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/const/comp/
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-array/
+-rw-r--r--   0 plq       (1000) users      (100)     5977 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-array/neurons-array.html
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-complex-reference/
+-rw-r--r--   0 plq       (1000) users      (100)     6527 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-dropdown.html
+-rw-r--r--   0 plq       (1000) users      (100)     5530 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-href.html
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-date-time/
+-rw-r--r--   0 plq       (1000) users      (100)     9293 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-date-time/neurons-datetime-picker.html
+-rw-r--r--   0 plq       (1000) users      (100)      940 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/comp/neurons-date-time/neurons-moment-validator.html
+-rw-r--r--   0 plq       (1000) users      (100)     1679 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/comp/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     2277 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/polymer/const/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     6596 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/defn.js
+-rw-r--r--   0 plq       (1000) users      (100)     3306 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/dom_module.html
+-rw-r--r--   0 plq       (1000) users      (100)     3024 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/preamble.js
+-rw-r--r--   0 plq       (1000) users      (100)     3565 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/const/screen.html
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/protocol/
+-rw-r--r--   0 plq       (1000) users      (100)     1820 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/protocol/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)    13337 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/protocol/form.py
+-rw-r--r--   0 plq       (1000) users      (100)    14401 2018-11-22 08:52:59.000000 neurons-0.9.1/neurons/polymer/protocol/widget.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons/polymer/test/
+-rw-r--r--   0 plq       (1000) users      (100)     1695 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/test/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     1983 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/test/test_jsutil.py
+-rw-r--r--   0 plq       (1000) users      (100)     4322 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/test/test_widget.py
+-rw-r--r--   0 plq       (1000) users      (100)     1874 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     4899 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/app.py
+-rw-r--r--   0 plq       (1000) users      (100)     2842 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/jsutil.py
+-rw-r--r--   0 plq       (1000) users      (100)     8404 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/model.py
+-rw-r--r--   0 plq       (1000) users      (100)     8887 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/polymer/service.py
+-rw-r--r--   0 plq       (1000) users      (100)     2036 2020-01-10 10:17:51.000000 neurons-0.9.1/neurons/__init__.py
+-rw-r--r--   0 plq       (1000) users      (100)     2063 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/_base.py
+-rw-r--r--   0 plq       (1000) users      (100)     2053 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/application.py
+-rw-r--r--   0 plq       (1000) users      (100)     4310 2018-11-22 08:52:55.000000 neurons-0.9.1/neurons/context.py
+-rw-r--r--   0 plq       (1000) users      (100)     3500 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/model.py
+-rw-r--r--   0 plq       (1000) users      (100)     6441 2020-01-10 10:11:44.000000 neurons-0.9.1/neurons/version.py
+drwxr-xr-x   0 plq       (1000) users      (100)        0 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/
+-rw-r--r--   0 plq       (1000) users      (100)     1133 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/PKG-INFO
+-rw-r--r--   0 plq       (1000) users      (100)     3074 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/SOURCES.txt
+-rw-r--r--   0 plq       (1000) users      (100)        1 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/dependency_links.txt
+-rw-r--r--   0 plq       (1000) users      (100)       20 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/entry_points.txt
+-rw-r--r--   0 plq       (1000) users      (100)        1 2020-01-10 10:12:17.000000 neurons-0.9.1/neurons.egg-info/not-zip-safe
+-rw-r--r--   0 plq       (1000) users      (100)      148 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/requires.txt
+-rw-r--r--   0 plq       (1000) users      (100)        8 2020-01-10 10:17:57.000000 neurons-0.9.1/neurons.egg-info/top_level.txt
+-rw-------   0 plq       (1000) users      (100)       27 2015-11-22 19:25:21.000000 neurons-0.9.1/.coveragerc
+-rw-r--r--   0 plq       (1000) users      (100)      293 2018-11-22 08:52:55.000000 neurons-0.9.1/.editorconfig
+-rw-r--r--   0 plq       (1000) users      (100)      590 2018-11-22 08:52:55.000000 neurons-0.9.1/.gitignore
+-rw-r--r--   0 plq       (1000) users      (100)     1576 2018-11-22 08:52:55.000000 neurons-0.9.1/LICENSE
+-rw-r--r--   0 plq       (1000) users      (100)      923 2018-11-22 09:09:32.000000 neurons-0.9.1/README.md
+-rwx------   0 plq       (1000) users      (100)     5589 2015-11-22 15:16:05.000000 neurons-0.9.1/run_tests.sh
+-rwxr-xr-x   0 plq       (1000) users      (100)     3658 2020-01-10 10:17:17.000000 neurons-0.9.1/setup.py
+-rw-------   0 plq       (1000) users      (100)      464 2015-11-22 15:16:05.000000 neurons-0.9.1/tox.ini
+-rw-r--r--   0 plq       (1000) users      (100)     1133 2020-01-10 10:17:57.000000 neurons-0.9.1/PKG-INFO
+-rw-r--r--   0 plq       (1000) users      (100)       59 2020-01-10 10:17:57.000000 neurons-0.9.1/setup.cfg
```

### Comparing `neurons-0.8.4/assets/Makefile` & `neurons-0.9.1/assets/Makefile`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/examples/garage/garage/const/__init__.py` & `neurons-0.9.1/examples/garage/garage/const/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/examples/garage/garage/__init__.py` & `neurons-0.9.1/examples/garage/garage/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/examples/garage/garage/application.py` & `neurons-0.9.1/examples/garage/garage/application.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/examples/garage/garage/main.py` & `neurons-0.9.1/examples/garage/garage/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-# NO IMPORTS IN MAIN FUNCTION!!!
+# NO IMPORTS IN MAIN MODULE !!!
 
 def init(config):
     """Daemon initialization function. This is run after daemon configuration is
     applied. In other words, facilities like logging, database connections etc.
     all work at this point.
     """
```

### Comparing `neurons-0.8.4/examples/garage/garage/model.py` & `neurons-0.9.1/examples/garage/garage/model.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/examples/garage/garage/service.py` & `neurons-0.9.1/examples/garage/garage/service.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/examples/garage/setup.py` & `neurons-0.9.1/examples/garage/setup.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/__init__.py` & `neurons-0.9.1/neurons/base/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/const.py` & `neurons-0.9.1/neurons/base/const.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/error.py` & `neurons-0.9.1/neurons/base/error.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/event.py` & `neurons-0.9.1/neurons/base/event.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/model.py` & `neurons-0.9.1/neurons/base/model.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/screen.py` & `neurons-0.9.1/neurons/base/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         }, 1);
     }
 };
 """
 
 HIDE_EMPTY_COLUMNS = """
 neurons.hide_empty_columns = function ($table) {
-    $($table.find("tr")[1]).find("td").each(function (_, elt) {
+    $($($table.find("tr")[1]).find("td").get().reverse()).each(function (_, elt) {
         setTimeout(function () {
             var cc = $(elt).attr("class").split(" ")[0];
             if ($table.find("td." + cc).text() == "") {
                 $table.find("td." + cc).hide();
                 $table.find("th." + cc).hide();
             }
         }, 0);
```

### Comparing `neurons-0.8.4/neurons/base/service.py` & `neurons-0.9.1/neurons/base/service.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/base/session.py` & `neurons-0.9.1/neurons/base/session.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/__init__.py` & `neurons-0.9.1/neurons/daemon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/_base.py` & `neurons-0.9.1/neurons/daemon/config/_base.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/_wdict.py` & `neurons-0.9.1/neurons/daemon/config/_wdict.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/daemon.py` & `neurons-0.9.1/neurons/daemon/config/daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     String, UnsignedInteger16, M, Integer32, ComplexModelMeta, ComplexModelBase
 from spyne.protocol import ProtocolBase
 from spyne.protocol.yaml import YamlDocument
 from spyne.util import six
 from spyne.util.dictdoc import get_object_as_yaml, get_yaml_as_object
 
 from neurons import is_reactor_thread, CONFIG_FILE_VERSION
+from neurons.daemon  import get_package_version
 from neurons.daemon.cli import spyne_to_argparse
 from neurons.daemon.daemonize import daemonize_do
 
 from neurons.daemon.config import LOGLEVEL_STR_MAP
 from neurons.daemon.config._wdict import wdict, Twdict
 from neurons.daemon.config.limits import LimitsChoice
 
@@ -69,35 +70,40 @@
     TDynamicallyRotatedLog, TTwistedHandler
 from neurons.daemon.config.store import RelationalStore, StorageInfo
 
 
 _some_prot = ProtocolBase()
 
 meminfo = None
+fdinfo = None
 
-def update_meminfo():
+
+def update_psutil_calls():
     """Call this when the process pid changes."""
 
     global meminfo
+    global fdinfo
 
     try:
         import psutil
         process = psutil.Process(os.getpid())
         try:  # psutil 2
             meminfo = process.get_memory_info
         except AttributeError:  # psutil 3
             meminfo = process.memory_info
 
+        fdinfo = process
+
         del process
 
     except ImportError:
         pass
 
 
-update_meminfo()
+update_psutil_calls()
 
 
 class _SetStaticPathAction(Action):
     def __init__(self, option_strings, dest, const=None, help=None):
         super(_SetStaticPathAction, self).__init__(nargs=1, const=const,
                             option_strings=option_strings, dest=dest, help=help)
 
@@ -138,14 +144,16 @@
 
 
 class Daemon(ConfigBase):
     """This is a custom daemon with only pid files, forking, logging.
     No setuid/setgid support is implemented.
     """
 
+    logging_init_done = False
+
     LOGGING_DEBUG_FORMAT = \
                      "%(l)s %(r)s | %(module)12s:%(lineno)-4d | %(message)s"
     LOGGING_DEVEL_FORMAT = "%(l)s | %(module)12s:%(lineno)-4d | %(message)s"
     LOGGING_PROD_FORMAT = \
                "%(l)s %(asctime)s | %(module)12s:%(lineno)-4d | %(message)s"
 
     _type_info = [
@@ -203,26 +211,41 @@
         ('version', Boolean(help="Show version", no_file=True)),
 
         ('bootstrap', Boolean(
             no_file=True,
             help="Bootstrap the application instead of starting it. "
                  "Create database schema, insert initial data, etc.")),
 
-        ('log_rss', Boolean(default=False,
+        ('log_exclusive', Boolean(
+            help="Remove previously configured log handlers.")),
+        ('log_optional', Boolean(
+            help="Don't configure a log handler if there are others already.")),
+        ('log_rss', Boolean(
             help="Prepend resident set size to all logging messages. "
                  "Requires psutil")),
-        ('log_protocol', Boolean(default=False,
-                                              help="Log protocol operations.")),
-        ('log_model', Boolean(default=False, help="Log model operations.")),
-        ('log_cloth', Boolean(default=False, help="Log cloth generation.")),
-        ('log_interface', Boolean(default=False,
-                                          help="Log interface build process.")),
+        ('log_fdstats', Boolean(
+            help="Prepend resident set size to all logging messages. "
+                 "Requires psutil")),
+        ('log_protocol', Boolean(
+            help="Log protocol operations."
+        )),
+        ('log_model', Boolean(
+            help="Log model operations."
+        )),
+        ('log_cloth', Boolean(
+            help="Log cloth generation."
+        )),
+        ('log_interface', Boolean(
+            help="Log interface build process."
+        )),
 
-        ('write_config', Boolean(no_file=True,
-                                   help="Write configuration file and exit.")),
+        ('write_config', Boolean(
+            no_file=True,
+            help="Write configuration file and exit."
+        )),
 
         ('alert_dests', Array(AlertDestination, default=[])),
 
         ('shell', Boolean(
             no_file=True, default=False,
             help="Drop to IPython shell. Useful for trying ORM stuff")),
         ('ikernel', Boolean(
@@ -356,14 +379,27 @@
             self.pid_file = abspath(self.pid_file)
 
     def apply_logging(self):
         # We're using twisted logging only for IO.
         from twisted.logger import FileLogObserver
         from twisted.logger import globalLogPublisher
 
+        if Daemon.logging_init_done:
+            return self
+
+        if len(logging.root.handlers) > 0 and self.log_optional:
+            logger.debug("Not configuring a neurons logging "
+                 "handler because previous logging handler(s) are found "
+                                                     "and log_optional == True")
+            return self
+
+        if len(logging.root.handlers) > 0 and self.log_exclusive:
+            logger.debug("Deleting previous logging handler(s)")
+            del logging.root.handlers[:]
+
         loggers = {}
 
         if self.logger_dest is not None:
             DynamicallyRotatedLog = TDynamicallyRotatedLog(self,
                                           self.logger_dest_rotation_compression)
 
             self.logger_dest = abspath(self.logger_dest)
@@ -409,49 +445,57 @@
                     print("coloarama not loaded: %r" % e)
 
         record_as_string = Trecord_as_string(formatter)
         observer = FileLogObserver(log_dest, record_as_string)
         globalLogPublisher.addObserver(observer)
         self._clear_other_observers(globalLogPublisher, observer)
 
-        TwistedHandler = TTwistedHandler(self, loggers, meminfo)
+        TwistedHandler = TTwistedHandler(self, loggers, meminfo, fdinfo)
 
         handler = TwistedHandler()
         handler.setFormatter(formatter)
         logging.getLogger().addHandler(handler)
 
         self.pre_logging_apply()
 
         for l in self.loggers.values() or []:
             l.set_parent(self)
             l.apply()
 
         self.boot_message()
 
+        Daemon.logging_init_done = True
+
         return self
 
     def boot_message(self):
         if self._boot_messaged:
             return
         self._boot_messaged = True
 
         import spyne
         import neurons
         import twisted
         import sqlalchemy
 
-        logger.info("Booting daemon '%s' with spyne-%s, neurons-%s, "
-            "sqlalchemy-%s and twisted-%s.", self.name,
+        myver = get_package_version(self.name)
+        if myver != "unknown":
+            myname = "{}-{}".format(self.name, myver)
+        else:
+            myname = self.name
+
+        logger.info("Booting daemon %s with spyne-%s, neurons-%s, "
+            "sqlalchemy-%s and twisted-%s.", myname,
                                 spyne.__version__, neurons.__version__,
                                 sqlalchemy.__version__, twisted.version.short())
 
     @staticmethod
     def hello_darkness_my_old_friend():
         logger.info("If you see this, it means something else has also "
-                "initialized the logging subsystem. This means you will get "
+                "initialized the logging subsystem. This means you may get "
                                                      "duplicate logging lines.")
 
     def pre_logging_apply(self):
         if self.debug:
             print("Root logger level = %s" %
                                     LOGLEVEL_STR_MAP[logging.getLogger().level])
 
@@ -544,15 +588,15 @@
                             "output. Please set logger_dest in the config file."
 
             workdir = self.workdir
             if workdir is None:
                 workdir = '/'
             daemonize_do(workdir=workdir)
 
-            update_meminfo()
+            update_psutil_calls()
 
         else:
             if self.workdir is not None:
                 os.chdir(self.workdir)
                 logger.debug("Change working directory to: %s", self.workdir)
 
 
@@ -696,15 +740,15 @@
         string and returns the new one.
 
         This is not supposed to be overridden. Override migrate_dict if you
         want add migration
         """
 
         import yaml
-        config_dict = yaml.load(s)
+        config_dict = yaml.safe_load(s)
         key, = config_dict.keys()
 
         config_root = config_dict[key]
         config_version = config_root.get(FILE_VERSION_KEY, None)
 
         if config_version is None:
             # Perform relational store migration
@@ -974,9 +1018,12 @@
 
                 if self.log_results:
                     self._set_log_level('sqlalchemy.engine', logging.DEBUG)
 
     def get_main_store(self):
         return self.stores[self.main_store].itself
 
+    def has_main_store(self):
+        return self.main_store in self.stores
+
     def get_main_store_config(self):
         return self.stores[self.main_store]
```

### Comparing `neurons-0.8.4/neurons/daemon/config/endpoint.py` & `neurons-0.9.1/neurons/daemon/config/endpoint.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/limits.py` & `neurons-0.9.1/neurons/daemon/config/limits.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/logutils.py` & `neurons-0.9.1/neurons/daemon/config/logutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             logger.info("Root logger level override: %s", self.level)
         else:
             logger.info("Logger level override %s = %s", self.path, self.level)
 
         return self
 
 
-def TTwistedHandler(config, loggers, _meminfo):
+def TTwistedHandler(config, loggers, _meminfo, _fdinfo):
     from twisted.logger import LogLevel
 
     # this is supposed to override the Logger object above. that's not cool but
     # that's the way it has to be
     from twisted.logger import Logger
 
     LOGLEVEL_TWISTED_MAP = {
@@ -125,34 +125,50 @@
         logging.CRITICAL: LogLevel.critical,
     }
 
     class TwistedHandler(logging.Handler):
         if config.log_rss:
             if _meminfo is None:
                 @staticmethod
-                def _modify_record(record):
+                def _modify_record_rss(record):
                     record.msg = '[psutil?] %s' % record.msg
             else:
                 @staticmethod
-                def _modify_record(record):
+                def _modify_record_rss(record):
                     meminfo = _meminfo()
                     record.msg = '[%.2f] %s' % \
                                          (meminfo.rss / 1024.0 ** 2, record.msg)
 
         else:
-            def _modify_record(self, record):
+            def _modify_record_rss(self, record):
+                pass
+
+        if config.log_fdstats:
+            if _fdinfo is None:
+                @staticmethod
+                def _modify_record_fd(record):
+                    record.msg = '[psutil?] %s' % record.msg
+            else:
+                @staticmethod
+                def _modify_record_fd(record):
+                    record.msg = '[%d/%d] %s' % \
+                      (len(_fdinfo.open_files()), _fdinfo.num_fds(), record.msg)
+
+        else:
+            def _modify_record_fd(self, record):
                 pass
 
         def emit(self, record):
             assert isinstance(record, logging.LogRecord)
 
             record.l = LOGLEVEL_MAP_ABB.get(record.levelno, "?")
             record.r = _get_reactor_thread_sigil(record)
 
-            self._modify_record(record)
+            self._modify_record_fd(record)
+            self._modify_record_rss(record)
 
             _logger = loggers.get(record.name, None)
             if _logger is None:
                 _logger = loggers[record.name] = Logger(record.name)
 
             if six.PY2 and hasattr(record, 'msg') \
                                                 and isinstance(record.msg, str):
```

### Comparing `neurons-0.8.4/neurons/daemon/config/static_file.py` & `neurons-0.9.1/neurons/daemon/config/static_file.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/config/store.py` & `neurons-0.9.1/neurons/daemon/config/store.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/const/__init__.py` & `neurons-0.9.1/neurons/daemon/dowser/const/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/const/graphs.html` & `neurons-0.9.1/neurons/daemon/dowser/const/graphs.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/const/main.css` & `neurons-0.9.1/neurons/daemon/dowser/const/main.css`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/const/trace.html` & `neurons-0.9.1/neurons/daemon/dowser/const/trace.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/const/tree.html` & `neurons-0.9.1/neurons/daemon/dowser/const/tree.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/__init__.py` & `neurons-0.9.1/neurons/daemon/dowser/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/app.py` & `neurons-0.9.1/neurons/daemon/dowser/app.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/dowser/reftree.py` & `neurons-0.9.1/neurons/daemon/dowser/reftree.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.maxdepth = maxdepth
         count = 0
         for result in self._gen(self.obj):
             yield result
             count += 1
             if maxresults and count >= maxresults:
                 yield 0, 0, "==== Max results reached ===="
-                raise StopIteration
+                return
 
     def print_tree(self, maxresults=100, maxdepth=None):
         """Walk the object tree, pretty-printing each branch."""
         self.ignore_caller()
         for depth, refid, rep in self.walk(maxresults, maxdepth):
             print ("%9d" % refid), (" " * depth * 2), rep
 
@@ -119,15 +119,15 @@
     return result
 
 
 class ReferentTree(Tree):
     def _gen(self, obj, depth=0):
         if self.maxdepth and depth >= self.maxdepth:
             yield depth, 0, "---- Max depth reached ----"
-            raise StopIteration
+            return
 
         for ref in gc.get_referents(obj):
             if id(ref) in self._ignore:
                 continue
             elif id(ref) in self.seen:
                 yield depth, id(ref), "!" + get_repr(ref)
                 continue
@@ -139,15 +139,15 @@
                 yield child
 
 
 class ReferrerTree(Tree):
     def _gen(self, obj, depth=0):
         if self.maxdepth and depth >= self.maxdepth:
             yield depth, 0, "---- Max depth reached ----"
-            raise StopIteration
+            return
 
         refs = gc.get_referrers(obj)
         refiter = iter(refs)
         self.ignore(refs, refiter)
         for ref in refiter:
             # Exclude all frames that are from this module.
             if isinstance(ref, FrameType):
@@ -180,20 +180,20 @@
         self.maxdepth = maxdepth
         count = 0
         for result in self._gen(self.obj):
             yield result
             count += 1
             if maxresults and count >= maxresults:
                 yield 0, 0, "==== Max results reached ===="
-                raise StopIteration
+                return
 
     def _gen(self, obj, depth=0, trail=None):
         if self.maxdepth and depth >= self.maxdepth:
             self.stops += 1
-            raise StopIteration
+            return
 
         if trail is None:
             trail = []
 
         for ref in gc.get_referents(obj):
             if id(ref) in self._ignore:
                 continue
```

### Comparing `neurons-0.8.4/neurons/daemon/dowser/service.py` & `neurons-0.9.1/neurons/daemon/dowser/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,18 @@
 import os
 import gc
 import sys
 
 from types import FrameType, ModuleType
 from collections import defaultdict
 
+from lxml.html.builder import E
 from neurons.daemon.dowser.const import ASSETS_DIR
 
-from spyne import rpc, Unicode, Service, ByteArray, AnyHtml
+from spyne import rpc, Unicode, Service, ByteArray, AnyHtml, Iterable
 from spyne import Integer
 from spyne.protocol.http import HttpPattern, HttpRpc
 from spyne.util.six import BytesIO
 
 from neurons.daemon.dowser import reftree
 
 
@@ -89,44 +90,89 @@
     p = {
         'maincss': "/assets/main.css",
         'home': "/",
     }
     p.update(params)
     return open(os.path.join(ASSETS_DIR, name)).read() % p
 
+"""
+curl $(python -c \
+    "from neurons.daemon.ipc import get_dowser_address_for_pid; \
+    print '%s:%d' % get_dowser_address_for_pid( $(pgrep ink_) )" )
+"""
 
 class DowserServices(Service):
     period = 5
     maxhistory = 300
     history = {}
     samples = 0
     id_history = []
-    max_id_history = 2
+    max_id_history = 200
+
+    @rpc(_returns=AnyHtml)
+    def snapshot(ctx):
+        ids = set()
+        for obj in gc.get_objects():
+            ids.add(id(obj))
+
+        DowserServices.id_history.append(ids)
+        if len(DowserServices.id_history) > DowserServices.max_id_history:
+            DowserServices.id_history.pop(0)
+
+        idhist = DowserServices.id_history
+        retval = E.table()
+        if len(idhist) > 1:
+            new, old = idhist[-1], idhist[0]
+            ids = sorted(new | old)
+            for oid in ids:
+                tr = E.tr()
+
+                if oid in new and not (oid in old):
+                    tr.append(E.td("New: {}".format(oid)))
+                    try:
+                        obj = next(ob for ob in gc.get_objects() if id(ob) == oid)
+                        if obj in idhist:
+                            continue
+                        try:
+                            if obj.__name__ in ('cell', 'frame'):
+                                continue
+                            if obj.__class__.__name__ in ('cell', 'frame'):
+                                continue
+                        except:
+                            pass
+
+                        reprobj = repr(obj)
+                        if len (reprobj) > 1024:
+                            reprobj = reprobj[:1024]
+                        tr.append(E.td(E.pre(repr(type(obj)))))
+                        tr.append(E.td(E.pre(reprobj)))
+                    except StopIteration:
+                        continue
+
+                    retval.append(tr)
+
+        return E.html(
+            E.head(E.style("td { vertical-align:top; }\n")),
+            E.body(retval)
+        )
 
     @classmethod
     def tick(cls):
         logger.debug("Dowser tick")
         gc.collect()
 
         typecounts = {}
-        new_ids = defaultdict(set)
         for obj in gc.get_objects():
             objtype = type(obj)
-            typename = ".".join((objtype.__module__, objtype.__name__))
-            new_ids[typename].add(id(obj))
 
             if objtype in typecounts:
                 typecounts[objtype] += 1
             else:
                 typecounts[objtype] = 1
 
-        if len(DowserServices.id_history) > DowserServices.max_id_history:
-            DowserServices.id_history.pop(0)
-        DowserServices.id_history.append(new_ids)
-
         for objtype, count in typecounts.items():
             typename = objtype.__module__ + "." + objtype.__name__
             if typename not in cls.history:
                 cls.history[typename] = [0] * cls.samples
             cls.history[typename].append(count)
 
         samples = cls.samples + 1
@@ -167,18 +213,19 @@
             hist = ctx.descriptor.service_class.history[typename]
 
             # get numbers
             maxhist = max(hist)
             minhist = max(hist)
             cur = hist[-1]
 
-            idhist = DowserServices.id_history
-            last = idhist[-1][typename]
-            first = idhist[0][typename]
-            diff = len(last) - len(first)
+            # idhist = DowserServices.id_history
+            # last = idhist[-1][typename]
+            # first = idhist[0][typename]
+            # diff = len(last) - len(first)
+            diff = -1  # FIXME
 
             # check floors
             show_this = cur >= cur_floor and \
                         minhist >= min_floor and \
                         maxhist >= max_floor and \
                         abs(diff) >= diff_floor
 
@@ -349,18 +396,18 @@
 
 class ReferrerTree(reftree.Tree):
     ignore_modules = True
 
     def _gen(self, obj, depth=0):
         if self.maxdepth and depth >= self.maxdepth:
             yield depth, 0, "---- Max depth reached ----"
-            raise StopIteration()
+            return
 
         if isinstance(obj, ModuleType) and self.ignore_modules:
-            raise StopIteration()
+            return
 
         refs = gc.get_referrers(obj)
         refiter = iter(refs)
         self.ignore(refs, refiter)
         thisfile = sys._getframe().f_code.co_filename
         for ref in refiter:
             # Exclude all frames that are from this module or reftree.
```

### Comparing `neurons-0.8.4/neurons/daemon/test/test_config.py` & `neurons-0.9.1/neurons/daemon/test/test_config.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/__init__.py` & `neurons-0.9.1/neurons/daemon/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,22 @@
 EXIT_ERR_UNKNOWN = 1
 # EXIT_SIGNAL = 100
 EXIT_ERR_MEMORY = 201
 EXIT_ERR_LISTEN_TCP = 100000
 EXIT_ERR_LISTEN_UDP = 200000
 
 
+def get_package_version(pkg_name):
+    try:
+        import pkg_resources
+        return pkg_resources.get_distribution(pkg_name).version
+    except Exception:
+        return 'unknown'
+
+
 from neurons.daemon import dowser
 from neurons.daemon.main import main
 
 from neurons.daemon.config import Service
 from neurons.daemon.config import Client
 from neurons.daemon.config import Server
 from neurons.daemon.config import SslServer
```

### Comparing `neurons-0.8.4/neurons/daemon/cli.py` & `neurons-0.9.1/neurons/daemon/cli.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/daemonize.py` & `neurons-0.9.1/neurons/daemon/daemonize.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/ipc.py` & `neurons-0.9.1/neurons/daemon/ipc.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/daemon/main.py` & `neurons-0.9.1/neurons/daemon/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,48 +29,39 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 from __future__ import print_function
 
-from time import time
-py_start_t = time()
-"""Approximate start time of the python code"""
-
 import logging
 logger = logging.getLogger(__name__)
 
 import os
 import threading
 import warnings
 import inspect
 
+from time import time
 from os.path import isfile, join, dirname
 
 from colorama import Fore
 
 from spyne.util.six import StringIO
 from spyne.util.color import DARK_R
 from spyne.store.relational.util import database_exists, create_database
 
 from sqlalchemy import MetaData
 
+from neurons import py_start_t
+from neurons.daemon import get_package_version
 from neurons.daemon.config import FileStore, ServiceDaemon, \
     RelationalStore, LdapStore, Server
 
 
-def get_package_version(pkg_name):
-    try:
-        import pkg_resources
-        return pkg_resources.get_distribution(pkg_name).version
-    except Exception:
-        return 'unknown'
-
-
 def _print_version(config):
     myver = get_package_version(config.name)
     if myver == 'unknown':
         print("Package '%s' version could not be determined. Please make "
               "sure a root package name is passed as daemon_name to the main "
               "function and also the package is correctly installed.")
     else:
@@ -162,24 +153,25 @@
     return 0  # to force exit
 
 
 def _do_bootstrap(config, init, bootstrap, bootstrapper):
     if bootstrap is None:
         bootstrap = bootstrapper(init)
     else:
-        config.apply()
+        config.apply(daemonize=False)
 
     assert callable(bootstrap), \
-                      "'bootstrap' must be a callable. It's %r." % bootstrap
+                          "'bootstrap' must be a callable. It's %r." % bootstrap
 
     # perform bootstrap
     retval = bootstrap(config)
 
     if retval is None:
         return 0  # to force exit
+
     return retval
 
 
 def _do_drop_all_tables(config, init):
     config.log_queries = True
     config.apply()
 
@@ -259,17 +251,20 @@
     if isinstance(config, ServiceDaemon):
         if config.main_store is None:
             config.main_store = 'sql_main'
 
         if config.debug_reactor:
             config.add_reactor_checks()
 
-        from neurons import TableModel
-        TableModel.Attributes.sqla_metadata.bind = \
+        if config.has_main_store():
+            from neurons import TableModel
+            TableModel.Attributes.sqla_metadata.bind = \
                                                   config.get_main_store().engine
+        else:
+            logger.debug('No sql data store configured.')
 
     # initialize applications
     items = init(config)
     if hasattr(items, 'items'):  # if it's a dict
         items = items.items()
 
     # apply app-specific config
@@ -565,14 +560,17 @@
 
     func_start_t = time()
     """Start time of post-import initialization code"""
 
     retcode, config = boot(config_name, argv, init, bootstrap,
                                                  bootstrapper, cls, daemon_name)
 
+    if retcode is not None:
+        return retcode
+
     # at this point it's safe to import the reactor (or anything else from
     # twisted) because the decision on whether to fork has already been made.
     from twisted.internet import reactor
     from twisted.internet.task import deferLater
 
     deferLater(reactor, 0, _compile_mappers) \
         .addErrback(lambda err: logger.error("%s", err.getTraceback()))
@@ -589,13 +587,13 @@
     if config.autoreload:
         from spyne.util.autorel import AutoReloader
         frequency = 0.5
         autorel = AutoReloader(frequency=frequency)
         assert autorel.start() is not None
         num_files = len(autorel.sysfiles() | autorel.files)
         logger.info("Auto reloader init success: Watching %d files "
-                                      "every %g seconds.", num_files, frequency)
+                                    "every %g second(s).", num_files, frequency)
 
     if config.dry_run:
         return 0
 
     return reactor.run()
```

### Comparing `neurons-0.8.4/neurons/daemon/store.py` & `neurons-0.9.1/neurons/daemon/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,11 +311,12 @@
             logger.info("{%s} (sqla) %r started with args: %r dsn: %r",
                                        self.name, self.engine, self.kwargs, dsn)
 
 
 def get_data_store(type, *args, **kwargs):
     if type == 'ldap':
         return LdapDataStore(*args, **kwargs)
-    elif type == 'sqlalchemy':
+
+    if type == 'sqlalchemy':
         return SqlDataStore(*args, **kwargs)
-    else:
-        raise ValueError("Unrecognized data store %r" % type)
+
+    raise ValueError("Unrecognized data store %r" % type)
```

### Comparing `neurons-0.8.4/neurons/form/const/__init__.py` & `neurons-0.9.1/neurons/form/const/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/const/test.html` & `neurons-0.9.1/neurons/form/const/test.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/test/__init__.py` & `neurons-0.9.1/neurons/form/test/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/test/test_form.py` & `neurons-0.9.1/neurons/form/test/test_form.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/test/test_form_table.py` & `neurons-0.9.1/neurons/form/test/test_form_table.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/__init__.py` & `neurons-0.9.1/neurons/form/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/form.py` & `neurons-0.9.1/neurons/form/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     $(".%(field_name)s_btn_add").click(add);
     $(".%(field_name)s_btn_del").click(del);
 });""" % {"field_name": key}, type="text/javascript"))
 
 
 _jstag = lambda src: E.script(src=src, type="text/javascript")
 _csstag = lambda src: E.link(href=src, type="text/css", rel="stylesheet")
-
+_NONEXISTENT = type('_NONEXISTENT', (object,), {})()
 
 
 def THtmlFormRoot(Base):
     class HtmlFormRoot(Base):
         def __init__(self, app=None, encoding='utf8',
                                       ignore_uncap=False, ignore_wrappers=False,
                 cloth=None, cloth_parser=None, polymorphic=True, hier_delim='.',
@@ -314,14 +314,45 @@
 
             # FIXME: hack! why do we have top-level object receiving name?
             if name == cls.get_type_name():
                 name = ''
 
             if in_fset:
                 default_text = cls.get_type_name()
+                if self.polymorphic:
+                    # give priority to sqla polymorphic types
+
+                    cls_attrs = self.get_cls_attrs(cls)
+                    mapper = cls_attrs.sqla_mapper
+                    if mapper is not None and mapper.polymorphic_on is not None:
+                        pmap = mapper.polymorphic_map
+                        pon = mapper.polymorphic_on.key
+
+                        pval = getattr(inst, pon, _NONEXISTENT)
+                        if pval is not _NONEXISTENT:
+                            ptype = pmap.get(pval)
+                            if ptype is None:
+                                pval = mapper.polymorphic_identity
+                                ptype = pmap.get(pval)
+
+                        else:
+                            pval = mapper.polymorphic_identity
+                            ptype = pmap.get(pval)
+
+                        if ptype is not None:
+                            if isinstance(ptype.class_, cls):
+                                default_text = ptype.class_.get_type_name()
+                            else:
+                                logger.debug("Ignoring sqla subclass %r "
+                                             "because not subclass of %r",
+                                                              ptype.class_, cls)
+
+                    elif isinstance(inst, cls):
+                        default_text = inst.__class__.get_type_name()
+
                 tr = self.trc(cls, ctx.locale, default_text)
                 parent.write(E.legend(tr))
 
             for k, v in fti:
                 subattr = self.get_cls_attrs(v)
                 if subattr.exc:
                     logger.debug("Excluding %s", k)
```

### Comparing `neurons-0.8.4/neurons/form/table.py` & `neurons-0.9.1/neurons/form/table.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/form/widget.py` & `neurons-0.9.1/neurons/form/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,21 +637,35 @@
             AnyUri: self.any_uri_to_parent,
             ComplexModelBase: self.complex_model_to_parent,
         })
 
     def _gen_text_str(self, cls, inst, **kwargs):
         text_str = self.to_unicode(cls, inst, **kwargs)
 
+        cls_attr = self.get_cls_attrs(cls)
         if text_str is None:
             text_str = ''
 
-            cls_attr = self.get_cls_attrs(cls)
             if cls_attr.min_occurs == 0:
                 return None
 
+        vd = cls_attr.values_dict
+        if vd is not None and len(vd) > 0:
+            try:
+                data =vd.get(text_str, None)
+            except TypeError:
+                logger.error("Invalid value %r for dict %r", text_str,
+                                                           cls_attr.values_dict)
+                raise
+
+            if data is None:
+                return "{} (!?)".format(text_str)
+
+            return data
+
         return text_str
 
     def _wrap_with_label_simple(self, ctx, cls, text_str, parent, name):
         label = self._gen_label_for(ctx, cls, name)
         attrib = self._gen_label_wrapper_class(ctx, cls, name)
 
         with parent.element('div', attrib=attrib):
```

### Comparing `neurons-0.8.4/neurons/geojson/__init__.py` & `neurons-0.9.1/neurons/geojson/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/geojson/model.py` & `neurons-0.9.1/neurons/geojson/model.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/log/__init__.py` & `neurons-0.9.1/neurons/log/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/log/method_call.py` & `neurons-0.9.1/neurons/log/method_call.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/log/method_return.py` & `neurons-0.9.1/neurons/log/method_return.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/log/model.py` & `neurons-0.9.1/neurons/log/model.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/comp/neurons-array/neurons-array.html` & `neurons-0.9.1/neurons/polymer/const/comp/neurons-array/neurons-array.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-dropdown.html` & `neurons-0.9.1/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-dropdown.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-href.html` & `neurons-0.9.1/neurons/polymer/const/comp/neurons-complex-reference/neurons-complex-href.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/comp/neurons-date-time/neurons-datetime-picker.html` & `neurons-0.9.1/neurons/polymer/const/comp/neurons-date-time/neurons-datetime-picker.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/comp/neurons-date-time/neurons-moment-validator.html` & `neurons-0.9.1/neurons/polymer/const/comp/neurons-date-time/neurons-moment-validator.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/comp/__init__.py` & `neurons-0.9.1/neurons/polymer/const/comp/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/__init__.py` & `neurons-0.9.1/neurons/polymer/const/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-from spyne.util.resource import parse_cloth_resource, read_resource_contents, \
+from spyne.util.resource import parse_cloth_resource, get_resource_file_contents, \
     parse_html_resource
 
 T_SCREEN = parse_html_resource(__name__, 'screen.html')
 T_DOM_MODULE = parse_cloth_resource(__name__, 'dom_module.html')
-POLYMER_PREAMBLE = read_resource_contents(__name__, 'preamble.js')
-POLYMER_DEFN_TEMPLATE = read_resource_contents(__name__, 'defn.js')
+POLYMER_PREAMBLE = get_resource_file_contents(__name__, 'preamble.js')
+POLYMER_DEFN_TEMPLATE = get_resource_file_contents(__name__, 'defn.js')
 
 DEFAULT_URL_POLYFILL = \
             '/static/bower_components/webcomponentsjs/webcomponents-lite.min.js'
 
 from . import comp
 
 del parse_cloth_resource
-del read_resource_contents
+del get_resource_file_contents
 del parse_html_resource
```

### Comparing `neurons-0.8.4/neurons/polymer/const/defn.js` & `neurons-0.9.1/neurons/polymer/const/defn.js`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/dom_module.html` & `neurons-0.9.1/neurons/polymer/const/dom_module.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/preamble.js` & `neurons-0.9.1/neurons/polymer/const/preamble.js`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/const/screen.html` & `neurons-0.9.1/neurons/polymer/const/screen.html`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/protocol/__init__.py` & `neurons-0.9.1/neurons/polymer/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/protocol/form.py` & `neurons-0.9.1/neurons/polymer/protocol/form.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/protocol/widget.py` & `neurons-0.9.1/neurons/polymer/protocol/widget.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/test/__init__.py` & `neurons-0.9.1/neurons/polymer/test/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/test/test_jsutil.py` & `neurons-0.9.1/neurons/polymer/test/test_jsutil.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/test/test_widget.py` & `neurons-0.9.1/neurons/polymer/test/test_widget.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/__init__.py` & `neurons-0.9.1/neurons/polymer/__init__.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/app.py` & `neurons-0.9.1/neurons/polymer/app.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/jsutil.py` & `neurons-0.9.1/neurons/polymer/jsutil.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/model.py` & `neurons-0.9.1/neurons/polymer/model.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/polymer/service.py` & `neurons-0.9.1/neurons/polymer/service.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/__init__.py` & `neurons-0.9.1/neurons/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '0.8.4'
+__version__ = '0.9.1'
 
 CONFIG_FILE_VERSION = 2
 
 REACTOR_THREAD = None
 REACTOR_THREAD_ID = None
 
 from neurons._base import _is_reactor_thread_none as is_reactor_thread
+from neurons._base import py_start_t
 
 from neurons.application import Application
 from neurons.model import TableModel
 from neurons.context import ReadContext, WriteContext
```

### Comparing `neurons-0.8.4/neurons/_base.py` & `neurons-0.9.1/neurons/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,7 +40,12 @@
 
 def _is_reactor_thread():
     return threading.current_thread().ident == neurons.REACTOR_THREAD_ID
 
 
 def _is_reactor_thread_none():
     return None
+
+
+from time import time
+py_start_t = time()
+"""Approximate start time of the python code"""
```

### Comparing `neurons-0.8.4/neurons/application.py` & `neurons-0.9.1/neurons/application.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/context.py` & `neurons-0.9.1/neurons/context.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/model.py` & `neurons-0.9.1/neurons/model.py`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/neurons/version.py` & `neurons-0.9.1/neurons/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,22 +71,21 @@
         for migopt in Version.migopts:
             Version.migrate(config, *migopt)
 
     @staticmethod
     def migrate(config, submodule, migration_dict, current_version,
                                                                   migrate_init):
         num_migops = 0
-        table_name = Version.Attributes.table_name
         Version.Attributes.sqla_table.create(checkfirst=True)
 
         db = config.get_main_store()
+        lock_name = "pg_advisory_xact_lock(0)"
         with closing(db.Session()) as session:
-            logger.info("Acquiring pg_advisory_xact_lock(0) "
-                                                    "for schema version checks")
-            session.connection().execute("select pg_advisory_xact_lock(0)")
+            logger.info("Acquiring %s for schema version checks", lock_name)
+            session.connection().execute("select {}".format(lock_name))
 
             # Create missing tables
             TableModel.Attributes.sqla_metadata.create_all(checkfirst=True)
 
             db_version = session.query(Version) \
                                          .filter_by(submodule=submodule).first()
 
@@ -114,14 +113,18 @@
             keys.sort()
 
             if len(keys) > 0:
                 logger.info("%s schema version detected as %s. "
                                 "Migration operation(s) %r will be performed",
                                             submodule, db_version.version, keys)
 
+            if config.dry_run:
+                logger.warning("Skipping migration due to dry run")
+                return
+
             for vernum in keys:
                 migrate = migration_dict[vernum]
 
                 with closing(db.Session()) as inner_session:
                     inner_db_version = inner_session.query(Version) \
                                            .filter_by(submodule=submodule).one()
                     inner_db_version.version = vernum
@@ -143,14 +146,14 @@
                     inner_session.commit()
 
                 num_migops += 1
                 logger.info("%s schema migration to version %d took %.1fs.",
                                             submodule, vernum, time() - start_t)
 
         if num_migops == 0:
-            logger.info("%s schema version detected as %s. Table unlocked.",
-                                                     submodule, current_version)
+            logger.info("%s schema version detected as %s, released %s.",
+                                          submodule, current_version, lock_name)
 
         elif num_migops > 0:
             logger.info("%s schema version upgraded to %s "
-                           "after %d migration operations. Table unlocked.",
-                                         submodule, current_version, num_migops)
+                           "after %d migration operations, released %s.",
+                              submodule, current_version, num_migops, lock_name)
```

### Comparing `neurons-0.8.4/neurons.egg-info/PKG-INFO` & `neurons-0.9.1/neurons.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-Metadata-Version: 1.2
+Metadata-Version: 1.1
 Name: neurons
-Version: 0.8.4
+Version: 0.9.1
 Summary: Neurons is a web framework tying together Spyne, Twisted and SQLAlchemy.
 Home-page: http://spyne.io/neurons
 Author: Burak Arslan
 Author-email: burak+neurons@arskom.com.tr
-Maintainer: Burak Arslan
-Maintainer-email: burak+neurons@arskom.com.tr
 License: LGPL-2.1
 Description: Neurons is a web framework tying together Spyne, Twisted and SQLAlchemy.
 Keywords: http
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `neurons-0.8.4/neurons.egg-info/SOURCES.txt` & `neurons-0.9.1/neurons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/.gitignore` & `neurons-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/LICENSE` & `neurons-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/README.md` & `neurons-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/run_tests.sh` & `neurons-0.9.1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `neurons-0.8.4/setup.py` & `neurons-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 try:
     os.stat('CHANGELOG.rst')
     LONG_DESC += "\n\n" + open('CHANGELOG.rst', 'r').read()
 except OSError:
     pass
 
 
-common_reqs = ('spyne>=2.12', 'SQLAlchemy', 'Twisted>=15.2',
+common_reqs = ('spyne>=2.12', 'SQLAlchemy<1.2.99', 'Twisted>=15.2',
     'lxml>=3.8.0', 'pyyaml', 'msgpack-python', 'pycrypto', 'slimit',
     'txpostgres', 'colorama',
 )
 
 
 test_reqs = common_reqs + ('pytest', 'pytest-cov', 'pytest-twisted',
     'tox',
@@ -98,23 +98,23 @@
     description=SHORT_DESC,
     long_description=LONG_DESC,
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'Natural Language :: English',
-        'Development Status :: 1 - Planning',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     keywords=('http',),
     author='Burak Arslan',
     author_email='burak+neurons@arskom.com.tr',
     maintainer='Burak Arslan',
```

### Comparing `neurons-0.8.4/PKG-INFO` & `neurons-0.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-Metadata-Version: 1.2
+Metadata-Version: 1.1
 Name: neurons
-Version: 0.8.4
+Version: 0.9.1
 Summary: Neurons is a web framework tying together Spyne, Twisted and SQLAlchemy.
 Home-page: http://spyne.io/neurons
 Author: Burak Arslan
 Author-email: burak+neurons@arskom.com.tr
-Maintainer: Burak Arslan
-Maintainer-email: burak+neurons@arskom.com.tr
 License: LGPL-2.1
 Description: Neurons is a web framework tying together Spyne, Twisted and SQLAlchemy.
 Keywords: http
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

