# Comparing `tmp/octodns-0.9.9.tar.gz` & `tmp/octodns-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/octodns-0.9.9.tar", last modified: Mon Nov  4 23:03:19 2019, max compression
+gzip compressed data, was "octodns-1.0.0rc0.tar", last modified: Wed May 17 16:58:26 2023, max compression
```

## Comparing `octodns-0.9.9.tar` & `octodns-1.0.0rc0.tar`

### file list

```diff
@@ -1,144 +1,231 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:19.000000 octodns-0.9.9/
--rw-r--r--   0 ross       (501) staff       (20)    15862 2019-11-04 23:03:19.000000 octodns-0.9.9/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     1056 2017-10-19 21:26:51.000000 octodns-0.9.9/LICENSE
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:19.000000 octodns-0.9.9/octodns/record/
--rw-r--r--   0 ross       (501) staff       (20)     2200 2019-03-28 20:58:28.000000 octodns-0.9.9/octodns/record/geo.py
--rw-r--r--   0 ross       (501) staff       (20)    36987 2019-11-04 22:54:07.000000 octodns-0.9.9/octodns/record/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    14562 2018-12-14 19:33:23.000000 octodns-0.9.9/octodns/record/geo_data.py
--rw-r--r--   0 ross       (501) staff       (20)    35133 2018-12-14 17:49:10.000000 octodns-0.9.9/octodns/record.pyc
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:19.000000 octodns-0.9.9/octodns/source/
--rw-r--r--   0 ross       (501) staff       (20)       96 2017-10-19 21:26:51.000000 octodns-0.9.9/octodns/source/__init__.py
--rwxr-xr-x   0 ross       (501) staff       (20)     8420 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/source/tinydns.py
--rw-r--r--   0 ross       (501) staff       (20)     6950 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/source/axfr.py
--rw-r--r--   0 ross       (501) staff       (20)     1708 2019-03-28 20:59:07.000000 octodns-0.9.9/octodns/source/base.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:19.000000 octodns-0.9.9/octodns/provider/
--rw-r--r--   0 ross       (501) staff       (20)    14125 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/constellix.py
--rw-r--r--   0 ross       (501) staff       (20)    10276 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/plan.py
--rw-r--r--   0 ross       (501) staff       (20)    11395 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/transip.py
--rw-r--r--   0 ross       (501) staff       (20)    13320 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/ns1.py
--rw-r--r--   0 ross       (501) staff       (20)    54766 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/dyn.py
--rw-r--r--   0 ross       (501) staff       (20)     4775 2019-03-28 20:59:01.000000 octodns-0.9.9/octodns/provider/etc_hosts.py
--rw-r--r--   0 ross       (501) staff       (20)    10098 2019-10-05 14:20:16.000000 octodns-0.9.9/octodns/provider/selectel.py
--rw-r--r--   0 ross       (501) staff       (20)    13737 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/ovh.py
--rw-r--r--   0 ross       (501) staff       (20)    14210 2019-03-28 20:59:03.000000 octodns-0.9.9/octodns/provider/powerdns.py
--rw-r--r--   0 ross       (501) staff       (20)       96 2017-10-19 21:26:51.000000 octodns-0.9.9/octodns/provider/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    21228 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/cloudflare.py
--rw-r--r--   0 ross       (501) staff       (20)    14258 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/mythicbeasts.py
--rw-r--r--   0 ross       (501) staff       (20)    11113 2019-07-19 15:10:35.000000 octodns-0.9.9/octodns/provider/digitalocean.py
--rw-r--r--   0 ross       (501) staff       (20)    13449 2019-03-28 20:58:57.000000 octodns-0.9.9/octodns/provider/dnsimple.py
--rw-r--r--   0 ross       (501) staff       (20)     8006 2019-05-15 03:09:51.000000 octodns-0.9.9/octodns/provider/yaml.py
--rw-r--r--   0 ross       (501) staff       (20)    56498 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/route53.py
--rw-r--r--   0 ross       (501) staff       (20)    12818 2019-03-28 20:58:58.000000 octodns-0.9.9/octodns/provider/dnsmadeeasy.py
--rw-r--r--   0 ross       (501) staff       (20)    13427 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/rackspace.py
--rw-r--r--   0 ross       (501) staff       (20)    12263 2019-03-28 20:59:01.000000 octodns-0.9.9/octodns/provider/googlecloud.py
--rw-r--r--   0 ross       (501) staff       (20)     3520 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/base.py
--rw-r--r--   0 ross       (501) staff       (20)    15286 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/fastdns.py
--rw-r--r--   0 ross       (501) staff       (20)    19339 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/provider/azuredns.py
--rw-r--r--   0 ross       (501) staff       (20)      187 2019-11-04 23:03:08.000000 octodns-0.9.9/octodns/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns/cmds/
--rwxr-xr-x   0 ross       (501) staff       (20)     1542 2018-03-15 13:21:54.000000 octodns-0.9.9/octodns/cmds/sync.py
--rw-r--r--   0 ross       (501) staff       (20)       96 2017-10-19 21:26:51.000000 octodns-0.9.9/octodns/cmds/__init__.py
--rwxr-xr-x   0 ross       (501) staff       (20)     1365 2019-04-27 21:13:19.000000 octodns-0.9.9/octodns/cmds/dump.py
--rwxr-xr-x   0 ross       (501) staff       (20)      600 2017-11-13 14:01:56.000000 octodns-0.9.9/octodns/cmds/validate.py
--rw-r--r--   0 ross       (501) staff       (20)     2760 2018-11-05 17:47:06.000000 octodns-0.9.9/octodns/cmds/args.py
--rwxr-xr-x   0 ross       (501) staff       (20)     1002 2017-10-19 21:26:51.000000 octodns-0.9.9/octodns/cmds/compare.py
--rwxr-xr-x   0 ross       (501) staff       (20)     3620 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/cmds/report.py
--rw-r--r--   0 ross       (501) staff       (20)     1783 2019-10-18 17:14:18.000000 octodns-0.9.9/octodns/equality.pyc
--rw-r--r--   0 ross       (501) staff       (20)      808 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/equality.py
--rw-r--r--   0 ross       (501) staff       (20)     2869 2019-10-18 17:14:18.000000 octodns-0.9.9/octodns/yaml.pyc
--rw-r--r--   0 ross       (501) staff       (20)     1979 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/yaml.py
--rw-r--r--   0 ross       (501) staff       (20)    12288 2019-11-04 22:54:30.000000 octodns-0.9.9/octodns/.__init__.py.swp
--rw-r--r--   0 ross       (501) staff       (20)    13257 2019-10-18 17:14:18.000000 octodns-0.9.9/octodns/manager.pyc
--rw-r--r--   0 ross       (501) staff       (20)     7492 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/zone.py
--rw-r--r--   0 ross       (501) staff       (20)      415 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns/__init__.pyc
--rw-r--r--   0 ross       (501) staff       (20)    15929 2019-10-18 17:06:59.000000 octodns-0.9.9/octodns/manager.py
--rw-r--r--   0 ross       (501) staff       (20)     5776 2019-10-18 17:14:18.000000 octodns-0.9.9/octodns/zone.pyc
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:19.000000 octodns-0.9.9/tests/
--rw-r--r--   0 ross       (501) staff       (20)    89726 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_route53.py
--rw-r--r--   0 ross       (501) staff       (20)    12363 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_zone.py
--rw-r--r--   0 ross       (501) staff       (20)    22635 2019-10-18 17:14:22.000000 octodns-0.9.9/tests/test_octodns_provider_rackspace.pyc
--rw-r--r--   0 ross       (501) staff       (20)     4625 2019-03-29 18:55:00.000000 octodns-0.9.9/tests/test_octodns_provider_etc_hosts.pyc
--rw-r--r--   0 ross       (501) staff       (20)    12626 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_base.py
--rw-r--r--   0 ross       (501) staff       (20)    14324 2019-10-18 17:14:21.000000 octodns-0.9.9/tests/test_octodns_provider_mythicbeasts.pyc
--rw-r--r--   0 ross       (501) staff       (20)     5887 2019-10-18 17:14:21.000000 octodns-0.9.9/tests/test_octodns_provider_dnsmadeeasy.pyc
--rw-r--r--   0 ross       (501) staff       (20)   122188 2019-11-04 22:54:07.000000 octodns-0.9.9/tests/test_octodns_record.py
--rw-r--r--   0 ross       (501) staff       (20)     1543 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_yaml.py
--rw-r--r--   0 ross       (501) staff       (20)    12691 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_selectel.py
--rw-r--r--   0 ross       (501) staff       (20)    10469 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_powerdns.py
--rw-r--r--   0 ross       (501) staff       (20)    28687 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_rackspace.py
--rw-r--r--   0 ross       (501) staff       (20)    52729 2019-10-18 17:14:23.000000 octodns-0.9.9/tests/test_octodns_provider_route53.pyc
--rw-r--r--   0 ross       (501) staff       (20)    12463 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_manager.py
--rw-r--r--   0 ross       (501) staff       (20)    16145 2019-10-18 17:14:21.000000 octodns-0.9.9/tests/test_octodns_provider_googlecloud.pyc
--rw-r--r--   0 ross       (501) staff       (20)     9838 2019-10-18 17:14:24.000000 octodns-0.9.9/tests/test_octodns_provider_transip.pyc
--rw-r--r--   0 ross       (501) staff       (20)     4328 2019-10-18 17:14:21.000000 octodns-0.9.9/tests/test_octodns_provider_fastdns.pyc
--rw-r--r--   0 ross       (501) staff       (20)    29044 2019-10-18 17:14:20.000000 octodns-0.9.9/tests/test_octodns_provider_cloudflare.pyc
--rw-r--r--   0 ross       (501) staff       (20)     5317 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_fastdns.py
--rw-r--r--   0 ross       (501) staff       (20)    13221 2019-10-18 17:14:18.000000 octodns-0.9.9/tests/test_octodns_manager.pyc
--rw-r--r--   0 ross       (501) staff       (20)     2730 2019-10-18 17:14:32.000000 octodns-0.9.9/tests/test_octodns_source_axfr.pyc
--rw-r--r--   0 ross       (501) staff       (20)     5958 2019-10-18 17:14:20.000000 octodns-0.9.9/tests/test_octodns_provider_dnsimple.pyc
--rw-r--r--   0 ross       (501) staff       (20)    10891 2019-10-18 17:14:24.000000 octodns-0.9.9/tests/test_octodns_provider_selectel.pyc
--rw-r--r--   0 ross       (501) staff       (20)     5134 2019-04-27 22:05:45.000000 octodns-0.9.9/tests/test_octodns_source_tinydns.pyc
--rw-r--r--   0 ross       (501) staff       (20)    14792 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_yaml.py
--rw-r--r--   0 ross       (501) staff       (20)     1680 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_equality.py
--r--r--r--   0 ross       (501) staff       (20)    56124 2019-04-01 13:57:18.000000 octodns-0.9.9/tests/test_octodns_provider_route53.py.dynamic
--rw-r--r--   0 ross       (501) staff       (20)     6066 2019-04-27 21:13:19.000000 octodns-0.9.9/tests/test_octodns_source_tinydns.py
--rw-r--r--   0 ross       (501) staff       (20)     8776 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_digitalocean.py
--rw-r--r--   0 ross       (501) staff       (20)    16766 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_mythicbeasts.py
--rw-r--r--   0 ross       (501) staff       (20)     6196 2019-10-18 17:14:20.000000 octodns-0.9.9/tests/test_octodns_provider_digitalocean.pyc
--rw-r--r--   0 ross       (501) staff       (20)     2198 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_source_axfr.py
--rw-r--r--   0 ross       (501) staff       (20)    20306 2019-04-08 19:34:11.000000 octodns-0.9.9/tests/test_octodns_provider_azuredns.py
--rw-r--r--   0 ross       (501) staff       (20)    15258 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_ovh.py
--rw-r--r--   0 ross       (501) staff       (20)    43670 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_cloudflare.py
--rw-r--r--   0 ross       (501) staff       (20)    10574 2019-10-18 17:14:32.000000 octodns-0.9.9/tests/test_octodns_zone.pyc
--rw-r--r--   0 ross       (501) staff       (20)    11271 2019-10-18 17:14:22.000000 octodns-0.9.9/tests/test_octodns_provider_ns1.pyc
--rw-r--r--   0 ross       (501) staff       (20)     2443 2019-10-18 17:14:18.000000 octodns-0.9.9/tests/test_octodns_equality.pyc
--rw-r--r--   0 ross       (501) staff       (20)    10674 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_transip.py
--rw-r--r--   0 ross       (501) staff       (20)     5050 2019-10-18 17:14:18.000000 octodns-0.9.9/tests/test_octodns_plan.pyc
--rw-r--r--   0 ross       (501) staff       (20)     3232 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_plan.py
--rw-r--r--   0 ross       (501) staff       (20)     5765 2019-10-18 17:14:20.000000 octodns-0.9.9/tests/test_octodns_provider_constellix.pyc
--rw-r--r--   0 ross       (501) staff       (20)     9780 2019-10-18 17:14:22.000000 octodns-0.9.9/tests/test_octodns_provider_ovh.pyc
--rw-r--r--   0 ross       (501) staff       (20)     6009 2019-03-28 20:58:28.000000 octodns-0.9.9/tests/test_octodns_provider_etc_hosts.py
--rw-r--r--   0 ross       (501) staff       (20)    15372 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_googlecloud.py
--rw-r--r--   0 ross       (501) staff       (20)    16653 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_ns1.py
--rw-r--r--   0 ross       (501) staff       (20)    11526 2019-10-18 17:14:32.000000 octodns-0.9.9/tests/test_octodns_provider_yaml.pyc
--rw-r--r--   0 ross       (501) staff       (20)     7140 2019-10-18 17:14:22.000000 octodns-0.9.9/tests/test_octodns_provider_powerdns.pyc
--rw-r--r--   0 ross       (501) staff       (20)    94568 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_dyn.py
--rw-r--r--   0 ross       (501) staff       (20)     7914 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_dnsmadeeasy.py
--rw-r--r--   0 ross       (501) staff       (20)    13100 2019-10-18 17:14:20.000000 octodns-0.9.9/tests/test_octodns_provider_base.pyc
--rw-r--r--   0 ross       (501) staff       (20)     3110 2019-03-28 20:58:28.000000 octodns-0.9.9/tests/test_octodns_record_geo.py
--rw-r--r--   0 ross       (501) staff       (20)     1759 2018-12-14 19:33:23.000000 octodns-0.9.9/tests/helpers.py
--rw-r--r--   0 ross       (501) staff       (20)     1847 2019-10-18 17:14:32.000000 octodns-0.9.9/tests/test_octodns_yaml.pyc
--rw-r--r--   0 ross       (501) staff       (20)    15965 2019-04-08 19:36:03.000000 octodns-0.9.9/tests/test_octodns_provider_azuredns.pyc
--rw-r--r--   0 ross       (501) staff       (20)     8122 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_dnsimple.py
--rw-r--r--   0 ross       (501) staff       (20)     4520 2018-12-17 17:12:02.000000 octodns-0.9.9/tests/helpers.pyc
--rw-r--r--   0 ross       (501) staff       (20)    66468 2019-11-04 22:56:57.000000 octodns-0.9.9/tests/test_octodns_record.pyc
--rw-r--r--   0 ross       (501) staff       (20)     2960 2019-03-29 18:55:02.000000 octodns-0.9.9/tests/test_octodns_record_geo.pyc
--rw-r--r--   0 ross       (501) staff       (20)    59472 2019-10-18 17:14:21.000000 octodns-0.9.9/tests/test_octodns_provider_dyn.pyc
--rw-r--r--   0 ross       (501) staff       (20)     7751 2019-10-18 17:06:59.000000 octodns-0.9.9/tests/test_octodns_provider_constellix.py
--rw-r--r--   0 ross       (501) staff       (20)      124 2017-11-08 13:58:43.000000 octodns-0.9.9/MANIFEST.in
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:18.000000 octodns-0.9.9/docs/
--rw-r--r--   0 ross       (501) staff       (20)     3331 2019-05-06 15:13:22.000000 octodns-0.9.9/docs/geo_records.md
--rw-r--r--   0 ross       (501) staff       (20)     3821 2019-05-06 15:13:22.000000 octodns-0.9.9/docs/dynamic_records.md
--rw-r--r--   0 ross       (501) staff       (20)     3222 2019-05-06 15:13:22.000000 octodns-0.9.9/docs/records.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:19.000000 octodns-0.9.9/script/
--rwxr-xr-x   0 ross       (501) staff       (20)      394 2018-04-15 17:03:35.000000 octodns-0.9.9/script/lint
--rwxr-xr-x   0 ross       (501) staff       (20)     1070 2019-11-04 23:03:08.000000 octodns-0.9.9/script/cibuild
--rwxr-xr-x   0 ross       (501) staff       (20)      770 2019-04-27 21:13:19.000000 octodns-0.9.9/script/bootstrap
--rwxr-xr-x   0 ross       (501) staff       (20)      549 2017-10-30 18:15:33.000000 octodns-0.9.9/script/test
--rwxr-xr-x   0 ross       (501) staff       (20)     1633 2018-12-14 19:33:23.000000 octodns-0.9.9/script/generate-geo-data
--rwxr-xr-x   0 ross       (501) staff       (20)      586 2019-10-05 14:20:16.000000 octodns-0.9.9/script/release
--rwxr-xr-x   0 ross       (501) staff       (20)      283 2019-04-27 21:13:19.000000 octodns-0.9.9/script/sdist
--rwxr-xr-x   0 ross       (501) staff       (20)       39 2018-10-17 00:52:03.000000 octodns-0.9.9/script/entrypoint.sh
--rwxr-xr-x   0 ross       (501) staff       (20)      830 2019-10-18 17:06:59.000000 octodns-0.9.9/script/coverage
--rw-r--r--   0 ross       (501) staff       (20)    16987 2019-10-12 15:23:02.000000 octodns-0.9.9/README.md
--rw-r--r--   0 ross       (501) staff       (20)     2325 2019-10-18 17:06:59.000000 octodns-0.9.9/setup.py
--rw-r--r--   0 ross       (501) staff       (20)     3482 2018-07-16 17:04:58.000000 octodns-0.9.9/CONTRIBUTING.md
--rw-r--r--   0 ross       (501) staff       (20)       38 2019-11-04 23:03:19.000000 octodns-0.9.9/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)    15862 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     3891 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)      227 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/entry_points.txt
--rw-r--r--   0 ross       (501) staff       (20)      198 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)        8 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2019-11-04 23:03:18.000000 octodns-0.9.9/octodns.egg-info/dependency_links.txt
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/
+-rw-r--r--   0 neo       (1000) neo       (1000)    26907 2023-05-17 16:57:30.000000 octodns-1.0.0rc0/CHANGELOG.md
+-rw-r--r--   0 neo       (1000) neo       (1000)     3229 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 neo       (1000) neo       (1000)     3761 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/CONTRIBUTING.md
+-rw-r--r--   0 neo       (1000) neo       (1000)     1056 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/LICENSE
+-rw-r--r--   0 neo       (1000) neo       (1000)      292 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/MANIFEST.in
+-rw-r--r--   0 neo       (1000) neo       (1000)    26279 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)    26000 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.530521 octodns-1.0.0rc0/docs/
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.530521 octodns-1.0.0rc0/docs/assets/
+-rw-r--r--   0 neo       (1000) neo       (1000)    82371 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/assets/deploy.png
+-rw-r--r--   0 neo       (1000) neo       (1000)    75814 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/assets/noop.png
+-rw-r--r--   0 neo       (1000) neo       (1000)   212872 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/assets/pr.png
+-rw-r--r--   0 neo       (1000) neo       (1000)     2917 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/docs/auto_arpa.md
+-rw-r--r--   0 neo       (1000) neo       (1000)     7482 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/docs/dynamic_records.md
+-rw-r--r--   0 neo       (1000) neo       (1000)     3427 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/geo_records.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.530521 octodns-1.0.0rc0/docs/logos/
+-rw-r--r--   0 neo       (1000) neo       (1000)     3983 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/docs/logos/octodns-logo.png
+-rw-r--r--   0 neo       (1000) neo       (1000)     7720 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/docs/records.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.533854 octodns-1.0.0rc0/octodns/
+-rw-r--r--   0 neo       (1000) neo       (1000)      101 2023-05-17 16:57:30.000000 octodns-1.0.0rc0/octodns/__init__.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.533854 octodns-1.0.0rc0/octodns/cmds/
+-rw-r--r--   0 neo       (1000) neo       (1000)        6 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3786 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/cmds/args.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1423 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/cmds/compare.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1536 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/dump.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     3360 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/cmds/report.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1544 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/sync.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      517 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/validate.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      444 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/cmds/versions.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      717 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/equality.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2373 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/idna.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    32891 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/manager.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.537188 octodns-1.0.0rc0/octodns/processor/
+-rw-r--r--   0 neo       (1000) neo       (1000)        6 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1824 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/acme.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2153 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/processor/arpa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2960 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/base.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     5052 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/processor/filter.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3664 2023-05-16 17:41:42.000000 octodns-1.0.0rc0/octodns/processor/ownership.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2276 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/processor/restrict.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3803 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/processor/spf.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.537188 octodns-1.0.0rc0/octodns/provider/
+-rw-r--r--   0 neo       (1000) neo       (1000)      108 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/provider/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    12356 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/provider/base.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    11096 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/provider/plan.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    12103 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/provider/yaml.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.543854 octodns-1.0.0rc0/octodns/record/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1471 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      412 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/a.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      423 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/aaaa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      488 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/alias.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    10392 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/base.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2342 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/caa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1407 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/change.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1495 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/chunked.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      534 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/cname.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      296 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/dname.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3442 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ds.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    15080 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/record/dynamic.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      450 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/exception.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     5311 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/geo.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    13426 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/octodns/record/geo_data.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1385 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ip.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    10626 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/loc.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3328 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/mx.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     4382 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/naptr.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      235 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ns.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      412 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/ptr.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      644 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/rr.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      220 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/spf.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     4223 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/srv.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3491 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/sshfp.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      465 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/record/subnet.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2000 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/target.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     4987 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/tlsa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      257 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/txt.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3263 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/record/urlfwd.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.543854 octodns-1.0.0rc0/octodns/source/
+-rw-r--r--   0 neo       (1000) neo       (1000)        6 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/source/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1713 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/octodns/source/base.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3280 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/octodns/source/envvar.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     8240 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/source/tinydns.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2194 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/yaml.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    10479 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/octodns/zone.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.533854 octodns-1.0.0rc0/octodns.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)    26279 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)     6243 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      272 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/entry_points.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      292 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        8 2023-05-17 16:58:26.000000 octodns-1.0.0rc0/octodns.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      209 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/pyproject.toml
+-rw-r--r--   0 neo       (1000) neo       (1000)      943 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/requirements-dev.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      179 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/requirements.txt
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.547188 octodns-1.0.0rc0/script/
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1273 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/bootstrap
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      177 2021-10-12 19:58:05.000000 octodns-1.0.0rc0/script/changelog
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1085 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/cibuild
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      796 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/cibuild-setup-py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      998 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/script/coverage
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      184 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/format
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     2486 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/generate-geo-data
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      387 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/lint
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      738 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/script/release
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      283 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/script/sdist
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      662 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/script/test
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1705 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/script/test-module
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1940 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/script/update-requirements
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)     2907 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.553855 octodns-1.0.0rc0/tests/
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/
+-rw-r--r--   0 neo       (1000) neo       (1000)      363 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/alias-zone-loop.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      447 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/always-dry-run.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      129 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-plan-output-config.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       63 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-plan-output-missing-class.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       81 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-provider-class-module.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       59 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-provider-class-no-module.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       67 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/bad-provider-class.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)     4749 2023-04-06 21:25:05.000000 octodns-1.0.0rc0/tests/config/dynamic.tests.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)        4 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/empty.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       32 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-provider-class.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       75 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-provider-config.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      121 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-provider-env.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       44 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/missing-sources.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      235 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/no-dump.yaml
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/override/
+-rw-r--r--   0 neo       (1000) neo       (1000)      167 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/override/dynamic.tests.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      115 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/plan-output-filehandle.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      389 2021-06-25 17:49:24.000000 octodns-1.0.0rc0/tests/config/processors-missing-class.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      493 2021-06-25 17:49:24.000000 octodns-1.0.0rc0/tests/config/processors-wants-config.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      940 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/processors.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      461 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/provider-problems.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      400 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/simple-alias-zone.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      626 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/simple-arpa.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      841 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/simple-split.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      216 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/simple-validate.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)     1016 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/config/simple.yaml
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.527188 octodns-1.0.0rc0/tests/config/split/
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/
+-rw-r--r--   0 neo       (1000) neo       (1000)      749 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/a.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      993 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/aaaa.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      785 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/cname.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)     1689 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/real-ish-a.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      277 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/dynamic.tests.tst/simple-weighted.yaml
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.563855 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/12.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       36 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/2.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       37 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/subzone.unit.tests.tst/test.yaml
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.567188 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/
+-rw-r--r--   0 neo       (1000) neo       (1000)      640 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/$unit.tests.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      198 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/_srv._tcp.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       81 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/aaaa.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/cname.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/dname.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       85 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/excluded.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       69 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/ignored.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       85 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/included.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      248 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/mx.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      313 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/naptr.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-08-20 18:14:19.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/ptr.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       71 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/spf.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       56 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/sub.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      166 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/txt.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      241 2021-07-27 03:02:31.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/urlfwd.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       51 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/www.sub.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       47 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unit.tests.tst/www.yaml
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.567188 octodns-1.0.0rc0/tests/config/split/unordered.tst/
+-rw-r--r--   0 neo       (1000) neo       (1000)       36 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unordered.tst/abc.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       57 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/split/unordered.tst/xyz.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)        4 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/config/sub.txt.unit.tests.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       99 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/subzone.unit.tests.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)     3328 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/config/unit.tests.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      307 2021-06-25 17:49:24.000000 octodns-1.0.0rc0/tests/config/unknown-processor.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      217 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/unknown-provider.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)      328 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/unknown-source-zone.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)       89 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/config/unordered.yaml
+-rw-r--r--   0 neo       (1000) neo       (1000)     2874 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/helpers.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1579 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_equality.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     4690 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_idna.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    38035 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_manager.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     9527 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_plan.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3135 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_processor_acme.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     7812 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_processor_arpa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     6302 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_processor_filter.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     5156 2023-05-16 17:41:42.000000 octodns-1.0.0rc0/tests/test_octodns_processor_ownership.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3653 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/test_octodns_processor_restrict.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    12859 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_processor_spf.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    33602 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/tests/test_octodns_provider_base.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    22494 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_provider_yaml.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    17628 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     6241 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_a.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     7294 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_aaaa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     3468 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_alias.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     8813 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_caa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2926 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_change.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      952 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_chunked.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     4291 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_cname.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2879 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_dname.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     6371 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ds.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    53366 2023-05-11 06:07:49.000000 octodns-1.0.0rc0/tests/test_octodns_record_dynamic.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     9241 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_geo.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      681 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ip.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    23625 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_loc.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     8611 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_mx.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    12946 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_naptr.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2537 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ns.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2802 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_ptr.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     2166 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_spf.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    13678 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_srv.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    10648 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_sshfp.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      738 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_target.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    14105 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_tlsa.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     5264 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_txt.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    12418 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_record_urlfwd.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1419 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_source_envvar.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     6080 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_source_tinydns.py
+-rw-r--r--   0 neo       (1000) neo       (1000)     1402 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_yaml.py
+-rw-r--r--   0 neo       (1000) neo       (1000)    18104 2023-04-02 09:50:58.000000 octodns-1.0.0rc0/tests/test_octodns_zone.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/tests/zones/
+-rw-r--r--   0 neo       (1000) neo       (1000)      599 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/zones/2.0.192.in-addr.arpa.
+-rw-r--r--   0 neo       (1000) neo       (1000)      474 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/ext.unit.tests.extension
+-rw-r--r--   0 neo       (1000) neo       (1000)     1541 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/invalid.records.tst
+-rw-r--r--   0 neo       (1000) neo       (1000)      362 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/invalid.zone.tst
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-05-17 16:58:26.570521 octodns-1.0.0rc0/tests/zones/tinydns/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1024 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/tinydns/.is-needed-for-tests
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1345 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/zones/tinydns/example.com
+-rw-r--r--   0 neo       (1000) neo       (1000)      166 2021-04-23 07:46:28.000000 octodns-1.0.0rc0/tests/zones/tinydns/other.foo
+-rw-r--r--   0 neo       (1000) neo       (1000)     1769 2022-01-14 22:24:33.000000 octodns-1.0.0rc0/tests/zones/unit.tests.
+-rw-r--r--   0 neo       (1000) neo       (1000)     1932 2022-11-12 22:01:11.000000 octodns-1.0.0rc0/tests/zones/unit.tests.tst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `octodns-0.9.9/LICENSE` & `octodns-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns-0.9.9/octodns/record/geo_data.py` & `octodns-1.0.0rc0/octodns/record/geo_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,315 +2,350 @@
 # -*- coding: utf-8 -*-
 #
 # This file is generated using
 #   ./script/generate-geo-data > octodns/record/geo_data.py
 # do not modify it directly
 #
 
-geo_data = \
-    {'AF': {'AO': {'name': 'Angola'},
-            'BF': {'name': 'Burkina Faso'},
-            'BI': {'name': 'Burundi'},
-            'BJ': {'name': 'Benin'},
-            'BW': {'name': 'Botswana'},
-            'CD': {'name': 'Congo, The Democratic Republic of the'},
-            'CF': {'name': 'Central African Republic'},
-            'CG': {'name': 'Congo'},
-            'CI': {'name': "Côte d'Ivoire"},
-            'CM': {'name': 'Cameroon'},
-            'CV': {'name': 'Cabo Verde'},
-            'DJ': {'name': 'Djibouti'},
-            'DZ': {'name': 'Algeria'},
-            'EG': {'name': 'Egypt'},
-            'EH': {'name': 'Western Sahara'},
-            'ER': {'name': 'Eritrea'},
-            'ET': {'name': 'Ethiopia'},
-            'GA': {'name': 'Gabon'},
-            'GH': {'name': 'Ghana'},
-            'GM': {'name': 'Gambia'},
-            'GN': {'name': 'Guinea'},
-            'GQ': {'name': 'Equatorial Guinea'},
-            'GW': {'name': 'Guinea-Bissau'},
-            'KE': {'name': 'Kenya'},
-            'KM': {'name': 'Comoros'},
-            'LR': {'name': 'Liberia'},
-            'LS': {'name': 'Lesotho'},
-            'LY': {'name': 'Libya'},
-            'MA': {'name': 'Morocco'},
-            'MG': {'name': 'Madagascar'},
-            'ML': {'name': 'Mali'},
-            'MR': {'name': 'Mauritania'},
-            'MU': {'name': 'Mauritius'},
-            'MW': {'name': 'Malawi'},
-            'MZ': {'name': 'Mozambique'},
-            'NA': {'name': 'Namibia'},
-            'NE': {'name': 'Niger'},
-            'NG': {'name': 'Nigeria'},
-            'RE': {'name': 'Réunion'},
-            'RW': {'name': 'Rwanda'},
-            'SC': {'name': 'Seychelles'},
-            'SD': {'name': 'Sudan'},
-            'SH': {'name': 'Saint Helena, Ascension and Tristan da Cunha'},
-            'SL': {'name': 'Sierra Leone'},
-            'SN': {'name': 'Senegal'},
-            'SO': {'name': 'Somalia'},
-            'SS': {'name': 'South Sudan'},
-            'ST': {'name': 'Sao Tome and Principe'},
-            'SZ': {'name': 'Swaziland'},
-            'TD': {'name': 'Chad'},
-            'TG': {'name': 'Togo'},
-            'TN': {'name': 'Tunisia'},
-            'TZ': {'name': 'Tanzania, United Republic of'},
-            'UG': {'name': 'Uganda'},
-            'YT': {'name': 'Mayotte'},
-            'ZA': {'name': 'South Africa'},
-            'ZM': {'name': 'Zambia'},
-            'ZW': {'name': 'Zimbabwe'}},
-     'AN': {'AQ': {'name': 'Antarctica'},
-            'BV': {'name': 'Bouvet Island'},
-            'HM': {'name': 'Heard Island and McDonald Islands'},
-            'TF': {'name': 'French Southern Territories'}},
-     'AS': {'AE': {'name': 'United Arab Emirates'},
-            'AF': {'name': 'Afghanistan'},
-            'AM': {'name': 'Armenia'},
-            'AZ': {'name': 'Azerbaijan'},
-            'BD': {'name': 'Bangladesh'},
-            'BH': {'name': 'Bahrain'},
-            'BN': {'name': 'Brunei Darussalam'},
-            'BT': {'name': 'Bhutan'},
-            'CC': {'name': 'Cocos (Keeling) Islands'},
-            'CN': {'name': 'China'},
-            'CX': {'name': 'Christmas Island'},
-            'CY': {'name': 'Cyprus'},
-            'GE': {'name': 'Georgia'},
-            'HK': {'name': 'Hong Kong'},
-            'ID': {'name': 'Indonesia'},
-            'IL': {'name': 'Israel'},
-            'IN': {'name': 'India'},
-            'IO': {'name': 'British Indian Ocean Territory'},
-            'IQ': {'name': 'Iraq'},
-            'IR': {'name': 'Iran, Islamic Republic of'},
-            'JO': {'name': 'Jordan'},
-            'JP': {'name': 'Japan'},
-            'KG': {'name': 'Kyrgyzstan'},
-            'KH': {'name': 'Cambodia'},
-            'KP': {'name': "Korea, Democratic People's Republic of"},
-            'KR': {'name': 'Korea, Republic of'},
-            'KW': {'name': 'Kuwait'},
-            'KZ': {'name': 'Kazakhstan'},
-            'LA': {'name': "Lao People's Democratic Republic"},
-            'LB': {'name': 'Lebanon'},
-            'LK': {'name': 'Sri Lanka'},
-            'MM': {'name': 'Myanmar'},
-            'MN': {'name': 'Mongolia'},
-            'MO': {'name': 'Macao'},
-            'MV': {'name': 'Maldives'},
-            'MY': {'name': 'Malaysia'},
-            'NP': {'name': 'Nepal'},
-            'OM': {'name': 'Oman'},
-            'PH': {'name': 'Philippines'},
-            'PK': {'name': 'Pakistan'},
-            'PS': {'name': 'Palestine, State of'},
-            'QA': {'name': 'Qatar'},
-            'SA': {'name': 'Saudi Arabia'},
-            'SG': {'name': 'Singapore'},
-            'SY': {'name': 'Syrian Arab Republic'},
-            'TH': {'name': 'Thailand'},
-            'TJ': {'name': 'Tajikistan'},
-            'TM': {'name': 'Turkmenistan'},
-            'TR': {'name': 'Turkey'},
-            'TW': {'name': 'Taiwan, Province of China'},
-            'UZ': {'name': 'Uzbekistan'},
-            'VN': {'name': 'Viet Nam'},
-            'YE': {'name': 'Yemen'}},
-     'EU': {'AD': {'name': 'Andorra'},
-            'AL': {'name': 'Albania'},
-            'AT': {'name': 'Austria'},
-            'AX': {'name': 'Åland Islands'},
-            'BA': {'name': 'Bosnia and Herzegovina'},
-            'BE': {'name': 'Belgium'},
-            'BG': {'name': 'Bulgaria'},
-            'BY': {'name': 'Belarus'},
-            'CH': {'name': 'Switzerland'},
-            'CZ': {'name': 'Czechia'},
-            'DE': {'name': 'Germany'},
-            'DK': {'name': 'Denmark'},
-            'EE': {'name': 'Estonia'},
-            'ES': {'name': 'Spain'},
-            'FI': {'name': 'Finland'},
-            'FO': {'name': 'Faroe Islands'},
-            'FR': {'name': 'France'},
-            'GB': {'name': 'United Kingdom'},
-            'GG': {'name': 'Guernsey'},
-            'GI': {'name': 'Gibraltar'},
-            'GR': {'name': 'Greece'},
-            'HR': {'name': 'Croatia'},
-            'HU': {'name': 'Hungary'},
-            'IE': {'name': 'Ireland'},
-            'IM': {'name': 'Isle of Man'},
-            'IS': {'name': 'Iceland'},
-            'IT': {'name': 'Italy'},
-            'JE': {'name': 'Jersey'},
-            'LI': {'name': 'Liechtenstein'},
-            'LT': {'name': 'Lithuania'},
-            'LU': {'name': 'Luxembourg'},
-            'LV': {'name': 'Latvia'},
-            'MC': {'name': 'Monaco'},
-            'MD': {'name': 'Moldova, Republic of'},
-            'ME': {'name': 'Montenegro'},
-            'MK': {'name': 'Macedonia, Republic of'},
-            'MT': {'name': 'Malta'},
-            'NL': {'name': 'Netherlands'},
-            'NO': {'name': 'Norway'},
-            'PL': {'name': 'Poland'},
-            'PT': {'name': 'Portugal'},
-            'RO': {'name': 'Romania'},
-            'RS': {'name': 'Serbia'},
-            'RU': {'name': 'Russian Federation'},
-            'SE': {'name': 'Sweden'},
-            'SI': {'name': 'Slovenia'},
-            'SJ': {'name': 'Svalbard and Jan Mayen'},
-            'SK': {'name': 'Slovakia'},
-            'SM': {'name': 'San Marino'},
-            'UA': {'name': 'Ukraine'},
-            'VA': {'name': 'Holy See (Vatican City State)'}},
-     'ID': {'TL': {'name': 'Timor-Leste'}},
-     'NA': {'AG': {'name': 'Antigua and Barbuda'},
-            'AI': {'name': 'Anguilla'},
-            'AW': {'name': 'Aruba'},
-            'BB': {'name': 'Barbados'},
-            'BL': {'name': 'Saint Barthélemy'},
-            'BM': {'name': 'Bermuda'},
-            'BQ': {'name': 'Bonaire, Sint Eustatius and Saba'},
-            'BS': {'name': 'Bahamas'},
-            'BZ': {'name': 'Belize'},
-            'CA': {'name': 'Canada'},
-            'CR': {'name': 'Costa Rica'},
-            'CU': {'name': 'Cuba'},
-            'CW': {'name': 'Curaçao'},
-            'DM': {'name': 'Dominica'},
-            'DO': {'name': 'Dominican Republic'},
-            'GD': {'name': 'Grenada'},
-            'GL': {'name': 'Greenland'},
-            'GP': {'name': 'Guadeloupe'},
-            'GT': {'name': 'Guatemala'},
-            'HN': {'name': 'Honduras'},
-            'HT': {'name': 'Haiti'},
-            'JM': {'name': 'Jamaica'},
-            'KN': {'name': 'Saint Kitts and Nevis'},
-            'KY': {'name': 'Cayman Islands'},
-            'LC': {'name': 'Saint Lucia'},
-            'MF': {'name': 'Saint Martin (French part)'},
-            'MQ': {'name': 'Martinique'},
-            'MS': {'name': 'Montserrat'},
-            'MX': {'name': 'Mexico'},
-            'NI': {'name': 'Nicaragua'},
-            'PA': {'name': 'Panama'},
-            'PM': {'name': 'Saint Pierre and Miquelon'},
-            'PR': {'name': 'Puerto Rico'},
-            'SV': {'name': 'El Salvador'},
-            'SX': {'name': 'Sint Maarten (Dutch part)'},
-            'TC': {'name': 'Turks and Caicos Islands'},
-            'TT': {'name': 'Trinidad and Tobago'},
-            'US': {'name': 'United States',
-                   'provinces': {'AK': {'name': 'Alaska'},
-                                 'AL': {'name': 'Alabama'},
-                                 'AR': {'name': 'Arkansas'},
-                                 'AS': {'name': 'American Samoa'},
-                                 'AZ': {'name': 'Arizona'},
-                                 'CA': {'name': 'California'},
-                                 'CO': {'name': 'Colorado'},
-                                 'CT': {'name': 'Connecticut'},
-                                 'DC': {'name': 'District of Columbia'},
-                                 'DE': {'name': 'Delaware'},
-                                 'FL': {'name': 'Florida'},
-                                 'GA': {'name': 'Georgia'},
-                                 'GU': {'name': 'Guam'},
-                                 'HI': {'name': 'Hawaii'},
-                                 'IA': {'name': 'Iowa'},
-                                 'ID': {'name': 'Idaho'},
-                                 'IL': {'name': 'Illinois'},
-                                 'IN': {'name': 'Indiana'},
-                                 'KS': {'name': 'Kansas'},
-                                 'KY': {'name': 'Kentucky'},
-                                 'LA': {'name': 'Louisiana'},
-                                 'MA': {'name': 'Massachusetts'},
-                                 'MD': {'name': 'Maryland'},
-                                 'ME': {'name': 'Maine'},
-                                 'MI': {'name': 'Michigan'},
-                                 'MN': {'name': 'Minnesota'},
-                                 'MO': {'name': 'Missouri'},
-                                 'MP': {'name': 'Northern Mariana Islands'},
-                                 'MS': {'name': 'Mississippi'},
-                                 'MT': {'name': 'Montana'},
-                                 'NC': {'name': 'North Carolina'},
-                                 'ND': {'name': 'North Dakota'},
-                                 'NE': {'name': 'Nebraska'},
-                                 'NH': {'name': 'New Hampshire'},
-                                 'NJ': {'name': 'New Jersey'},
-                                 'NM': {'name': 'New Mexico'},
-                                 'NV': {'name': 'Nevada'},
-                                 'NY': {'name': 'New York'},
-                                 'OH': {'name': 'Ohio'},
-                                 'OK': {'name': 'Oklahoma'},
-                                 'OR': {'name': 'Oregon'},
-                                 'PA': {'name': 'Pennsylvania'},
-                                 'PR': {'name': 'Puerto Rico'},
-                                 'RI': {'name': 'Rhode Island'},
-                                 'SC': {'name': 'South Carolina'},
-                                 'SD': {'name': 'South Dakota'},
-                                 'TN': {'name': 'Tennessee'},
-                                 'TX': {'name': 'Texas'},
-                                 'UM': {'name': 'United States Minor Outlying '
-                                                'Islands'},
-                                 'UT': {'name': 'Utah'},
-                                 'VA': {'name': 'Virginia'},
-                                 'VI': {'name': 'Virgin Islands'},
-                                 'VT': {'name': 'Vermont'},
-                                 'WA': {'name': 'Washington'},
-                                 'WI': {'name': 'Wisconsin'},
-                                 'WV': {'name': 'West Virginia'},
-                                 'WY': {'name': 'Wyoming'}}},
-            'VC': {'name': 'Saint Vincent and the Grenadines'},
-            'VG': {'name': 'Virgin Islands, British'},
-            'VI': {'name': 'Virgin Islands, U.S.'}},
-     'OC': {'AS': {'name': 'American Samoa'},
-            'AU': {'name': 'Australia'},
-            'CK': {'name': 'Cook Islands'},
-            'FJ': {'name': 'Fiji'},
-            'FM': {'name': 'Micronesia, Federated States of'},
-            'GU': {'name': 'Guam'},
-            'KI': {'name': 'Kiribati'},
-            'MH': {'name': 'Marshall Islands'},
-            'MP': {'name': 'Northern Mariana Islands'},
-            'NC': {'name': 'New Caledonia'},
-            'NF': {'name': 'Norfolk Island'},
-            'NR': {'name': 'Nauru'},
-            'NU': {'name': 'Niue'},
-            'NZ': {'name': 'New Zealand'},
-            'PF': {'name': 'French Polynesia'},
-            'PG': {'name': 'Papua New Guinea'},
-            'PN': {'name': 'Pitcairn'},
-            'PW': {'name': 'Palau'},
-            'SB': {'name': 'Solomon Islands'},
-            'TK': {'name': 'Tokelau'},
-            'TO': {'name': 'Tonga'},
-            'TV': {'name': 'Tuvalu'},
-            'UM': {'name': 'United States Minor Outlying Islands'},
-            'VU': {'name': 'Vanuatu'},
-            'WF': {'name': 'Wallis and Futuna'},
-            'WS': {'name': 'Samoa'}},
-     'SA': {'AR': {'name': 'Argentina'},
-            'BO': {'name': 'Bolivia, Plurinational State of'},
-            'BR': {'name': 'Brazil'},
-            'CL': {'name': 'Chile'},
-            'CO': {'name': 'Colombia'},
-            'EC': {'name': 'Ecuador'},
-            'FK': {'name': 'Falkland Islands (Malvinas)'},
-            'GF': {'name': 'French Guiana'},
-            'GS': {'name': 'South Georgia and the South Sandwich Islands'},
-            'GY': {'name': 'Guyana'},
-            'PE': {'name': 'Peru'},
-            'PY': {'name': 'Paraguay'},
-            'SR': {'name': 'Suriname'},
-            'UY': {'name': 'Uruguay'},
-            'VE': {'name': 'Venezuela, Bolivarian Republic of'}}}
+geo_data = {
+    'AF': {
+        'AO': {'name': 'Angola'},
+        'BF': {'name': 'Burkina Faso'},
+        'BI': {'name': 'Burundi'},
+        'BJ': {'name': 'Benin'},
+        'BW': {'name': 'Botswana'},
+        'CD': {'name': 'Congo, The Democratic Republic of the'},
+        'CF': {'name': 'Central African Republic'},
+        'CG': {'name': 'Congo'},
+        'CI': {'name': "Côte d'Ivoire"},
+        'CM': {'name': 'Cameroon'},
+        'CV': {'name': 'Cabo Verde'},
+        'DJ': {'name': 'Djibouti'},
+        'DZ': {'name': 'Algeria'},
+        'EG': {'name': 'Egypt'},
+        'EH': {'name': 'Western Sahara'},
+        'ER': {'name': 'Eritrea'},
+        'ET': {'name': 'Ethiopia'},
+        'GA': {'name': 'Gabon'},
+        'GH': {'name': 'Ghana'},
+        'GM': {'name': 'Gambia'},
+        'GN': {'name': 'Guinea'},
+        'GQ': {'name': 'Equatorial Guinea'},
+        'GW': {'name': 'Guinea-Bissau'},
+        'KE': {'name': 'Kenya'},
+        'KM': {'name': 'Comoros'},
+        'LR': {'name': 'Liberia'},
+        'LS': {'name': 'Lesotho'},
+        'LY': {'name': 'Libya'},
+        'MA': {'name': 'Morocco'},
+        'MG': {'name': 'Madagascar'},
+        'ML': {'name': 'Mali'},
+        'MR': {'name': 'Mauritania'},
+        'MU': {'name': 'Mauritius'},
+        'MW': {'name': 'Malawi'},
+        'MZ': {'name': 'Mozambique'},
+        'NA': {'name': 'Namibia'},
+        'NE': {'name': 'Niger'},
+        'NG': {'name': 'Nigeria'},
+        'RE': {'name': 'Réunion'},
+        'RW': {'name': 'Rwanda'},
+        'SC': {'name': 'Seychelles'},
+        'SD': {'name': 'Sudan'},
+        'SH': {'name': 'Saint Helena, Ascension and Tristan da Cunha'},
+        'SL': {'name': 'Sierra Leone'},
+        'SN': {'name': 'Senegal'},
+        'SO': {'name': 'Somalia'},
+        'SS': {'name': 'South Sudan'},
+        'ST': {'name': 'Sao Tome and Principe'},
+        'SZ': {'name': 'Eswatini'},
+        'TD': {'name': 'Chad'},
+        'TG': {'name': 'Togo'},
+        'TN': {'name': 'Tunisia'},
+        'TZ': {'name': 'Tanzania, United Republic of'},
+        'UG': {'name': 'Uganda'},
+        'YT': {'name': 'Mayotte'},
+        'ZA': {'name': 'South Africa'},
+        'ZM': {'name': 'Zambia'},
+        'ZW': {'name': 'Zimbabwe'},
+    },
+    'AN': {
+        'AQ': {'name': 'Antarctica'},
+        'BV': {'name': 'Bouvet Island'},
+        'HM': {'name': 'Heard Island and McDonald Islands'},
+        'TF': {'name': 'French Southern Territories'},
+    },
+    'AS': {
+        'AE': {'name': 'United Arab Emirates'},
+        'AF': {'name': 'Afghanistan'},
+        'AM': {'name': 'Armenia'},
+        'AZ': {'name': 'Azerbaijan'},
+        'BD': {'name': 'Bangladesh'},
+        'BH': {'name': 'Bahrain'},
+        'BN': {'name': 'Brunei Darussalam'},
+        'BT': {'name': 'Bhutan'},
+        'CC': {'name': 'Cocos (Keeling) Islands'},
+        'CN': {'name': 'China'},
+        'CX': {'name': 'Christmas Island'},
+        'CY': {'name': 'Cyprus'},
+        'GE': {'name': 'Georgia'},
+        'HK': {'name': 'Hong Kong'},
+        'ID': {'name': 'Indonesia'},
+        'IL': {'name': 'Israel'},
+        'IN': {'name': 'India'},
+        'IO': {'name': 'British Indian Ocean Territory'},
+        'IQ': {'name': 'Iraq'},
+        'IR': {'name': 'Iran, Islamic Republic of'},
+        'JO': {'name': 'Jordan'},
+        'JP': {'name': 'Japan'},
+        'KG': {'name': 'Kyrgyzstan'},
+        'KH': {'name': 'Cambodia'},
+        'KP': {'name': "Korea, Democratic People's Republic of"},
+        'KR': {'name': 'Korea, Republic of'},
+        'KW': {'name': 'Kuwait'},
+        'KZ': {'name': 'Kazakhstan'},
+        'LA': {'name': "Lao People's Democratic Republic"},
+        'LB': {'name': 'Lebanon'},
+        'LK': {'name': 'Sri Lanka'},
+        'MM': {'name': 'Myanmar'},
+        'MN': {'name': 'Mongolia'},
+        'MO': {'name': 'Macao'},
+        'MV': {'name': 'Maldives'},
+        'MY': {'name': 'Malaysia'},
+        'NP': {'name': 'Nepal'},
+        'OM': {'name': 'Oman'},
+        'PH': {'name': 'Philippines'},
+        'PK': {'name': 'Pakistan'},
+        'PS': {'name': 'Palestine, State of'},
+        'QA': {'name': 'Qatar'},
+        'SA': {'name': 'Saudi Arabia'},
+        'SG': {'name': 'Singapore'},
+        'SY': {'name': 'Syrian Arab Republic'},
+        'TH': {'name': 'Thailand'},
+        'TJ': {'name': 'Tajikistan'},
+        'TL': {'name': 'Timor-Leste'},
+        'TM': {'name': 'Turkmenistan'},
+        'TR': {'name': 'Turkey'},
+        'TW': {'name': 'Taiwan, Province of China'},
+        'UZ': {'name': 'Uzbekistan'},
+        'VN': {'name': 'Viet Nam'},
+        'YE': {'name': 'Yemen'},
+    },
+    'EU': {
+        'AD': {'name': 'Andorra'},
+        'AL': {'name': 'Albania'},
+        'AT': {'name': 'Austria'},
+        'AX': {'name': 'Åland Islands'},
+        'BA': {'name': 'Bosnia and Herzegovina'},
+        'BE': {'name': 'Belgium'},
+        'BG': {'name': 'Bulgaria'},
+        'BY': {'name': 'Belarus'},
+        'CH': {'name': 'Switzerland'},
+        'CZ': {'name': 'Czechia'},
+        'DE': {'name': 'Germany'},
+        'DK': {'name': 'Denmark'},
+        'EE': {'name': 'Estonia'},
+        'ES': {'name': 'Spain'},
+        'FI': {'name': 'Finland'},
+        'FO': {'name': 'Faroe Islands'},
+        'FR': {'name': 'France'},
+        'GB': {'name': 'United Kingdom'},
+        'GG': {'name': 'Guernsey'},
+        'GI': {'name': 'Gibraltar'},
+        'GR': {'name': 'Greece'},
+        'HR': {'name': 'Croatia'},
+        'HU': {'name': 'Hungary'},
+        'IE': {'name': 'Ireland'},
+        'IM': {'name': 'Isle of Man'},
+        'IS': {'name': 'Iceland'},
+        'IT': {'name': 'Italy'},
+        'JE': {'name': 'Jersey'},
+        'LI': {'name': 'Liechtenstein'},
+        'LT': {'name': 'Lithuania'},
+        'LU': {'name': 'Luxembourg'},
+        'LV': {'name': 'Latvia'},
+        'MC': {'name': 'Monaco'},
+        'MD': {'name': 'Moldova, Republic of'},
+        'ME': {'name': 'Montenegro'},
+        'MK': {'name': 'North Macedonia'},
+        'MT': {'name': 'Malta'},
+        'NL': {'name': 'Netherlands'},
+        'NO': {'name': 'Norway'},
+        'PL': {'name': 'Poland'},
+        'PT': {'name': 'Portugal'},
+        'RO': {'name': 'Romania'},
+        'RS': {'name': 'Serbia'},
+        'RU': {'name': 'Russian Federation'},
+        'SE': {'name': 'Sweden'},
+        'SI': {'name': 'Slovenia'},
+        'SJ': {'name': 'Svalbard and Jan Mayen'},
+        'SK': {'name': 'Slovakia'},
+        'SM': {'name': 'San Marino'},
+        'UA': {'name': 'Ukraine'},
+        'VA': {'name': 'Holy See (Vatican City State)'},
+    },
+    'NA': {
+        'AG': {'name': 'Antigua and Barbuda'},
+        'AI': {'name': 'Anguilla'},
+        'AW': {'name': 'Aruba'},
+        'BB': {'name': 'Barbados'},
+        'BL': {'name': 'Saint Barthélemy'},
+        'BM': {'name': 'Bermuda'},
+        'BQ': {'name': 'Bonaire, Sint Eustatius and Saba'},
+        'BS': {'name': 'Bahamas'},
+        'BZ': {'name': 'Belize'},
+        'CA': {
+            'name': 'Canada',
+            'provinces': {
+                'AB': {'name': 'Alberta'},
+                'BC': {'name': 'British Columbia'},
+                'MB': {'name': 'Manitoba'},
+                'NB': {'name': 'New Brunswick'},
+                'NL': {'name': 'Newfoundland and Labrador'},
+                'NS': {'name': 'Nova Scotia'},
+                'NT': {'name': 'Northwest Territories'},
+                'NU': {'name': 'Nunavut'},
+                'ON': {'name': 'Ontario'},
+                'PE': {'name': 'Prince Edward Island'},
+                'QC': {'name': 'Quebec'},
+                'SK': {'name': 'Saskatchewan'},
+                'YT': {'name': 'Yukon'},
+            },
+        },
+        'CR': {'name': 'Costa Rica'},
+        'CU': {'name': 'Cuba'},
+        'CW': {'name': 'Curaçao'},
+        'DM': {'name': 'Dominica'},
+        'DO': {'name': 'Dominican Republic'},
+        'GD': {'name': 'Grenada'},
+        'GL': {'name': 'Greenland'},
+        'GP': {'name': 'Guadeloupe'},
+        'GT': {'name': 'Guatemala'},
+        'HN': {'name': 'Honduras'},
+        'HT': {'name': 'Haiti'},
+        'JM': {'name': 'Jamaica'},
+        'KN': {'name': 'Saint Kitts and Nevis'},
+        'KY': {'name': 'Cayman Islands'},
+        'LC': {'name': 'Saint Lucia'},
+        'MF': {'name': 'Saint Martin (French part)'},
+        'MQ': {'name': 'Martinique'},
+        'MS': {'name': 'Montserrat'},
+        'MX': {'name': 'Mexico'},
+        'NI': {'name': 'Nicaragua'},
+        'PA': {'name': 'Panama'},
+        'PM': {'name': 'Saint Pierre and Miquelon'},
+        'PR': {'name': 'Puerto Rico'},
+        'SV': {'name': 'El Salvador'},
+        'SX': {'name': 'Sint Maarten (Dutch part)'},
+        'TC': {'name': 'Turks and Caicos Islands'},
+        'TT': {'name': 'Trinidad and Tobago'},
+        'US': {
+            'name': 'United States',
+            'provinces': {
+                'AK': {'name': 'Alaska'},
+                'AL': {'name': 'Alabama'},
+                'AR': {'name': 'Arkansas'},
+                'AS': {'name': 'American Samoa'},
+                'AZ': {'name': 'Arizona'},
+                'CA': {'name': 'California'},
+                'CO': {'name': 'Colorado'},
+                'CT': {'name': 'Connecticut'},
+                'DC': {'name': 'District of Columbia'},
+                'DE': {'name': 'Delaware'},
+                'FL': {'name': 'Florida'},
+                'GA': {'name': 'Georgia'},
+                'GU': {'name': 'Guam'},
+                'HI': {'name': 'Hawaii'},
+                'IA': {'name': 'Iowa'},
+                'ID': {'name': 'Idaho'},
+                'IL': {'name': 'Illinois'},
+                'IN': {'name': 'Indiana'},
+                'KS': {'name': 'Kansas'},
+                'KY': {'name': 'Kentucky'},
+                'LA': {'name': 'Louisiana'},
+                'MA': {'name': 'Massachusetts'},
+                'MD': {'name': 'Maryland'},
+                'ME': {'name': 'Maine'},
+                'MI': {'name': 'Michigan'},
+                'MN': {'name': 'Minnesota'},
+                'MO': {'name': 'Missouri'},
+                'MP': {'name': 'Northern Mariana Islands'},
+                'MS': {'name': 'Mississippi'},
+                'MT': {'name': 'Montana'},
+                'NC': {'name': 'North Carolina'},
+                'ND': {'name': 'North Dakota'},
+                'NE': {'name': 'Nebraska'},
+                'NH': {'name': 'New Hampshire'},
+                'NJ': {'name': 'New Jersey'},
+                'NM': {'name': 'New Mexico'},
+                'NV': {'name': 'Nevada'},
+                'NY': {'name': 'New York'},
+                'OH': {'name': 'Ohio'},
+                'OK': {'name': 'Oklahoma'},
+                'OR': {'name': 'Oregon'},
+                'PA': {'name': 'Pennsylvania'},
+                'PR': {'name': 'Puerto Rico'},
+                'RI': {'name': 'Rhode Island'},
+                'SC': {'name': 'South Carolina'},
+                'SD': {'name': 'South Dakota'},
+                'TN': {'name': 'Tennessee'},
+                'TX': {'name': 'Texas'},
+                'UM': {'name': 'United States Minor Outlying Islands'},
+                'UT': {'name': 'Utah'},
+                'VA': {'name': 'Virginia'},
+                'VI': {'name': 'Virgin Islands, U.S.'},
+                'VT': {'name': 'Vermont'},
+                'WA': {'name': 'Washington'},
+                'WI': {'name': 'Wisconsin'},
+                'WV': {'name': 'West Virginia'},
+                'WY': {'name': 'Wyoming'},
+            },
+        },
+        'VC': {'name': 'Saint Vincent and the Grenadines'},
+        'VG': {'name': 'Virgin Islands, British'},
+        'VI': {'name': 'Virgin Islands, U.S.'},
+    },
+    'OC': {
+        'AS': {'name': 'American Samoa'},
+        'AU': {'name': 'Australia'},
+        'CK': {'name': 'Cook Islands'},
+        'FJ': {'name': 'Fiji'},
+        'FM': {'name': 'Micronesia, Federated States of'},
+        'GU': {'name': 'Guam'},
+        'KI': {'name': 'Kiribati'},
+        'MH': {'name': 'Marshall Islands'},
+        'MP': {'name': 'Northern Mariana Islands'},
+        'NC': {'name': 'New Caledonia'},
+        'NF': {'name': 'Norfolk Island'},
+        'NR': {'name': 'Nauru'},
+        'NU': {'name': 'Niue'},
+        'NZ': {'name': 'New Zealand'},
+        'PF': {'name': 'French Polynesia'},
+        'PG': {'name': 'Papua New Guinea'},
+        'PN': {'name': 'Pitcairn'},
+        'PW': {'name': 'Palau'},
+        'SB': {'name': 'Solomon Islands'},
+        'TK': {'name': 'Tokelau'},
+        'TO': {'name': 'Tonga'},
+        'TV': {'name': 'Tuvalu'},
+        'UM': {'name': 'United States Minor Outlying Islands'},
+        'VU': {'name': 'Vanuatu'},
+        'WF': {'name': 'Wallis and Futuna'},
+        'WS': {'name': 'Samoa'},
+    },
+    'SA': {
+        'AR': {'name': 'Argentina'},
+        'BO': {'name': 'Bolivia, Plurinational State of'},
+        'BR': {'name': 'Brazil'},
+        'CL': {'name': 'Chile'},
+        'CO': {'name': 'Colombia'},
+        'EC': {'name': 'Ecuador'},
+        'FK': {'name': 'Falkland Islands (Malvinas)'},
+        'GF': {'name': 'French Guiana'},
+        'GS': {'name': 'South Georgia and the South Sandwich Islands'},
+        'GY': {'name': 'Guyana'},
+        'PE': {'name': 'Peru'},
+        'PY': {'name': 'Paraguay'},
+        'SR': {'name': 'Suriname'},
+        'UY': {'name': 'Uruguay'},
+        'VE': {'name': 'Venezuela, Bolivarian Republic of'},
+    },
+}
```

