# Comparing `tmp/pybgpkit_parser-0.4.2.tar.gz` & `tmp/pybgpkit_parser-0.4.3.tar.gz`

## Comparing `pybgpkit_parser-0.4.2.tar` & `pybgpkit_parser-0.4.3.tar`

### file list

```diff
@@ -1,109 +1,11 @@
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.toml
--rw-r--r--   0      501       20       23 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/.gitignore
--rw-r--r--   0      501       20    49749 2022-08-10 17:21:22.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.lock
--rw-r--r--   0      501       20     1069 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/LICENSE
--rw-r--r--   0      501       20      624 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/README.md
--rw-r--r--   0      501       20     5024 2023-02-25 16:01:29.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/bench_main.rs
--rw-r--r--   0      501       20     5326 2023-03-09 20:32:42.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/data_source.rs
--rw-r--r--   0      501       20     3428 2023-02-25 16:01:14.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/internals.rs
--rw-r--r--   0      501       20      858 2023-04-09 05:55:46.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/cache_reading.rs
--rw-r--r--   0      501       20      335 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/count_elems.rs
--rw-r--r--   0      501       20      365 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/display_elems.rs
--rw-r--r--   0      501       20     1062 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/extended_communities.rs
--rw-r--r--   0      501       20     1750 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/filters.rs
--rw-r--r--   0      501       20     1381 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/find_as_set_messages.rs
--rw-r--r--   0      501       20      441 2023-03-26 05:27:50.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/only-to-customer.rs
--rw-r--r--   0      501       20      992 2023-03-09 20:37:57.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-files-from-broker-parallel.rs
--rw-r--r--   0      501       20     1292 2023-04-03 03:02:57.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-files-from-broker.rs
--rw-r--r--   0      501       20      701 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-single-file.rs
--rw-r--r--   0      501       20      594 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/peer_index_table.rs
--rw-r--r--   0      501       20     1354 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/real-time-ris-live-websocket.rs
--rw-r--r--   0      501       20     2612 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/real-time-routeviews-kafka-openbmp.rs
--rw-r--r--   0      501       20     1436 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/records_iter.rs
--rw-r--r--   0      501       20     4537 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/bin/README.md
--rw-r--r--   0      501       20     5291 2023-03-26 07:22:12.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/bin/main.rs
--rw-r--r--   0      501       20     2540 2023-03-12 16:52:38.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/error.rs
--rw-r--r--   0      501       20    13426 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/lib.rs
--rw-r--r--   0      501       20     7528 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/aspath.rs
--rw-r--r--   0      501       20      809 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/atomic_aggregate.rs
--rw-r--r--   0      501       20     4353 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/mod.rs
--rw-r--r--   0      501       20     1057 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/nlri.rs
--rw-r--r--   0      501       20      718 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/origin.rs
--rw-r--r--   0      501       20     6822 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/capabilities.rs
--rw-r--r--   0      501       20     9926 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/community.rs
--rw-r--r--   0      501       20     6267 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/elem.rs
--rw-r--r--   0      501       20    20404 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/error.rs
--rw-r--r--   0      501       20     3208 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/mod.rs
--rw-r--r--   0      501       20     3338 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/role.rs
--rw-r--r--   0      501       20      635 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/err.rs
--rw-r--r--   0      501       20     3179 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mod.rs
--rw-r--r--   0      501       20     1742 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/bgp4mp.rs
--rw-r--r--   0      501       20     5569 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/mod.rs
--rw-r--r--   0      501       20     6963 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/tabledump.rs
--rw-r--r--   0      501       20      512 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/afi.rs
--rw-r--r--   0      501       20     1479 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/asn.rs
--rw-r--r--   0      501       20      152 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/mod.rs
--rw-r--r--   0      501       20      899 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/nexthop.rs
--rw-r--r--   0      501       20     1035 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/prefix.rs
--rw-r--r--   0      501       20     1658 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/README.md
--rw-r--r--   0      501       20     1887 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_01_origin.rs
--rw-r--r--   0      501       20     5573 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_02_17_as_path.rs
--rw-r--r--   0      501       20     3095 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_03_next_hop.rs
--rw-r--r--   0      501       20      508 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_04_med.rs
--rw-r--r--   0      501       20      508 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_05_local_pref.rs
--rw-r--r--   0      501       20     2197 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_07_18_aggregator.rs
--rw-r--r--   0      501       20     1986 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_08_communities.rs
--rw-r--r--   0      501       20     1117 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_09_originator.rs
--rw-r--r--   0      501       20     1252 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_10_13_cluster.rs
--rw-r--r--   0      501       20     6012 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_14_15_nlri.rs
--rw-r--r--   0      501       20    12414 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_16_25_extended_communities.rs
--rw-r--r--   0      501       20     1663 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_32_large_communities.rs
--rw-r--r--   0      501       20     2034 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_35_otc.rs
--rw-r--r--   0      501       20     8076 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/mod.rs
--rw-r--r--   0      501       20     8727 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/messages.rs
--rw-r--r--   0      501       20      116 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/mod.rs
--rw-r--r--   0      501       20     1198 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/error.rs
--rw-r--r--   0      501       20     5207 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/headers.rs
--rw-r--r--   0      501       20     1189 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/initiation_message.rs
--rw-r--r--   0      501       20     1473 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/mod.rs
--rw-r--r--   0      501       20     2419 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_down_notification.rs
--rw-r--r--   0      501       20     1627 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_up_notification.rs
--rw-r--r--   0      501       20     1684 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_mirroring.rs
--rw-r--r--   0      501       20      569 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_monitoring.rs
--rw-r--r--   0      501       20     1086 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/stats_report.rs
--rw-r--r--   0      501       20     1184 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/termination_message.rs
--rw-r--r--   0      501       20     5380 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/mod.rs
--rw-r--r--   0      501       20     5766 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/openbmp.rs
--rw-r--r--   0      501       20    16954 2023-04-09 04:44:23.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/filter.rs
--rw-r--r--   0      501       20     6855 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/iters.rs
--rw-r--r--   0      501       20     5212 2023-04-09 05:55:46.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mod.rs
--rw-r--r--   0      501       20     7368 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/bgp4mp.rs
--rw-r--r--   0      501       20       96 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/mod.rs
--rw-r--r--   0      501       20     3808 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_message.rs
--rw-r--r--   0      501       20     6910 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_v2_message.rs
--rw-r--r--   0      501       20      360 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mod.rs
--rw-r--r--   0      501       20    14992 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_elem.rs
--rw-r--r--   0      501       20     6843 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_record.rs
--rw-r--r--   0      501       20     1934 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/error.rs
--rw-r--r--   0      501       20     2412 2023-03-30 03:44:46.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/mod.rs
--rw-r--r--   0      501       20       98 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/pong.rs
--rw-r--r--   0      501       20     4109 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/raw_bytes.rs
--rw-r--r--   0      501       20      128 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_error.rs
--rw-r--r--   0      501       20     3916 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_message.rs
--rw-r--r--   0      501       20      104 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_rrc_list.rs
--rw-r--r--   0      501       20      191 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_subscribe_ok.rs
--rw-r--r--   0      501       20    10786 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/mod.rs
--rw-r--r--   0      501       20    10214 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/utils.rs
--rw-r--r--   0      501       20      792 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/tests/bgpkit-parser-tests.rs
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.2/Cargo.toml
--rw-r--r--   0      501       20        5 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/.gitignore
--rw-r--r--   0      501       20      952 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.2/Dockerfile
--rw-r--r--   0      501       20     1063 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/LICENSE
--rw-r--r--   0      501       20     2182 2023-03-30 05:18:22.000000 pybgpkit_parser-0.4.2/README.md
--rw-r--r--   0      501       20       71 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/build.rs
--rw-r--r--   0      501       20       76 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/pyproject.toml
--rw-r--r--   0      501       20     3940 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/src/lib.rs
--rw-r--r--   0      501       20      297 2023-04-09 06:00:05.000000 pybgpkit_parser-0.4.2/test-cache.py
--rw-r--r--   0      501       20      315 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.2/test.py
--rw-r--r--   0      501       20    36797 2022-11-03 17:46:36.000000 pybgpkit_parser-0.4.2/Cargo.lock
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.3/Cargo.toml
+-rw-r--r--   0      501       20        5 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.3/.gitignore
+-rw-r--r--   0      501       20      952 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.3/Dockerfile
+-rw-r--r--   0      501       20     1063 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.3/LICENSE
+-rw-r--r--   0      501       20     2182 2023-03-30 05:18:22.000000 pybgpkit_parser-0.4.3/README.md
+-rw-r--r--   0      501       20       71 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.3/build.rs
+-rw-r--r--   0      501       20       76 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.3/pyproject.toml
+-rw-r--r--   0      501       20     3940 2023-05-17 17:40:45.000000 pybgpkit_parser-0.4.3/src/lib.rs
+-rw-r--r--   0      501       20      315 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.3/test.py
+-rw-r--r--   0      501       20    36797 2022-11-03 17:46:36.000000 pybgpkit_parser-0.4.3/Cargo.lock
+-rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.3/PKG-INFO
```

