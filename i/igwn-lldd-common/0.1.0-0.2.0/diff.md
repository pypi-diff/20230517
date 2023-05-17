# Comparing `tmp/igwn-lldd-common-0.1.0.tar.gz` & `tmp/igwn-lldd-common-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igwn-lldd-common-0.1.0.tar", last modified: Wed Oct 12 07:20:17 2022, max compression
+gzip compressed data, was "igwn-lldd-common-0.2.0.tar", last modified: Wed May 17 08:51:10 2023, max compression
```

## Comparing `igwn-lldd-common-0.1.0.tar` & `igwn-lldd-common-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 07:20:17.482239 igwn-lldd-common-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    35131 2022-10-10 12:15:08.000000 igwn-lldd-common-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1017 2022-10-12 07:20:17.482239 igwn-lldd-common-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2022-10-10 12:15:08.000000 igwn-lldd-common-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     3586 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn-lldd-common.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 07:20:17.462239 igwn-lldd-common-0.1.0/igwn_lldd_common/
--rw-r--r--   0 root         (0) root         (0)      840 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9938 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/frame2kafka.py
--rw-r--r--   0 root         (0) root         (0)    30309 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/framekafkaconsumer.py
--rw-r--r--   0 root         (0) root         (0)    13423 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/framekafkaproducer.py
--rw-r--r--   0 root         (0) root         (0)    11131 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/framelen.py
--rw-r--r--   0 root         (0) root         (0)     2096 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/io.py
--rw-r--r--   0 root         (0) root         (0)    10971 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/kafka2frame.py
--rw-r--r--   0 root         (0) root         (0)    10017 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/messageparser.py
--rw-r--r--   0 root         (0) root         (0)     4904 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/statustopic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 07:20:17.462239 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 07:20:17.472239 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      154 2022-10-10 12:24:18.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3393 2022-10-10 14:40:00.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_inteface.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     3456 2022-10-10 12:31:20.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_inteface_inotify.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     4059 2022-10-10 12:15:08.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_inteface_multiple.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     5676 2022-10-10 12:24:18.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_kafka_fast_forward.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     4275 2022-10-10 12:15:08.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_kafka_fast_forward_multiple.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     5567 2022-10-10 12:24:18.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_kafka_single.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     1471 2022-10-10 12:24:18.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_frame_length.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     1383 2022-10-10 12:24:18.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_message_parser.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     6884 2022-10-10 12:24:18.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_status_updates.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 root         (0) root         (0)     3054 2022-10-10 12:24:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/__pycache__/test_utils.cpython-39-pytest-7.1.2.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 07:20:17.482239 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/
--rw-r--r--   0 root         (0) root         (0)     9098 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000000-1.gwf
--rw-r--r--   0 root         (0) root         (0)     9098 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000001-1.gwf
--rw-r--r--   0 root         (0) root         (0)     9098 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000002-1.gwf
--rw-r--r--   0 root         (0) root         (0)     3949 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_inteface.py
--rw-r--r--   0 root         (0) root         (0)     9297 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_kafka_fast_forward.py
--rw-r--r--   0 root         (0) root         (0)     9132 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_kafka_single.py
--rw-r--r--   0 root         (0) root         (0)      671 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_length.py
--rw-r--r--   0 root         (0) root         (0)     1163 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_message_parser.py
--rw-r--r--   0 root         (0) root         (0)     7719 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_status_updates.py
--rw-r--r--   0 root         (0) root         (0)     5520 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    11389 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/igwn_lldd_common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 07:20:17.462239 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2022-10-12 07:20:11.000000 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2137 2022-10-12 07:20:12.000000 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-12 07:20:11.000000 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2022-10-12 07:20:11.000000 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2022-10-12 07:20:11.000000 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-10-12 07:20:11.000000 igwn-lldd-common-0.1.0/igwn_lldd_common.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      288 2022-10-12 07:19:19.000000 igwn-lldd-common-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1417 2022-10-12 07:20:17.482239 igwn-lldd-common-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       37 2022-10-10 12:15:08.000000 igwn-lldd-common-0.1.0/setup.py
+drwxrwxr-x   0 poulton  (189600316) cascina   (1000)        0 2023-05-17 08:51:10.556258 igwn-lldd-common-0.2.0/
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    35131 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/LICENSE
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      150 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/MANIFEST.in
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     1775 2023-05-17 08:51:10.558261 igwn-lldd-common-0.2.0/PKG-INFO
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      438 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/README.md
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     3505 2023-05-17 08:49:44.000000 igwn-lldd-common-0.2.0/igwn-lldd-common.spec
+drwxrwxr-x   0 poulton  (189600316) cascina   (1000)        0 2023-05-17 08:51:10.388263 igwn-lldd-common-0.2.0/igwn_lldd_common/
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      840 2023-05-17 08:49:44.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/__init__.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     9681 2023-03-20 15:06:37.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/frame2kafka.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    30309 2023-05-16 08:06:00.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/framekafkaconsumer.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    13423 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/framekafkaproducer.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    11131 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/framelen.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     2703 2023-05-17 08:49:44.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/io.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    11332 2023-03-20 15:06:37.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/kafka2frame.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    10017 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/messageparser.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     4841 2023-05-17 08:49:44.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/statustopic.py
+drwxrwxr-x   0 poulton  (189600316) cascina   (1000)        0 2023-05-17 08:51:10.515261 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)        0 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/__init__.py
+drwxrwxr-x   0 poulton  (189600316) cascina   (1000)        0 2023-05-17 08:51:10.548261 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     9098 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000000-1.gwf
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     9098 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000001-1.gwf
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     9098 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000002-1.gwf
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     3949 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_inteface.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     9297 2022-10-06 13:45:56.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_kafka_fast_forward.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     9132 2022-10-06 13:45:56.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_kafka_single.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      671 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_length.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     1163 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_message_parser.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     7692 2023-05-17 08:49:44.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_status_updates.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     5520 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_utils.py
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)    11389 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/igwn_lldd_common/utils.py
+drwxrwxr-x   0 poulton  (189600316) cascina   (1000)        0 2023-05-17 08:51:10.439262 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     1775 2023-05-17 08:51:10.000000 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/PKG-INFO
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     1209 2023-05-17 08:51:10.000000 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)        1 2023-05-17 08:51:10.000000 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      114 2023-05-17 08:51:10.000000 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/entry_points.txt
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      136 2023-05-17 08:51:10.000000 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/requires.txt
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)       17 2023-05-17 08:51:10.000000 igwn-lldd-common-0.2.0/igwn_lldd_common.egg-info/top_level.txt
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)      439 2023-05-17 08:49:44.000000 igwn-lldd-common-0.2.0/pyproject.toml
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)     1734 2023-05-17 08:51:10.570265 igwn-lldd-common-0.2.0/setup.cfg
+-rw-rw-r--   0 poulton  (189600316) cascina   (1000)       37 2022-10-03 13:40:51.000000 igwn-lldd-common-0.2.0/setup.py
```

### Comparing `igwn-lldd-common-0.1.0/LICENSE` & `igwn-lldd-common-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn-lldd-common.spec` & `igwn-lldd-common-0.2.0/igwn-lldd-common.spec`

 * *Files 6% similar despite different names*

```diff
@@ -46,28 +46,25 @@
 #   https://git.ligo.org/computing/packaging/rhel/python-confluent-kafka/-/merge_requests/3
 # No plans to package kafka-python for Python 3.
 # If/when this package becomes available for Python3, then we can use:
 #   (see https://rpm-software-management.github.io/rpm/manual/boolean_dependencies.html )
 #   Requires: (python%{python3_pkgversion}-confluent-kafka or python%{python3_pkgversion}-kafka)
 Requires: python%{python3_pkgversion}-confluent-kafka
 