### Comparing `octodns-0.9.9/octodns/source/tinydns.py` & `octodns-1.0.0rc0/octodns/source/tinydns.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,154 +1,143 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
+import logging
+import re
+import textwrap
 from collections import defaultdict
 from ipaddress import ip_address
 from os import listdir
 from os.path import join
-import logging
-import re
-import textwrap
 
 from ..record import Record
 from ..zone import DuplicateRecordException, SubzoneRecordException
 from .base import BaseSource
 
 
 class TinyDnsBaseSource(BaseSource):
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = False
     SUPPORTS = set(('A', 'CNAME', 'MX', 'NS', 'TXT', 'AAAA'))
 
     split_re = re.compile(r':+')
 
     def __init__(self, id, default_ttl=3600):
-        super(TinyDnsBaseSource, self).__init__(id)
+        super().__init__(id)
         self.default_ttl = default_ttl
 
     def _data_for_A(self, _type, records):
         values = []
         for record in records:
             if record[0] != '0.0.0.0':
                 values.append(record[0])
         if len(values) == 0:
             return
         try:
             ttl = records[0][1]
         except IndexError:
             ttl = self.default_ttl
-        return {
-            'ttl': ttl,
-            'type': _type,
-            'values': values,
-        }
+        return {'ttl': ttl, 'type': _type, 'values': values}
 
     def _data_for_AAAA(self, _type, records):
         values = []
         for record in records:
             # TinyDNS files have the ipv6 address written in full, but with the
             # colons removed. This inserts a colon every 4th character to make
             # the address correct.
             values.append(u":".join(textwrap.wrap(record[0], 4)))
         try:
             ttl = records[0][1]
         except IndexError:
             ttl = self.default_ttl