### Comparing `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.lock` & `pybgpkit_parser-0.4.3/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "addr2line"
-version = "0.17.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ecd88a8c8378ca913a680cd98f0f13ac67383d35993f86c90a70e3f137816b"
-dependencies = [
- "gimli",
-]
-
-[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aho-corasick"
@@ -35,32 +26,17 @@
  "hermit-abi",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
-
-[[package]]
-name = "backtrace"
-version = "0.3.65"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a17d453482a265fd5f8479f2a3f405566e6ca627837aaddb85af8b1ab8ef61"
-dependencies = [
- "addr2line",
- "cc",
- "cfg-if",
- "libc",
- "miniz_oxide",
- "object",
- "rustc-demangle",
-]
+checksum = "cdb031dd78e28731d87d56cc8ffef4a8f36ca26c38fe2de700543e627f8a464a"
 
 [[package]]
 name = "base64"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "904dfeac50f3cdaba28fc6f57fdcddb75f49ed61346676a78c4ffe55877802fd"
 
@@ -69,108 +45,54 @@
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "545094a914719f374c1ed4d9bfa788aa8a5b4ba82f9f863b5f680b735d9ca3a3"
 dependencies = [
  "enum-primitive-derive",
  "ipnetwork",
  "itertools",
- "log 0.4.17",
- "num-traits 0.2.15",
- "serde",
-]
-
-[[package]]
-name = "bgpkit-broker"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "556be3703d7cb7ce747728175c2ded6461652632f084206c49abdd8a8164a0cb"
-dependencies = [
- "log 0.4.17",
- "reqwest",
+ "log",
+ "num-traits 0.2.14",
  "serde",
 ]
 
 [[package]]
 name = "bgpkit-parser"
 version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd4129f8e436b8bc1f7d074c85dd4fdcdff4be7bf14306ff0d9eb5b021546bbb"
 dependencies = [
  "bgp-models",
- "bgpkit-broker",
  "chrono",
- "clap 3.2.16",
- "criterion",
+ "clap",
  "enum-primitive-derive",
  "env_logger",
  "hex",
  "ipnetwork",
  "itertools",
- "kafka",
- "log 0.4.17",
+ "log",
  "num-traits 0.1.43",
  "oneio",
- "rayon",
  "regex",
  "serde",
  "serde_json",
- "tungstenite",
- "url",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "block-buffer"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
-name = "bstr"
-version = "0.2.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
-dependencies = [
- "lazy_static",
- "memchr",
- "regex-automata",
- "serde",
-]
-
-[[package]]
-name = "build_const"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4ae4235e6dac0694637c763029ecea1a2ec9e4e06ec2729bd21ba4d9c863eb7"
-
-[[package]]
 name = "bumpalo"
 version = "3.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4a45a46ab1f2412e53d3a0ade76ffad2025804294569aae387231a0cd6e0899"
 
 [[package]]
-name = "byteorder"
-version = "0.5.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc10e8cc6b2580fda3f36eb6dc5316657f812a3df879a44a66fc9f0fdbc4855"
-
-[[package]]
-name = "byteorder"
-version = "1.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
-
-[[package]]
 name = "bytes"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4872d67bab6358e59559027aa3b9157c53d9358c51423c17554809a8858e0f8"
 
 [[package]]
 name = "bzip2"
@@ -190,27 +112,18 @@
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
-name = "cast"
-version = "0.2.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c24dab4283a142afa2fdca129b80ad2c6284e073930f964c3a1293c225ee39a"
-dependencies = [
- "rustc_version",
-]
-
-[[package]]
 name = "cc"
-version = "1.0.73"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fff2a6927b3bb87f9595d67196a70493f627687a71d87a0d692242c33f58c11"
+checksum = "22a9137b95ea06864e018375b72adfb7db6e6f68cfc8df5a04d00288050485ee"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -218,52 +131,41 @@
 name = "chrono"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "670ad68c9088c2a963aaa298cb369688cf3f9465ce5e2d4ca10e6e0098a1ce73"
 dependencies = [
  "libc",
  "num-integer",
- "num-traits 0.2.15",
+ "num-traits 0.2.14",
  "time",
  "winapi",
 ]
 
 [[package]]
 name = "clap"
-version = "2.34.0"
+version = "3.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
-dependencies = [
- "bitflags",
- "textwrap 0.11.0",
- "unicode-width",
-]
-
-[[package]]
-name = "clap"
-version = "3.2.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3dbbb6653e7c55cc8595ad3e1f7be8f32aba4eb7ff7f0fd1163d4f3d137c0a9"
+checksum = "8e538f9ee5aa3b3963f09a997035f883677966ed50fce0292611927ce6f6d8c6"
 dependencies = [
  "atty",
  "bitflags",
  "clap_derive",
  "clap_lex",
  "indexmap",
- "once_cell",
+ "lazy_static",
  "strsim",
  "termcolor",
- "textwrap 0.15.0",
+ "textwrap",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.15"
+version = "3.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ba52acd3b0a5c33aeada5cdaa3267cdc7c594a98731d4268cdc1532f4264cb4"
+checksum = "a7f98063cac4652f23ccda556b8d04347a7fc4b2cff1f7577cc8c6546e0d8078"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn",
 ]
@@ -275,241 +177,105 @@
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "6888e10551bb93e424d8df1d07f1a8b4fceb0001a3a4b048bfc47554946f47b3"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
 
 [[package]]
-name = "cpufeatures"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59a6001667ab124aebae2a495118e11d30984c3a653e99d86d58971708cf5e4b"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "crc"
-version = "1.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d663548de7f5cca343f1e0a48d14dcfb0e9eb4e079ec58883b7251539fa10aeb"
-dependencies = [
- "build_const",
-]
-
-[[package]]
 name = "crc32fast"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "criterion"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1604dafd25fba2fe2d5895a9da139f8dc9b319a5fe5354ca137cbbce4e178d10"
-dependencies = [
- "atty",
- "cast",
- "clap 2.34.0",
- "criterion-plot",
- "csv",
- "itertools",
- "lazy_static",
- "num-traits 0.2.15",
- "oorandom",
- "plotters",
- "rayon",
- "regex",
- "serde",
- "serde_cbor",
- "serde_derive",
- "serde_json",
- "tinytemplate",
- "walkdir",
-]
-
-[[package]]
-name = "criterion-plot"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d00996de9f2f7559f7f4dc286073197f83e92256a59ed395f9aac01fe717da57"
-dependencies = [
- "cast",
- "itertools",
-]
-
-[[package]]
-name = "crossbeam-channel"
-version = "0.5.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aaa7bd5fb665c6864b5f963dd9097905c54125909c7aa94c9e18507cdbe6c53"
-dependencies = [
- "cfg-if",
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-deque"
-version = "0.8.1"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6455c0ca19f0d2fbf751b908d5c55c1f5cbc65e03c4225427254b46890bdde1e"
+checksum = "738c290dfaea84fc1ca15ad9c168d083b05a714e1efddd8edaab678dc28d2836"
 dependencies = [
  "cfg-if",
- "crossbeam-epoch",
- "crossbeam-utils",
 ]
 
 [[package]]
-name = "crossbeam-epoch"
-version = "0.9.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1145cf131a2c6ba0615079ab6a638f7e1973ac9c2634fcbeaaad6114246efe8c"
-dependencies = [
- "autocfg",
- "cfg-if",
- "crossbeam-utils",
- "lazy_static",
- "memoffset",
- "scopeguard",
-]
-
-[[package]]
-name = "crossbeam-utils"
-version = "0.8.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bf124c720b7686e3c2663cf54062ab0f68a88af2fb6a030e87e30bf721fcb38"
-dependencies = [
- "cfg-if",
- "lazy_static",
-]
-
-[[package]]
-name = "csv"
-version = "1.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22813a6dc45b335f9bade10bf7271dc477e81113e89eb251a0bc2a8a81c536e1"
-dependencies = [
- "bstr",
- "csv-core",
- "itoa 0.4.8",
- "ryu",
- "serde",
-]
-
-[[package]]
-name = "csv-core"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
-dependencies = [
- "memchr",
-]
-
-[[package]]
-name = "digest"
-version = "0.9.0"
+name = "dict_derive"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
+checksum = "6207f46b33b2bf00858b0edb03d188d31a46fedfde4aa53a27d69fe25acd80cf"
 dependencies = [
- "generic-array",
+ "proc-macro2",
+ "quote",
+ "syn",
 ]
 
 [[package]]
 name = "either"
 version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e78d4f1cc4ae33bbfc157ed5d5a5ef3bc29227303d595861deb238fcec4e9457"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.31"
+version = "0.8.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9852635589dc9f9ea1b6fe9f05b50ef208c85c834a562f0c6abb1c475736ec2b"
+checksum = "7896dc8abb250ffdda33912550faa54c88ec8b998dec0b2c55ab224921ce11df"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "enum-primitive-derive"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c375b9c5eadb68d0a6efee2999fef292f45854c3444c86f09d8ab086ba942b0e"
 dependencies = [
- "num-traits 0.2.15",
+ "num-traits 0.2.14",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b2cf0344971ee6c64c31be0d530793fba457d322dfec2810c453d0ef228f9c3"
 dependencies = [
  "atty",
  "humantime",
- "log 0.4.17",
+ "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
-name = "error-chain"
-version = "0.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9435d864e017c3c6afeac1654189b06cdb491cf2ff73dbf0d73b0f292f42ff8"
-dependencies = [
- "backtrace",
-]
-
-[[package]]
 name = "fastrand"
-version = "1.7.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3fcf0cee53519c866c09b5de1f6c56ff9d647101f81c1964fa632e148896cdf"
+checksum = "779d043b6a0b90cc4c0ed7ee380a6504394cee7efd7db050e3774eee387324b2"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "flate2"
-version = "0.2.20"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6234dd4468ae5d1e2dbb06fe2b058696fdc50a339c68a393aefbf00bc81e423"
-dependencies = [
- "libc",
- "miniz-sys",
-]
-
-[[package]]
-name = "flate2"
-version = "1.0.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f82b0f4c27ad9f8bfd1f3208d882da2b09c301bc1c828fd3a00d0216d2fbbff6"
+checksum = "1e6988e897c1c9c485f43b47a529cef42fde0547f9d8d41a7062518f1d8fc53f"
 dependencies = [
+ "cfg-if",
  "crc32fast",
+ "libc",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -538,92 +304,65 @@
 dependencies = [
  "matches",
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.21"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3083ce4b914124575708913bca19bfe887522d6e2e6d0952943f5eac4a74010"
+checksum = "ba3dda0b6588335f360afc675d0564c17a77a2bda81ca178a4b6081bd86c7f0b"
 dependencies = [
  "futures-core",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.21"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c09fd04b7e4073ac7156a9539b57a484a8ea920f79c7c675d05d289ab6110d3"
+checksum = "d0c8ff0461b82559810cdccfde3215c3f373807f5e5232b71479bff7bb2583d7"
 
 [[package]]
 name = "futures-io"
-version = "0.3.21"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc4045962a5a5e935ee2fdedaa4e08284547402885ab326734432bed5d12966b"
+checksum = "b1f9d34af5a1aac6fb380f735fe510746c38067c5bf16c7fd250280503c971b2"
 
 [[package]]
 name = "futures-sink"
-version = "0.3.21"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21163e139fa306126e6eedaf49ecdb4588f939600f0b1e770f4205ee4b7fa868"
+checksum = "e3055baccb68d74ff6480350f8d6eb8fcfa3aa11bdc1a1ae3afdd0514617d508"
 
 [[package]]
 name = "futures-task"
-version = "0.3.21"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57c66a976bf5909d801bbef33416c41372779507e7a6b3a5e25e4749c58f776a"
+checksum = "6ee7c6485c30167ce4dfb83ac568a849fe53274c831081476ee13e0dce1aad72"
 
 [[package]]
 name = "futures-util"
-version = "0.3.21"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8b7abd5d659d9b90c8cba917f6ec750a74e2dc23902ef9cd4cc8c8b22e6036a"
+checksum = "d9b5cf40b47a271f77a8b1bec03ca09044d99d2372c0de244e66430761127164"
 dependencies = [
  "futures-core",
  "futures-io",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
-name = "generic-array"
-version = "0.14.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd48d33ec7f05fbfa152300fdad764757cbded343c1aa1cff2fbaf4134851803"
-dependencies = [
- "typenum",
- "version_check",
-]
-
-[[package]]
-name = "getrandom"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9be70c98951c83b8d2f8f60d7065fa6d5146873094452a1008da8c2f1e4205ad"
-dependencies = [
- "cfg-if",
- "libc",
- "wasi 0.10.2+wasi-snapshot-preview1",
-]
-
-[[package]]
-name = "gimli"
-version = "0.26.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78cc372d058dcf6d5ecd98510e7fbc9e5aec4d21de70f65fea8fecebcd881bd4"
-
-[[package]]
 name = "h2"
-version = "0.3.13"
+version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37a82c6d637fc9515a4694bbf1cb2457b79d81ce52b3108bdeea58b07dd34a57"
+checksum = "0c9de88456263e249e241fcd211d3954e2c9b0ef7ccfc235a444eb367cae3689"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -631,20 +370,14 @@
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
-name = "half"
-version = "1.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
-
-[[package]]
 name = "hashbrown"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ab5ef0d4909ef3724cc8cce6ccc8572c5c817592e9285f5464f8e86f8bd3726e"
 
 [[package]]
 name = "heck"
@@ -665,39 +398,39 @@
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "http"
-version = "0.2.7"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff8670570af52249509a86f5e3e18a08c60b177071826898fde8997cf5f6bfbb"
+checksum = "31f4c6746584866f0feabcc69893c5b51beef3831656a968ed7ae254cdc4fd03"
 dependencies = [
  "bytes",
  "fnv",
- "itoa 1.0.2",
+ "itoa 1.0.1",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "1ff4f84919677303da5f147645dbea6b1881f368d03ac84e1dc09031ebd7b2c6"
 dependencies = [
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
-version = "1.7.1"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "496ce29bb5a52785b44e0f7ca2847ae0bb839c9bd28f69acac9b99d461c0c04c"
+checksum = "acd94fdbe1d4ff688b67b04eee2e17bd50995534a61539e45adfefb45e5e5503"
 
 [[package]]
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
@@ -705,28 +438,28 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.19"
+version = "0.14.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42dc3c131584288d375f2d07f822b0cb012d8c6fb899a5b9fdb3cb7eb9b6004f"
+checksum = "b7ec3e62bdc98a2f0393a5048e4c30ef659440ea6e0e572965103e72bd836f55"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
- "itoa 1.0.2",
+ "itoa 0.4.8",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
@@ -753,36 +486,42 @@
  "matches",
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.8.2"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6012d540c5baa3589337a98ce73408de9b5a25ec9fc2c6fd6be8f0d39e0ca5a"
+checksum = "282a6247722caba404c065016bbfa522806e51714c34f5dfc3e4a3a46fcb4223"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
+name = "indoc"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+
+[[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.5.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "879d54834c8c76457ef4293a689b2a8c59b076067ad77b15efafbb05f92a592b"
+checksum = "68f2d64f2edebec4ce84ad108148e67e1064789bee435edc5b60ad398714a3a9"
 
 [[package]]
 name = "ipnetwork"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4088d739b183546b239688ddbc79891831df421773df95e236daf7867866d355"
 
@@ -799,71 +538,53 @@
 name = "itoa"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
 
 [[package]]
 name = "itoa"
-version = "1.0.2"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "112c678d4050afce233f4f2852bb2eb519230b3cf12f33585275537d7e41578d"
+checksum = "1aab8fc367588b89dcee83ab0fd66b72b50b72fa1904d7095045ace2b0c81c35"
 
 [[package]]
 name = "js-sys"
-version = "0.3.57"
+version = "0.3.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "671a26f820db17c2a2750743f1dd03bafd15b98c9f30c7c2628c024c05d73397"
+checksum = "7cc9ffccd38c451a86bf13657df244e9c3f37493cce8e5e21e940963777acc84"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "kafka"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f37f068eb07305e1141453ea2dccfb4f278153a4261bb9a519f10d1eb13d25a8"
-dependencies = [
- "byteorder 0.5.3",
- "crc",
- "error-chain",
- "flate2 0.2.20",
- "fnv",
- "log 0.3.9",
- "openssl",
- "ref_slice",
- "snap",
- "twox-hash",
-]
-
-[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.126"
+version = "0.2.112"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "349d5a591cd28b49e1d1037471617a32ddcda5731b99419008085f72d5a53836"
+checksum = "1b03d17f364a3a042d5e5d46b053bbbf82c92c9430c592dd4c064dc6ee997125"
 
 [[package]]
-name = "log"
-version = "0.3.9"
+name = "lock_api"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e19e8d5c34a3e0e2223db8e060f9e8264aeeb5c5fc64a4ee9965c062211c024b"
+checksum = "712a4d093c9976e24e7dbca41db895dabcbac38eb5f4045393d17a95bdfb1109"
 dependencies = [
- "log 0.4.17",
+ "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
+checksum = "51b9bbe6c47d51fc3e1a9b945965946b4c44142ab8792c50835a980d362c2710"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "lz4"
 version = "1.23.3"
@@ -888,17 +609,17 @@
 name = "matches"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e378b66a060d48947b590737b30a1be76706c8dd7b8ba0f2fe3989c68a853f"
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "308cc39be01b73d0d18f82a0e7b2a3df85245f84af96fdddc5d202d27e47b86a"
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
@@ -908,86 +629,96 @@
 [[package]]
 name = "mime"
 version = "0.3.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a60c7ce501c71e03a9c9c0d35b861413ae925bd979cc7a4e30d060069aaac8d"
 
 [[package]]
-name = "miniz-sys"
-version = "0.1.12"
+name = "miniz_oxide"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e9e3ae51cea1576ceba0dde3d484d30e6e5b86dee0b2d412fe3a16a15c98202"
+checksum = "a92518e98c078586bc6c934028adcca4c92a53d6a958196de835170a01d84e4b"
 dependencies = [
- "cc",
- "libc",
+ "adler",
+ "autocfg",
 ]
 
 [[package]]
-name = "miniz_oxide"
-version = "0.5.1"
+name = "mio"
+version = "0.7.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2b29bd4bc3f33391105ebee3589c19197c4271e3e5a9ec9bfe8127eeff8f082"
+checksum = "8067b404fe97c70829f082dec8bcf4f71225d7eaea1d8645349cb76fa06205cc"
 dependencies = [
- "adler",
+ "libc",
+ "log",
+ "miow",
+ "ntapi",
+ "winapi",
 ]
 
 [[package]]
-name = "mio"
-version = "0.8.3"
+name = "miow"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713d550d9b44d89174e066b7a6217ae06234c10cb47819a88290d2b353c31799"
+checksum = "b9f1c5b025cda876f66ef43a113f91ebc9f4ccef34843000e0adf6ebbab84e21"
 dependencies = [
- "libc",
- "log 0.4.17",
- "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys",
+ "winapi",
 ]
 
 [[package]]
 name = "native-tls"
-version = "0.2.10"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd7e2f3618557f980e0b17e8856252eee3c97fa12c54dff0ca290fb6266ca4a9"
+checksum = "48ba9f7719b5a0f42f338907614285fb5fd70e53858141f69898a1fb7203b24d"
 dependencies = [
  "lazy_static",
  "libc",
- "log 0.4.17",
+ "log",
  "openssl",
  "openssl-probe",
  "openssl-sys",
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
+name = "ntapi"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f6bb902e437b6d86e03cce10a7e2af662292c5dfef23b65899ea3ac9354ad44"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "d2cc698a63b549a70bc047073d2949cce27cd1c7b0a4a862d08a8031bc2801db"
 dependencies = [
  "autocfg",
- "num-traits 0.2.15",
+ "num-traits 0.2.14",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.1.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92e5113e9fd4cc14ded8e499429f396a20f98c772a47cc8622a736e1ec843c31"
 dependencies = [
- "num-traits 0.2.15",
+ "num-traits 0.2.14",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "9a64b1ec5cda2586e284722486d802acf1f7dbdc623e2bfc57e65ca1cd099290"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.13.1"
@@ -995,161 +726,129 @@
 checksum = "19e64526ebdee182341572e50e9ad03965aa510cd94427a4549448f285e957a1"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
-name = "object"
-version = "0.28.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e42c982f2d955fac81dd7e1d0e1426a7d702acd9c98d19ab01083a6a0328c424"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "once_cell"
-version = "1.12.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7709cef83f0c1f58f666e746a08b21e0085f7440fa6a29cc194d68aac97a4225"
+checksum = "da32515d9f6e6e489d7bc9d84c71b060db7247dc035bbe44eac88cf87486d8d5"
 
 [[package]]
 name = "oneio"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "afa7566ace2c81105d7255e403b0cef556b6374d67e53fc4678fc2b4f8936c52"
 dependencies = [
  "bzip2",
- "clap 3.2.16",
- "flate2 1.0.24",
+ "clap",
+ "flate2",
  "lz4",
  "reqwest",
 ]
 
 [[package]]
-name = "oorandom"
-version = "11.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
-
-[[package]]
-name = "opaque-debug"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
-
-[[package]]
 name = "openssl"
-version = "0.10.40"
+version = "0.10.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb81a6430ac911acb25fe5ac8f1d2af1b4ea8a4fdfda0f1ee4292af2e2d8eb0e"
+checksum = "0c7ae222234c30df141154f159066c5093ff73b63204dcda7121eb082fc56a95"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
- "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
-name = "openssl-macros"
-version = "0.1.0"
+name = "openssl-probe"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
+checksum = "28988d872ab76095a6e6ac88d99b54fd267702734fd7ffe610ca27f533ddb95a"
 
 [[package]]
-name = "openssl-probe"
-version = "0.1.5"
+name = "openssl-src"
+version = "111.24.0+1.1.1s"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
+checksum = "3498f259dab01178c6228c6b00dcef0ed2a2d5e20d648c017861227773ea4abd"
+dependencies = [
+ "cc",
+]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.73"
+version = "0.9.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d5fd19fb3e0a8191c1e34935718976a3e70c112ab9a24af6d7cadccd9d90bc0"
+checksum = "7e46109c383602735fa0a2e48dd2b7c892b048e1bf69e5c3b1d804b7d9c203cb"
 dependencies = [
  "autocfg",
  "cc",
  "libc",
+ "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "os_str_bytes"
 version = "6.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "648001efe5d5c0102d8cea768e348da85d90af8ba91f0bea908f157951493cd4"
 
 [[package]]
+name = "parking_lot"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+dependencies = [
+ "instant",
+ "lock_api",
+ "parking_lot_core",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d76e8e1493bcac0d2766c42737f34458f1c8c50c0d23bcb24ea953affb273216"
+dependencies = [
+ "cfg-if",
+ "instant",
+ "libc",
+ "redox_syscall",
+ "smallvec",
+ "winapi",
+]
+
+[[package]]
 name = "percent-encoding"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4fd5641d01c8f18a23da7b6fe29298ff4b55afcccdf78973b24cf3175fee32e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "e280fbe77cc62c91527259e9442153f4688736748d24660126286329742b4c6c"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.25"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1df8c4ec4b0627e53bdf214615ad287367e482558cf84b109250b37464dc03ae"
-
-[[package]]
-name = "plotters"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32a3fd9ec30b9749ce28cd91f255d569591cdf937fe280c312143e3c4bad6f2a"
-dependencies = [
- "num-traits 0.2.15",
- "plotters-backend",
- "plotters-svg",
- "wasm-bindgen",
- "web-sys",
-]
-
-[[package]]
-name = "plotters-backend"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d88417318da0eaf0fdcdb51a0ee6c3bed624333bff8f946733049380be67ac1c"
-
-[[package]]
-name = "plotters-svg"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "521fa9638fa597e1dc53e9412a4f9cefb01187ee1f7413076f9e6749e2885ba9"
-dependencies = [
- "plotters-backend",
-]
-
-[[package]]
-name = "ppv-lite86"
-version = "0.2.16"
+version = "0.3.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb9f9e6e233e5c4a35559a617bf40a4ec447db2e84c20b55a6f83167b7e57872"
+checksum = "58893f751c9b0412871a09abd62ecd2a00298c6c83befa223ef98c52aef40cbe"
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
@@ -1169,151 +868,156 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.39"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c54b25569025b7fc9651de43004ae593a75ad88543b17178aa5e1b9c4f15f56f"
+checksum = "c7342d5883fbccae1cc37a2353b09c87c9b0f3afd73f5fb9bba687a1f733b029"
 dependencies = [
- "unicode-ident",
+ "unicode-xid",
 ]
 
 [[package]]
-name = "quote"
-version = "1.0.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1feb54ed693b93a84e14094943b84b7c4eae204c512b7ccb95ab0c66d278ad1"
+name = "pybgpkit-parser"
+version = "0.3.0"
 dependencies = [
- "proc-macro2",
+ "bgpkit-parser",
+ "dict_derive",
+ "openssl",
+ "pyo3",
+ "pyo3-build-config",
 ]
 
 [[package]]
-name = "rand"
-version = "0.8.5"
+name = "pyo3"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
 dependencies = [
+ "cfg-if",
+ "indoc",
  "libc",
- "rand_chacha",
- "rand_core",
+ "memoffset",
+ "parking_lot",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "pyo3-macros",
+ "unindent",
 ]
 
 [[package]]
-name = "rand_chacha"
-version = "0.3.1"
+name = "pyo3-build-config"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
 dependencies = [
- "ppv-lite86",
- "rand_core",
+ "once_cell",
+ "target-lexicon",
 ]
 
 [[package]]
-name = "rand_core"
-version = "0.6.3"
+name = "pyo3-ffi"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d34f1408f55294453790c48b2f1ebbb1c5b4b7563eb1f418bcfcfdbb06ebb4e7"
+checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
 dependencies = [
- "getrandom",
+ "libc",
+ "pyo3-build-config",
 ]
 
 [[package]]
-name = "rayon"
-version = "1.5.3"
+name = "pyo3-macros"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd99e5772ead8baa5215278c9b15bf92087709e9c1b2d1f97cdb5a183c933a7d"
+checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
- "autocfg",
- "crossbeam-deque",
- "either",
- "rayon-core",
+ "proc-macro2",
+ "pyo3-macros-backend",
+ "quote",
+ "syn",
 ]
 
 [[package]]
-name = "rayon-core"
-version = "1.9.3"
+name = "pyo3-macros-backend"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "258bcdb5ac6dad48491bb2992db6b7cf74878b0384908af124823d118c99683f"
+checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
- "crossbeam-channel",
- "crossbeam-deque",
- "crossbeam-utils",
- "num_cpus",
+ "proc-macro2",
+ "quote",
+ "syn",
 ]
 
 [[package]]
-name = "redox_syscall"
-version = "0.2.13"
+name = "quote"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62f25bc4c7e55e0b0b7a1d43fb893f4fa1361d0abe38b9ce4f323c2adfe6ef42"
+checksum = "47aa80447ce4daf1717500037052af176af5d38cc3e571d9ec1c7353fc10c87d"
 dependencies = [
- "bitflags",
+ "proc-macro2",
 ]
 
 [[package]]
-name = "ref_slice"
-version = "1.2.1"
+name = "redox_syscall"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4ed1d73fb92eba9b841ba2aef69533a060ccc0d3ec71c90aeda5996d4afb7a9"
+checksum = "8383f39639269cde97d255a32bdb68c047337295414940c68bdd30c2e13203ff"
+dependencies = [
+ "bitflags",
+]
 
 [[package]]
 name = "regex"
-version = "1.5.6"
+version = "1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d83f127d94bdbcda4c8cc2e50f6f84f4b611f69c902699ca385a39c3a75f9ff1"
+checksum = "d07a8629359eb56f1e2fb1652bb04212c072a87ba68546a04065d525673ac461"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
-name = "regex-automata"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
-
-[[package]]
 name = "regex-syntax"
-version = "0.6.26"
+version = "0.6.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49b3de9ec5dc0a3417da371aab17d729997c15010e7fd24ff707773a33bddb64"
+checksum = "f497285884f3fcff424ffc933e56d7cbca511def0c9831a7f9b5f6153e3cc89b"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.10"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46a1f7aa4f35e5e8b4160449f51afc758f0ce6454315a9fa7d0d113e958c41eb"
+checksum = "87f242f1488a539a79bac6dbe7c8609ae43b7914b7736210f239a37cccb32525"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "hyper",
  "hyper-tls",
  "ipnet",
  "js-sys",
  "lazy_static",
- "log 0.4.17",
+ "log",
  "mime",
  "native-tls",
  "percent-encoding",
  "pin-project-lite",
  "serde",
  "serde_json",
  "serde_urlencoded",
@@ -1323,204 +1027,147 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
-name = "rustc-demangle"
-version = "0.1.21"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
-
-[[package]]
-name = "rustc_version"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
-dependencies = [
- "semver",
-]
-
-[[package]]
 name = "ryu"
-version = "1.0.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3f6f92acf49d1b98f7a81226834412ada05458b7364277387724a237f062695"
-
-[[package]]
-name = "same-file"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
-dependencies = [
- "winapi-util",
-]
+checksum = "73b4b750c782965c211b42f022f59af1fbceabdd026623714f104152f1ec149f"
 
 [[package]]
 name = "schannel"
-version = "0.1.20"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d6731146462ea25d9244b2ed5fd1d716d25c52e4d54aa4fb0f3c4e9854dbe2"
+checksum = "8f05ba609c234e60bee0d547fe94a4c7e9da733d1c962cf6e59efa4cd9c8bc75"
 dependencies = [
  "lazy_static",
- "windows-sys",
+ "winapi",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "security-framework"
-version = "2.6.1"
+version = "2.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dc14f172faf8a0194a3aded622712b0de276821addc574fa54fc0a1167e10dc"
+checksum = "525bc1abfda2e1998d152c45cf13e696f76d0a4972310b22fac1658b05df7c87"
 dependencies = [
  "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.6.1"
+version = "2.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0160a13a177a45bfb43ce71c01580998474f556ad854dcbca936dd2841a5c556"
+checksum = "a9dd14d83160b528b7bfd66439110573efcfbe281b17fc2ca9f39f550d619c7e"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
-name = "semver"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cb243bdfdb5936c8dc3c45762a19d12ab4550cdc753bc247637d4ec35a040fd"
-
-[[package]]
 name = "serde"
-version = "1.0.137"
+version = "1.0.133"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61ea8d54c77f8315140a05f4c7237403bf38b72704d031543aa1d16abbf517d1"
+checksum = "97565067517b60e2d1ea8b268e59ce036de907ac523ad83a0475da04e818989a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
-name = "serde_cbor"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bef2ebfde456fb76bbcf9f59315333decc4fda0b2b44b420243c11e0f5ec1f5"
-dependencies = [
- "half",
- "serde",
-]
-
-[[package]]
 name = "serde_derive"
-version = "1.0.137"
+version = "1.0.133"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f26faba0c3959972377d3b2d306ee9f71faee9714294e41bb777f83f88578be"
+checksum = "ed201699328568d8d08208fdd080e3ff594e6c422e438b6705905da01005d537"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.81"
+version = "1.0.74"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7ce2b32a1aed03c558dc61a5cd328f15aff2dbc17daad8fb8af04d2100e15c"
+checksum = "ee2bb9cd061c5865d345bb02ca49fcef1391741b672b54a0bf7b679badec3142"
 dependencies = [
- "itoa 1.0.2",
+ "itoa 1.0.1",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
-version = "0.7.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+checksum = "edfa57a7f8d9c1d260a549e7224100f6c43d43f9103e06dd8b4095a9b2b43ce9"
 dependencies = [
  "form_urlencoded",
- "itoa 1.0.2",
+ "itoa 0.4.8",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "sha-1"
-version = "0.9.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99cd6713db3cf16b6c84e06321e049a9b9f699826e16096d23bbcc44d15d51a6"
-dependencies = [
- "block-buffer",
- "cfg-if",
- "cpufeatures",
- "digest",
- "opaque-debug",
-]
-
-[[package]]
 name = "slab"
-version = "0.4.6"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb703cfe953bccee95685111adeedb76fabe4e97549a58d16f03ea7b9367bb32"
+checksum = "9def91fd1e018fe007022791f865d0ccc9b3a0d5001e01aabb8b40e46000afb5"
 
 [[package]]
-name = "snap"
-version = "0.2.5"
+name = "smallvec"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95d697d63d44ad8b78b8d235bf85b34022a78af292c8918527c5f0cffdde7f43"
-dependencies = [
- "byteorder 1.4.3",
- "lazy_static",
-]
+checksum = "1ecab6c735a6bb4139c0caafd0cc3635748bbb3acf4550e8138122099251f309"
 
 [[package]]
 name = "socket2"
-version = "0.4.4"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66d72b759436ae32898a2af0a14218dbf55efde3feeb170eb623637db85ee1e0"
+checksum = "5dc90fe6c7be1a323296982db1836d1ea9e47b6839496dde9a541bc496df3516"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
-name = "static_assertions"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
-
-[[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "1.0.95"
+version = "1.0.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbaf6116ab8924f39d52792136fb74fd60a80194cf1b1c6ffa6453eef1c3f942"
+checksum = "a684ac3dcd8913827e18cd09a68384ee66c1de24157e3c556c9ab16d85695fb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "unicode-ident",
+ "unicode-xid",
 ]
 
 [[package]]
+name = "target-lexicon"
+version = "0.12.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+
+[[package]]
 name = "tempfile"
 version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cdb1ef4eaeeaddc8fbd371e5017057064af0911902ef36b39801f67cc6d79e4"
 dependencies = [
  "cfg-if",
  "fastrand",
@@ -1528,105 +1175,65 @@
  "redox_syscall",
  "remove_dir_all",
  "winapi",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "2dfed899f0eb03f32ee8c6a0aabdb8a7949659e3466561fc0adf54e26d88c5f4"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "textwrap"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
-dependencies = [
- "unicode-width",
-]
-
-[[package]]
-name = "textwrap"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1141d4d61095b28419e22cb0bbf02755f5e54e0526f97f1e3d1d160e60885fb"
 
 [[package]]
-name = "thiserror"
-version = "1.0.31"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd829fe32373d27f76265620b5309d0340cb8550f523c1dda251d6298069069a"
-dependencies = [
- "thiserror-impl",
-]
-
-[[package]]
-name = "thiserror-impl"
-version = "1.0.31"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0396bc89e626244658bef819e22d0cc459e795a5ebe878e6ec336d1674a8d79a"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "time"
-version = "0.1.43"
+version = "0.1.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca8a50ef2360fbd1eeb0ecd46795a87a19024eb4b53c5dc916ca1fd95fe62438"
+checksum = "6db9e6914ab8b1ae1c260a4ae7a49b6c5611b40328a735b21862567685e73255"
 dependencies = [
  "libc",
+ "wasi",
  "winapi",
 ]
 
 [[package]]
-name = "tinytemplate"
-version = "1.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
-dependencies = [
- "serde",
- "serde_json",
-]
-
-[[package]]
 name = "tinyvec"
-version = "1.6.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+checksum = "2c1c1d5a42b6245520c249549ec267180beaffcc0615401ac8e31853d4b6d8d2"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
 
 [[package]]
 name = "tokio"
-version = "1.18.2"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4903bf0427cf68dddd5aa6a93220756f8be0c34fcfa9f5e6191e103e15a31395"
+checksum = "fbbf1c778ec206785635ce8ad57fe52b3009ae9e0c9f574a728f3049d3e55838"
 dependencies = [
  "bytes",
  "libc",
  "memchr",
  "mio",
  "num_cpus",
- "once_cell",
  "pin-project-lite",
- "socket2",
  "winapi",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1634,267 +1241,196 @@
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.2"
+version = "0.6.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f988a1a1adc2fb21f9c12aa96441da33a1728193ae0b95d2be22dbd17fcb4e5c"
+checksum = "9e99e1983e5d376cd8eb4b66604d2e99e79f5bd988c3055891dcd8c9e2604cc0"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
+ "log",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "360dfd1d6d30e05fda32ace2c8c70e9c0a9da713275777f5a4dbb8a1893930c6"
 
 [[package]]
 name = "tracing"
-version = "0.1.34"
+version = "0.1.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d0ecdcb44a79f0fe9844f0c4f33a342cbcbb5117de8001e6ba0dc2351327d09"
+checksum = "375a639232caf30edfc78e8d89b2d4c375515393e7af7e16f01cd96917fb2105"
 dependencies = [
  "cfg-if",
  "pin-project-lite",
- "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
-name = "tracing-attributes"
-version = "0.1.21"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc6b8ad3567499f98a1db7a752b07a7c8c7c7c34c332ec00effb2b0027974b7c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "tracing-core"
-version = "0.1.26"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f54c8ca710e81886d498c2fd3331b56c93aa248d49de2222ad2742247c60072f"
+checksum = "1f4ed65637b8390770814083d20756f87bfa2c21bf2f110babdc5438351746e4"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "try-lock"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59547bce71d9c38b83d9c0e92b6066c4253371f15005def0c30d9657f50c7642"
 
 [[package]]
-name = "tungstenite"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ad3713a14ae247f22a728a0456a545df14acf3867f905adff84be99e23b3ad1"
-dependencies = [
- "base64",
- "byteorder 1.4.3",
- "bytes",
- "http",
- "httparse",
- "log 0.4.17",
- "rand",
- "sha-1",
- "thiserror",
- "url",
- "utf-8",
-]
-
-[[package]]
-name = "twox-hash"
-version = "1.6.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
-dependencies = [
- "cfg-if",
- "rand",
- "static_assertions",
-]
-
-[[package]]
-name = "typenum"
-version = "1.15.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
-
-[[package]]
 name = "unicode-bidi"
-version = "0.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099b7128301d285f79ddd55b9a83d5e6b9e97c92e0ea0daebee7263e932de992"
-
-[[package]]
-name = "unicode-ident"
-version = "1.0.0"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d22af068fba1eb5edcb4aea19d382b2a3deb4c8f9d475c589b6ada9e0fd493ee"
+checksum = "1a01404663e3db436ed2746d9fefef640d868edae3cceb81c3b8d5732fda678f"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d54590932941a9e9266f0832deed84ebe1bf2e4c9e4a3554d393d18f5e854bf9"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
-name = "unicode-width"
-version = "0.1.9"
+name = "unicode-xid"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ed742d4ea2bd1176e236172c8429aaf54486e7ac098db29ffe6529e0ce50973"
+checksum = "8ccb82d61f80a663efe1f787a51b16b5a51e3314d6ac365b08639f52387b33f3"
+
+[[package]]
+name = "unindent"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f14ee04d9415b52b3aeab06258a3f07093182b88ba0f9b8d203f211a7a7d41c7"
 
 [[package]]
 name = "url"
 version = "2.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507c383b2d33b5fc35d1861e77e6b383d158b2da5e14fe51b83dfedf6fd578c"
 dependencies = [
  "form_urlencoded",
  "idna",
  "matches",
  "percent-encoding",
 ]
 
 [[package]]
-name = "utf-8"
-version = "0.7.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
-
-[[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "walkdir"
-version = "2.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
-dependencies = [
- "same-file",
- "winapi",
- "winapi-util",
-]
-
-[[package]]
 name = "want"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
 dependencies = [
- "log 0.4.17",
+ "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
-version = "0.10.2+wasi-snapshot-preview1"
+version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd6fbd9a79829dd1ad0cc20627bf1ed606756a7f77edff7b66b7064f9cb327c6"
-
-[[package]]
-name = "wasi"
-version = "0.11.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.80"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27370197c907c55e3f1a9fbe26f44e937fe6451368324e009cba39e139dc08ad"
+checksum = "632f73e236b219150ea279196e54e610f5dbafa5d61786303d4da54f84e47fce"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.80"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53e04185bfa3a779273da532f5025e33398409573f348985af9a1cbf3774d3f4"
+checksum = "a317bf8f9fba2476b4b2c85ef4c4af8ff39c3c7f0cdfeed4f82c34a880aa837b"
 dependencies = [
  "bumpalo",
  "lazy_static",
- "log 0.4.17",
+ "log",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.30"
+version = "0.4.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f741de44b75e14c35df886aff5f1eb73aa114fa5d4d00dcd37b5e01259bf3b2"
+checksum = "8e8d7523cb1f2a4c96c1317ca690031b714a51cc14e05f712446691f413f5d39"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.80"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17cae7ff784d7e83a2fe7611cfe766ecf034111b49deb850a3dc7699c08251f5"
+checksum = "d56146e7c495528bf6587663bea13a8eb588d39b36b679d83972e1a2dbbdacf9"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.80"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99ec0dc7a4756fffc231aab1b9f2f578d23cd391390ab27f952ae0c9b3ece20b"
+checksum = "7803e0eea25835f8abdc585cd3021b3deb11543c6fe226dcd30b228857c5c5ab"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.80"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d554b7f530dee5964d9a9468d95c1f8b8acae4f282807e7d27d4b03099a46744"
+checksum = "0237232789cf037d5480773fe568aac745bfe2afbc11a863e97901780a6b47cc"
 
 [[package]]
 name = "web-sys"
-version = "0.3.57"
+version = "0.3.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b17e741662c70c8bd24ac5c5b18de314a2c26c32bf8346ee1e6f53de919c283"
+checksum = "38eb105f1c59d9eaa6b5cdc92b859d85b926e82cb2e0945cd0c9259faa6fe9fb"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -1924,57 +1460,14 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.36.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
-dependencies = [
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_msvc",
-]
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.36.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.36.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.36.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.36.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.36.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
-
-[[package]]
 name = "winreg"
-version = "0.10.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+checksum = "0120db82e8a1e0b9fb3345a539c478767c0048d842860994d96113d5b667bd69"
 dependencies = [
  "winapi",
 ]
```

### Comparing `pybgpkit_parser-0.4.2/Dockerfile` & `pybgpkit_parser-0.4.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.2/LICENSE` & `pybgpkit_parser-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.2/README.md` & `pybgpkit_parser-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.2/src/lib.rs` & `pybgpkit_parser-0.4.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.2/PKG-INFO` & `pybgpkit_parser-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit-parser
-Version: 0.4.2
+Version: 0.4.3
 Summary: BGPKIT Parser Python Binding
 Keywords: bgp,mrt,parser
 Author: Mingwei Zhang <mingwei@bgpkit.com>
 Author-email: Mingwei Zhang <mingwei@bgpkit.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/bgpkit/bgpkit-parser/tree/main/bgpkit-parser-py
```