-%if 0%{?rhel} == 0 || 0%{?rhel} >= 8
-Requires: python%{python3_pkgversion}-ujson
-%endif
 %{?python_provide:%python_provide python%{python3_pkgversion}-%{srcname}}
 %description -n python%{python3_pkgversion}-%{srcname}
 The IGWN - Low Latency Data Distribution (lldd) is software to
 distribute low latency data used by the International
 Gravitational-Wave Observatory Network (IGWN).
 This package provides the Python %{python3_version} libraries.
 
 %package -n %{srcname}
 Summary: Command line utilities for igwn-lldd-common
 Requires: python%{python3_pkgversion}-%{srcname} = %{version}-%{release}
-Requires: python%{python3_pkgversion}-inotify
+Requires: python%{python3_pkgversion}-inotify_simple
 %description -n %{srcname}
 The IGWN - Low Latency Data Distribution (lldd) is software to
 distribute low latency data used by the International
 Gravitational-Wave Observatory Network (IGWN).
 This package provides the command-line interfaces.
 
 # -- build steps
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/__init__.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # igwn-lldd-common is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with igwn-lldd-common.  If not, see <http://www.gnu.org/licenses/>.
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/frame2kafka.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/frame2kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,30 +80,20 @@
         "-fd",
         "--frame-directory",
         type=str,
         help="The directory where the frames are written to"
     )
     parser.add_argument("-l", "--log", type=str, help="Standard log file")
     parser.add_argument(
-        "-nl",
-        "--no-log",
-        action="store_const",
+        "-v",
+        "--verbose",
         const=True,
         default=False,
-        help="no standard log",
-    )
-    parser.add_argument("-v", "--verbose", type=str, help="Verbose log file")
-    parser.add_argument(
-        "-nv",
-        "--no-verbose",
-        action="store_const",
-        const=True,
-        default=False,
-        help="no verbose log",
-    )
+        action='store_const',
+        help="Verbose log file")
     parser.add_argument("-g", "--group-id", type=str, help="Kafka group ID")
     parser.add_argument(
         "-S",
         "--split-bytes",
         type=int,
         default=100000,
         help="Split messages into this many bytes when adding to Kafka",
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/framekafkaconsumer.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/framekafkaconsumer.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/framekafkaproducer.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/framekafkaproducer.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/framelen.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/framelen.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/io.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import logging
+import shutil
 
 logger = logging.getLogger()
 
 try:
     from watchdog.events import PatternMatchingEventHandler
 
     class FrameFileEventHandler(PatternMatchingEventHandler):
@@ -18,59 +19,77 @@
             if event.is_directory:
                 return
 
             self.queue.put(event.src_path)
 
 except ImportError:
     import threading
-    import inotify.adapters
+    from inotify_simple import INotify, flags
 
     # Thread to watch over watch_dir
     def monitor_dir_inotify(queue, watch_dir):
 
-        # create a watcher thread only watching for in close write event
-        i = inotify.adapters.Inotify()
-        i.add_watch(watch_dir, inotify.constants.IN_CLOSE_WRITE)
+        # create a watcher thread watching for write or moved events
+        i = INotify()
+        i.add_watch(watch_dir, flags.CLOSE_WRITE | flags.MOVED_TO)
 
         # Get the current thread
         t = threading.currentThread()
 
         # Check if this thread should stop
         while not t.stop:
 
             # Loop over the events and check when a file has been created
-            for event in i.event_gen(yield_nones=False, timeout_s=1):
+            for event in i.read(timeout=1):
 
-                # Check if the event was a close write
-                (_, _, path, filename) = event
+                # directory was removed, so the corresponding watch was
+                # also removed
+                if flags.IGNORED in flags.from_mask(event.mask):
+                    break
+
+                # ignore temporary files
+                filename = event.name
+                extension = os.path.splitext(filename)[1]
+                if extension != ".gwf":
+                    continue
 
                 # Add the filename to the queue
-                queue.put(os.path.join(path, filename))
+                queue.put(os.path.join(watch_dir, filename))
 
         # Remove the watch
-        i.remove_watch(watch_dir)
+        i.rm_watch(watch_dir)
 
 
-def write_frame(file_name, frame_data, fl_ringn, file_name_dq):
-
-    # write to disk
-    with open(file_name, "wb") as fl_file:
-        fl_file.write(frame_data)
-        fl_file.close()
+def write_frame(file_name, frame_data, fl_ringn, file_name_dq, tmpdir=None):
+    # determine temporary filename/directory
+    if tmpdir:
+        file = os.path.basename(file_name)
+    else:
+        tmpdir, file = os.path.split(file_name)
+    tmp_file_name = os.path.join(tmpdir, f".{file}.tmp")
+
+    # write frame to disk
+    # NOTE: this is atomic if on the same filesystem
+    with open(tmp_file_name, "wb") as f:
+        f.write(frame_data)
+        # ensure all data is on disk
+        f.flush()
+        os.fsync(f.fileno())
+    shutil.move(tmp_file_name, file_name)
+
+    #
+    # ring of frame_log files?
+    if fl_ringn:
+        #
+        # name queue full?
+        if len(file_name_dq) == fl_ringn:
+            old_file = file_name_dq.popleft()
+            try:
+                os.unlink(old_file)
+            except OSError:
+                logger.error(
+                    f"Error: could not delete file [{old_file}]"
+                )
 
         #
-        # ring of frame_log files?
-        if fl_ringn:
-            #
-            # name queue full?
-            if len(file_name_dq) == fl_ringn:
-                old_file = file_name_dq.popleft()
-                try:
-                    os.unlink(old_file)
-                except OSError:
-                    logger.error(
-                        f"Error: could not delete file [{old_file}]"
-                    )
-
-            #
-            # add this file to queue
-            file_name_dq.append(file_name)
+        # add this file to queue
+        file_name_dq.append(file_name)
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/kafka2frame.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/kafka2frame.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         help="specify the Kafka cluster bootstrap servers",
     )
     parser.add_argument(
         "-a",
         "--add-topic-partition",
         type=str,
         action="append",
+        required=True,
         help="/topic=LHO_Data/partition=KLHO_Data/nbuf=16/lbuf=1000000 \
 /delta-t=4/crc-check=true/",
     )
     parser.add_argument(
         "-x",
         "--exit-if-missing-topics",
         action="store_const",
@@ -326,23 +327,32 @@
                 frame_filename = re.sub(
                     "%tag%",
                     payload_info["topic"],
                     frame_filename,
                 )
 
                 # do we have to calculate dynamically the length of the frame?
-                if dyn_frame_len[payload_info["topic"]]:
+                if (
+                    dyn_frame_len[payload_info["topic"]]
+                    or "frame_duration" not in payload_info.keys()
+                ):
                     (
                         frame_start_time,
                         frame_stop_time,
                         frame_duration,
                     ) = frame_length(frame_buffer)
                     frame_filename = re.sub(
                         "%delta_t%", str(int(frame_duration)), frame_filename
                     )
+                else:
+                    frame_filename = re.sub(
+                        "%delta_t%",
+                        str(int(payload_info["frame_duration"])),
+                        frame_filename
+                    )
 
                 # now write this to the shared memory partition
                 write_frame(
                     frame_filename,
                     frame_buffer,
                     ringn_topic[topic],
                     file_name_dq[topic]
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/messageparser.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/messageparser.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/statustopic.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/statustopic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,17 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with igwn-lldd-common.  If not, see <http://www.gnu.org/licenses/>.
 
 # Code for getting the name of this host/node
 import socket
+import json
 import logging
 
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-
 logger = logging.getLogger(__name__)
 
 
 class StatusUpdater:
     def __init__(self, args):
 
         self.load_kafka_python = args.load_kafka_python
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000000-1.gwf` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000000-1.gwf`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000001-1.gwf` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000001-1.gwf`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000002-1.gwf` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/data/Z-igwn_lldd_common_test-1000000002-1.gwf`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_inteface.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_inteface.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_kafka_fast_forward.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_kafka_fast_forward.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_kafka_single.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_kafka_single.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_frame_length.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_frame_length.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_message_parser.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_message_parser.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_status_updates.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_status_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from igwn_lldd_common.statustopic import StatusUpdater
 import confluent_kafka
 import kafka
 import os
 import pytest
-import ujson
+import json
 import time
 
 
 CONFLUENT_TOPIC = "TestStatusConfluent"
 KAFKA_TOPIC = "TestStatusKafka"
 
 
@@ -86,16 +86,16 @@
 
     # Double check the correct topic was consumed
     assert topic == CONFLUENT_TOPIC, "Error: wrong topic was consumed"
 
     # Check to see if the payload is empty
     assert len(payload) != 0, "Payload is empty"
 
-    # Decode the payload using ujson
-    status = ujson.loads(payload)
+    # Decode the payload
+    status = json.loads(payload)
 
     # Check the values in the message
     if "status" in status.keys():
         assert status["status"] == "test", \
             "The status is incorrect in the message"
     else:
         pytest.exit("The 'status' key was not in the status message")
@@ -189,16 +189,16 @@
     # Extract the message payload and topic
     payload = message.value
     topic = message.topic
 
     # Double check the correct topic was consumed
     assert topic == KAFKA_TOPIC, "Error: wrong topic was consumed"
 
-    # Decode the payload using ujson
-    status = ujson.loads(payload)
+    # Decode the payload
+    status = json.loads(payload)
 
     # Check the values in the message
     if "status" in status.keys():
         assert status["status"] == "test", \
             "The status is incorrect in the message"
     else:
         pytest.exit("The 'status' key was not in the status message")
```

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/tests/test_utils.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/igwn_lldd_common/utils.py` & `igwn-lldd-common-0.2.0/igwn_lldd_common/utils.py`

 * *Files identical despite different names*

### Comparing `igwn-lldd-common-0.1.0/setup.cfg` & `igwn-lldd-common-0.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 [metadata]
 name = igwn-lldd-common
 version = attr: igwn_lldd_common.__version__
 author = Rhys Poulton
 author_email = poulton@ego-gw.it
 description = International Gravitational Wave Network (IGWN) low latency data distribution
+long_description = file: README.md
+long_description_content_type = text/markdown
 license = GPL-3.0-or-later
 license_files = LICENSE
+url = https://git.ligo.org/computing/lowlatency/igwn-lldd-common/
+project_urls = 
+	Bug Tracker = https://git.ligo.org/computing/lowlatency/igwn-lldd-common/-/issues
+	Source Code = https://git.ligo.org/computing/lowlatency/igwn-lldd-common
 classifiers = 
 	Development Status :: 1 - Planning
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
@@ -21,34 +27,34 @@
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 packages = find:
 python_requires = >=3.6
-setup_requires = 
-	setuptools >= 38.2.5
 install_requires = 
 	confluent-kafka
 	configargparse
-	ujson
 	gpstime
 	watchdog
 include_package_data = true
 
 [options.entry_points]
 console_scripts = 
 	kafka2frame = igwn_lldd_common.kafka2frame:main
 	frame2kafka = igwn_lldd_common.frame2kafka:main
 
 [options.extras_require]
+apache-kafka = 
+	kafka-python
 test = 
+	flaky
+	kafka-python
 	pytest >=3.9.1
 	pytest-cov >=2.4.0
-	flaky
 
 [flake8]
 select = 
 	E,
 	EXE,
 	F,
 	W,
```