-        return {
-            'ttl': ttl,
-            'type': _type,
-            'values': values,
-        }
+        return {'ttl': ttl, 'type': _type, 'values': values}
 
     def _data_for_TXT(self, _type, records):
         values = []
 
         for record in records:
-            new_value = record[0].encode('latin1').decode('unicode-escape') \
+            new_value = (
+                record[0]
+                .encode('latin1')
+                .decode('unicode-escape')
                 .replace(";", "\\;")
+            )
             values.append(new_value)
 
         try:
             ttl = records[0][1]
         except IndexError:
             ttl = self.default_ttl
-        return {
-            'ttl': ttl,
-            'type': _type,
-            'values': values,
-        }
+        return {'ttl': ttl, 'type': _type, 'values': values}
 
     def _data_for_CNAME(self, _type, records):
         first = records[0]
         try:
             ttl = first[1]
         except IndexError:
             ttl = self.default_ttl
-        return {
-            'ttl': ttl,
-            'type': _type,
-            'value': '{}.'.format(first[0])
-        }
+        return {'ttl': ttl, 'type': _type, 'value': f'{first[0]}.'}
 
     def _data_for_MX(self, _type, records):
         try:
             ttl = records[0][2]
         except IndexError:
             ttl = self.default_ttl
         return {
             'ttl': ttl,
             'type': _type,
-            'values': [{
-                'preference': r[1],
-                'exchange': '{}.'.format(r[0])
-            } for r in records]
+            'values': [
+                {'preference': r[1], 'exchange': f'{r[0]}.'} for r in records
+            ],
         }
 
     def _data_for_NS(self, _type, records):
         try:
             ttl = records[0][1]
         except IndexError:
             ttl = self.default_ttl
         return {
             'ttl': ttl,
             'type': _type,
-            'values': ['{}.'.format(r[0]) for r in records]
+            'values': [f'{r[0]}.' for r in records],
         }
 
     def populate(self, zone, target=False, lenient=False):
-        self.log.debug('populate: name=%s, target=%s, lenient=%s', zone.name,
-                       target, lenient)
+        self.log.debug(
+            'populate: name=%s, target=%s, lenient=%s',
+            zone.name,
+            target,
+            lenient,
+        )
 
         before = len(zone.records)
 
         if zone.name.endswith('in-addr.arpa.'):
             self._populate_in_addr_arpa(zone, lenient)
         else:
             self._populate_normal(zone, lenient)
 
-        self.log.info('populate:   found %s records',
-                      len(zone.records) - before)
+        self.log.info(
+            'populate:   found %s records', len(zone.records) - before
+        )
 
     def _populate_normal(self, zone, lenient):
         type_map = {
             '=': 'A',
             '^': None,
             '.': 'NS',
             'C': 'CNAME',
             '+': 'A',
             '@': 'MX',
             '\'': 'TXT',
             '3': 'AAAA',
             '6': 'AAAA',
         }
-        name_re = re.compile(r'((?P<name>.+)\.)?{}$'.format(zone.name[:-1]))
+        name_re = re.compile(fr'((?P<name>.+)\.)?{zone.name[:-1]}$')
 
         data = defaultdict(lambda: defaultdict(list))
         for line in self._lines():
             _type = line[0]
             if _type not in type_map:
                 # Something we don't care about
                 continue
@@ -164,27 +153,30 @@
             if not match:
                 continue
             name = zone.hostname_from_fqdn(line[0])
             data[name][_type].append(line[1:])
 
         for name, types in data.items():
             for _type, d in types.items():
-                data_for = getattr(self, '_data_for_{}'.format(_type))
+                data_for = getattr(self, f'_data_for_{_type}')
                 data = data_for(_type, d)
                 if data:
-                    record = Record.new(zone, name, data, source=self,
-                                        lenient=lenient)
+                    record = Record.new(
+                        zone, name, data, source=self, lenient=lenient
+                    )
                     try:
                         zone.add_record(record, lenient=lenient)
                     except SubzoneRecordException:
-                        self.log.debug('_populate_normal: skipping subzone '
-                                       'record=%s', record)
+                        self.log.debug(
+                            '_populate_normal: skipping subzone record=%s',
+                            record,
+                        )
 
     def _populate_in_addr_arpa(self, zone, lenient):
-        name_re = re.compile(r'(?P<name>.+)\.{}$'.format(zone.name[:-1]))
+        name_re = re.compile(fr'(?P<name>.+)\.{zone.name[:-1]}$')
 
         for line in self._lines():
             _type = line[0]
             # We're only interested in = (A+PTR), and ^ (PTR) records
             if _type not in ('=', '^'):
                 continue
 
@@ -192,37 +184,40 @@
             line = line[1:].split('#', 1)[0]
             # Split on :'s including :: and strip leading/trailing ws
             line = [p.strip() for p in self.split_re.split(line)]
 
             if line[0].endswith('in-addr.arpa'):
                 # since it's already in in-addr.arpa format
                 match = name_re.match(line[0])
-                value = '{}.'.format(line[1])
+                value = f'{line[1]}.'
             else:
                 addr = ip_address(line[1])
                 match = name_re.match(addr.reverse_pointer)
-                value = '{}.'.format(line[0])
+                value = f'{line[0]}.'
 
             if match:
                 try:
                     ttl = line[2]
                 except IndexError:
                     ttl = self.default_ttl
 
                 name = match.group('name')
-                record = Record.new(zone, name, {
-                    'ttl': ttl,
-                    'type': 'PTR',
-                    'value': value
-                }, source=self, lenient=lenient)
+                record = Record.new(
+                    zone,
+                    name,
+                    {'ttl': ttl, 'type': 'PTR', 'value': value},
+                    source=self,
+                    lenient=lenient,
+                )
                 try:
                     zone.add_record(record, lenient=lenient)
                 except DuplicateRecordException:
-                    self.log.warn('Duplicate PTR record for {}, '
-                                  'skipping'.format(addr))
+                    self.log.warning(
+                        f'Duplicate PTR record for {addr}, skipping'
+                    )
 
 
 class TinyDnsFileSource(TinyDnsBaseSource):
     '''
     A basic TinyDNS zonefile importer created to import legacy data.
 
     tinydns:
@@ -231,19 +226,24 @@
         directory: ./zones
         # The ttl to use for records when not specified in the data
         # (optional, default 3600)
         default_ttl: 3600
 
     NOTE: timestamps & lo fields are ignored if present.
     '''
+
     def __init__(self, id, directory, default_ttl=3600):
-        self.log = logging.getLogger('TinyDnsFileSource[{}]'.format(id))
-        self.log.debug('__init__: id=%s, directory=%s, default_ttl=%d', id,
-                       directory, default_ttl)
-        super(TinyDnsFileSource, self).__init__(id, default_ttl)
+        self.log = logging.getLogger(f'TinyDnsFileSource[{id}]')
+        self.log.debug(
+            '__init__: id=%s, directory=%s, default_ttl=%d',
+            id,
+            directory,
+            default_ttl,
+        )
+        super().__init__(id, default_ttl)
         self.directory = directory
         self._cache = None
 
     def _lines(self):
         if self._cache is None:
             # We unfortunately don't know where to look since tinydns stuff can
             # be defined anywhere so we'll just read all files
```

### Comparing `octodns-0.9.9/octodns/source/base.py` & `octodns-1.0.0rc0/octodns/source/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
 
 class BaseSource(object):
 
+    SUPPORTS_MULTIVALUE_PTR = False
+    SUPPORTS_POOL_VALUE_STATUS = False
+    SUPPORTS_ROOT_NS = False
+    SUPPORTS_DYNAMIC_SUBNETS = False
+
     def __init__(self, id):
         self.id = id
         if not getattr(self, 'log', False):
-            raise NotImplementedError('Abstract base class, log property '
-                                      'missing')
+            raise NotImplementedError(
+                'Abstract base class, log property missing'
+            )
         if not hasattr(self, 'SUPPORTS_GEO'):
-            raise NotImplementedError('Abstract base class, SUPPORTS_GEO '
-                                      'property missing')
+            raise NotImplementedError(
+                'Abstract base class, SUPPORTS_GEO property missing'
+            )
         if not hasattr(self, 'SUPPORTS'):
-            raise NotImplementedError('Abstract base class, SUPPORTS '
-                                      'property missing')
+            raise NotImplementedError(
+                'Abstract base class, SUPPORTS property missing'
+            )
 
     @property
     def SUPPORTS_DYNAMIC(self):
         return False
 
     def populate(self, zone, target=False, lenient=False):
         '''
@@ -30,20 +35,21 @@
 
         When `target` is True the populate call is being made to load the
         current state of the provider.
 
         When `lenient` is True the populate call may skip record validation and
         do a "best effort" load of data. That will allow through some common,
         but not best practices stuff that we otherwise would reject. E.g. no
-        trailing . or mising escapes for ;.
+        trailing . or missing escapes for ;.
 
         When target is True (loading current state) this method should return
         True if the zone exists or False if it does not.
         '''
-        raise NotImplementedError('Abstract base class, populate method '
-                                  'missing')
+        raise NotImplementedError(
+            'Abstract base class, populate method missing'
+        )
 
     def supports(self, record):
         return record._type in self.SUPPORTS
 
     def __repr__(self):
         return self.__class__.__name__
```

### Comparing `octodns-0.9.9/octodns/provider/plan.py` & `octodns-1.0.0rc0/octodns/provider/plan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,188 +1,231 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
+from io import StringIO
 from logging import DEBUG, ERROR, INFO, WARN, getLogger
 from sys import stdout
 
-from six import StringIO, text_type
-
 
 class UnsafePlan(Exception):
     pass
 
 
+class RootNsChange(UnsafePlan):
+    def __init__(self):
+        super().__init__('Root NS record change, force required')
+
+
+class TooMuchChange(UnsafePlan):
+    def __init__(
+        self, why, update_pcent, update_threshold, change_count, existing_count
+    ):
+        msg = (
+            f'{why}, {update_pcent:.2f}% is over {update_threshold:.2f}% '
+            f'({change_count}/{existing_count}), force required'
+        )
+        super().__init__(msg)
+
+
 class Plan(object):
     log = getLogger('Plan')
 
-    MAX_SAFE_UPDATE_PCENT = .3
-    MAX_SAFE_DELETE_PCENT = .3
+    MAX_SAFE_UPDATE_PCENT = 0.3
+    MAX_SAFE_DELETE_PCENT = 0.3
     MIN_EXISTING_RECORDS = 10
 
-    def __init__(self, existing, desired, changes, exists,
-                 update_pcent_threshold=MAX_SAFE_UPDATE_PCENT,
-                 delete_pcent_threshold=MAX_SAFE_DELETE_PCENT):
+    def __init__(
+        self,
+        existing,
+        desired,
+        changes,
+        exists,
+        update_pcent_threshold=MAX_SAFE_UPDATE_PCENT,
+        delete_pcent_threshold=MAX_SAFE_DELETE_PCENT,
+    ):
         self.existing = existing
         self.desired = desired
         # Sort changes to ensure we always have a consistent ordering for
         # things that make assumptions about that. Many providers will do their
         # own ordering to ensure things happen in a way that makes sense to
         # them and/or is as safe as possible.
         self.changes = sorted(changes)
         self.exists = exists
         self.update_pcent_threshold = update_pcent_threshold
         self.delete_pcent_threshold = delete_pcent_threshold
 
-        change_counts = {
-            'Create': 0,
-            'Delete': 0,
-            'Update': 0
-        }
+        change_counts = {'Create': 0, 'Delete': 0, 'Update': 0}
         for change in changes:
             change_counts[change.__class__.__name__] += 1
         self.change_counts = change_counts
 
         try:
             existing_n = len(self.existing.records)
         except AttributeError:
             existing_n = 0
 
-        self.log.debug('__init__: Creates=%d, Updates=%d, Deletes=%d'
-                       'Existing=%d',
-                       self.change_counts['Create'],
-                       self.change_counts['Update'],
-                       self.change_counts['Delete'], existing_n)
+        self.log.debug(
+            '__init__: Creates=%d, Updates=%d, Deletes=%d Existing=%d',
+            self.change_counts['Create'],
+            self.change_counts['Update'],
+            self.change_counts['Delete'],
+            existing_n,
+        )
 
     def raise_if_unsafe(self):
         # TODO: what is safe really?
-        if self.existing and \
-           len(self.existing.records) >= self.MIN_EXISTING_RECORDS:
+        if (
+            self.existing
+            and len(self.existing.records) >= self.MIN_EXISTING_RECORDS
+        ):
 
             existing_record_count = len(self.existing.records)
-            update_pcent = self.change_counts['Update'] / existing_record_count
-            delete_pcent = self.change_counts['Delete'] / existing_record_count
+            if existing_record_count > 0:
+                update_pcent = (
+                    self.change_counts['Update'] / existing_record_count
+                )
+                delete_pcent = (
+                    self.change_counts['Delete'] / existing_record_count
+                )
+            else:
+                update_pcent = 0
+                delete_pcent = 0
 
             if update_pcent > self.update_pcent_threshold:
-                raise UnsafePlan('Too many updates, {:.2f} is over {:.2f} %'
-                                 '({}/{})'.format(
-                                     update_pcent * 100,
-                                     self.update_pcent_threshold * 100,
-                                     self.change_counts['Update'],
-                                     existing_record_count))
+                raise TooMuchChange(
+                    'Too many updates',
+                    update_pcent * 100,
+                    self.update_pcent_threshold * 100,
+                    self.change_counts['Update'],
+                    existing_record_count,
+                )
             if delete_pcent > self.delete_pcent_threshold:
-                raise UnsafePlan('Too many deletes, {:.2f} is over {:.2f} %'
-                                 '({}/{})'.format(
-                                     delete_pcent * 100,
-                                     self.delete_pcent_threshold * 100,
-                                     self.change_counts['Delete'],
-                                     existing_record_count))
+                raise TooMuchChange(
+                    'Too many deletes',
+                    delete_pcent * 100,
+                    self.delete_pcent_threshold * 100,
+                    self.change_counts['Delete'],
+                    existing_record_count,
+                )
+
+        # If we have any changes of the root NS record for the zone it's a huge
+        # deal and force should always be required for extra care
+        if self.exists and any(
+            c
+            for c in self.changes
+            if c.record and c.record._type == 'NS' and c.record.name == ''
+        ):
+            raise RootNsChange()
 
     def __repr__(self):
-        return 'Creates={}, Updates={}, Deletes={}, Existing Records={}' \
-            .format(self.change_counts['Create'], self.change_counts['Update'],
-                    self.change_counts['Delete'],
-                    len(self.existing.records))
+        creates = self.change_counts['Create']
+        updates = self.change_counts['Update']
+        deletes = self.change_counts['Delete']
+        existing = len(self.existing.records)
+        return (
+            f'Creates={creates}, Updates={updates}, Deletes={deletes}, '
+            f'Existing Records={existing}'
+        )
 
 
 class _PlanOutput(object):
-
     def __init__(self, name):
         self.name = name
 
 
 class PlanLogger(_PlanOutput):
-
     def __init__(self, name, level='info'):
-        super(PlanLogger, self).__init__(name)
+        super().__init__(name)
         try:
             self.level = {
                 'debug': DEBUG,
                 'info': INFO,
                 'warn': WARN,
                 'warning': WARN,
-                'error': ERROR
+                'error': ERROR,
             }[level.lower()]
         except (AttributeError, KeyError):
-            raise Exception('Unsupported level: {}'.format(level))
+            raise Exception(f'Unsupported level: {level}')
 
     def run(self, log, plans, *args, **kwargs):
-        hr = '*************************************************************' \
+        hr = (
+            '*************************************************************'
             '*******************\n'
+        )
         buf = StringIO()
         buf.write('\n')
         if plans:
             current_zone = None
             for target, plan in plans:
-                if plan.desired.name != current_zone:
-                    current_zone = plan.desired.name
+                if plan.desired.decoded_name != current_zone:
+                    current_zone = plan.desired.decoded_name
                     buf.write(hr)
                     buf.write('* ')
                     buf.write(current_zone)
                     buf.write('\n')
                     buf.write(hr)
 
                 buf.write('* ')
                 buf.write(target.id)
                 buf.write(' (')
-                buf.write(text_type(target))
+                buf.write(str(target))
                 buf.write(')\n*   ')
 
                 if plan.exists is False:
                     buf.write('Create ')
                     buf.write(str(plan.desired))
                     buf.write('\n*   ')
 
                 for change in plan.changes:
                     buf.write(change.__repr__(leader='* '))
                     buf.write('\n*   ')
 
                 buf.write('Summary: ')
-                buf.write(text_type(plan))
+                buf.write(str(plan))
                 buf.write('\n')
         else:
             buf.write(hr)
             buf.write('No changes were planned\n')
         buf.write(hr)
         buf.write('\n')
+
         log.log(self.level, buf.getvalue())
 
 
 def _value_stringifier(record, sep):
     try:
-        values = [text_type(v) for v in record.values]
+        values = [str(v) for v in record.values]
     except AttributeError:
         values = [record.value]
     for code, gv in sorted(getattr(record, 'geo', {}).items()):
-        vs = ', '.join([text_type(v) for v in gv.values])
-        values.append('{}: {}'.format(code, vs))
+        vs = ', '.join([str(v) for v in gv.values])
+        values.append(f'{code}: {vs}')
     return sep.join(values)
 
 
 class PlanMarkdown(_PlanOutput):
-
     def run(self, plans, fh=stdout, *args, **kwargs):
         if plans:
             current_zone = None
             for target, plan in plans:
-                if plan.desired.name != current_zone:
-                    current_zone = plan.desired.name
+                if plan.desired.decoded_name != current_zone:
+                    current_zone = plan.desired.decoded_name
                     fh.write('## ')
                     fh.write(current_zone)
                     fh.write('\n\n')
 
                 fh.write('### ')
                 fh.write(target.id)
                 fh.write('\n\n')
 
-                fh.write('| Operation | Name | Type | TTL | Value | Source |\n'
-                         '|--|--|--|--|--|--|\n')
+                fh.write(
+                    '| Operation | Name | Type | TTL | Value | Source |\n'
+                    '|--|--|--|--|--|--|\n'
+                )
 
                 if plan.exists is False:
                     fh.write('| Create | ')
                     fh.write(str(plan.desired))
                     fh.write(' | | | | |\n')
 
                 for change in plan.changes:
@@ -194,62 +237,63 @@
                     fh.write(' | ')
                     fh.write(record.name)
                     fh.write(' | ')
                     fh.write(record._type)
                     fh.write(' | ')
                     # TTL
                     if existing:
-                        fh.write(text_type(existing.ttl))
+                        fh.write(str(existing.ttl))
                         fh.write(' | ')
                         fh.write(_value_stringifier(existing, '; '))
                         fh.write(' | |\n')
                         if new:
                             fh.write('| | | | ')
 
                     if new:
-                        fh.write(text_type(new.ttl))
+                        fh.write(str(new.ttl))
                         fh.write(' | ')
                         fh.write(_value_stringifier(new, '; '))
                         fh.write(' | ')
                         if new.source:
                             fh.write(new.source.id)
                         fh.write(' |\n')
 
                 fh.write('\nSummary: ')
-                fh.write(text_type(plan))
+                fh.write(str(plan))
                 fh.write('\n\n')
         else:
             fh.write('## No changes were planned\n')
 
 
 class PlanHtml(_PlanOutput):
-
     def run(self, plans, fh=stdout, *args, **kwargs):
         if plans:
             current_zone = None
             for target, plan in plans:
-                if plan.desired.name != current_zone:
-                    current_zone = plan.desired.name
+                if plan.desired.decoded_name != current_zone:
+                    current_zone = plan.desired.decoded_name
                     fh.write('<h2>')
                     fh.write(current_zone)
                     fh.write('</h2>\n')
 
                 fh.write('<h3>')
                 fh.write(target.id)
-                fh.write('''</h3>
+                fh.write(
+                    '''</h3>
 <table>
   <tr>
     <th>Operation</th>
     <th>Name</th>
     <th>Type</th>
     <th>TTL</th>
     <th>Value</th>
     <th>Source</th>
   </tr>
-''')
+'''
+                )
 
                 if plan.exists is False:
                     fh.write('  <tr>\n    <td>Create</td>\n    <td colspan=5>')
                     fh.write(str(plan.desired))
                     fh.write('</td>\n  </tr>\n')
 
                 for change in plan.changes:
@@ -262,29 +306,29 @@
                     fh.write(record.name)
                     fh.write('</td>\n    <td>')
                     fh.write(record._type)
                     fh.write('</td>\n')
                     # TTL
                     if existing:
                         fh.write('    <td>')
-                        fh.write(text_type(existing.ttl))
+                        fh.write(str(existing.ttl))
                         fh.write('</td>\n    <td>')
                         fh.write(_value_stringifier(existing, '<br/>'))
                         fh.write('</td>\n    <td></td>\n  </tr>\n')
                         if new:
                             fh.write('  <tr>\n    <td colspan=3></td>\n')
 
                     if new:
                         fh.write('    <td>')
-                        fh.write(text_type(new.ttl))
+                        fh.write(str(new.ttl))
                         fh.write('</td>\n    <td>')
                         fh.write(_value_stringifier(new, '<br/>'))
                         fh.write('</td>\n    <td>')
                         if new.source:
                             fh.write(new.source.id)
                         fh.write('</td>\n  </tr>\n')
 
                 fh.write('  <tr>\n    <td colspan=6>Summary: ')
-                fh.write(text_type(plan))
+                fh.write(str(plan))
                 fh.write('</td>\n  </tr>\n</table>\n')
         else:
             fh.write('<b>No changes were planned</b>')
```

### Comparing `octodns-0.9.9/octodns/provider/transip.py` & `octodns-1.0.0rc0/octodns/record/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,353 +1,340 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
-from suds import WebFault
-
 from collections import defaultdict
-from .base import BaseProvider
 from logging import getLogger
-from ..record import Record
-from transip.service.domain import DomainService
-from transip.service.objects import DnsEntry
-
-
-class TransipException(Exception):
-    pass
-
-
-class TransipConfigException(TransipException):
-    pass
-
-
-class TransipNewZoneException(TransipException):
-    pass
-
-
-class TransipProvider(BaseProvider):
-    '''
-    Transip DNS provider
-
-    transip:
-        class: octodns.provider.transip.TransipProvider
-        # Your Transip account name (required)
-        account: yourname
-        # Path to a private key file (required if key is not used)
-        key_file: /path/to/file
-        # The api key as string (required if key_file is not used)
-        key: |
-            \'''
-            -----BEGIN PRIVATE KEY-----
-            ...
-            -----END PRIVATE KEY-----
-            \'''
-        # if both `key_file` and `key` are presented `key_file` is used
-
-    '''
-    SUPPORTS_GEO = False
-    SUPPORTS_DYNAMIC = False
-    SUPPORTS = set(
-        ('A', 'AAAA', 'CNAME', 'MX', 'SRV', 'SPF', 'TXT', 'SSHFP', 'CAA'))
-    # unsupported by OctoDNS: 'TLSA'
-    MIN_TTL = 120
-    TIMEOUT = 15
-    ROOT_RECORD = '@'
-
-    def __init__(self, id, account, key=None, key_file=None,  *args, **kwargs):
-        self.log = getLogger('TransipProvider[{}]'.format(id))
-        self.log.debug('__init__: id=%s, account=%s, token=***', id,
-                       account)
-        super(TransipProvider, self).__init__(id, *args, **kwargs)
-
-        if key_file is not None:
-            self._client = DomainService(account, private_key_file=key_file)
-        elif key is not None:
-            self._client = DomainService(account, private_key=key)
-        else:
-            raise TransipConfigException(
-                'Missing `key` of `key_file` parameter in config'
-            )
-
-        self.account = account
-        self.key = key
 
-        self._currentZone = {}
-
-    def populate(self, zone, target=False, lenient=False):
-
-        exists = False
-        self._currentZone = zone
-        self.log.debug('populate: name=%s, target=%s, lenient=%s', zone.name,
-                       target, lenient)
-
-        before = len(zone.records)
+from ..equality import EqualityTupleMixin
+from ..idna import IdnaError, idna_decode, idna_encode
+from .change import Update
+from .exception import RecordException, ValidationError
+
+
+class Record(EqualityTupleMixin):
+    log = getLogger('Record')
+
+    _CLASSES = {}
+
+    @classmethod
+    def register_type(cls, _class, _type=None):
+        if _type is None:
+            _type = _class._type
+        existing = cls._CLASSES.get(_type)
+        if existing:
+            module = existing.__module__
+            name = existing.__name__
+            msg = f'Type "{_type}" already registered by {module}.{name}'
+            raise RecordException(msg)
+        cls._CLASSES[_type] = _class
+
+    @classmethod
+    def registered_types(cls):
+        return cls._CLASSES
+
+    @classmethod
+    def new(cls, zone, name, data, source=None, lenient=False):
+        reasons = []
+        try:
+            name = idna_encode(str(name))
+        except IdnaError as e:
+            # convert the error into a reason
+            reasons.append(str(e))
+            name = str(name)
+        fqdn = f'{name}.{zone.name}' if name else zone.name
         try:
-            zoneInfo = self._client.get_info(zone.name[:-1])
-        except WebFault as e:
-            if e.fault.faultcode == '102' and target is False:
-                # Zone not found in account, and not a target so just
-                # leave an empty zone.
-                return exists
-            elif e.fault.faultcode == '102' and target is True:
-                self.log.warning('populate: Transip can\'t create new zones')
-                raise TransipNewZoneException(
-                    ('populate: ({}) Transip used ' +
-                     'as target for non-existing zone: {}').format(
-                        e.fault.faultcode, zone.name))
+            _type = data['type']
+        except KeyError:
+            raise Exception(f'Invalid record {idna_decode(fqdn)}, missing type')
+        try:
+            _class = cls._CLASSES[_type]
+        except KeyError:
+            raise Exception(f'Unknown record type: "{_type}"')
+        reasons.extend(_class.validate(name, fqdn, data))
+        try:
+            lenient |= data['octodns']['lenient']
+        except KeyError:
+            pass
+        if reasons:
+            if lenient:
+                cls.log.warning(ValidationError.build_message(fqdn, reasons))
             else:
-                self.log.error('populate: (%s) %s ', e.fault.faultcode,
-                               e.fault.faultstring)
-                raise e
-
-        self.log.debug('populate: found %s records for zone %s',
-                       len(zoneInfo.dnsEntries), zone.name)
-        exists = True
-        if zoneInfo.dnsEntries:
-            values = defaultdict(lambda: defaultdict(list))
-            for record in zoneInfo.dnsEntries:
-                name = zone.hostname_from_fqdn(record['name'])
-                if name == self.ROOT_RECORD:
-                    name = ''
-
-                if record['type'] in self.SUPPORTS:
-                    values[name][record['type']].append(record)
-
-            for name, types in values.items():
-                for _type, records in types.items():
-                    data_for = getattr(self, '_data_for_{}'.format(_type))
-                    record = Record.new(zone, name, data_for(_type, records),
-                                        source=self, lenient=lenient)
-                    zone.add_record(record, lenient=lenient)
-        self.log.info('populate:   found %s records, exists = %s',
-                      len(zone.records) - before, exists)
-
-        self._currentZone = {}
-        return exists
-
-    def _apply(self, plan):
-        desired = plan.desired
-        changes = plan.changes
-        self.log.debug('apply: zone=%s, changes=%d', desired.name,
-                       len(changes))
+                raise ValidationError(fqdn, reasons)
+        return _class(zone, name, data, source=source)
 
-        self._currentZone = plan.desired
+    @classmethod
+    def validate(cls, name, fqdn, data):
+        reasons = []
+        if name == '@':
+            reasons.append('invalid name "@", use "" instead')
+        n = len(fqdn)
+        if n > 253:
+            reasons.append(
+                f'invalid fqdn, "{idna_decode(fqdn)}" is too long at {n} '
+                'chars, max is 253'
+            )
+        for label in name.split('.'):
+            n = len(label)
+            if n > 63:
+                reasons.append(
+                    f'invalid label, "{label}" is too long at {n}'
+                    ' chars, max is 63'
+                )
+        # TODO: look at the idna lib for a lot more potential validations...
         try:
-            self._client.get_info(plan.desired.name[:-1])
-        except WebFault as e:
-            self.log.exception('_apply: get_info failed')
-            raise e
-
-        _dns_entries = []
-        for record in plan.desired.records:
-            if record._type in self.SUPPORTS:
-                entries_for = getattr(self,
-                                      '_entries_for_{}'.format(record._type))
-
-                # Root records have '@' as name
-                name = record.name
-                if name == '':
-                    name = self.ROOT_RECORD
-
-                _dns_entries.extend(entries_for(name, record))
-
+            ttl = int(data['ttl'])
+            if ttl < 0:
+                reasons.append('invalid ttl')
+        except KeyError:
+            reasons.append('missing ttl')
         try:
-            self._client.set_dns_entries(plan.desired.name[:-1], _dns_entries)
-        except WebFault as e:
-            self.log.warning(('_apply: Set DNS returned ' +
-                              'one or more errors: {}').format(
-                e.fault.faultstring))
-            raise TransipException(200, e.fault.faultstring)
-
-        self._currentZone = {}
-
-    def _entries_for_multiple(self, name, record):
-        _entries = []
-
-        for value in record.values:
-            _entries.append(DnsEntry(name, record.ttl, record._type, value))
-
-        return _entries
-
-    def _entries_for_single(self, name, record):
-
-        return [DnsEntry(name, record.ttl, record._type, record.value)]
-
-    _entries_for_A = _entries_for_multiple
-    _entries_for_AAAA = _entries_for_multiple
-    _entries_for_NS = _entries_for_multiple
-    _entries_for_SPF = _entries_for_multiple
-    _entries_for_CNAME = _entries_for_single
-
-    def _entries_for_MX(self, name, record):
-        _entries = []
-
-        for value in record.values:
-            content = "{} {}".format(value.preference, value.exchange)
-            _entries.append(DnsEntry(name, record.ttl, record._type, content))
-
-        return _entries
-
-    def _entries_for_SRV(self, name, record):
-        _entries = []
-
-        for value in record.values:
-            content = "{} {} {} {}".format(value.priority, value.weight,
-                                           value.port, value.target)
-            _entries.append(DnsEntry(name, record.ttl, record._type, content))
-
-        return _entries
-
-    def _entries_for_SSHFP(self, name, record):
-        _entries = []
-
-        for value in record.values:
-            content = "{} {} {}".format(value.algorithm,
-                                        value.fingerprint_type,
-                                        value.fingerprint)
-            _entries.append(DnsEntry(name, record.ttl, record._type, content))
-
-        return _entries
-
-    def _entries_for_CAA(self, name, record):
-        _entries = []
-
-        for value in record.values:
-            content = "{} {} {}".format(value.flags, value.tag,
-                                        value.value)
-            _entries.append(DnsEntry(name, record.ttl, record._type, content))
-
-        return _entries
-
-    def _entries_for_TXT(self, name, record):
-        _entries = []
-
-        for value in record.values:
-            value = value.replace('\\;', ';')
-            _entries.append(DnsEntry(name, record.ttl, record._type, value))
-
-        return _entries
-
-    def _parse_to_fqdn(self, value):
-
-        # Enforce switch from suds.sax.text.Text to string
-        value = str(value)
-
-        # TransIP allows '@' as value to alias the root record.
-        # this provider won't set an '@' value, but can be an existing record
-        if value == self.ROOT_RECORD:
-            value = self._currentZone.name
-
-        if value[-1] != '.':
-            self.log.debug('parseToFQDN: changed %s to %s', value,
-                           '{}.{}'.format(value, self._currentZone.name))
-            value = '{}.{}'.format(value, self._currentZone.name)
-
-        return value
-
-    def _get_lowest_ttl(self, records):
-        _ttl = 100000
-        for record in records:
-            _ttl = min(_ttl, record['expire'])
-        return _ttl
-
-    def _data_for_multiple(self, _type, records):
-
-        _values = []
-        for record in records:
-            # Enforce switch from suds.sax.text.Text to string
-            _values.append(str(record['content']))
-
-        return {
-            'ttl': self._get_lowest_ttl(records),
-            'type': _type,
-            'values': _values
-        }
-
-    _data_for_A = _data_for_multiple
-    _data_for_AAAA = _data_for_multiple
-    _data_for_NS = _data_for_multiple
-    _data_for_SPF = _data_for_multiple
-
-    def _data_for_CNAME(self, _type, records):
-        return {
-            'ttl': records[0]['expire'],
-            'type': _type,
-            'value': self._parse_to_fqdn(records[0]['content'])
-        }
-
-    def _data_for_MX(self, _type, records):
-        _values = []
-        for record in records:
-            preference, exchange = record['content'].split(" ", 1)
-            _values.append({
-                'preference': preference,
-                'exchange': self._parse_to_fqdn(exchange)
-            })
-        return {
-            'ttl': self._get_lowest_ttl(records),
-            'type': _type,
-            'values': _values
-        }
-
-    def _data_for_SRV(self, _type, records):
-        _values = []
-        for record in records:
-            priority, weight, port, target = record['content'].split(' ', 3)
-            _values.append({
-                'port': port,
-                'priority': priority,
-                'target': self._parse_to_fqdn(target),
-                'weight': weight
-            })
-
-        return {
-            'type': _type,
-            'ttl': self._get_lowest_ttl(records),
-            'values': _values
-        }
-
-    def _data_for_SSHFP(self, _type, records):
-        _values = []
-        for record in records:
-            algorithm, fp_type, fingerprint = record['content'].split(' ', 2)
-            _values.append({
-                'algorithm': algorithm,
-                'fingerprint': fingerprint.lower(),
-                'fingerprint_type': fp_type
-            })
+            if data['octodns']['healthcheck']['protocol'] not in (
+                'HTTP',
+                'HTTPS',
+                'TCP',
+            ):
+                reasons.append('invalid healthcheck protocol')
+        except KeyError:
+            pass
+        return reasons
+
+    @classmethod
+    def from_rrs(cls, zone, rrs, lenient=False):
+        # group records by name & type so that multiple rdatas can be combined
+        # into a single record when needed
+        grouped = defaultdict(list)
+        for rr in rrs:
+            grouped[(rr.name, rr._type)].append(rr)
+
+        records = []
+        # walk the grouped rrs converting each one to data and then create a
+        # record with that data
+        for _, rrs in sorted(grouped.items()):
+            rr = rrs[0]
+            name = zone.hostname_from_fqdn(rr.name)
+            _class = cls._CLASSES[rr._type]
+            data = _class.data_from_rrs(rrs)
+            record = Record.new(zone, name, data, lenient=lenient)
+            records.append(record)
+
+        return records
+
+    def __init__(self, zone, name, data, source=None):
+        self.zone = zone
+        if name:
+            # internally everything is idna
+            self.name = idna_encode(str(name))
+            # we'll keep a decoded version around for logs and errors
+            self.decoded_name = idna_decode(self.name)
+        else:
+            self.name = self.decoded_name = name
+        self.log.debug(
+            '__init__: zone.name=%s, type=%11s, name=%s',
+            zone.decoded_name,
+            self.__class__.__name__,
+            self.decoded_name,
+        )
+        self.source = source
+        self.ttl = int(data['ttl'])
+
+        self._octodns = data.get('octodns', {})
+
+    def _data(self):
+        return {'ttl': self.ttl}
+
+    @property
+    def data(self):
+        return self._data()
+
+    @property
+    def fqdn(self):
+        # TODO: these should be calculated and set in __init__ rather than on
+        # each use
+        if self.name:
+            return f'{self.name}.{self.zone.name}'
+        return self.zone.name
+
+    @property
+    def decoded_fqdn(self):
+        if self.decoded_name:
+            return f'{self.decoded_name}.{self.zone.decoded_name}'
+        return self.zone.decoded_name
+
+    @property
+    def ignored(self):
+        return self._octodns.get('ignored', False)
+
+    @property
+    def excluded(self):
+        return self._octodns.get('excluded', [])
+
+    @property
+    def included(self):
+        return self._octodns.get('included', [])
+
+    def healthcheck_host(self, value=None):
+        healthcheck = self._octodns.get('healthcheck', {})
+        if healthcheck.get('protocol', None) == 'TCP':
+            return None
+        return healthcheck.get('host', self.fqdn[:-1]) or value
+
+    @property
+    def healthcheck_path(self):
+        healthcheck = self._octodns.get('healthcheck', {})
+        if healthcheck.get('protocol', None) == 'TCP':
+            return None
+        try:
+            return healthcheck['path']
+        except KeyError:
+            return '/_dns'
 
-        return {
-            'type': _type,
-            'ttl': self._get_lowest_ttl(records),
-            'values': _values
-        }
+    @property
+    def healthcheck_protocol(self):
+        try:
+            return self._octodns['healthcheck']['protocol']
+        except KeyError:
+            return 'HTTPS'
 
-    def _data_for_CAA(self, _type, records):
-        _values = []
-        for record in records:
-            flags, tag, value = record['content'].split(' ', 2)
-            _values.append({
-                'flags': flags,
-                'tag': tag,
-                'value': value
-            })
+    @property
+    def healthcheck_port(self):
+        try:
+            return int(self._octodns['healthcheck']['port'])
+        except KeyError:
+            return 443
+
+    def changes(self, other, target):
+        # We're assuming we have the same name and type if we're being compared
+        if self.ttl != other.ttl:
+            return Update(self, other)
+
+    def copy(self, zone=None):
+        data = self.data
+        data['type'] = self._type
+        data['octodns'] = self._octodns
+
+        return Record.new(
+            zone if zone else self.zone,
+            self.name,
+            data,
+            self.source,
+            lenient=True,
+        )
+
+    # NOTE: we're using __hash__ and ordering methods that consider Records
+    # equivalent if they have the same name & _type. Values are ignored. This
+    # is useful when computing diffs/changes.
+
+    def __hash__(self):
+        return f'{self.name}:{self._type}'.__hash__()
+
+    def _equality_tuple(self):
+        return (self.name, self._type)
+
+    def __repr__(self):
+        # Make sure this is always overridden
+        raise NotImplementedError('Abstract base class, __repr__ required')
+
+
+class ValuesMixin(object):
+    @classmethod
+    def validate(cls, name, fqdn, data):
+        reasons = super().validate(name, fqdn, data)
+
+        values = data.get('values', data.get('value', []))
+
+        reasons.extend(cls._value_type.validate(values, cls._type))
+
+        return reasons
+
+    @classmethod
+    def data_from_rrs(cls, rrs):
+        # type and TTL come from the first rr
+        rr = rrs[0]
+        # values come from parsing the rdata portion of all rrs
+        values = [cls._value_type.parse_rdata_text(rr.rdata) for rr in rrs]
+        return {'ttl': rr.ttl, 'type': rr._type, 'values': values}
 
+    def __init__(self, zone, name, data, source=None):
+        super().__init__(zone, name, data, source=source)
+        try:
+            values = data['values']
+        except KeyError:
+            values = [data['value']]
+        self.values = sorted(self._value_type.process(values))
+
+    def changes(self, other, target):
+        if self.values != other.values:
+            return Update(self, other)
+        return super().changes(other, target)
+
+    def _data(self):
+        ret = super()._data()
+        if len(self.values) > 1:
+            values = [getattr(v, 'data', v) for v in self.values if v]
+            if len(values) > 1:
+                ret['values'] = values
+            elif len(values) == 1:
+                ret['value'] = values[0]
+        elif len(self.values) == 1:
+            v = self.values[0]
+            if v:
+                ret['value'] = getattr(v, 'data', v)
+
+        return ret
+
+    @property
+    def rrs(self):
+        return (
+            self.fqdn,
+            self.ttl,
+            self._type,
+            [v.rdata_text for v in self.values],
+        )
+
+    def __repr__(self):
+        values = "', '".join([str(v) for v in self.values])
+        klass = self.__class__.__name__
+        return f"<{klass} {self._type} {self.ttl}, {self.decoded_fqdn}, ['{values}']>"
+
+
+class ValueMixin(object):
+    @classmethod
+    def validate(cls, name, fqdn, data):
+        reasons = super().validate(name, fqdn, data)
+        reasons.extend(
+            cls._value_type.validate(data.get('value', None), cls._type)
+        )
+        return reasons
+
+    @classmethod
+    def data_from_rrs(cls, rrs):
+        # single value, so single rr only...
+        rr = rrs[0]
         return {
-            'type': _type,
-            'ttl': self._get_lowest_ttl(records),
-            'values': _values
+            'ttl': rr.ttl,
+            'type': rr._type,
+            'value': cls._value_type.parse_rdata_text(rr.rdata),
         }
 
-    def _data_for_TXT(self, _type, records):
-        _values = []
-        for record in records:
-            _values.append(record['content'].replace(';', '\\;'))
-
-        return {
-            'type': _type,
-            'ttl': self._get_lowest_ttl(records),
-            'values': _values
-        }
+    def __init__(self, zone, name, data, source=None):
+        super().__init__(zone, name, data, source=source)
+        self.value = self._value_type.process(data['value'])
+
+    def changes(self, other, target):
+        if self.value != other.value:
+            return Update(self, other)
+        return super().changes(other, target)
+
+    def _data(self):
+        ret = super()._data()
+        if self.value:
+            ret['value'] = getattr(self.value, 'data', self.value)
+        return ret
+
+    @property
+    def rrs(self):
+        return self.fqdn, self.ttl, self._type, [self.value.rdata_text]
+
+    def __repr__(self):
+        klass = self.__class__.__name__
+        return f'<{klass} {self._type} {self.ttl}, {self.decoded_fqdn}, {self.value}>'
```

### Comparing `octodns-0.9.9/octodns/provider/digitalocean.py` & `octodns-1.0.0rc0/octodns/zone.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,348 +1,291 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
+import re
 from collections import defaultdict
-from requests import Session
-import logging
+from logging import getLogger
 
-from ..record import Record
-from .base import BaseProvider
+from .idna import idna_decode, idna_encode
+from .record import Create, Delete
 
 
-class DigitalOceanClientException(Exception):
+class SubzoneRecordException(Exception):
     pass
 
 
-class DigitalOceanClientNotFound(DigitalOceanClientException):
-
-    def __init__(self):
-        super(DigitalOceanClientNotFound, self).__init__('Not Found')
-
-
-class DigitalOceanClientUnauthorized(DigitalOceanClientException):
-
-    def __init__(self):
-        super(DigitalOceanClientUnauthorized, self).__init__('Unauthorized')
-
-
-class DigitalOceanClient(object):
-    BASE = 'https://api.digitalocean.com/v2'
-
-    def __init__(self, token):
-        sess = Session()
-        sess.headers.update({'Authorization': 'Bearer {}'.format(token)})
-        self._sess = sess
-
-    def _request(self, method, path, params=None, data=None):
-        url = '{}{}'.format(self.BASE, path)
-        resp = self._sess.request(method, url, params=params, json=data)
-        if resp.status_code == 401:
-            raise DigitalOceanClientUnauthorized()
-        if resp.status_code == 404:
-            raise DigitalOceanClientNotFound()
-        resp.raise_for_status()
-        return resp
-
-    def domain(self, name):
-        path = '/domains/{}'.format(name)
-        return self._request('GET', path).json()
+class DuplicateRecordException(Exception):
+    pass
 
-    def domain_create(self, name):
-        # Digitalocean requires an IP on zone creation
-        self._request('POST', '/domains', data={'name': name,
-                                                'ip_address': '192.0.2.1'})
 
-        # After the zone is created, immediately delete the record
-        records = self.records(name)
-        for record in records:
-            if record['name'] == '' and record['type'] == 'A':
-                self.record_delete(name, record['id'])
+class InvalidNodeException(Exception):
+    pass
 
-    def records(self, zone_name):
-        path = '/domains/{}/records'.format(zone_name)
-        ret = []
 
-        page = 1
-        while True:
-            data = self._request('GET', path, {'page': page}).json()
+class Zone(object):
+    log = getLogger('Zone')
 
-            ret += data['domain_records']
-            links = data['links']
+    def __init__(self, name, sub_zones):
+        if not name[-1] == '.':
+            raise Exception(f'Invalid zone name {name}, missing ending dot')
+        # internally everything is idna
+        self.name = idna_encode(str(name)) if name else name
+        # we'll keep a decoded version around for logs and errors
+        self.decoded_name = idna_decode(self.name)
+        self.sub_zones = sub_zones
+        # We're grouping by node, it allows us to efficiently search for
+        # duplicates and detect when CNAMEs co-exist with other records. Also
+        # node that we always store things with Record.name which will be idna
+        # encoded thus we don't have to deal with idna/utf8 collisions
+        self._records = defaultdict(set)
+        self._root_ns = None
+        # optional leading . to match empty hostname
+        # optional trailing . b/c some sources don't have it on their fqdn
+        self._utf8_name_re = re.compile(fr'\.?{idna_decode(name)}?$')
+        self._idna_name_re = re.compile(fr'\.?{self.name}?$')
+
+        # Copy-on-write semantics support, when `not None` this property will
+        # point to a location with records for this `Zone`. Once `hydrated`
+        # this property will be set to None
+        self._origin = None
+
+        self.log.debug('__init__: zone=%s, sub_zones=%s', self, sub_zones)
+
+    @property
+    def records(self):
+        if self._origin:
+            return self._origin.records
+        return set([r for _, node in self._records.items() for r in node])
+
+    @property
+    def root_ns(self):
+        if self._origin:
+            return self._origin.root_ns
+        return self._root_ns
 
-            # https://developers.digitalocean.com/documentation/v2/#links
-            # pages exists if there is more than 1 page
-            # last doesn't exist if you're on the last page
+    def hostname_from_fqdn(self, fqdn):
+        try:
+            fqdn.encode('ascii')
+            # it's non-idna or idna encoded
+            return self._idna_name_re.sub('', idna_encode(fqdn))
+        except UnicodeEncodeError:
+            # it has utf8 chars
+            return self._utf8_name_re.sub('', fqdn)
+
+    def add_record(self, record, replace=False, lenient=False):
+        if self._origin:
+            self.hydrate()
+
+        name = record.name
+
+        if not lenient:
+            if name in self.sub_zones:
+                # It's an exact match for a sub-zone
+                if not record._type == 'NS':
+                    # and not a NS record, this should be in the sub
+                    raise SubzoneRecordException(
+                        f'Record {record.fqdn} is a managed sub-zone and not of type NS'
+                    )
+            else:
+                # It's not an exact match so there has to be a `.` before the
+                # sub-zone for it to belong in there
+                for sub_zone in self.sub_zones:
+                    if name.endswith(f'.{sub_zone}'):
+                        # this should be in a sub
+                        raise SubzoneRecordException(
+                            f'Record {record.fqdn} is under a managed subzone'
+                        )
+
+        if replace:
+            # will remove it if it exists
+            self._records[name].discard(record)
+
+        node = self._records[name]
+        if record in node:
+            # We already have a record at this node of this type
+            raise DuplicateRecordException(
+                f'Duplicate record {record.fqdn}, ' f'type {record._type}'
+            )
+        elif not lenient and (
+            (record._type == 'CNAME' and len(node) > 0)
+            or ('CNAME' in [r._type for r in node])
+        ):
+            # We're adding a CNAME to existing records or adding to an existing
+            # CNAME
+            raise InvalidNodeException(
+                'Invalid state, CNAME at '
+                f'{record.fqdn} cannot coexist with '
+                'other records'
+            )
+
+        if record._type == 'NS' and record.name == '':
+            self._root_ns = record
+
+        node.add(record)
+
+    def remove_record(self, record):
+        if self._origin:
+            self.hydrate()
+
+        if record._type == 'NS' and record.name == '':
+            self._root_ns = None
+
+        self._records[record.name].discard(record)
+
+    # TODO: delete this
+    _remove_record = remove_record
+
+    def changes(self, desired, target):
+        self.log.debug('changes: zone=%s, target=%s', self, target)
+
+        # Build up a hash of the desired records, thanks to our special
+        # __hash__ and __cmp__ on Record we'll be able to look up records that
+        # match name and _type with it
+        desired_records = {r: r for r in desired.records}
+
+        changes = []
+
+        # Find diffs & removes
+        for record in self.records:
+            if record.ignored:
+                continue
+            elif len(record.included) > 0 and target.id not in record.included:
+                self.log.debug(
+                    'changes:  skipping record=%s %s - %s not included ',
+                    record.fqdn,
+                    record._type,
+                    target.id,
+                )
+                continue
+            elif target.id in record.excluded:
+                self.log.debug(
+                    'changes:  skipping record=%s %s - %s excluded ',
+                    record.fqdn,
+                    record._type,
+                    target.id,
+                )
+                continue
             try:
-                links['pages']['last']
-                page += 1
+                desired_record = desired_records[record]
+                if desired_record.ignored:
+                    continue
+                elif (
+                    len(desired_record.included) > 0
+                    and target.id not in desired_record.included
+                ):
+                    self.log.debug(
+                        'changes:  skipping record=%s %s - %s not included',
+                        record.fqdn,
+                        record._type,
+                        target.id,
+                    )
+                    continue
+                elif target.id in desired_record.excluded:
+                    continue
             except KeyError:
-                break
-
-        for record in ret:
-            # change any apex record to empty string
-            if record['name'] == '@':
-                record['name'] = ''
-
-            # change any apex value to zone name
-            if record['data'] == '@':
-                record['data'] = zone_name
-
-        return ret
-
-    def record_create(self, zone_name, params):
-        path = '/domains/{}/records'.format(zone_name)
-        # change empty name string to @, DO uses @ for apex record names
-        if params['name'] == '':
-            params['name'] = '@'
-
-        self._request('POST', path, data=params)
-
-    def record_delete(self, zone_name, record_id):
-        path = '/domains/{}/records/{}'.format(zone_name, record_id)
-        self._request('DELETE', path)
-
-
-class DigitalOceanProvider(BaseProvider):
-    '''
-    DigitalOcean DNS provider using API v2
-
-    digitalocean:
-        class: octodns.provider.digitalocean.DigitalOceanProvider
-        # Your DigitalOcean API token (required)
-        token: foo
-    '''
-    SUPPORTS_GEO = False
-    SUPPORTS_DYNAMIC = False
-    SUPPORTS = set(('A', 'AAAA', 'CAA', 'CNAME', 'MX', 'NS', 'TXT', 'SRV'))
-
-    def __init__(self, id, token, *args, **kwargs):
-        self.log = logging.getLogger('DigitalOceanProvider[{}]'.format(id))
-        self.log.debug('__init__: id=%s, token=***', id)
-        super(DigitalOceanProvider, self).__init__(id, *args, **kwargs)
-        self._client = DigitalOceanClient(token)
-
-        self._zone_records = {}
-
-    def _data_for_multiple(self, _type, records):
-        return {
-            'ttl': records[0]['ttl'],
-            'type': _type,
-            'values': [r['data'] for r in records]
-        }
-
-    _data_for_A = _data_for_multiple
-    _data_for_AAAA = _data_for_multiple
-
-    def _data_for_CAA(self, _type, records):
-        values = []
-        for record in records:
-            values.append({
-                'flags': record['flags'],
-                'tag': record['tag'],
-                'value': record['data'],
-            })
-        return {
-            'ttl': records[0]['ttl'],
-            'type': _type,
-            'values': values
-        }
-
-    def _data_for_CNAME(self, _type, records):
-        record = records[0]
-        return {
-            'ttl': record['ttl'],
-            'type': _type,
-            'value': '{}.'.format(record['data'])
-        }
-
-    def _data_for_MX(self, _type, records):
-        values = []
-        for record in records:
-            values.append({
-                'preference': record['priority'],
-                'exchange': '{}.'.format(record['data'])
-            })
-        return {
-            'ttl': records[0]['ttl'],
-            'type': _type,
-            'values': values
-        }
-
-    def _data_for_NS(self, _type, records):
-        values = []
-        for record in records:
-            data = '{}.'.format(record['data'])
-            values.append(data)
-        return {
-            'ttl': records[0]['ttl'],
-            'type': _type,
-            'values': values,
-        }
-
-    def _data_for_SRV(self, _type, records):
-        values = []
-        for record in records:
-            values.append({
-                'port': record['port'],
-                'priority': record['priority'],
-                'target': '{}.'.format(record['data']),
-                'weight': record['weight']
-            })
-        return {
-            'type': _type,
-            'ttl': records[0]['ttl'],
-            'values': values
-        }
-
-    def _data_for_TXT(self, _type, records):
-        values = [value['data'].replace(';', '\\;') for value in records]
-        return {
-            'ttl': records[0]['ttl'],
-            'type': _type,
-            'values': values
-        }
+                if not target.supports(record):
+                    self.log.debug(
+                        'changes:  skipping record=%s %s - %s does '
+                        'not support it',
+                        record.fqdn,
+                        record._type,
+                        target.id,
+                    )
+                    continue
+                # record has been removed
+                self.log.debug(
+                    'changes: zone=%s, removed record=%s', self, record
+                )
+                changes.append(Delete(record))
+            else:
+                change = record.changes(desired_record, target)
+                if change:
+                    self.log.debug(
+                        'changes: zone=%s, modified\n'
+                        '    existing=%s,\n     desired=%s',
+                        self,
+                        record,
+                        desired_record,
+                    )
+                    changes.append(change)
+                else:
+                    self.log.debug(
+                        'changes: zone=%s, n.c. record=%s', self, record
+                    )
+
+        # Find additions, things that are in desired, but missing in ourselves.
+        # This uses set math and our special __hash__ and __cmp__ functions as
+        # well
+        for record in desired.records - self.records:
+            if record.ignored:
+                continue
+            elif len(record.included) > 0 and target.id not in record.included:
+                self.log.debug(
+                    'changes:  skipping record=%s %s - %s not included ',
+                    record.fqdn,
+                    record._type,
+                    target.id,
+                )
+                continue
+            elif target.id in record.excluded:
+                self.log.debug(
+                    'changes:  skipping record=%s %s - %s excluded ',
+                    record.fqdn,
+                    record._type,
+                    target.id,
+                )
+                continue
 
-    def zone_records(self, zone):
-        if zone.name not in self._zone_records:
-            try:
-                self._zone_records[zone.name] = \
-                    self._client.records(zone.name[:-1])
-            except DigitalOceanClientNotFound:
-                return []
-
-        return self._zone_records[zone.name]
-
-    def populate(self, zone, target=False, lenient=False):
-        self.log.debug('populate: name=%s, target=%s, lenient=%s', zone.name,
-                       target, lenient)
-
-        values = defaultdict(lambda: defaultdict(list))
-        for record in self.zone_records(zone):
-            _type = record['type']
-            if _type not in self.SUPPORTS:
-                self.log.warning('populate: skipping unsupported %s record',
-                                 _type)
+            if not target.supports(record):
+                self.log.debug(
+                    'changes:  skipping record=%s %s - %s does not '
+                    'support it',
+                    record.fqdn,
+                    record._type,
+                    target.id,
+                )
                 continue
-            values[record['name']][record['type']].append(record)
+            self.log.debug('changes: zone=%s, create record=%s', self, record)
+            changes.append(Create(record))
 
-        before = len(zone.records)
-        for name, types in values.items():
-            for _type, records in types.items():
-                data_for = getattr(self, '_data_for_{}'.format(_type))
-                record = Record.new(zone, name, data_for(_type, records),
-                                    source=self, lenient=lenient)
-                zone.add_record(record, lenient=lenient)
-
-        exists = zone.name in self._zone_records
-        self.log.info('populate:   found %s records, exists=%s',
-                      len(zone.records) - before, exists)
-        return exists
-
-    def _params_for_multiple(self, record):
-        for value in record.values:
-            yield {
-                'data': value,
-                'name': record.name,
-                'ttl': record.ttl,
-                'type': record._type
-            }
-
-    _params_for_A = _params_for_multiple
-    _params_for_AAAA = _params_for_multiple
-    _params_for_NS = _params_for_multiple
-
-    def _params_for_CAA(self, record):
-        for value in record.values:
-            yield {
-                'data': '{}.'.format(value.value),
-                'flags': value.flags,
-                'name': record.name,
-                'tag': value.tag,
-                'ttl': record.ttl,
-                'type': record._type
-            }
-
-    def _params_for_single(self, record):
-        yield {
-            'data': record.value,
-            'name': record.name,
-            'ttl': record.ttl,
-            'type': record._type
-        }
-
-    _params_for_CNAME = _params_for_single
-
-    def _params_for_MX(self, record):
-        for value in record.values:
-            yield {
-                'data': value.exchange,
-                'name': record.name,
-                'priority': value.preference,
-                'ttl': record.ttl,
-                'type': record._type
-            }
-
-    def _params_for_SRV(self, record):
-        for value in record.values:
-            yield {
-                'data': value.target,
-                'name': record.name,
-                'port': value.port,
-                'priority': value.priority,
-                'ttl': record.ttl,
-                'type': record._type,
-                'weight': value.weight
-            }
-
-    def _params_for_TXT(self, record):
-        # DigitalOcean doesn't want things escaped in values so we
-        # have to strip them here and add them when going the other way
-        for value in record.values:
-            yield {
-                'data': value.replace('\\;', ';'),
-                'name': record.name,
-                'ttl': record.ttl,
-                'type': record._type
-            }
-
-    def _apply_Create(self, change):
-        new = change.new
-        params_for = getattr(self, '_params_for_{}'.format(new._type))
-        for params in params_for(new):
-            self._client.record_create(new.zone.name[:-1], params)
-
-    def _apply_Update(self, change):
-        self._apply_Delete(change)
-        self._apply_Create(change)
-
-    def _apply_Delete(self, change):
-        existing = change.existing
-        zone = existing.zone
-        for record in self.zone_records(zone):
-            if existing.name == record['name'] and \
-               existing._type == record['type']:
-                self._client.record_delete(zone.name[:-1], record['id'])
-
-    def _apply(self, plan):
-        desired = plan.desired
-        changes = plan.changes
-        self.log.debug('_apply: zone=%s, len(changes)=%d', desired.name,
-                       len(changes))
+        return changes
 
-        domain_name = desired.name[:-1]
-        try:
-            self._client.domain(domain_name)
-        except DigitalOceanClientNotFound:
-            self.log.debug('_apply:   no matching zone, creating domain')
-            self._client.domain_create(domain_name)
-
-        for change in changes:
-            class_name = change.__class__.__name__
-            getattr(self, '_apply_{}'.format(class_name))(change)
+    def hydrate(self):
+        '''
+        Take a shallow copy Zone and make it a deeper copy holding its own
+        reference to records. These records will still be the originals and
+        they should not be modified. Changes should be made by calling
+        `add_record`, often with `replace=True`, and/or `remove_record`.
+
+        Note: This method does not need to be called under normal circumstances
+        as `add_record` and `remove_record` will automatically call it when
+        appropriate.
+        '''
+        origin = self._origin
+        if origin is None:
+            return False
+        # Need to clear this before the copy to prevent recursion
+        self._origin = None
+        for record in origin.records:
+            # Use lenient as we're copying origin and should take its records
+            # regardless
+            self.add_record(record, lenient=True)
+        return True
+
+    def copy(self):
+        '''
+        Copy-on-write semantics support. This method will create a shallow
+        clone of the zone which will be hydrated the first time `add_record` or
+        `remove_record` is called.
+
+        This allows low-cost copies of things to be made in situations where
+        changes are unlikely and only incurs the "expense" of actually
+        copying the records when required. The actual record copy will not be
+        "deep" meaning that records should not be modified directly.
+        '''
+        copy = Zone(self.name, self.sub_zones)
+        copy._origin = self
+        return copy
 
-        # Clear out the cache if any
-        self._zone_records.pop(desired.name, None)
+    def __repr__(self):
+        return f'Zone<{self.decoded_name}>'
```

### Comparing `octodns-0.9.9/octodns/cmds/report.py` & `octodns-1.0.0rc0/octodns/cmds/report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,98 +1,104 @@
 #!/usr/bin/env python
 '''
 Octo-DNS Reporter
 '''
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
+import re
 from concurrent.futures import ThreadPoolExecutor
-from dns.exception import Timeout
-from dns.resolver import NXDOMAIN, NoAnswer, NoNameservers, Resolver, query
 from logging import getLogger
 from sys import stdout
-import re
 
-from six import text_type
+from dns.exception import Timeout
+from dns.resolver import NXDOMAIN, NoAnswer, NoNameservers, Resolver, query
 
 from octodns.cmds.args import ArgumentParser
 from octodns.manager import Manager
-from octodns.zone import Zone
 
 
 class AsyncResolver(Resolver):
-
     def __init__(self, num_workers, *args, **kwargs):
-        super(AsyncResolver, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.executor = ThreadPoolExecutor(max_workers=num_workers)
 
     def query(self, *args, **kwargs):
-        return self.executor.submit(super(AsyncResolver, self).query, *args,
-                                    **kwargs)
+        return self.executor.submit(super().query, *args, **kwargs)
 
 
 def main():
     parser = ArgumentParser(description=__doc__.split('\n')[1])
 
-    parser.add_argument('--config-file', required=True,
-                        help='The Manager configuration file to use')
+    parser.add_argument(
+        '--config-file',
+        required=True,
+        help='The Manager configuration file to use',
+    )
     parser.add_argument('--zone', required=True, help='Zone to dump')
-    parser.add_argument('--source', required=True, default=[], action='append',
-                        help='Source(s) to pull data from')
-    parser.add_argument('--num-workers', default=4,
-                        help='Number of background workers')
-    parser.add_argument('--timeout', default=1,
-                        help='Number seconds to wait for an answer')
+    parser.add_argument(
+        '--source',
+        required=True,
+        default=[],
+        action='append',
+        help='Source(s) to pull data from',
+    )
+    parser.add_argument(
+        '--num-workers', default=4, help='Number of background workers'
+    )
+    parser.add_argument(
+        '--timeout', default=1, help='Number seconds to wait for an answer'
+    )
     parser.add_argument('server', nargs='+', help='Servers to query')
 
     args = parser.parse_args()
 
     manager = Manager(args.config_file)
 
     log = getLogger('report')
 
     try:
         sources = [manager.providers[source] for source in args.source]
     except KeyError as e:
-        raise Exception('Unknown source: {}'.format(e.args[0]))
+        raise Exception(f'Unknown source: {e.args[0]}')
 
-    zone = Zone(args.zone, manager.configured_sub_zones(args.zone))
+    zone = manager.get_zone(args.zone)
     for source in sources:
         source.populate(zone)
 
-    print('name,type,ttl,{},consistent'.format(','.join(args.server)))
+    servers = ','.join(args.server)
+    print(f'name,type,ttl,{servers},consistent')
     resolvers = []
     ip_addr_re = re.compile(r'^[\d\.]+$')
     for server in args.server:
-        resolver = AsyncResolver(configure=False,
-                                 num_workers=int(args.num_workers))
+        resolver = AsyncResolver(
+            configure=False, num_workers=int(args.num_workers)
+        )
         if not ip_addr_re.match(server):
-            server = text_type(query(server, 'A')[0])
+            server = str(query(server, 'A')[0])
         log.info('server=%s', server)
         resolver.nameservers = [server]
         resolver.lifetime = int(args.timeout)
         resolvers.append(resolver)
 
     queries = {}
     for record in sorted(zone.records):
-        queries[record] = [r.query(record.fqdn, record._type)
-                           for r in resolvers]
+        queries[record] = [
+            r.query(record.fqdn, record._type) for r in resolvers
+        ]
 
     for record, futures in sorted(queries.items(), key=lambda d: d[0]):
-        stdout.write(record.fqdn)
+        stdout.write(record.decoded_fqdn)
         stdout.write(',')
         stdout.write(record._type)
         stdout.write(',')
-        stdout.write(text_type(record.ttl))
+        stdout.write(str(record.ttl))
         compare = {}
         for future in futures:
             stdout.write(',')
             try:
-                answers = [text_type(r) for r in future.result()]
+                answers = [str(r) for r in future.result()]
             except (NoAnswer, NoNameservers):
                 answers = ['*no answer*']
             except NXDOMAIN:
                 answers = ['*does not exist*']
             except Timeout:
                 answers = ['*timeout*']
             stdout.write(' '.join(answers))
```

### Comparing `octodns-0.9.9/octodns/equality.py` & `octodns-1.0.0rc0/octodns/equality.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
 
 class EqualityTupleMixin(object):
-
     def _equality_tuple(self):
         raise NotImplementedError('_equality_tuple method not implemented')
 
     def __eq__(self, other):
         return self._equality_tuple() == other._equality_tuple()
 
     def __ne__(self, other):
```

### Comparing `octodns-0.9.9/octodns/yaml.py` & `octodns-1.0.0rc0/octodns/yaml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
 from natsort import natsort_keygen
-from yaml import SafeDumper, SafeLoader, load, dump
+from yaml import SafeDumper, SafeLoader, dump, load
 from yaml.constructor import ConstructorError
-
+from yaml.representer import SafeRepresenter
 
 _natsort_key = natsort_keygen()
 
 
 # Found http://stackoverflow.com/a/21912744 which guided me on how to hook in
 # here
 class SortEnforcingLoader(SafeLoader):
-
     def _construct(self, node):
         self.flatten_mapping(node)
         ret = self.construct_pairs(node)
         keys = [d[0] for d in ret]
         keys_sorted = sorted(keys, key=_natsort_key)
         for key in keys:
             expected = keys_sorted.pop(0)
             if key != expected:
-                raise ConstructorError(None, None, 'keys out of order: '
-                                       'expected {} got {} at {}'
-                                       .format(expected, key, node.start_mark))
+                raise ConstructorError(
+                    None,
+                    None,
+                    'keys out of order: '
+                    f'expected {expected} got {key} at ' + str(node.start_mark),
+                )
         return dict(ret)
 
 
-SortEnforcingLoader.add_constructor(SortEnforcingLoader.DEFAULT_MAPPING_TAG,
-                                    SortEnforcingLoader._construct)
+SortEnforcingLoader.add_constructor(
+    SortEnforcingLoader.DEFAULT_MAPPING_TAG, SortEnforcingLoader._construct
+)
 
 
 def safe_load(stream, enforce_order=True):
     return load(stream, SortEnforcingLoader if enforce_order else SafeLoader)
 
 
 class SortingDumper(SafeDumper):
@@ -50,19 +50,23 @@
 
     def _representer(self, data):
         data = sorted(data.items(), key=lambda d: _natsort_key(d[0]))
         return self.represent_mapping(self.DEFAULT_MAPPING_TAG, data)
 
 
 SortingDumper.add_representer(dict, SortingDumper._representer)
+# This should handle all the record value types which are ultimately either str
+# or dict at some point in their inheritance hierarchy
+SortingDumper.add_multi_representer(str, SafeRepresenter.represent_str)
+SortingDumper.add_multi_representer(dict, SortingDumper._representer)
 
 
 def safe_dump(data, fh, **options):
     kwargs = {
         'canonical': False,
         'indent': 2,
         'default_style': '',
         'default_flow_style': False,
-        'explicit_start': True
+        'explicit_start': True,
     }
     kwargs.update(options)
     dump(data, fh, SortingDumper, **kwargs)
```

### Comparing `octodns-0.9.9/tests/test_octodns_yaml.py` & `octodns-1.0.0rc0/tests/test_octodns_yaml.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,64 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
-from six import StringIO
+from io import StringIO
 from unittest import TestCase
+
 from yaml.constructor import ConstructorError
 
 from octodns.yaml import safe_dump, safe_load
 
 
 class TestYaml(TestCase):
-
     def test_stuff(self):
-        self.assertEquals({
-            1: 'a',
-            2: 'b',
-            '3': 'c',
-            10: 'd',
-            '11': 'e',
-        }, safe_load('''
+        self.assertEqual(
+            {1: 'a', 2: 'b', '3': 'c', 10: 'd', '11': 'e'},
+            safe_load(
+                '''
 1: a
 2: b
 '3': c
 10: d
 '11': e
-'''))
-
-        self.assertEquals({
-            '*.1.2': 'a',
-            '*.2.2': 'b',
-            '*.10.1': 'c',
-            '*.11.2': 'd',
-        }, safe_load('''
+'''
+            ),
+        )
+
+        self.assertEqual(
+            {'*.1.2': 'a', '*.2.2': 'b', '*.10.1': 'c', '*.11.2': 'd'},
+            safe_load(
+                '''
 '*.1.2': 'a'
 '*.2.2': 'b'
 '*.10.1': 'c'
 '*.11.2': 'd'
-'''))
+'''
+            ),
+        )
 
         with self.assertRaises(ConstructorError) as ctx:
-            safe_load('''
+            safe_load(
+                '''
 '*.2.2': 'b'
 '*.1.2': 'a'
 '*.11.2': 'd'
 '*.10.1': 'c'
-''')
-        self.assertTrue('keys out of order: expected *.1.2 got *.2.2 at' in
-                        ctx.exception.problem)
+'''
+            )
+        self.assertTrue(
+            'keys out of order: expected *.1.2 got *.2.2 at'
+            in ctx.exception.problem
+        )
 
         buf = StringIO()
-        safe_dump({
-            '*.1.1': 42,
-            '*.11.1': 43,
-            '*.2.1': 44,
-        }, buf)
-        self.assertEquals("---\n'*.1.1': 42\n'*.2.1': 44\n'*.11.1': 43\n",
-                          buf.getvalue())
+        safe_dump({'*.1.1': 42, '*.11.1': 43, '*.2.1': 44}, buf)
+        self.assertEqual(
+            "---\n'*.1.1': 42\n'*.2.1': 44\n'*.11.1': 43\n", buf.getvalue()
+        )
 
         # hex sorting isn't ideal, not treated as hex, this make sure we don't
         # change the behavior
         buf = StringIO()
-        safe_dump({
-            '45a03129': 42,
-            '45a0392a': 43,
-        }, buf)
-        self.assertEquals("---\n45a0392a: 43\n45a03129: 42\n", buf.getvalue())
+        safe_dump({'45a03129': 42, '45a0392a': 43}, buf)
+        self.assertEqual("---\n45a0392a: 43\n45a03129: 42\n", buf.getvalue())
```

### Comparing `octodns-0.9.9/tests/test_octodns_provider_yaml.py` & `octodns-1.0.0rc0/tests/test_octodns_provider_yaml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
 from os import makedirs
 from os.path import basename, dirname, isdir, isfile, join
 from unittest import TestCase
-from six import text_type
+
+from helpers import TemporaryDirectory
 from yaml import safe_load
 from yaml.constructor import ConstructorError
 
-from octodns.record import Create
+from octodns.idna import idna_encode
+from octodns.provider import ProviderException
 from octodns.provider.base import Plan
-from octodns.provider.yaml import _list_all_yaml_files, \
-    SplitYamlProvider, YamlProvider
+from octodns.provider.yaml import (
+    SplitYamlProvider,
+    YamlProvider,
+    _list_all_yaml_files,
+)
+from octodns.record import Create, NsValue, Record, ValuesMixin
 from octodns.zone import SubzoneRecordException, Zone
 
-from helpers import TemporaryDirectory
-
 
 class TestYamlProvider(TestCase):
-
     def test_provider(self):
         source = YamlProvider('test', join(dirname(__file__), 'config'))
 
         zone = Zone('unit.tests.', [])
         dynamic_zone = Zone('dynamic.tests.', [])
 
         # With target we don't add anything
         source.populate(zone, target=source)
-        self.assertEquals(0, len(zone.records))
+        self.assertEqual(0, len(zone.records))
 
         # without it we see everything
         source.populate(zone)
-        self.assertEquals(18, len(zone.records))
+        self.assertEqual(25, len(zone.records))
 
         source.populate(dynamic_zone)
-        self.assertEquals(5, len(dynamic_zone.records))
+        self.assertEqual(6, len(dynamic_zone.records))
 
         # Assumption here is that a clean round-trip means that everything
         # worked as expected, data that went in came back out and could be
         # pulled in yet again and still match up. That assumes that the input
         # data completely exercises things. This assumption can be tested by
         # relatively well by running
         #   ./script/coverage tests/test_octodns_provider_yaml.py and
@@ -50,77 +50,95 @@
         #   ./htmlcov/octodns_provider_yaml_py.html
 
         with TemporaryDirectory() as td:
             # Add some subdirs to make sure that it can create them
             directory = join(td.dirname, 'sub', 'dir')
             yaml_file = join(directory, 'unit.tests.yaml')
             dynamic_yaml_file = join(directory, 'dynamic.tests.yaml')
-            target = YamlProvider('test', directory)
+            target = YamlProvider(
+                'test', directory, supports_root_ns=False, strict_supports=False
+            )
 
             # We add everything
             plan = target.plan(zone)
-            self.assertEquals(15, len([c for c in plan.changes
-                                       if isinstance(c, Create)]))
+            self.assertEqual(
+                22, len([c for c in plan.changes if isinstance(c, Create)])
+            )
             self.assertFalse(isfile(yaml_file))
 
             # Now actually do it
-            self.assertEquals(15, target.apply(plan))
+            self.assertEqual(22, target.apply(plan))
             self.assertTrue(isfile(yaml_file))
 
             # Dynamic plan
             plan = target.plan(dynamic_zone)
-            self.assertEquals(5, len([c for c in plan.changes
-                                      if isinstance(c, Create)]))
+            self.assertEqual(
+                6, len([c for c in plan.changes if isinstance(c, Create)])
+            )
             self.assertFalse(isfile(dynamic_yaml_file))
             # Apply it
-            self.assertEquals(5, target.apply(plan))
+            self.assertEqual(6, target.apply(plan))
             self.assertTrue(isfile(dynamic_yaml_file))
 
             # There should be no changes after the round trip
             reloaded = Zone('unit.tests.', [])
             target.populate(reloaded)
             self.assertDictEqual(
                 {'included': ['test']},
-                [x for x in reloaded.records
-                 if x.name == 'included'][0]._octodns)
+                [x for x in reloaded.records if x.name == 'included'][
+                    0
+                ]._octodns,
+            )
+
+            # manually copy over the root since it will have been ignored
+            # when things were written out
+            reloaded.add_record(zone.root_ns)
 
             self.assertFalse(zone.changes(reloaded, target=source))
 
             # A 2nd sync should still create everything
             plan = target.plan(zone)
-            self.assertEquals(15, len([c for c in plan.changes
-                                       if isinstance(c, Create)]))
+            self.assertEqual(
+                22, len([c for c in plan.changes if isinstance(c, Create)])
+            )
 
             with open(yaml_file) as fh:
                 data = safe_load(fh.read())
 
                 # '' has some of both
                 roots = sorted(data.pop(''), key=lambda r: r['type'])
                 self.assertTrue('values' in roots[0])  # A
                 self.assertTrue('geo' in roots[0])  # geo made the trip
-                self.assertTrue('value' in roots[1])   # CAA
+                self.assertTrue('value' in roots[1])  # CAA
                 self.assertTrue('values' in roots[2])  # SSHFP
 
                 # these are stored as plural 'values'
                 self.assertTrue('values' in data.pop('_srv._tcp'))
                 self.assertTrue('values' in data.pop('mx'))
                 self.assertTrue('values' in data.pop('naptr'))
                 self.assertTrue('values' in data.pop('sub'))
                 self.assertTrue('values' in data.pop('txt'))
+                self.assertTrue('values' in data.pop('loc'))
+                self.assertTrue('values' in data.pop('urlfwd'))
+                self.assertTrue('values' in data.pop('sub.txt'))
+                self.assertTrue('values' in data.pop('subzone'))
                 # these are stored as singular 'value'
+                self.assertTrue('value' in data.pop('_imap._tcp'))
+                self.assertTrue('value' in data.pop('_pop3._tcp'))
                 self.assertTrue('value' in data.pop('aaaa'))
                 self.assertTrue('value' in data.pop('cname'))
+                self.assertTrue('value' in data.pop('dname'))
                 self.assertTrue('value' in data.pop('included'))
                 self.assertTrue('value' in data.pop('ptr'))
                 self.assertTrue('value' in data.pop('spf'))
                 self.assertTrue('value' in data.pop('www'))
                 self.assertTrue('value' in data.pop('www.sub'))
 
                 # make sure nothing is left
-                self.assertEquals([], list(data.keys()))
+                self.assertEqual([], list(data.keys()))
 
             with open(dynamic_yaml_file) as fh:
                 data = safe_load(fh.read())
 
                 # make sure new dynamic records made the trip
                 dyna = data.pop('a')
                 self.assertTrue('values' in dyna)
@@ -140,53 +158,150 @@
                 self.assertTrue('values' in dyna)
                 # self.assertTrue('dynamic' in dyna)
 
                 dyna = data.pop('simple-weighted')
                 self.assertTrue('value' in dyna)
                 # self.assertTrue('dynamic' in dyna)
 
+                dyna = data.pop('pool-only-in-fallback')
+                self.assertTrue('value' in dyna)
+                # self.assertTrue('dynamic' in dyna)
+
                 # make sure nothing is left
-                self.assertEquals([], list(data.keys()))
+                self.assertEqual([], list(data.keys()))
+
+    def test_idna(self):
+        with TemporaryDirectory() as td:
+            name = 'déjà.vu.'
+            filename = f'{name}yaml'
+
+            provider = YamlProvider('test', td.dirname)
+            zone = Zone(idna_encode(name), [])
+
+            # create a idna named file
+            with open(join(td.dirname, idna_encode(filename)), 'w') as fh:
+                fh.write(
+                    '''---
+'':
+  type: A
+  value: 1.2.3.4
+# something in idna notation
+xn--dj-kia8a:
+  type: A
+  value: 2.3.4.5
+# something with utf-8
+これはテストです:
+  type: A
+  value: 3.4.5.6
+'''
+                )
+
+            # populates fine when there's just the idna version (as a fallback)
+            provider.populate(zone)
+            d = {r.name: r for r in zone.records}
+            self.assertEqual(3, len(d))
+            # verify that we loaded the expected records, including idna/utf-8
+            # named ones
+            self.assertEqual(['1.2.3.4'], d[''].values)
+            self.assertEqual(['2.3.4.5'], d['xn--dj-kia8a'].values)
+            self.assertEqual(['3.4.5.6'], d['xn--28jm5b5a8k5k8cra'].values)
+
+            # create a utf8 named file (provider always writes utf-8 filenames
+            plan = provider.plan(zone)
+            provider.apply(plan)
+
+            with open(join(td.dirname, filename), 'r') as fh:
+                content = fh.read()
+                # verify that the non-ascii records were written out in utf-8
+                self.assertTrue('déjà:' in content)
+                self.assertTrue('これはテストです:' in content)
+
+            # does not allow both idna and utf8 named files
+            with self.assertRaises(ProviderException) as ctx:
+                provider.populate(zone)
+            msg = str(ctx.exception)
+            self.assertTrue('Both UTF-8' in msg)
 
     def test_empty(self):
-        source = YamlProvider('test', join(dirname(__file__), 'config'))
+        source = YamlProvider(
+            'test', join(dirname(__file__), 'config'), supports_root_ns=False
+        )
 
         zone = Zone('empty.', [])
 
         # without it we see everything
         source.populate(zone)
-        self.assertEquals(0, len(zone.records))
+        self.assertEqual(0, len(zone.records))
 
     def test_unsorted(self):
-        source = YamlProvider('test', join(dirname(__file__), 'config'))
+        source = YamlProvider(
+            'test', join(dirname(__file__), 'config'), supports_root_ns=False
+        )
 
         zone = Zone('unordered.', [])
 
         with self.assertRaises(ConstructorError):
             source.populate(zone)
 
-        source = YamlProvider('test', join(dirname(__file__), 'config'),
-                              enforce_order=False)
+        source = YamlProvider(
+            'test',
+            join(dirname(__file__), 'config'),
+            enforce_order=False,
+            supports_root_ns=False,
+        )
         # no exception
         source.populate(zone)
         self.assertEqual(2, len(zone.records))
 
     def test_subzone_handling(self):
-        source = YamlProvider('test', join(dirname(__file__), 'config'))
+        source = YamlProvider(
+            'test', join(dirname(__file__), 'config'), supports_root_ns=False
+        )
 
         # If we add `sub` as a sub-zone we'll reject `www.sub`
         zone = Zone('unit.tests.', ['sub'])
         with self.assertRaises(SubzoneRecordException) as ctx:
             source.populate(zone)
-        self.assertEquals('Record www.sub.unit.tests. is under a managed '
-                          'subzone', text_type(ctx.exception))
+        self.assertEqual(
+            'Record www.sub.unit.tests. is under a managed subzone',
+            str(ctx.exception),
+        )
 
+    def test_SUPPORTS(self):
+        source = YamlProvider('test', join(dirname(__file__), 'config'))
+        # make sure the provider supports all the registered types
+        self.assertEqual(Record.registered_types().keys(), source.SUPPORTS)
 
-class TestSplitYamlProvider(TestCase):
+        class YamlRecord(ValuesMixin, Record):
+            _type = 'YAML'
+            _value_type = NsValue
+
+        # don't know anything about a yaml type
+        self.assertTrue('YAML' not in source.SUPPORTS)
+        # register it
+        Record.register_type(YamlRecord)
+        # when asked again we'll now include it in our list of supports
+        self.assertTrue('YAML' in source.SUPPORTS)
+
+    def test_supports(self):
+        source = YamlProvider('test', join(dirname(__file__), 'config'))
 
+        class DummyType(object):
+            def __init__(self, _type):
+                self._type = _type
+
+        # No matter what we check it's always supported
+        self.assertTrue(source.supports(DummyType(None)))
+        self.assertTrue(source.supports(DummyType(42)))
+        self.assertTrue(source.supports(DummyType('A')))
+        self.assertTrue(source.supports(DummyType(source)))
+        self.assertTrue(source.supports(DummyType(self)))
+
+
+class TestSplitYamlProvider(TestCase):
     def test_list_all_yaml_files(self):
         yaml_files = ('foo.yaml', '1.yaml', '$unit.tests.yaml')
         all_files = ('something', 'else', '1', '$$', '-f') + yaml_files
         all_dirs = ('dir1', 'dir2/sub', 'tricky.yaml')
 
         with TemporaryDirectory() as td:
             directory = join(td.dirname)
@@ -202,171 +317,295 @@
             # This isn't great, but given the variable nature of the temp dir
             # names, it's necessary.
             d = list(basename(f) for f in _list_all_yaml_files(directory))
             self.assertEqual(len(yaml_files), len(d))
 
     def test_zone_directory(self):
         source = SplitYamlProvider(
-            'test', join(dirname(__file__), 'config/split'))
+            'test', join(dirname(__file__), 'config/split'), extension='.tst'
+        )
 
         zone = Zone('unit.tests.', [])
 
         self.assertEqual(
-            join(dirname(__file__), 'config/split/unit.tests.'),
-            source._zone_directory(zone))
+            join(dirname(__file__), 'config/split', 'unit.tests.tst'),
+            source._zone_directory(zone),
+        )
 
     def test_apply_handles_existing_zone_directory(self):
         with TemporaryDirectory() as td:
-            provider = SplitYamlProvider('test', join(td.dirname, 'config'))
-            makedirs(join(td.dirname, 'config', 'does.exist.'))
+            provider = SplitYamlProvider(
+                'test', join(td.dirname, 'config'), extension='.tst'
+            )
+            makedirs(join(td.dirname, 'config', 'does.exist.tst'))
 
             zone = Zone('does.exist.', [])
             self.assertTrue(isdir(provider._zone_directory(zone)))
             provider.apply(Plan(None, zone, [], True))
             self.assertTrue(isdir(provider._zone_directory(zone)))
 
     def test_provider(self):
         source = SplitYamlProvider(
-            'test', join(dirname(__file__), 'config/split'))
+            'test',
+            join(dirname(__file__), 'config/split'),
+            extension='.tst',
+            strict_supports=False,
+        )
 
         zone = Zone('unit.tests.', [])
         dynamic_zone = Zone('dynamic.tests.', [])
 
         # With target we don't add anything
         source.populate(zone, target=source)
-        self.assertEquals(0, len(zone.records))
+        self.assertEqual(0, len(zone.records))
 
         # without it we see everything
         source.populate(zone)
-        self.assertEquals(18, len(zone.records))
+        self.assertEqual(20, len(zone.records))
 
         source.populate(dynamic_zone)
-        self.assertEquals(5, len(dynamic_zone.records))
+        self.assertEqual(5, len(dynamic_zone.records))
 
         with TemporaryDirectory() as td:
             # Add some subdirs to make sure that it can create them
             directory = join(td.dirname, 'sub', 'dir')
-            zone_dir = join(directory, 'unit.tests.')
-            dynamic_zone_dir = join(directory, 'dynamic.tests.')
-            target = SplitYamlProvider('test', directory)
+            zone_dir = join(directory, 'unit.tests.tst')
+            dynamic_zone_dir = join(directory, 'dynamic.tests.tst')
+            target = SplitYamlProvider(
+                'test',
+                directory,
+                extension='.tst',
+                supports_root_ns=False,
+                strict_supports=False,
+            )
 
             # We add everything
             plan = target.plan(zone)
-            self.assertEquals(15, len([c for c in plan.changes
-                                       if isinstance(c, Create)]))
+            self.assertEqual(
+                17, len([c for c in plan.changes if isinstance(c, Create)])
+            )
             self.assertFalse(isdir(zone_dir))
 
             # Now actually do it
-            self.assertEquals(15, target.apply(plan))
+            self.assertEqual(17, target.apply(plan))
 
             # Dynamic plan
             plan = target.plan(dynamic_zone)
-            self.assertEquals(5, len([c for c in plan.changes
-                                      if isinstance(c, Create)]))
+            self.assertEqual(
+                5, len([c for c in plan.changes if isinstance(c, Create)])
+            )
             self.assertFalse(isdir(dynamic_zone_dir))
             # Apply it
-            self.assertEquals(5, target.apply(plan))
+            self.assertEqual(5, target.apply(plan))
             self.assertTrue(isdir(dynamic_zone_dir))
 
             # There should be no changes after the round trip
             reloaded = Zone('unit.tests.', [])
             target.populate(reloaded)
             self.assertDictEqual(
                 {'included': ['test']},
-                [x for x in reloaded.records
-                 if x.name == 'included'][0]._octodns)
+                [x for x in reloaded.records if x.name == 'included'][
+                    0
+                ]._octodns,
+            )
+
+            # manually copy over the root since it will have been ignored
+            # when things were written out
+            reloaded.add_record(zone.root_ns)
 
             self.assertFalse(zone.changes(reloaded, target=source))
 
             # A 2nd sync should still create everything
             plan = target.plan(zone)
-            self.assertEquals(15, len([c for c in plan.changes
-                                       if isinstance(c, Create)]))
+            self.assertEqual(
+                17, len([c for c in plan.changes if isinstance(c, Create)])
+            )
 
             yaml_file = join(zone_dir, '$unit.tests.yaml')
             self.assertTrue(isfile(yaml_file))
             with open(yaml_file) as fh:
                 data = safe_load(fh.read())
                 roots = sorted(data.pop(''), key=lambda r: r['type'])
                 self.assertTrue('values' in roots[0])  # A
                 self.assertTrue('geo' in roots[0])  # geo made the trip
-                self.assertTrue('value' in roots[1])   # CAA
+                self.assertTrue('value' in roots[1])  # CAA
                 self.assertTrue('values' in roots[2])  # SSHFP
 
             # These records are stored as plural "values." Check each file to
             # ensure correctness.
-            for record_name in ('_srv._tcp', 'mx', 'naptr', 'sub', 'txt'):
-                yaml_file = join(zone_dir, '{}.yaml'.format(record_name))
+            for record_name in (
+                '_srv._tcp',
+                'mx',
+                'naptr',
+                'sub',
+                'txt',
+                'urlfwd',
+            ):
+                yaml_file = join(zone_dir, f'{record_name}.yaml')
                 self.assertTrue(isfile(yaml_file))
                 with open(yaml_file) as fh:
                     data = safe_load(fh.read())
                     self.assertTrue('values' in data.pop(record_name))
 
             # These are stored as singular "value." Again, check each file.
-            for record_name in ('aaaa', 'cname', 'included', 'ptr', 'spf',
-                                'www.sub', 'www'):
-                yaml_file = join(zone_dir, '{}.yaml'.format(record_name))
+            for record_name in (
+                'aaaa',
+                'cname',
+                'dname',
+                'included',
+                'ptr',
+                'spf',
+                'www.sub',
+                'www',
+            ):
+                yaml_file = join(zone_dir, f'{record_name}.yaml')
                 self.assertTrue(isfile(yaml_file))
                 with open(yaml_file) as fh:
                     data = safe_load(fh.read())
                     self.assertTrue('value' in data.pop(record_name))
 
             # Again with the plural, this time checking dynamic.tests.
             for record_name in ('a', 'aaaa', 'real-ish-a'):
-                yaml_file = join(
-                    dynamic_zone_dir, '{}.yaml'.format(record_name))
+                yaml_file = join(dynamic_zone_dir, f'{record_name}.yaml')
                 self.assertTrue(isfile(yaml_file))
                 with open(yaml_file) as fh:
                     data = safe_load(fh.read())
                     dyna = data.pop(record_name)
                     self.assertTrue('values' in dyna)
                     self.assertTrue('dynamic' in dyna)
 
             # Singular again.
             for record_name in ('cname', 'simple-weighted'):
-                yaml_file = join(
-                    dynamic_zone_dir, '{}.yaml'.format(record_name))
+                yaml_file = join(dynamic_zone_dir, f'{record_name}.yaml')
                 self.assertTrue(isfile(yaml_file))
                 with open(yaml_file) as fh:
                     data = safe_load(fh.read())
                     dyna = data.pop(record_name)
                     self.assertTrue('value' in dyna)
                     self.assertTrue('dynamic' in dyna)
 
     def test_empty(self):
         source = SplitYamlProvider(
-            'test', join(dirname(__file__), 'config/split'))
+            'test', join(dirname(__file__), 'config/split'), extension='.tst'
+        )
 
         zone = Zone('empty.', [])
 
         # without it we see everything
         source.populate(zone)
-        self.assertEquals(0, len(zone.records))
+        self.assertEqual(0, len(zone.records))
 
     def test_unsorted(self):
         source = SplitYamlProvider(
-            'test', join(dirname(__file__), 'config/split'))
+            'test', join(dirname(__file__), 'config/split'), extension='.tst'
+        )
 
         zone = Zone('unordered.', [])
 
         with self.assertRaises(ConstructorError):
             source.populate(zone)
 
         zone = Zone('unordered.', [])
 
         source = SplitYamlProvider(
-            'test', join(dirname(__file__), 'config/split'),
-            enforce_order=False)
+            'test',
+            join(dirname(__file__), 'config/split'),
+            extension='.tst',
+            enforce_order=False,
+        )
         # no exception
         source.populate(zone)
         self.assertEqual(2, len(zone.records))
 
     def test_subzone_handling(self):
         source = SplitYamlProvider(
-            'test', join(dirname(__file__), 'config/split'))
+            'test', join(dirname(__file__), 'config/split'), extension='.tst'
+        )
 
         # If we add `sub` as a sub-zone we'll reject `www.sub`
         zone = Zone('unit.tests.', ['sub'])
         with self.assertRaises(SubzoneRecordException) as ctx:
             source.populate(zone)
-        self.assertEquals('Record www.sub.unit.tests. is under a managed '
-                          'subzone', text_type(ctx.exception))
+        self.assertEqual(
+            'Record www.sub.unit.tests. is under a managed subzone',
+            str(ctx.exception),
+        )
+
+    def test_copy(self):
+        # going to put some sentinal values in here to ensure, these aren't
+        # valid, but we shouldn't hit any code that cares during this test
+        source = YamlProvider(
+            'test',
+            42,
+            default_ttl=43,
+            enforce_order=44,
+            populate_should_replace=45,
+            supports_root_ns=46,
+        )
+        copy = source.copy()
+        self.assertEqual(source.directory, copy.directory)
+        self.assertEqual(source.default_ttl, copy.default_ttl)
+        self.assertEqual(source.enforce_order, copy.enforce_order)
+        self.assertEqual(
+            source.populate_should_replace, copy.populate_should_replace
+        )
+        self.assertEqual(source.supports_root_ns, copy.supports_root_ns)
+
+        # same for split
+        source = SplitYamlProvider(
+            'test',
+            42,
+            extension=42.5,
+            default_ttl=43,
+            enforce_order=44,
+            populate_should_replace=45,
+            supports_root_ns=46,
+        )
+        copy = source.copy()
+        self.assertEqual(source.directory, copy.directory)
+        self.assertEqual(source.extension, copy.extension)
+        self.assertEqual(source.default_ttl, copy.default_ttl)
+        self.assertEqual(source.enforce_order, copy.enforce_order)
+        self.assertEqual(
+            source.populate_should_replace, copy.populate_should_replace
+        )
+        self.assertEqual(source.supports_root_ns, copy.supports_root_ns)
+
+
+class TestOverridingYamlProvider(TestCase):
+    def test_provider(self):
+        config = join(dirname(__file__), 'config')
+        override_config = join(dirname(__file__), 'config', 'override')
+        base = YamlProvider(
+            'base',
+            config,
+            populate_should_replace=False,
+            supports_root_ns=False,
+        )
+        override = YamlProvider(
+            'test',
+            override_config,
+            populate_should_replace=True,
+            supports_root_ns=False,
+        )
+
+        zone = Zone('dynamic.tests.', [])
+
+        # Load the base, should see the 5 records
+        base.populate(zone)
+        got = {r.name: r for r in zone.records}
+        self.assertEqual(6, len(got))
+        # We get the "dynamic" A from the base config
+        self.assertTrue('dynamic' in got['a'].data)
+        # No added
+        self.assertFalse('added' in got)
+
+        # Load the overrides, should replace one and add 1
+        override.populate(zone)
+        got = {r.name: r for r in zone.records}
+        self.assertEqual(7, len(got))
+        # 'a' was replaced with a generic record
+        self.assertEqual(
+            {'ttl': 3600, 'values': ['4.4.4.4', '5.5.5.5']}, got['a'].data
+        )
+        # And we have the new one
+        self.assertTrue('added' in got)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `octodns-0.9.9/tests/test_octodns_equality.py` & `octodns-1.0.0rc0/tests/test_octodns_equality.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
 from unittest import TestCase
 
 from octodns.equality import EqualityTupleMixin
 
 
 class TestEqualityTupleMixin(TestCase):
-
     def test_basics(self):
-
         class Simple(EqualityTupleMixin):
-
             def __init__(self, a, b, c):
                 self.a = a
                 self.b = b
                 self.c = c
 
             def _equality_tuple(self):
                 return (self.a, self.b)
 
         one = Simple(1, 2, 3)
         same = Simple(1, 2, 3)
         matches = Simple(1, 2, 'ignored')
         doesnt = Simple(2, 3, 4)
 
         # equality
-        self.assertEquals(one, one)
-        self.assertEquals(one, same)
-        self.assertEquals(same, one)
+        self.assertEqual(one, one)
+        self.assertEqual(one, same)
+        self.assertEqual(same, one)
         # only a & c are considered
-        self.assertEquals(one, matches)
-        self.assertEquals(matches, one)
-        self.assertNotEquals(one, doesnt)
-        self.assertNotEquals(doesnt, one)
+        self.assertEqual(one, matches)
+        self.assertEqual(matches, one)
+        self.assertNotEqual(one, doesnt)
+        self.assertNotEqual(doesnt, one)
 
         # lt
         self.assertTrue(one < doesnt)
         self.assertFalse(doesnt < one)
         self.assertFalse(one < same)
 
         # le
@@ -56,13 +50,12 @@
 
         # ge
         self.assertFalse(one >= doesnt)
         self.assertTrue(doesnt >= one)
         self.assertTrue(one >= same)
 
     def test_not_implemented(self):
-
         class MissingMethod(EqualityTupleMixin):
             pass
 
         with self.assertRaises(NotImplementedError):
             MissingMethod() == MissingMethod()
```

### Comparing `octodns-0.9.9/tests/test_octodns_source_tinydns.py` & `octodns-1.0.0rc0/tests/test_octodns_source_tinydns.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,187 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
 from unittest import TestCase
 
+from helpers import SimpleProvider
+
 from octodns.record import Record
 from octodns.source.tinydns import TinyDnsFileSource
 from octodns.zone import Zone
 
-from helpers import SimpleProvider
-
 
 class TestTinyDnsFileSource(TestCase):
     source = TinyDnsFileSource('test', './tests/zones/tinydns')
 
     def test_populate_normal(self):
         got = Zone('example.com.', [])
         self.source.populate(got)
-        self.assertEquals(17, len(got.records))
+        self.assertEqual(17, len(got.records))
 
         expected = Zone('example.com.', [])
         for name, data in (
-            ('', {
-                'type': 'A',
-                'ttl': 30,
-                'values': ['10.2.3.4', '10.2.3.5'],
-            }),
-            ('sub', {
-                'type': 'NS',
-                'ttl': 30,
-                'values': ['ns1.ns.com.', 'ns2.ns.com.'],
-            }),
-            ('www', {
-                'type': 'A',
-                'ttl': 3600,
-                'value': '10.2.3.6',
-            }),
-            ('cname', {
-                'type': 'CNAME',
-                'ttl': 3600,
-                'value': 'www.example.com.',
-            }),
-            ('some-host-abc123', {
-                'type': 'A',
-                'ttl': 1800,
-                'value': '10.2.3.7',
-            }),
-            ('has-dup-def123', {
-                'type': 'A',
-                'ttl': 3600,
-                'value': '10.2.3.8',
-            }),
-            ('www.sub', {
-                'type': 'A',
-                'ttl': 3600,
-                'value': '1.2.3.4',
-            }),
-            ('has-dup-def456', {
-                'type': 'A',
-                'ttl': 3600,
-                'value': '10.2.3.8',
-            }),
-            ('', {
-                'type': 'MX',
-                'ttl': 3600,
-                'values': [{
-                    'preference': 10,
-                    'exchange': 'smtp-1-host.example.com.',
-                }, {
-                    'preference': 20,
-                    'exchange': 'smtp-2-host.example.com.',
-                }]
-            }),
-            ('smtp', {
-                'type': 'MX',
-                'ttl': 1800,
-                'values': [{
-                    'preference': 30,
-                    'exchange': 'smtp-1-host.example.com.',
-                }, {
-                    'preference': 40,
-                    'exchange': 'smtp-2-host.example.com.',
-                }]
-            }),
-            ('', {
-                'type': 'TXT',
-                'ttl': 300,
-                'value': 'test TXT',
-            }),
-            ('colon', {
-                'type': 'TXT',
-                'ttl': 300,
-                'value': 'test : TXT',
-            }),
-            ('nottl', {
-                'type': 'TXT',
-                'ttl': 3600,
-                'value': 'nottl test TXT',
-            }),
-            ('ipv6-3', {
-                'type': 'AAAA',
-                'ttl': 300,
-                'value': '2a02:1348:017c:d5d0:0024:19ff:fef3:5742',
-            }),
-            ('ipv6-6', {
-                'type': 'AAAA',
-                'ttl': 3600,
-                'value': '2a02:1348:017c:d5d0:0024:19ff:fef3:5743',
-            }),
-            ('semicolon', {
-                'type': 'TXT',
-                'ttl': 300,
-                'value': 'v=DKIM1\\; k=rsa\\; p=blah',
-            }),
+            ('', {'type': 'A', 'ttl': 30, 'values': ['10.2.3.4', '10.2.3.5']}),
+            (
+                '',
+                {
+                    'type': 'NS',
+                    'ttl': 3600,
+                    'values': ['ns1.ns.com.', 'ns2.ns.com.'],
+                },
+            ),
+            (
+                'sub',
+                {
+                    'type': 'NS',
+                    'ttl': 30,
+                    'values': ['ns3.ns.com.', 'ns4.ns.com.'],
+                },
+            ),
+            ('www', {'type': 'A', 'ttl': 3600, 'value': '10.2.3.6'}),
+            (
+                'cname',
+                {'type': 'CNAME', 'ttl': 3600, 'value': 'www.example.com.'},
+            ),
+            (
+                'some-host-abc123',
+                {'type': 'A', 'ttl': 1800, 'value': '10.2.3.7'},
+            ),
+            ('has-dup-def123', {'type': 'A', 'ttl': 3600, 'value': '10.2.3.8'}),
+            ('www.sub', {'type': 'A', 'ttl': 3600, 'value': '1.2.3.4'}),
+            ('has-dup-def456', {'type': 'A', 'ttl': 3600, 'value': '10.2.3.8'}),
+            (
+                '',
+                {
+                    'type': 'MX',
+                    'ttl': 3600,
+                    'values': [
+                        {
+                            'preference': 10,
+                            'exchange': 'smtp-1-host.example.com.',
+                        },
+                        {
+                            'preference': 20,
+                            'exchange': 'smtp-2-host.example.com.',
+                        },
+                    ],
+                },
+            ),
+            (
+                'smtp',
+                {
+                    'type': 'MX',
+                    'ttl': 1800,
+                    'values': [
+                        {
+                            'preference': 30,
+                            'exchange': 'smtp-1-host.example.com.',
+                        },
+                        {
+                            'preference': 40,
+                            'exchange': 'smtp-2-host.example.com.',
+                        },
+                    ],
+                },
+            ),
+            ('', {'type': 'TXT', 'ttl': 300, 'value': 'test TXT'}),
+            ('colon', {'type': 'TXT', 'ttl': 300, 'value': 'test : TXT'}),
+            ('nottl', {'type': 'TXT', 'ttl': 3600, 'value': 'nottl test TXT'}),
+            (
+                'ipv6-3',
+                {
+                    'type': 'AAAA',
+                    'ttl': 300,
+                    'value': '2a02:1348:017c:d5d0:0024:19ff:fef3:5742',
+                },
+            ),
+            (
+                'ipv6-6',
+                {
+                    'type': 'AAAA',
+                    'ttl': 3600,
+                    'value': '2a02:1348:017c:d5d0:0024:19ff:fef3:5743',
+                },
+            ),
+            (
+                'semicolon',
+                {
+                    'type': 'TXT',
+                    'ttl': 300,
+                    'value': 'v=DKIM1\\; k=rsa\\; p=blah',
+                },
+            ),
         ):
             record = Record.new(expected, name, data)
             expected.add_record(record)
 
         changes = expected.changes(got, SimpleProvider())
-        self.assertEquals([], changes)
+        self.assertEqual([], changes)
 
     def test_populate_normal_sub1(self):
         got = Zone('asdf.subtest.com.', [])
         self.source.populate(got)
-        self.assertEquals(1, len(got.records))
+        self.assertEqual(1, len(got.records))
 
         expected = Zone('asdf.subtest.com.', [])
         for name, data in (
-            ('a3', {
-                'type': 'A',
-                'ttl': 3600,
-                'values': ['10.2.3.7'],
-            }),
+            ('a3', {'type': 'A', 'ttl': 3600, 'values': ['10.2.3.7']}),
         ):
             record = Record.new(expected, name, data)
             expected.add_record(record)
 
         changes = expected.changes(got, SimpleProvider())
-        self.assertEquals([], changes)
+        self.assertEqual([], changes)
 
     def test_populate_normal_sub2(self):
         got = Zone('blah-asdf.subtest.com.', [])
         self.source.populate(got)
-        self.assertEquals(2, len(got.records))
+        self.assertEqual(2, len(got.records))
 
         expected = Zone('sub-asdf.subtest.com.', [])
         for name, data in (
-            ('a1', {
-                'type': 'A',
-                'ttl': 3600,
-                'values': ['10.2.3.5'],
-            }),
-            ('a2', {
-                'type': 'A',
-                'ttl': 3600,
-                'values': ['10.2.3.6'],
-            }),
+            ('a1', {'type': 'A', 'ttl': 3600, 'values': ['10.2.3.5']}),
+            ('a2', {'type': 'A', 'ttl': 3600, 'values': ['10.2.3.6']}),
         ):
             record = Record.new(expected, name, data)
             expected.add_record(record)
 
         changes = expected.changes(got, SimpleProvider())
-        self.assertEquals([], changes)
+        self.assertEqual([], changes)
 
     def test_populate_in_addr_arpa(self):
 
         got = Zone('3.2.10.in-addr.arpa.', [])
         self.source.populate(got)
 
         expected = Zone('3.2.10.in-addr.arpa.', [])
         for name, data in (
-            ('10', {
-                'type': 'PTR',
-                'ttl': 3600,
-                'value': 'a-ptr.example.com.'
-            }),
-            ('11', {
-                'type': 'PTR',
-                'ttl': 30,
-                'value': 'a-ptr-2.example.com.'
-            }),
-            ('8', {
-                'type': 'PTR',
-                'ttl': 3600,
-                'value': 'has-dup-def123.example.com.'
-            }),
-            ('7', {
-                'type': 'PTR',
-                'ttl': 1800,
-                'value': 'some-host-abc123.example.com.'
-            }),
+            ('10', {'type': 'PTR', 'ttl': 3600, 'value': 'a-ptr.example.com.'}),
+            ('11', {'type': 'PTR', 'ttl': 30, 'value': 'a-ptr-2.example.com.'}),
+            (
+                '8',
+                {
+                    'type': 'PTR',
+                    'ttl': 3600,
+                    'value': 'has-dup-def123.example.com.',
+                },
+            ),
+            (
+                '7',
+                {
+                    'type': 'PTR',
+                    'ttl': 1800,
+                    'value': 'some-host-abc123.example.com.',
+                },
+            ),
         ):
             record = Record.new(expected, name, data)
             expected.add_record(record)
 
         changes = expected.changes(got, SimpleProvider())
-        self.assertEquals([], changes)
+        self.assertEqual([], changes)
 
     def test_ignores_subs(self):
         got = Zone('example.com.', ['sub'])
         self.source.populate(got)
-        self.assertEquals(16, len(got.records))
+        self.assertEqual(16, len(got.records))
```

### Comparing `octodns-0.9.9/tests/helpers.py` & `octodns-1.0.0rc0/tests/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #
 #
 #
 
-from __future__ import absolute_import, division, print_function, \
-    unicode_literals
-
+from logging import getLogger
 from shutil import rmtree
 from tempfile import mkdtemp
 
+from octodns.processor.base import BaseProcessor
+from octodns.provider.base import BaseProvider
+from octodns.provider.yaml import YamlProvider
 
-class SimpleSource(object):
 
+class SimpleSource(object):
     def __init__(self, id='test'):
         pass
 
 
 class SimpleProvider(object):
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = False
@@ -33,14 +34,15 @@
     def __repr__(self):
         return self.__class__.__name__
 
 
 class GeoProvider(object):
     SUPPORTS_GEO = True
     SUPPORTS_DYNAMIC = False
+    SUPPORTS = set(('A', 'AAAA', 'TXT'))
     id = 'test'
 
     def __init__(self, id='test'):
         pass
 
     def populate(self, zone, source=False, lenient=False):
         pass
@@ -51,14 +53,15 @@
     def __repr__(self):
         return self.__class__.__name__
 
 
 class DynamicProvider(object):
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = True
+    SUPPORTS = set(('A', 'AAAA', 'TXT'))
     id = 'test'
 
     def __init__(self, id='test'):
         pass
 
     def populate(self, zone, source=False, lenient=False):
         pass
@@ -67,26 +70,67 @@
         return True
 
     def __repr__(self):
         return self.__class__.__name__
 
 
 class NoSshFpProvider(SimpleProvider):
-
     def supports(self, record):
         return record._type != 'SSHFP'
 
 
 class TemporaryDirectory(object):
-
     def __init__(self, delete_on_exit=True):
         self.delete_on_exit = delete_on_exit
 
     def __enter__(self):
         self.dirname = mkdtemp()
         return self
 
     def __exit__(self, *args, **kwargs):
         if self.delete_on_exit:
             rmtree(self.dirname)
         else:
             raise Exception(self.dirname)
+
+
+class WantsConfigProcessor(BaseProcessor):
+    def __init__(self, name, some_config):
+        super().__init__(name)
+
+
+class PlannableProvider(BaseProvider):
+    log = getLogger('PlannableProvider')
+
+    SUPPORTS_GEO = False
+    SUPPORTS_DYNAMIC = False
+    SUPPORTS = set(('A', 'AAAA', 'TXT'))
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def populate(self, zone, source=False, target=False, lenient=False):
+        pass
+
+    def supports(self, record):
+        return True
+
+    def __repr__(self):
+        return self.__class__.__name__
+
+
+class TestYamlProvider(YamlProvider):
+    pass
+
+
+class TestBaseProcessor(BaseProcessor):
+    pass
+
+
+class CountingProcessor(BaseProcessor):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.count = 0
+
+    def process_source_zone(self, zone, *args, **kwargs):
+        self.count += len(zone.records)
+        return zone
```

### Comparing `octodns-0.9.9/docs/geo_records.md` & `octodns-1.0.0rc0/docs/geo_records.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Geo Record Support
 
-Note: Geo DNS records are still supported for the time being, but it is still strongy encouraged that you look at [Dynamic Records](/docs/dynamic_records.md) instead as they are a superset of functionality.
+Note: Geo DNS records are still supported for the time being, but it is still strongly encouraged that you look at [Dynamic Records](/docs/dynamic_records.md) instead as they are a superset of functionality.
 
 GeoDNS is currently supported for `A` and `AAAA` records on the Dyn (via Traffic Directors) and Route53 providers. Records with geo information pushed to providers without support for them will be managed as non-geo records using the base values.
 
 Configuring GeoDNS is complex and the details of the functionality vary widely from provider to provider. OctoDNS has an opinionated view of how GeoDNS should be set up and does its best to map that to each provider's offering in a way that will result in similar behavior. It may not fit your needs or use cases, in which case please open an issue for discussion. We expect this functionality to grow and evolve over time as it's more widely used.
 
 The following is an example of GeoDNS with three entries NA-US-CA, NA-US-NY, OC-AU. Octodns creates another one labeled 'default' with the details for the actual A record, This default record is the failover record if the monitoring check fails.
 
@@ -82,20 +82,22 @@
 | protocol | HTTP/HTTPS | HTTPS |
 
 #### Route53 Healtch Check Options
 
 | Key  | Description | Default |
 |--|--|--|
 | measure_latency | Show latency in AWS console | true |
+| request_interval | Healthcheck interval [10\|30] seconds | 10 |
 
 ```yaml
 ---
   octodns:
     healthcheck:
       host: my-host-name
       path: /dns-health-check
       port: 443
       protocol: HTTPS
     route53:
       healthcheck:
         measure_latency: false
+        request_interval: 30
 ```
```

### Comparing `octodns-0.9.9/docs/records.md` & `octodns-1.0.0rc0/docs/auto_arpa.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,102 @@
-# OctoDNS records
+## Automatic PTR Generation With auto_arpa
 
-## Record types
+octoDNS supports the automatic generation of `PTR` records for in-addr.arpa. and ip6.arpa. zones. In order to enable the functionality the `auto_arpa` key needs to be passed to the manager configuration.
 
-OctoDNS supports the following record types:
+```yaml
+---
+manager:
+  auto_arpa: true
+```
 
-* `A`
-* `AAAA`
-* `CNAME`
-* `MX`
-* `NAPTR`
-* `NS`
-* `PTR`
-* `SSHFP`
-* `SPF`
-* `SRV`
-* `TXT`
+Alternatively the value can be a dictionary with configuration options for the AutoArpa processor/provider.
 
-Underlying provider support for each of these varies and some providers have extra requirements or limitations. In cases where a record type is not supported by a provider OctoDNS will ignore it there and continue to manage the record elsewhere. For example `SSHFP` is supported by Dyn, but not Route53. If your source data includes an SSHFP record OctoDNS will keep it in sync on Dyn, but not consider it when evaluating the state of Route53. The best way to find out what types are supported by a provider is to look for its `supports` method. If that method exists the logic will drive which records are supported and which are ignored. If the provider does not implement the method it will fall back to `BaseProvider.supports` which indicates full support.
+```yaml
+---
+manager:
+  auto_arpa:
+    # Whether duplicate records should replace rather than error
+    # (optiona, default False)
+    populate_should_replace: false
+    # Explicitly set the TTL of auto-created records, default is 3600s, 1hr
+    ttl: 1800
+```
 
-Adding new record types to OctoDNS is relatively straightforward, but will require careful evaluation of each provider to determine whether or not it will be supported and the addition of code in each to handle and test the new type.
+Once enabled a singleton `AutoArpa` instance, `auto-arpa`, will be added to the pool of providers and globally configured to run as the very last global processor so that it will see all records as they will be seen by targets. Further all zones ending with `arpa.` will be held back and processed after all other zones have been completed so that all `A` and `AAAA` records will have been seen prior to planning the `arpa.` zones.
 
-## Advanced Record Support (GeoDNS, Weighting)
+In order to add `PTR` records for a zone the `auto-arpa` source should be added to the list of sources for the zone.
 
-* [Dynamic Records](/docs/dynamic_records.md) - the preferred method for configuring geo-location, weights, and healthcheck based fallback between pools of services.
-* [Geo Records](/docs/geo_records.md) - the original implementation of geo-location based records, now superseded by Dynamic Records (above)
+```yaml
+# Zones are matched on suffix so `0.10.in-addr.arpa.` would match anything
+# under `10.0/16` or `0.8.e.f.ip6-.arpa.` would match any IPv6 address under
+# `fe80::`, 0.0.10 here matches 10.0.0/24.
+0.0.10.in-addr.arpa.:
+  sources:
+    # In most cases you'll have some statically configured records combined in
+    # with the auto-generated records as shown here, but that's not strictly
+    # required and this could just be `auto-arpa`.
+    # would throw an DuplicateRecordException.
+    - config
+    - auto-arpa
+  targets:
+    - ...
+```
+
+The above will add `PTR` records for any `A` records previously seen with IP addresses 10.0.0.*.
 
-## Config (`YamlProvider`)
+### A Complete Example
 
-OctoDNS records and `YamlProvider`'s schema is essentially a 1:1 match. Properties on the objects will match keys in the config.
+#### config/octodns.yaml
+
+```yaml
+manager:
+  auto_arpa: true
 
-### Names
+providers:
+  config:
+    class: octodns.provider.yaml.YamlProvider
+    directory: tests/config
+
+  route53:
+    class: octodns_route53.Route53Provider
+    access_key_id: env/AWS_ACCESS_KEY_ID
+    secret_access_key: env/AWS_SECRET_ACCESS_KEY
+
+zones:
+  exxampled.com.:
+    sources:
+      - config
+    targets:
+      - route53
+
+  0.0.10.in-addr.arpa.:
+    sources:
+      - auto-arpa
+    targets:
+      - route53
+```
 
-Each top-level key in the yaml file is a record name. Two common special cases are the root record `''`, and a wildcard `'*'`.
+#### config/exxampled.com.yaml
 
 ```yaml
----
-'':
-  type: A
+? ''
+: type: A
   values:
-    - 1.2.3.4
-    - 1.2.3.5
-'*':
-  type: CNAME
-  value: www.example.com.
-www:
+  - 10.0.0.101
+  - 10.0.0.102
+email:
   type: A
-  values:
-    - 1.2.3.4
-    - 1.2.3.5
-www.sub:
+  value: 10.0.0.103
+fileserver:
   type: A
-  values:
-    - 1.2.3.6
-    - 1.2.3.7
+  value: 10.0.0.103
 ```
 
-The above config lays out 4 records, `A`s for `example.com.`, `www.example.com.`, and `www.sub.example.com` and a wildcard `CNAME` mapping `*.example.com.` to `www.example.com.`.
-
-### Multiple records
-
-In the above example each name had a single record, but there are cases where a name will need to have multiple records associated with it. This can be accomplished by using a list.
-
-```yaml
----
-'':
-  - type: A
-    values:
-      - 1.2.3.4
-      - 1.2.3.5
-  - type: MX
-    values:
-      - exchange: mx1.example.com.
-        preference: 10
-      - exchange: mx2.example.com.
-        preference: 10
-```
+#### Auto-generated PTRs
 
-### Record data
+* 101.0.0.10: exxampled.com.
+* 102.0.0.10: exxampled.com.
+* 103.0.0.10: email.exxampled.com., fileserver.exxampled.com.
 
-Each record type has a corresponding set of required data. The easiest way to determine what's required is probably to look at the record object in [`octodns/record/__init__.py`](/octodns/record/__init__.py). You may also utilize `octodns-validate` which will throw errors about what's missing when run.
+### Notes
 
-`type` is required for all records. `ttl` is optional. When TTL is not specified the `YamlProvider`'s default will be used. In any situation where an array of `values` can be used you can opt to go with `value` as a single item if there's only one.
+Automatic `PTR` generation requires a "complete" picture of records and thus cannot be done during partial syncs. Thus syncing `arpa.` zones will throw an error any time filtering of zones, targets, or sources is being done.
```

### Comparing `octodns-0.9.9/script/cibuild` & `octodns-1.0.0rc0/script/cibuild`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/bin/sh
+
 set -e
 
 cd "$(dirname "$0")/.."
 
 echo "## bootstrap ###################################################################"
 script/bootstrap
 
-echo "## environment & versions ######################################################"
-python --version
-pip --version
-VVER=$(virtualenv --version)
-echo "virtualenv $VVER"
-
 if [ -z "$VENV_NAME" ]; then
     VENV_NAME="env"
 fi
 
 . "$VENV_NAME/bin/activate"
 
+echo "## environment & versions ######################################################"
+python --version
+pip --version
+
 echo "## clean up ####################################################################"
 find octodns tests -name "*.pyc" -exec rm {} \;
 rm -f *.pyc
 echo "## begin #######################################################################"
 # For now it's just lint...
 echo "## lint ########################################################################"
 script/lint
+echo "## formatting ##################################################################"
+script/format --check || (echo "Formatting check failed, run ./script/format" && exit 1)
 echo "## tests/coverage ##############################################################"
 script/coverage
-echo "## validate setup.py build #####################################################"
-python setup.py build
 echo "## complete ####################################################################"
```

### Comparing `octodns-0.9.9/script/test` & `octodns-1.0.0rc0/script/test`

 * *Files 24% similar despite different names*

```diff
@@ -21,9 +21,13 @@
 export CLOUDFLARE_TOKEN=
 export DNSIMPLE_ACCOUNT=
 export DNSIMPLE_TOKEN=
 export DYN_CUSTOMER=
 export DYN_PASSWORD=
 export DYN_USERNAME=
 export GOOGLE_APPLICATION_CREDENTIALS=
+export ARM_CLIENT_ID=
+export ARM_CLIENT_SECRET=
+export ARM_TENANT_ID=
+export ARM_SUBSCRIPTION_ID=
 
-nosetests "$@"
+pytest --disable-network "$@"
```

### Comparing `octodns-0.9.9/script/generate-geo-data` & `octodns-1.0.0rc0/script/generate-geo-data`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,88 @@
 #!/usr/bin/env python
 
 from collections import defaultdict
-from pprint import pformat
+
 from pycountry import countries, subdivisions
 from pycountry_convert import country_alpha2_to_continent_code
 
-
 subs = defaultdict(dict)
 for subdivision in subdivisions:
-    # Route53 only supports US states, Dyn supports US states and CA provinces, but for now we'll just do US
-    if subdivision.country_code not in ('US'):
+    # Route53 only supports US states, Dyn (and others) support US states and CA provinces
+    if subdivision.country_code not in ('US', 'CA'):
         continue
     subs[subdivision.country_code][subdivision.code[3:]] = {
         'name': subdivision.name
     }
 subs = dict(subs)
-#pprint(subs)
 
 # These are best guesses at things pycountry_convert doesn't map
 continent_backups = {
     'AQ': 'AN',
     'EH': 'AF',
     'PN': 'OC',
     'SX': 'NA',
     'TF': 'AN',
-    'TL': 'ID',
+    'TL': 'AS',
     'UM': 'OC',
     'VA': 'EU',
 }
 
 geos = defaultdict(dict)
 for country in countries:
     try:
         continent_code = country_alpha2_to_continent_code(country.alpha_2)
     except KeyError:
         try:
             continent_code = continent_backups[country.alpha_2]
         except KeyError:
             raise
-            print('{} {} {}'.format(country.alpha_2, country.name, getattr(country, 'official_name', '')))
+            print(
+                '{} {} {}'.format(
+                    country.alpha_2,
+                    country.name,
+                    getattr(country, 'official_name', ''),
+                )
+            )
 
-    geos[continent_code][country.alpha_2] = {
-        'name': country.name
-    }
+    geos[continent_code][country.alpha_2] = {'name': country.name}
 
     try:
-        geos[continent_code][country.alpha_2]['provinces'] = subs[country.alpha_2]
+        geos[continent_code][country.alpha_2]['provinces'] = subs[
+            country.alpha_2
+        ]
     except KeyError:
         pass
 
 geos = dict(geos)
-data = pformat(geos).replace('\n', '\n    ')
 
-print('''#
+print(
+    '''#
 # -*- coding: utf-8 -*-
 #
 # This file is generated using
 #   ./script/generate-geo-data > octodns/record/geo_data.py
 # do not modify it directly
 #
 
-geo_data = \\
-    {}'''.format(data))
+geo_data = {'''
+)
+
+for continent, details in sorted(geos.items()):
+    print(f"    '{continent}': {{")
+    for country, info in sorted(details.items()):
+        name = info['name']
+        quoted_name = f'"{name}"' if "'" in name else f"'{name}'"
+        if 'provinces' in info:
+            print(f"        '{country}': {{")
+            print(f"            'name': {quoted_name},")
+            print("            'provinces': {")
+            for prov, info in sorted(info['provinces'].items()):
+                name = info['name']
+                quoted_name = f'"{name}"' if "'" in name else f"'{name}'"
+                print(f"                '{prov}': {{'name': {quoted_name}}},")
+            print('            },')
+            print('        },')
+        else:
+            print(f"        '{country}': {{'name': {quoted_name}}},")
+    print('    },')
+print('}')
```

### Comparing `octodns-0.9.9/script/coverage` & `octodns-1.0.0rc0/script/coverage`

 * *Files 26% similar despite different names*

```diff
@@ -21,16 +21,30 @@
 export CLOUDFLARE_TOKEN=
 export DNSIMPLE_ACCOUNT=
 export DNSIMPLE_TOKEN=
 export DYN_CUSTOMER=
 export DYN_PASSWORD=
 export DYN_USERNAME=
 export GOOGLE_APPLICATION_CREDENTIALS=
+export ARM_CLIENT_ID=
+export ARM_CLIENT_SECRET=
+export ARM_TENANT_ID=
+export ARM_SUBSCRIPTION_ID=
 
-coverage run --branch --source=octodns --omit=octodns/cmds/* "$(command -v nosetests)" --with-xunit "$@"
-coverage html
-coverage xml
-coverage report --show-missing
-coverage report | grep ^TOTAL | grep -qv 100% && {
-    echo "Incomplete code coverage" >&2
+SOURCE_DIR="octodns/"
+
+# Don't allow disabling coverage
+grep -r -I --line-number "# pragma: +no.*cover" $SOURCE_DIR && {
+    echo "Code coverage should not be disabled"
     exit 1
-} || echo "Code coverage 100%"
+}
+
+pytest \
+  --disable-network \
+  --cov-reset \
+  --cov=$SOURCE_DIR \
+  --cov-fail-under=100 \
+  --cov-report=html \
+  --cov-report=xml \
+  --cov-report=term \
+  --cov-branch \
+  "$@"
```

### Comparing `octodns-0.9.9/CONTRIBUTING.md` & `octodns-1.0.0rc0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Contributing
 
 Hi there! We're thrilled that you'd like to contribute to OctoDNS. Your help is essential for keeping it great.
 
 Please note that this project adheres to the [Contributor Covenant Code of Conduct](/CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.
 
-If you have questions, or you'd like to check with us before embarking on a major development effort, please [open an issue](https://github.com/github/octodns/issues/new).
+If you have questions, or you'd like to check with us before embarking on a major development effort, please [open an issue](https://github.com/octodns/octodns/issues/new).
 
 ## How to contribute
 
-This project uses the [GitHub Flow](https://guides.github.com/introduction/flow/). That means that the `master` branch is stable and new development is done in feature branches. Feature branches are merged into the `master` branch via a Pull Request.
+This project uses the [GitHub Flow](https://guides.github.com/introduction/flow/). That means that the `main` branch is stable and new development is done in feature branches. Feature branches are merged into the `main` branch via a Pull Request.
 
 0. Fork and clone the repository
-0. Configure and install the dependencies: `script/bootstrap`
-0. Make sure the tests pass on your machine: `script/test`
+0. Configure and install the dependencies: `./script/bootstrap`
+0. Activate virtual environment: `source env/bin/activate`
+0. Make sure the tests pass on your machine: `./script/test`
 0. Create a new branch: `git checkout -b my-branch-name`
 0. Make your change, add tests, and make sure the tests still pass
 0. Make sure that `./script/lint` passes without any warnings
-0. Make sure that coverage is at :100:% `script/coverage` and open `htmlcov/index.html`
+0. Make sure that coverage is at :100:% `./script/coverage` and open `htmlcov/index.html`
    * You can open PRs for :eyes: & discussion prior to this
 0. Push to your fork and submit a pull request
 
 We will handle updating the version, tagging the release, and releasing the gem. Please don't bump the version or otherwise attempt to take on these administrative internal tasks as part of your pull request.
 
 Here are a few things you can do that will increase the likelihood of your pull request being accepted:
 
@@ -30,25 +31,27 @@
 
 - Bug fixes require specific tests covering the addressed behavior.
 
 - Write or update documentation. If you have added a feature or changed an existing one, please make appropriate changes to the docs. Doc-only PRs are always welcome.
 
 - Keep your change as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
 
-- We target Python 2.7, but have taken steps to make Python 3 support as easy as possible when someone decides it's needed. PR welcome.
+- We target Python 3, support for Python 2 has been dropped.
 
 - Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).
 
 ## Development setup
 
 ```
-pip install -r requirements.txt
-pip install -r requirements-dev.txt
+./script/bootstrap
+source env/bin/activate
 ```
 
+See the [`script/`](/script) if you'd like to run tests and coverage ([`script/coverage`](/script/coverage)) and coverage ([`script/lint`](/script/lint)). After bootstrapping and sourcing the `env/` commands in the [`octodns/cmds/`](/octodns/cmds) directory can be run with `PYTHONPATH=. ./octodns/cmds/sync.py ...`
+
 ## License note
 
 We can only accept contributions that are compatible with the MIT license.
 
 It's OK to depend on gems licensed under either Apache 2.0 or MIT, but we cannot add dependencies on any gems that are licensed under GPL.
 
 Any contributions you make must be under the MIT license.
```

