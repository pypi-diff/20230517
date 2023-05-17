# Comparing `tmp/pulumi_linode-4.1.0a1684215503.tar.gz` & `tmp/pulumi_linode-4.1.0a1684348483.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_linode-4.1.0a1684215503.tar", last modified: Tue May 16 05:49:05 2023, max compression
+gzip compressed data, was "pulumi_linode-4.1.0a1684348483.tar", last modified: Wed May 17 18:40:59 2023, max compression
```

## Comparing `pulumi_linode-4.1.0a1684215503.tar` & `pulumi_linode-4.1.0a1684348483.tar`

### file list

```diff
@@ -1,91 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:49:05.936182 pulumi_linode-4.1.0a1684215503/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-16 05:49:05.936182 pulumi_linode-4.1.0a1684215503/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:49:05.932182 pulumi_linode-4.1.0a1684215503/pulumi_linode/
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   135504 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/account_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:49:05.936182 pulumi_linode-4.1.0a1684215503/pulumi_linode/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/database_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    48347 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/database_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    42306 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    46601 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)    41162 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    34284 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    29693 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/firewall_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_mysql_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_domain_zonefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_linode_object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_lke_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_networking_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_stack_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_vlans.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    95659 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34192 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/instance_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/instance_shared_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    24387 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/object_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/object_storage_object.py
--rw-r--r--   0 runner    (1001) docker     (123)   256246 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/rdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    32829 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    40500 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:49:05.936182 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:49:05.936182 pulumi_linode-4.1.0a1684215503/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-16 05:49:05.000000 pulumi_linode-4.1.0a1684215503/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:40:59.284379 pulumi_linode-4.1.0a1684348483/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-17 18:40:59.284379 pulumi_linode-4.1.0a1684348483/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:40:59.284379 pulumi_linode-4.1.0a1684348483/pulumi_linode/
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130974 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/account_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:40:59.284379 pulumi_linode-4.1.0a1684348483/pulumi_linode/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/database_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/firewall_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_mysql_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_domain_zonefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_linode_object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_lke_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_networking_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_stack_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/instance_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/instance_shared_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/object_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/object_storage_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)   253542 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:40:59.284379 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-17 18:40:59.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-17 18:40:59.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:40:59.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:40:59.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 18:40:59.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 18:40:59.000000 pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:40:59.284379 pulumi_linode-4.1.0a1684348483/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-17 18:40:58.000000 pulumi_linode-4.1.0a1684348483/setup.py
```

### Comparing `pulumi_linode-4.1.0a1684215503/PKG-INFO` & `pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_linode
-Version: 4.1.0a1684215503
+Name: pulumi-linode
+Version: 4.1.0a1684348483
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.1.0a1684215503/README.md` & `pulumi_linode-4.1.0a1684348483/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/__init__.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .account_settings import *
 from .database_access_controls import *
-from .database_mongodb import *
 from .database_mysql import *
 from .database_postgresql import *
 from .domain import *
 from .domain_record import *
 from .firewall import *
 from .firewall_device import *
 from .get_account import *
 from .get_account_login import *
 from .get_account_logins import *
 from .get_account_settings import *
 from .get_database_backups import *
 from .get_database_engines import *
-from .get_database_mongodb import *
 from .get_database_mysql import *
 from .get_database_mysql_backups import *
 from .get_database_postgresql import *
 from .get_databases import *
 from .get_domain import *
 from .get_domain_record import *
 from .get_domain_zonefile import *
@@ -68,14 +66,15 @@
 from .object_storage_bucket import *
 from .object_storage_key import *
 from .object_storage_object import *
 from .provider import *
 from .rdns import *
 from .ssh_key import *
 from .stack_script import *
+from .token import *
 from .user import *
 from .volume import *
 from ._inputs import *
 from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
@@ -101,22 +100,14 @@
   "fqn": "pulumi_linode",
   "classes": {
    "linode:index/databaseAccessControls:DatabaseAccessControls": "DatabaseAccessControls"
   }
  },
  {
   "pkg": "linode",
-  "mod": "index/databaseMongodb",
-  "fqn": "pulumi_linode",
-  "classes": {
-   "linode:index/databaseMongodb:DatabaseMongodb": "DatabaseMongodb"
-  }
- },
- {
-  "pkg": "linode",
   "mod": "index/databaseMysql",
   "fqn": "pulumi_linode",
   "classes": {
    "linode:index/databaseMysql:DatabaseMysql": "DatabaseMysql"
   }
  },
  {
@@ -285,14 +276,22 @@
   "fqn": "pulumi_linode",
   "classes": {
    "linode:index/stackScript:StackScript": "StackScript"
   }
  },
  {
   "pkg": "linode",
+  "mod": "index/token",
+  "fqn": "pulumi_linode",
+  "classes": {
+   "linode:index/token:Token": "Token"
+  }
+ },
+ {
+  "pkg": "linode",
   "mod": "index/user",
   "fqn": "pulumi_linode",
   "classes": {
    "linode:index/user:User": "User"
   }
  },
  {
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/_inputs.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'DatabaseMongodbUpdatesArgs',
     'DatabaseMysqlUpdatesArgs',
     'DatabasePostgresqlUpdatesArgs',
     'FirewallDeviceArgs',
     'FirewallInboundArgs',
     'FirewallOutboundArgs',
     'InstanceAlertsArgs',
     'InstanceBackupsArgs',
@@ -60,89 +59,27 @@
     'GetDatabaseEnginesFilterArgs',
     'GetDatabaseMysqlBackupsFilterArgs',
     'GetDatabasesFilterArgs',
     'GetImagesFilterArgs',
     'GetInstanceTypesFilterArgs',
     'GetInstancesFilterArgs',
     'GetRegionsFilterArgs',
-    'GetStackScriptUserDefinedFieldArgs',
     'GetStackScriptsFilterArgs',
     'GetUserDomainGrantArgs',
     'GetUserFirewallGrantArgs',
     'GetUserImageGrantArgs',
     'GetUserLinodeGrantArgs',
     'GetUserLongviewGrantArgs',
     'GetUserNodebalancerGrantArgs',
     'GetUserStackscriptGrantArgs',
     'GetUserVolumeGrantArgs',
     'GetVlansFilterArgs',
 ]
 
 @pulumi.input_type
-class DatabaseMongodbUpdatesArgs:
-    def __init__(__self__, *,
-                 day_of_week: pulumi.Input[str],
-                 duration: pulumi.Input[int],
-                 frequency: pulumi.Input[str],
-                 hour_of_day: pulumi.Input[int],
-                 week_of_month: Optional[pulumi.Input[int]] = None):
-        pulumi.set(__self__, "day_of_week", day_of_week)
-        pulumi.set(__self__, "duration", duration)
-        pulumi.set(__self__, "frequency", frequency)
-        pulumi.set(__self__, "hour_of_day", hour_of_day)
-        if week_of_month is not None:
-            pulumi.set(__self__, "week_of_month", week_of_month)
-
-    @property
-    @pulumi.getter(name="dayOfWeek")
-    def day_of_week(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "day_of_week")
-
-    @day_of_week.setter
-    def day_of_week(self, value: pulumi.Input[str]):
-        pulumi.set(self, "day_of_week", value)
-
-    @property
-    @pulumi.getter
-    def duration(self) -> pulumi.Input[int]:
-        return pulumi.get(self, "duration")
-
-    @duration.setter
-    def duration(self, value: pulumi.Input[int]):
-        pulumi.set(self, "duration", value)
-
-    @property
-    @pulumi.getter
-    def frequency(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "frequency")
-
-    @frequency.setter
-    def frequency(self, value: pulumi.Input[str]):
-        pulumi.set(self, "frequency", value)
-
-    @property
-    @pulumi.getter(name="hourOfDay")
-    def hour_of_day(self) -> pulumi.Input[int]:
-        return pulumi.get(self, "hour_of_day")
-
-    @hour_of_day.setter
-    def hour_of_day(self, value: pulumi.Input[int]):
-        pulumi.set(self, "hour_of_day", value)
-
-    @property
-    @pulumi.getter(name="weekOfMonth")
-    def week_of_month(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "week_of_month")
-
-    @week_of_month.setter
-    def week_of_month(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "week_of_month", value)
-
-
-@pulumi.input_type
 class DatabaseMysqlUpdatesArgs:
     def __init__(__self__, *,
                  day_of_week: pulumi.Input[str],
                  duration: pulumi.Input[int],
                  frequency: pulumi.Input[str],
                  hour_of_day: pulumi.Input[int],
                  week_of_month: Optional[pulumi.Input[int]] = None):
@@ -714,14 +651,16 @@
         """
         :param pulumi.Input[str] label: The Linode's label is for display purposes only. If no label is provided for a Linode, a default will be assigned.
         :param pulumi.Input[str] comments: Arbitrary user comments about this `config`.
         :param pulumi.Input['InstanceConfigDevicesArgs'] devices: A list of `disk` or `volume` attachments for this `config`.  If the `boot_config_label` omits a `devices` block, the Linode will not be booted.
         :param pulumi.Input['InstanceConfigHelpersArgs'] helpers: Helpers enabled when booting to this Linode Config.
         :param pulumi.Input[str] kernel: A Kernel ID to boot a Linode with. Default is based on image choice. Examples are `linode/latest-64bit`, `linode/grub2`, `linode/direct-disk`, etc. See all kernels [here](https://api.linode.com/v4/linode/kernels). Note that this is a paginated API endpoint ([docs](https://developers.linode.com/api/v4/linode-kernels)).
         :param pulumi.Input[int] memory_limit: Defaults to the total RAM of the Linode
+               
+               * `interface` - (Optional) A list of network interfaces to be assigned to the Linode.
         :param pulumi.Input[str] root_device: The root device to boot. The corresponding disk must be attached to a `device` slot.  Example: `"/dev/sda"`
         :param pulumi.Input[str] run_level: Defines the state of your Linode after booting. Defaults to `"default"`.
         :param pulumi.Input[str] virt_mode: Controls the virtualization mode. Defaults to `"paravirt"`.
         """
         pulumi.set(__self__, "label", label)
         if comments is not None:
             pulumi.set(__self__, "comments", comments)
@@ -812,14 +751,16 @@
         pulumi.set(self, "kernel", value)
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[pulumi.Input[int]]:
         """
         Defaults to the total RAM of the Linode
+
+        * `interface` - (Optional) A list of network interfaces to be assigned to the Linode.
         """
         return pulumi.get(self, "memory_limit")
 
     @memory_limit.setter
     def memory_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "memory_limit", value)
 
@@ -1863,14 +1804,16 @@
                  count: pulumi.Input[int],
                  type: pulumi.Input[str],
                  autoscaler: Optional[pulumi.Input['LkeClusterPoolAutoscalerArgs']] = None,
                  id: Optional[pulumi.Input[int]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input['LkeClusterPoolNodeArgs']]]] = None):
         """
         :param pulumi.Input[int] count: The number of nodes in the Node Pool.
+               
+               * `autoscaler` - (Optional) If defined, an autoscaler will be enabled with the given configuration.
         :param pulumi.Input[str] type: A Linode Type for all of the nodes in the Node Pool. See all node types [here](https://api.linode.com/v4/linode/types).
         :param pulumi.Input[int] id: The ID of the node.
         """
         pulumi.set(__self__, "count", count)
         pulumi.set(__self__, "type", type)
         if autoscaler is not None:
             pulumi.set(__self__, "autoscaler", autoscaler)
@@ -1880,14 +1823,16 @@
             pulumi.set(__self__, "nodes", nodes)
 
     @property
     @pulumi.getter
     def count(self) -> pulumi.Input[int]:
         """
         The number of nodes in the Node Pool.
+
+        * `autoscaler` - (Optional) If defined, an autoscaler will be enabled with the given configuration.
         """
         return pulumi.get(self, "count")
 
     @count.setter
     def count(self, value: pulumi.Input[int]):
         pulumi.set(self, "count", value)
 
@@ -2165,14 +2110,18 @@
                  expiration: Optional[pulumi.Input['ObjectStorageBucketLifecycleRuleExpirationArgs']] = None,
                  id: Optional[pulumi.Input[str]] = None,
                  noncurrent_version_expiration: Optional[pulumi.Input['ObjectStorageBucketLifecycleRuleNoncurrentVersionExpirationArgs']] = None,
                  prefix: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] enabled: Specifies whether the lifecycle rule is active.
         :param pulumi.Input[int] abort_incomplete_multipart_upload_days: Specifies the number of days after initiating a multipart upload when the multipart upload must be completed.
+               
+               * `expiration` - (Optional) Specifies a period in the object's expire.
+               
+               * `noncurrent_version_expiration` - (Optional) Specifies when non-current object versions expire.
         :param pulumi.Input[str] id: The unique identifier for the rule.
         :param pulumi.Input[str] prefix: The object key prefix identifying one or more objects to which the rule applies.
         """
         pulumi.set(__self__, "enabled", enabled)
         if abort_incomplete_multipart_upload_days is not None:
             pulumi.set(__self__, "abort_incomplete_multipart_upload_days", abort_incomplete_multipart_upload_days)
         if expiration is not None:
@@ -2197,14 +2146,18 @@
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="abortIncompleteMultipartUploadDays")
     def abort_incomplete_multipart_upload_days(self) -> Optional[pulumi.Input[int]]:
         """
         Specifies the number of days after initiating a multipart upload when the multipart upload must be completed.
+
+        * `expiration` - (Optional) Specifies a period in the object's expire.
+
+        * `noncurrent_version_expiration` - (Optional) Specifies when non-current object versions expire.
         """
         return pulumi.get(self, "abort_incomplete_multipart_upload_days")
 
     @abort_incomplete_multipart_upload_days.setter
     def abort_incomplete_multipart_upload_days(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "abort_incomplete_multipart_upload_days", value)
 
@@ -2379,111 +2332,105 @@
     def permissions(self, value: pulumi.Input[str]):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class StackScriptUserDefinedFieldArgs:
     def __init__(__self__, *,
-                 default: Optional[pulumi.Input[str]] = None,
-                 example: Optional[pulumi.Input[str]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
-                 many_of: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 one_of: Optional[pulumi.Input[str]] = None):
+                 default: pulumi.Input[str],
+                 example: pulumi.Input[str],
+                 label: pulumi.Input[str],
+                 many_of: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 one_of: pulumi.Input[str]):
         """
         :param pulumi.Input[str] default: The default value. If not specified, this value will be used.
         :param pulumi.Input[str] example: An example value for the field.
         :param pulumi.Input[str] label: The StackScript's label is for display purposes only.
         :param pulumi.Input[str] many_of: A list of acceptable values for the field in any quantity, combination or order.
         :param pulumi.Input[str] name: The name of the field.
         :param pulumi.Input[str] one_of: A list of acceptable single values for the field.
         """
-        if default is not None:
-            pulumi.set(__self__, "default", default)
-        if example is not None:
-            pulumi.set(__self__, "example", example)
-        if label is not None:
-            pulumi.set(__self__, "label", label)
-        if many_of is not None:
-            pulumi.set(__self__, "many_of", many_of)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if one_of is not None:
-            pulumi.set(__self__, "one_of", one_of)
+        pulumi.set(__self__, "default", default)
+        pulumi.set(__self__, "example", example)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "many_of", many_of)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "one_of", one_of)
 
     @property
     @pulumi.getter
-    def default(self) -> Optional[pulumi.Input[str]]:
+    def default(self) -> pulumi.Input[str]:
         """
         The default value. If not specified, this value will be used.
         """
         return pulumi.get(self, "default")
 
     @default.setter
-    def default(self, value: Optional[pulumi.Input[str]]):
+    def default(self, value: pulumi.Input[str]):
         pulumi.set(self, "default", value)
 
     @property
     @pulumi.getter
-    def example(self) -> Optional[pulumi.Input[str]]:
+    def example(self) -> pulumi.Input[str]:
         """
         An example value for the field.
         """
         return pulumi.get(self, "example")
 
     @example.setter
-    def example(self, value: Optional[pulumi.Input[str]]):
+    def example(self, value: pulumi.Input[str]):
         pulumi.set(self, "example", value)
 
     @property
     @pulumi.getter
-    def label(self) -> Optional[pulumi.Input[str]]:
+    def label(self) -> pulumi.Input[str]:
         """
         The StackScript's label is for display purposes only.
         """
         return pulumi.get(self, "label")
 
     @label.setter
-    def label(self, value: Optional[pulumi.Input[str]]):
+    def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter(name="manyOf")
-    def many_of(self) -> Optional[pulumi.Input[str]]:
+    def many_of(self) -> pulumi.Input[str]:
         """
         A list of acceptable values for the field in any quantity, combination or order.
         """
         return pulumi.get(self, "many_of")
 
     @many_of.setter
-    def many_of(self, value: Optional[pulumi.Input[str]]):
+    def many_of(self, value: pulumi.Input[str]):
         pulumi.set(self, "many_of", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> pulumi.Input[str]:
         """
         The name of the field.
         """
         return pulumi.get(self, "name")
 
     @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
+    def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="oneOf")
-    def one_of(self) -> Optional[pulumi.Input[str]]:
+    def one_of(self) -> pulumi.Input[str]:
         """
         A list of acceptable single values for the field.
         """
         return pulumi.get(self, "one_of")
 
     @one_of.setter
-    def one_of(self, value: Optional[pulumi.Input[str]]):
+    def one_of(self, value: pulumi.Input[str]):
         pulumi.set(self, "one_of", value)
 
 
 @pulumi.input_type
 class UserDomainGrantArgs:
     def __init__(__self__, *,
                  id: pulumi.Input[int],
@@ -3322,111 +3269,14 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
-class GetStackScriptUserDefinedFieldArgs:
-    def __init__(__self__, *,
-                 default: str,
-                 example: str,
-                 label: str,
-                 many_of: str,
-                 name: str,
-                 one_of: str):
-        """
-        :param str default: The default value. If not specified, this value will be used.
-        :param str example: An example value for the field.
-        :param str label: A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
-        :param str many_of: A list of acceptable values for the field in any quantity, combination or order.
-        :param str name: The name of the field.
-        :param str one_of: A list of acceptable single values for the field.
-        """
-        pulumi.set(__self__, "default", default)
-        pulumi.set(__self__, "example", example)
-        pulumi.set(__self__, "label", label)
-        pulumi.set(__self__, "many_of", many_of)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "one_of", one_of)
-
-    @property
-    @pulumi.getter
-    def default(self) -> str:
-        """
-        The default value. If not specified, this value will be used.
-        """
-        return pulumi.get(self, "default")
-
-    @default.setter
-    def default(self, value: str):
-        pulumi.set(self, "default", value)
-
-    @property
-    @pulumi.getter
-    def example(self) -> str:
-        """
-        An example value for the field.
-        """
-        return pulumi.get(self, "example")
-
-    @example.setter
-    def example(self, value: str):
-        pulumi.set(self, "example", value)
-
-    @property
-    @pulumi.getter
-    def label(self) -> str:
-        """
-        A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
-        """
-        return pulumi.get(self, "label")
-
-    @label.setter
-    def label(self, value: str):
-        pulumi.set(self, "label", value)
-
-    @property
-    @pulumi.getter(name="manyOf")
-    def many_of(self) -> str:
-        """
-        A list of acceptable values for the field in any quantity, combination or order.
-        """
-        return pulumi.get(self, "many_of")
-
-    @many_of.setter
-    def many_of(self, value: str):
-        pulumi.set(self, "many_of", value)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        The name of the field.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: str):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="oneOf")
-    def one_of(self) -> str:
-        """
-        A list of acceptable single values for the field.
-        """
-        return pulumi.get(self, "one_of")
-
-    @one_of.setter
-    def one_of(self, value: str):
-        pulumi.set(self, "one_of", value)
-
-
-@pulumi.input_type
 class GetStackScriptsFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str],
                  match_by: Optional[str] = None):
         """
         :param str name: The name of the field to filter by. See the Filterable Fields section for a complete list of filterable fields.
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/_utilities.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/account_settings.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/config/vars.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/database_access_controls.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/database_access_controls.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/database_mongodb.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/database_mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,68 +7,72 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['DatabaseMongodbArgs', 'DatabaseMongodb']
+__all__ = ['DatabaseMysqlArgs', 'DatabaseMysql']
 
 @pulumi.input_type
-class DatabaseMongodbArgs:
+class DatabaseMysqlArgs:
     def __init__(__self__, *,
                  engine_id: pulumi.Input[str],
                  label: pulumi.Input[str],
                  region: pulumi.Input[str],
                  type: pulumi.Input[str],
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
-                 compression_type: Optional[pulumi.Input[str]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
+                 replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 storage_engine: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input['DatabaseMongodbUpdatesArgs']] = None):
+                 updates: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']] = None):
         """
-        The set of arguments for constructing a DatabaseMongodb resource.
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        The set of arguments for constructing a DatabaseMysql resource.
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[str] compression_type: The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
+        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input[str] storage_engine: The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
-        :param pulumi.Input['DatabaseMongodbUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input['DatabaseMysqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
         """
         pulumi.set(__self__, "engine_id", engine_id)
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "type", type)
         if allow_lists is not None:
             pulumi.set(__self__, "allow_lists", allow_lists)
         if cluster_size is not None:
             pulumi.set(__self__, "cluster_size", cluster_size)
-        if compression_type is not None:
-            pulumi.set(__self__, "compression_type", compression_type)
         if encrypted is not None:
             pulumi.set(__self__, "encrypted", encrypted)
+        if replication_type is not None:
+            pulumi.set(__self__, "replication_type", replication_type)
         if ssl_connection is not None:
             pulumi.set(__self__, "ssl_connection", ssl_connection)
-        if storage_engine is not None:
-            pulumi.set(__self__, "storage_engine", storage_engine)
         if updates is not None:
             pulumi.set(__self__, "updates", updates)
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> pulumi.Input[str]:
         """
-        The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         """
         return pulumi.get(self, "engine_id")
 
     @engine_id.setter
     def engine_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "engine_id", value)
 
@@ -97,14 +101,16 @@
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -129,168 +135,154 @@
         return pulumi.get(self, "cluster_size")
 
     @cluster_size.setter
     def cluster_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cluster_size", value)
 
     @property
-    @pulumi.getter(name="compressionType")
-    def compression_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
-        """
-        return pulumi.get(self, "compression_type")
-
-    @compression_type.setter
-    def compression_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "compression_type", value)
-
-    @property
     @pulumi.getter
     def encrypted(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether the Managed Databases is encrypted. (default `false`)
         """
         return pulumi.get(self, "encrypted")
 
     @encrypted.setter
     def encrypted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "encrypted", value)
 
     @property
+    @pulumi.getter(name="replicationType")
+    def replication_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+
+        * Must be `none` for a single node cluster.
+
+        * Must be `asynch` or `semi_synch` for a high availability cluster.
+        """
+        return pulumi.get(self, "replication_type")
+
+    @replication_type.setter
+    def replication_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "replication_type", value)
+
+    @property
     @pulumi.getter(name="sslConnection")
     def ssl_connection(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+
+        * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "ssl_connection")
 
     @ssl_connection.setter
     def ssl_connection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ssl_connection", value)
 
     @property
-    @pulumi.getter(name="storageEngine")
-    def storage_engine(self) -> Optional[pulumi.Input[str]]:
-        """
-        The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
-        """
-        return pulumi.get(self, "storage_engine")
-
-    @storage_engine.setter
-    def storage_engine(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "storage_engine", value)
-
-    @property
     @pulumi.getter
-    def updates(self) -> Optional[pulumi.Input['DatabaseMongodbUpdatesArgs']]:
+    def updates(self) -> Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]:
         """
         Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "updates")
 
     @updates.setter
-    def updates(self, value: Optional[pulumi.Input['DatabaseMongodbUpdatesArgs']]):
+    def updates(self, value: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]):
         pulumi.set(self, "updates", value)
 
 
 @pulumi.input_type
-class _DatabaseMongodbState:
+class _DatabaseMysqlState:
     def __init__(__self__, *,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ca_cert: Optional[pulumi.Input[str]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
-                 compression_type: Optional[pulumi.Input[str]] = None,
                  created: Optional[pulumi.Input[str]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  engine_id: Optional[pulumi.Input[str]] = None,
                  host_primary: Optional[pulumi.Input[str]] = None,
                  host_secondary: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
-                 peers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
-                 replica_set: Optional[pulumi.Input[str]] = None,
+                 replication_type: Optional[pulumi.Input[str]] = None,
                  root_password: Optional[pulumi.Input[str]] = None,
                  root_username: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
-                 storage_engine: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updated: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input['DatabaseMongodbUpdatesArgs']] = None,
+                 updates: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering DatabaseMongodb resources.
+        Input properties used for looking up and filtering DatabaseMysql resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[str] ca_cert: The base64-encoded SSL CA certificate for the Managed Database instance.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[str] compression_type: The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
         :param pulumi.Input[str] created: When this Managed Database was created.
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `mongodb`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `mysql`)
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         :param pulumi.Input[str] host_primary: The primary host for the Managed Database.
         :param pulumi.Input[str] host_secondary: The secondary/private network host for the Managed Database.
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] peers: A set of peer addresses for this Database.
-        :param pulumi.Input[int] port: The access port for this Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
-        :param pulumi.Input[str] replica_set: Label for configuring a MongoDB replica set. Choose the same label on multiple Databases to include them in the same replica set.
+        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[str] root_password: The randomly-generated root password for the Managed Database instance.
         :param pulumi.Input[str] root_username: The root username for the Managed Database instance.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] status: The operating status of the Managed Database.
-        :param pulumi.Input[str] storage_engine: The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
+               
+               - - -
         :param pulumi.Input[str] updated: When this Managed Database was last updated.
-        :param pulumi.Input['DatabaseMongodbUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input['DatabaseMysqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `v8.0.26`)
         """
         if allow_lists is not None:
             pulumi.set(__self__, "allow_lists", allow_lists)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cluster_size is not None:
             pulumi.set(__self__, "cluster_size", cluster_size)
-        if compression_type is not None:
-            pulumi.set(__self__, "compression_type", compression_type)
         if created is not None:
             pulumi.set(__self__, "created", created)
         if encrypted is not None:
             pulumi.set(__self__, "encrypted", encrypted)
         if engine is not None:
             pulumi.set(__self__, "engine", engine)
         if engine_id is not None:
             pulumi.set(__self__, "engine_id", engine_id)
         if host_primary is not None:
             pulumi.set(__self__, "host_primary", host_primary)
         if host_secondary is not None:
             pulumi.set(__self__, "host_secondary", host_secondary)
         if label is not None:
             pulumi.set(__self__, "label", label)
-        if peers is not None:
-            pulumi.set(__self__, "peers", peers)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
         if region is not None:
             pulumi.set(__self__, "region", region)
-        if replica_set is not None:
-            pulumi.set(__self__, "replica_set", replica_set)
+        if replication_type is not None:
+            pulumi.set(__self__, "replication_type", replication_type)
         if root_password is not None:
             pulumi.set(__self__, "root_password", root_password)
         if root_username is not None:
             pulumi.set(__self__, "root_username", root_username)
         if ssl_connection is not None:
             pulumi.set(__self__, "ssl_connection", ssl_connection)
         if status is not None:
             pulumi.set(__self__, "status", status)
-        if storage_engine is not None:
-            pulumi.set(__self__, "storage_engine", storage_engine)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if updated is not None:
             pulumi.set(__self__, "updated", updated)
         if updates is not None:
             pulumi.set(__self__, "updates", updates)
         if version is not None:
@@ -329,26 +321,14 @@
         return pulumi.get(self, "cluster_size")
 
     @cluster_size.setter
     def cluster_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cluster_size", value)
 
     @property
-    @pulumi.getter(name="compressionType")
-    def compression_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
-        """
-        return pulumi.get(self, "compression_type")
-
-    @compression_type.setter
-    def compression_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "compression_type", value)
-
-    @property
     @pulumi.getter
     def created(self) -> Optional[pulumi.Input[str]]:
         """
         When this Managed Database was created.
         """
         return pulumi.get(self, "created")
 
@@ -368,27 +348,27 @@
     def encrypted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "encrypted", value)
 
     @property
     @pulumi.getter
     def engine(self) -> Optional[pulumi.Input[str]]:
         """
-        The Managed Database engine. (e.g. `mongodb`)
+        The Managed Database engine. (e.g. `mysql`)
         """
         return pulumi.get(self, "engine")
 
     @engine.setter
     def engine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engine", value)
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         """
         return pulumi.get(self, "engine_id")
 
     @engine_id.setter
     def engine_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engine_id", value)
 
@@ -426,59 +406,39 @@
 
     @label.setter
     def label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
-    def peers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A set of peer addresses for this Database.
-        """
-        return pulumi.get(self, "peers")
-
-    @peers.setter
-    def peers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "peers", value)
-
-    @property
-    @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
-        """
-        The access port for this Managed Database.
-        """
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
-
-    @property
-    @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         The region to use for the Managed Database.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
-    @pulumi.getter(name="replicaSet")
-    def replica_set(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="replicationType")
+    def replication_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Label for configuring a MongoDB replica set. Choose the same label on multiple Databases to include them in the same replica set.
+        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+
+        * Must be `none` for a single node cluster.
+
+        * Must be `asynch` or `semi_synch` for a high availability cluster.
         """
-        return pulumi.get(self, "replica_set")
+        return pulumi.get(self, "replication_type")
 
-    @replica_set.setter
-    def replica_set(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "replica_set", value)
+    @replication_type.setter
+    def replication_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "replication_type", value)
 
     @property
     @pulumi.getter(name="rootPassword")
     def root_password(self) -> Optional[pulumi.Input[str]]:
         """
         The randomly-generated root password for the Managed Database instance.
         """
@@ -501,14 +461,16 @@
         pulumi.set(self, "root_username", value)
 
     @property
     @pulumi.getter(name="sslConnection")
     def ssl_connection(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+
+        * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "ssl_connection")
 
     @ssl_connection.setter
     def ssl_connection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ssl_connection", value)
 
@@ -521,30 +483,20 @@
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
-    @pulumi.getter(name="storageEngine")
-    def storage_engine(self) -> Optional[pulumi.Input[str]]:
-        """
-        The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
-        """
-        return pulumi.get(self, "storage_engine")
-
-    @storage_engine.setter
-    def storage_engine(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "storage_engine", value)
-
-    @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -558,22 +510,22 @@
 
     @updated.setter
     def updated(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated", value)
 
     @property
     @pulumi.getter
-    def updates(self) -> Optional[pulumi.Input['DatabaseMongodbUpdatesArgs']]:
+    def updates(self) -> Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]:
         """
         Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "updates")
 
     @updates.setter
-    def updates(self, value: Optional[pulumi.Input['DatabaseMongodbUpdatesArgs']]):
+    def updates(self, value: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]):
         pulumi.set(self, "updates", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
         The Managed Database engine version. (e.g. `v8.0.26`)
@@ -581,70 +533,68 @@
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class DatabaseMongodb(pulumi.CustomResource):
+class DatabaseMysql(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
-                 compression_type: Optional[pulumi.Input[str]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
                  engine_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 storage_engine: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMongodbUpdatesArgs']]] = None,
+                 updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
                  __props__=None):
         """
-        Provides a Linode Mongo Database resource. This can be used to create, modify, and delete Linode MongoDB Databases.
+        Provides a Linode MySQL Database resource. This can be used to create, modify, and delete Linode MySQL Databases.
         For more information, see the [Linode APIv4 docs](https://www.linode.com/docs/api/databases/).
 
         Please keep in mind that Managed Databases can take up to an hour to provision.
 
         ## Example Usage
 
-        Creating a simple MongoDB database instance:
+        Creating a simple MySQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMongodb("foobar",
-            engine_id="mongodb/4.4.10",
+        foobar = linode.DatabaseMysql("foobar",
+            engine_id="mysql/8.0.26",
             label="mydatabase",
             region="us-southeast",
             type="g6-nanode-1")
         ```
 
-        Creating a complex MongoDB database instance:
+        Creating a complex MySQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMongodb("foobar",
+        foobar = linode.DatabaseMysql("foobar",
             allow_lists=["0.0.0.0/0"],
             cluster_size=3,
-            compression_type="zlib",
             encrypted=True,
-            engine_id="mongodb/4.4.10",
+            engine_id="mysql/8.0.26",
             label="mydatabase",
             region="us-southeast",
+            replication_type="asynch",
             ssl_connection=True,
-            storage_engine="wiredtiger",
             type="g6-nanode-1",
-            updates=linode.DatabaseMongodbUpdatesArgs(
+            updates=linode.DatabaseMysqlUpdatesArgs(
                 day_of_week="saturday",
                 duration=1,
                 frequency="monthly",
                 hour_of_day=22,
                 week_of_month=2,
             ))
         ```
@@ -660,79 +610,85 @@
 
         * `hour_of_day` - (Required) The hour to begin maintenance based in UTC time. (`0`..`23`)
 
         * `week_of_month` - (Optional) The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
         ## Import
 
-        Linode MongoDB Databases can be imported using the `id`, e.g.
+        Linode MySQL Databases can be imported using the `id`, e.g.
 
         ```sh
-         $ pulumi import linode:index/databaseMongodb:DatabaseMongodb foobar 1234567
+         $ pulumi import linode:index/databaseMysql:DatabaseMysql foobar 1234567
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[str] compression_type: The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
+        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input[str] storage_engine: The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
-        :param pulumi.Input[pulumi.InputType['DatabaseMongodbUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+               
+               - - -
+        :param pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DatabaseMongodbArgs,
+                 args: DatabaseMysqlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Linode Mongo Database resource. This can be used to create, modify, and delete Linode MongoDB Databases.
+        Provides a Linode MySQL Database resource. This can be used to create, modify, and delete Linode MySQL Databases.
         For more information, see the [Linode APIv4 docs](https://www.linode.com/docs/api/databases/).
 
         Please keep in mind that Managed Databases can take up to an hour to provision.
 
         ## Example Usage
 
-        Creating a simple MongoDB database instance:
+        Creating a simple MySQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMongodb("foobar",
-            engine_id="mongodb/4.4.10",
+        foobar = linode.DatabaseMysql("foobar",
+            engine_id="mysql/8.0.26",
             label="mydatabase",
             region="us-southeast",
             type="g6-nanode-1")
         ```
 
-        Creating a complex MongoDB database instance:
+        Creating a complex MySQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMongodb("foobar",
+        foobar = linode.DatabaseMysql("foobar",
             allow_lists=["0.0.0.0/0"],
             cluster_size=3,
-            compression_type="zlib",
             encrypted=True,
-            engine_id="mongodb/4.4.10",
+            engine_id="mysql/8.0.26",
             label="mydatabase",
             region="us-southeast",
+            replication_type="asynch",
             ssl_connection=True,
-            storage_engine="wiredtiger",
             type="g6-nanode-1",
-            updates=linode.DatabaseMongodbUpdatesArgs(
+            updates=linode.DatabaseMysqlUpdatesArgs(
                 day_of_week="saturday",
                 duration=1,
                 frequency="monthly",
                 hour_of_day=22,
                 week_of_month=2,
             ))
         ```
@@ -748,184 +704,175 @@
 
         * `hour_of_day` - (Required) The hour to begin maintenance based in UTC time. (`0`..`23`)
 
         * `week_of_month` - (Optional) The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
         ## Import
 
-        Linode MongoDB Databases can be imported using the `id`, e.g.
+        Linode MySQL Databases can be imported using the `id`, e.g.
 
         ```sh
-         $ pulumi import linode:index/databaseMongodb:DatabaseMongodb foobar 1234567
+         $ pulumi import linode:index/databaseMysql:DatabaseMysql foobar 1234567
         ```
 
         :param str resource_name: The name of the resource.
-        :param DatabaseMongodbArgs args: The arguments to use to populate this resource's properties.
+        :param DatabaseMysqlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DatabaseMongodbArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DatabaseMysqlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
-                 compression_type: Optional[pulumi.Input[str]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
                  engine_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 storage_engine: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMongodbUpdatesArgs']]] = None,
+                 updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DatabaseMongodbArgs.__new__(DatabaseMongodbArgs)
+            __props__ = DatabaseMysqlArgs.__new__(DatabaseMysqlArgs)
 
             __props__.__dict__["allow_lists"] = allow_lists
             __props__.__dict__["cluster_size"] = cluster_size
-            __props__.__dict__["compression_type"] = compression_type
             __props__.__dict__["encrypted"] = encrypted
             if engine_id is None and not opts.urn:
                 raise TypeError("Missing required property 'engine_id'")
             __props__.__dict__["engine_id"] = engine_id
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
             __props__.__dict__["label"] = label
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
+            __props__.__dict__["replication_type"] = replication_type
             __props__.__dict__["ssl_connection"] = ssl_connection
-            __props__.__dict__["storage_engine"] = storage_engine
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
             __props__.__dict__["updates"] = updates
             __props__.__dict__["ca_cert"] = None
             __props__.__dict__["created"] = None
             __props__.__dict__["engine"] = None
             __props__.__dict__["host_primary"] = None
             __props__.__dict__["host_secondary"] = None
-            __props__.__dict__["peers"] = None
-            __props__.__dict__["port"] = None
-            __props__.__dict__["replica_set"] = None
             __props__.__dict__["root_password"] = None
             __props__.__dict__["root_username"] = None
             __props__.__dict__["status"] = None
             __props__.__dict__["updated"] = None
             __props__.__dict__["version"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["caCert", "rootPassword", "rootUsername"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(DatabaseMongodb, __self__).__init__(
-            'linode:index/databaseMongodb:DatabaseMongodb',
+        super(DatabaseMysql, __self__).__init__(
+            'linode:index/databaseMysql:DatabaseMysql',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ca_cert: Optional[pulumi.Input[str]] = None,
             cluster_size: Optional[pulumi.Input[int]] = None,
-            compression_type: Optional[pulumi.Input[str]] = None,
             created: Optional[pulumi.Input[str]] = None,
             encrypted: Optional[pulumi.Input[bool]] = None,
             engine: Optional[pulumi.Input[str]] = None,
             engine_id: Optional[pulumi.Input[str]] = None,
             host_primary: Optional[pulumi.Input[str]] = None,
             host_secondary: Optional[pulumi.Input[str]] = None,
             label: Optional[pulumi.Input[str]] = None,
-            peers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            port: Optional[pulumi.Input[int]] = None,
             region: Optional[pulumi.Input[str]] = None,
-            replica_set: Optional[pulumi.Input[str]] = None,
+            replication_type: Optional[pulumi.Input[str]] = None,
             root_password: Optional[pulumi.Input[str]] = None,
             root_username: Optional[pulumi.Input[str]] = None,
             ssl_connection: Optional[pulumi.Input[bool]] = None,
             status: Optional[pulumi.Input[str]] = None,
-            storage_engine: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             updated: Optional[pulumi.Input[str]] = None,
-            updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMongodbUpdatesArgs']]] = None,
-            version: Optional[pulumi.Input[str]] = None) -> 'DatabaseMongodb':
+            updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
+            version: Optional[pulumi.Input[str]] = None) -> 'DatabaseMysql':
         """
-        Get an existing DatabaseMongodb resource's state with the given name, id, and optional extra
+        Get an existing DatabaseMysql resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[str] ca_cert: The base64-encoded SSL CA certificate for the Managed Database instance.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[str] compression_type: The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
         :param pulumi.Input[str] created: When this Managed Database was created.
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `mongodb`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `mysql`)
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         :param pulumi.Input[str] host_primary: The primary host for the Managed Database.
         :param pulumi.Input[str] host_secondary: The secondary/private network host for the Managed Database.
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] peers: A set of peer addresses for this Database.
-        :param pulumi.Input[int] port: The access port for this Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
-        :param pulumi.Input[str] replica_set: Label for configuring a MongoDB replica set. Choose the same label on multiple Databases to include them in the same replica set.
+        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[str] root_password: The randomly-generated root password for the Managed Database instance.
         :param pulumi.Input[str] root_username: The root username for the Managed Database instance.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] status: The operating status of the Managed Database.
-        :param pulumi.Input[str] storage_engine: The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
+               
+               - - -
         :param pulumi.Input[str] updated: When this Managed Database was last updated.
-        :param pulumi.Input[pulumi.InputType['DatabaseMongodbUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `v8.0.26`)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DatabaseMongodbState.__new__(_DatabaseMongodbState)
+        __props__ = _DatabaseMysqlState.__new__(_DatabaseMysqlState)
 
         __props__.__dict__["allow_lists"] = allow_lists
         __props__.__dict__["ca_cert"] = ca_cert
         __props__.__dict__["cluster_size"] = cluster_size
-        __props__.__dict__["compression_type"] = compression_type
         __props__.__dict__["created"] = created
         __props__.__dict__["encrypted"] = encrypted
         __props__.__dict__["engine"] = engine
         __props__.__dict__["engine_id"] = engine_id
         __props__.__dict__["host_primary"] = host_primary
         __props__.__dict__["host_secondary"] = host_secondary
         __props__.__dict__["label"] = label
-        __props__.__dict__["peers"] = peers
-        __props__.__dict__["port"] = port
         __props__.__dict__["region"] = region
-        __props__.__dict__["replica_set"] = replica_set
+        __props__.__dict__["replication_type"] = replication_type
         __props__.__dict__["root_password"] = root_password
         __props__.__dict__["root_username"] = root_username
         __props__.__dict__["ssl_connection"] = ssl_connection
         __props__.__dict__["status"] = status
-        __props__.__dict__["storage_engine"] = storage_engine
         __props__.__dict__["type"] = type
         __props__.__dict__["updated"] = updated
         __props__.__dict__["updates"] = updates
         __props__.__dict__["version"] = version
-        return DatabaseMongodb(resource_name, opts=opts, __props__=__props__)
+        return DatabaseMysql(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="allowLists")
     def allow_lists(self) -> pulumi.Output[Sequence[str]]:
         """
         A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         """
@@ -944,22 +891,14 @@
     def cluster_size(self) -> pulumi.Output[Optional[int]]:
         """
         The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
         """
         return pulumi.get(self, "cluster_size")
 
     @property
-    @pulumi.getter(name="compressionType")
-    def compression_type(self) -> pulumi.Output[Optional[str]]:
-        """
-        The type of data compression for this Database. (`none`, `snappy`, `zlib`; default `none`)
-        """
-        return pulumi.get(self, "compression_type")
-
-    @property
     @pulumi.getter
     def created(self) -> pulumi.Output[str]:
         """
         When this Managed Database was created.
         """
         return pulumi.get(self, "created")
 
@@ -971,23 +910,23 @@
         """
         return pulumi.get(self, "encrypted")
 
     @property
     @pulumi.getter
     def engine(self) -> pulumi.Output[str]:
         """
-        The Managed Database engine. (e.g. `mongodb`)
+        The Managed Database engine. (e.g. `mysql`)
         """
         return pulumi.get(self, "engine")
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> pulumi.Output[str]:
         """
-        The Managed Database engine in engine/version format. (e.g. `mongo/4.4.10`)
+        The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
         """
         return pulumi.get(self, "engine_id")
 
     @property
     @pulumi.getter(name="hostPrimary")
     def host_primary(self) -> pulumi.Output[str]:
         """
@@ -1009,43 +948,31 @@
         """
         A unique, user-defined string referring to the Managed Database.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
-    def peers(self) -> pulumi.Output[Sequence[str]]:
-        """
-        A set of peer addresses for this Database.
-        """
-        return pulumi.get(self, "peers")
-
-    @property
-    @pulumi.getter
-    def port(self) -> pulumi.Output[int]:
-        """
-        The access port for this Managed Database.
-        """
-        return pulumi.get(self, "port")
-
-    @property
-    @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         The region to use for the Managed Database.
         """
         return pulumi.get(self, "region")
 
     @property
-    @pulumi.getter(name="replicaSet")
-    def replica_set(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="replicationType")
+    def replication_type(self) -> pulumi.Output[Optional[str]]:
         """
-        Label for configuring a MongoDB replica set. Choose the same label on multiple Databases to include them in the same replica set.
+        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+
+        * Must be `none` for a single node cluster.
+
+        * Must be `asynch` or `semi_synch` for a high availability cluster.
         """
-        return pulumi.get(self, "replica_set")
+        return pulumi.get(self, "replication_type")
 
     @property
     @pulumi.getter(name="rootPassword")
     def root_password(self) -> pulumi.Output[str]:
         """
         The randomly-generated root password for the Managed Database instance.
         """
@@ -1060,52 +987,48 @@
         return pulumi.get(self, "root_username")
 
     @property
     @pulumi.getter(name="sslConnection")
     def ssl_connection(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+
+        * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "ssl_connection")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
         The operating status of the Managed Database.
         """
         return pulumi.get(self, "status")
 
     @property
-    @pulumi.getter(name="storageEngine")
-    def storage_engine(self) -> pulumi.Output[Optional[str]]:
-        """
-        The type of storage engine for this Database. (`mmapv1`, `wiredtiger`; default `wiredtiger`)
-        """
-        return pulumi.get(self, "storage_engine")
-
-    @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def updated(self) -> pulumi.Output[str]:
         """
         When this Managed Database was last updated.
         """
         return pulumi.get(self, "updated")
 
     @property
     @pulumi.getter
-    def updates(self) -> pulumi.Output['outputs.DatabaseMongodbUpdates']:
+    def updates(self) -> pulumi.Output['outputs.DatabaseMysqlUpdates']:
         """
         Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "updates")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/database_mysql.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/database_postgresql.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,64 +7,80 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['DatabaseMysqlArgs', 'DatabaseMysql']
+__all__ = ['DatabasePostgresqlArgs', 'DatabasePostgresql']
 
 @pulumi.input_type
-class DatabaseMysqlArgs:
+class DatabasePostgresqlArgs:
     def __init__(__self__, *,
                  engine_id: pulumi.Input[str],
                  label: pulumi.Input[str],
                  region: pulumi.Input[str],
                  type: pulumi.Input[str],
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
+                 replication_commit_type: Optional[pulumi.Input[str]] = None,
                  replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 updates: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']] = None):
+                 updates: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']] = None):
         """
-        The set of arguments for constructing a DatabaseMysql resource.
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        The set of arguments for constructing a DatabasePostgresql resource.
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
+        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+               
+               * Must be `local` or `off` for the `asynch` replication type.
+               
+               * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
         :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input['DatabaseMysqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input['DatabasePostgresqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
         """
         pulumi.set(__self__, "engine_id", engine_id)
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "type", type)
         if allow_lists is not None:
             pulumi.set(__self__, "allow_lists", allow_lists)
         if cluster_size is not None:
             pulumi.set(__self__, "cluster_size", cluster_size)
         if encrypted is not None:
             pulumi.set(__self__, "encrypted", encrypted)
+        if replication_commit_type is not None:
+            pulumi.set(__self__, "replication_commit_type", replication_commit_type)
         if replication_type is not None:
             pulumi.set(__self__, "replication_type", replication_type)
         if ssl_connection is not None:
             pulumi.set(__self__, "ssl_connection", ssl_connection)
         if updates is not None:
             pulumi.set(__self__, "updates", updates)
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> pulumi.Input[str]:
         """
-        The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         """
         return pulumi.get(self, "engine_id")
 
     @engine_id.setter
     def engine_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "engine_id", value)
 
@@ -93,14 +109,16 @@
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -137,95 +155,133 @@
         return pulumi.get(self, "encrypted")
 
     @encrypted.setter
     def encrypted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "encrypted", value)
 
     @property
+    @pulumi.getter(name="replicationCommitType")
+    def replication_commit_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+
+        * Must be `local` or `off` for the `asynch` replication type.
+
+        * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
+        """
+        return pulumi.get(self, "replication_commit_type")
+
+    @replication_commit_type.setter
+    def replication_commit_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "replication_commit_type", value)
+
+    @property
     @pulumi.getter(name="replicationType")
     def replication_type(self) -> Optional[pulumi.Input[str]]:
         """
         The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+
+        * Must be `none` for a single node cluster.
+
+        * Must be `asynch` or `semi_synch` for a high availability cluster.
         """
         return pulumi.get(self, "replication_type")
 
     @replication_type.setter
     def replication_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "replication_type", value)
 
     @property
     @pulumi.getter(name="sslConnection")
     def ssl_connection(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+
+        * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "ssl_connection")
 
     @ssl_connection.setter
     def ssl_connection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ssl_connection", value)
 
     @property
     @pulumi.getter
-    def updates(self) -> Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]:
+    def updates(self) -> Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]:
         """
         Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "updates")
 
     @updates.setter
-    def updates(self, value: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]):
+    def updates(self, value: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]):
         pulumi.set(self, "updates", value)
 
 
 @pulumi.input_type
-class _DatabaseMysqlState:
+class _DatabasePostgresqlState:
     def __init__(__self__, *,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ca_cert: Optional[pulumi.Input[str]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
                  created: Optional[pulumi.Input[str]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  engine_id: Optional[pulumi.Input[str]] = None,
                  host_primary: Optional[pulumi.Input[str]] = None,
                  host_secondary: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 replication_commit_type: Optional[pulumi.Input[str]] = None,
                  replication_type: Optional[pulumi.Input[str]] = None,
                  root_password: Optional[pulumi.Input[str]] = None,
                  root_username: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updated: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']] = None,
+                 updates: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering DatabaseMysql resources.
+        Input properties used for looking up and filtering DatabasePostgresql resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[str] ca_cert: The base64-encoded SSL CA certificate for the Managed Database instance.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
         :param pulumi.Input[str] created: When this Managed Database was created.
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `mysql`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `postgresql`)
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         :param pulumi.Input[str] host_primary: The primary host for the Managed Database.
         :param pulumi.Input[str] host_secondary: The secondary/private network host for the Managed Database.
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
+        :param pulumi.Input[int] port: The access port for this Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
+        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+               
+               * Must be `local` or `off` for the `asynch` replication type.
+               
+               * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
         :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[str] root_password: The randomly-generated root password for the Managed Database instance.
         :param pulumi.Input[str] root_username: The root username for the Managed Database instance.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] status: The operating status of the Managed Database.
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
+               
+               - - -
         :param pulumi.Input[str] updated: When this Managed Database was last updated.
-        :param pulumi.Input['DatabaseMysqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
-        :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `v8.0.26`)
+        :param pulumi.Input['DatabasePostgresqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `13.2`)
         """
         if allow_lists is not None:
             pulumi.set(__self__, "allow_lists", allow_lists)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cluster_size is not None:
             pulumi.set(__self__, "cluster_size", cluster_size)
@@ -239,16 +295,20 @@
             pulumi.set(__self__, "engine_id", engine_id)
         if host_primary is not None:
             pulumi.set(__self__, "host_primary", host_primary)
         if host_secondary is not None:
             pulumi.set(__self__, "host_secondary", host_secondary)
         if label is not None:
             pulumi.set(__self__, "label", label)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if replication_commit_type is not None:
+            pulumi.set(__self__, "replication_commit_type", replication_commit_type)
         if replication_type is not None:
             pulumi.set(__self__, "replication_type", replication_type)
         if root_password is not None:
             pulumi.set(__self__, "root_password", root_password)
         if root_username is not None:
             pulumi.set(__self__, "root_username", root_username)
         if ssl_connection is not None:
@@ -324,27 +384,27 @@
     def encrypted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "encrypted", value)
 
     @property
     @pulumi.getter
     def engine(self) -> Optional[pulumi.Input[str]]:
         """
-        The Managed Database engine. (e.g. `mysql`)
+        The Managed Database engine. (e.g. `postgresql`)
         """
         return pulumi.get(self, "engine")
 
     @engine.setter
     def engine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engine", value)
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         """
         return pulumi.get(self, "engine_id")
 
     @engine_id.setter
     def engine_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engine_id", value)
 
@@ -382,29 +442,61 @@
 
     @label.setter
     def label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[int]]:
+        """
+        The access port for this Managed Database.
+        """
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         The region to use for the Managed Database.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="replicationCommitType")
+    def replication_commit_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+
+        * Must be `local` or `off` for the `asynch` replication type.
+
+        * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
+        """
+        return pulumi.get(self, "replication_commit_type")
+
+    @replication_commit_type.setter
+    def replication_commit_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "replication_commit_type", value)
+
+    @property
     @pulumi.getter(name="replicationType")
     def replication_type(self) -> Optional[pulumi.Input[str]]:
         """
         The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+
+        * Must be `none` for a single node cluster.
+
+        * Must be `asynch` or `semi_synch` for a high availability cluster.
         """
         return pulumi.get(self, "replication_type")
 
     @replication_type.setter
     def replication_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "replication_type", value)
 
@@ -433,14 +525,16 @@
         pulumi.set(self, "root_username", value)
 
     @property
     @pulumi.getter(name="sslConnection")
     def ssl_connection(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+
+        * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "ssl_connection")
 
     @ssl_connection.setter
     def ssl_connection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ssl_connection", value)
 
@@ -457,14 +551,16 @@
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -478,91 +574,93 @@
 
     @updated.setter
     def updated(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated", value)
 
     @property
     @pulumi.getter
-    def updates(self) -> Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]:
+    def updates(self) -> Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]:
         """
         Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "updates")
 
     @updates.setter
-    def updates(self, value: Optional[pulumi.Input['DatabaseMysqlUpdatesArgs']]):
+    def updates(self, value: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]):
         pulumi.set(self, "updates", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The Managed Database engine version. (e.g. `v8.0.26`)
+        The Managed Database engine version. (e.g. `13.2`)
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class DatabaseMysql(pulumi.CustomResource):
+class DatabasePostgresql(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
                  engine_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 replication_commit_type: Optional[pulumi.Input[str]] = None,
                  replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
+                 updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
                  __props__=None):
         """
-        Provides a Linode MySQL Database resource. This can be used to create, modify, and delete Linode MySQL Databases.
+        Provides a Linode PostgreSQL Database resource. This can be used to create, modify, and delete Linode PostgreSQL Databases.
         For more information, see the [Linode APIv4 docs](https://www.linode.com/docs/api/databases/).
 
         Please keep in mind that Managed Databases can take up to an hour to provision.
 
         ## Example Usage
 
-        Creating a simple MySQL database instance:
+        Creating a simple PostgreSQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMysql("foobar",
-            engine_id="mysql/8.0.26",
+        foobar = linode.DatabasePostgresql("foobar",
+            engine_id="postgresql/13.2",
             label="mydatabase",
             region="us-southeast",
             type="g6-nanode-1")
         ```
 
-        Creating a complex MySQL database instance:
+        Creating a complex PostgreSQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMysql("foobar",
+        foobar = linode.DatabasePostgresql("foobar",
             allow_lists=["0.0.0.0/0"],
             cluster_size=3,
             encrypted=True,
-            engine_id="mysql/8.0.26",
+            engine_id="postgresql/13.2",
             label="mydatabase",
             region="us-southeast",
-            replication_type="asynch",
+            replication_commit_type="remote_write",
+            replication_type="semi_synch",
             ssl_connection=True,
             type="g6-nanode-1",
-            updates=linode.DatabaseMysqlUpdatesArgs(
+            updates=linode.DatabasePostgresqlUpdatesArgs(
                 day_of_week="saturday",
                 duration=1,
                 frequency="monthly",
                 hour_of_day=22,
                 week_of_month=2,
             ))
         ```
@@ -578,77 +676,91 @@
 
         * `hour_of_day` - (Required) The hour to begin maintenance based in UTC time. (`0`..`23`)
 
         * `week_of_month` - (Optional) The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
         ## Import
 
-        Linode MySQL Databases can be imported using the `id`, e.g.
+        Linode PostgreSQL Databases can be imported using the `id`, e.g.
 
         ```sh
-         $ pulumi import linode:index/databaseMysql:DatabaseMysql foobar 1234567
+         $ pulumi import linode:index/databasePostgresql:DatabasePostgresql foobar 1234567
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
+        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+               
+               * Must be `local` or `off` for the `asynch` replication type.
+               
+               * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
         :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
-        :param pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+               
+               - - -
+        :param pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DatabaseMysqlArgs,
+                 args: DatabasePostgresqlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Linode MySQL Database resource. This can be used to create, modify, and delete Linode MySQL Databases.
+        Provides a Linode PostgreSQL Database resource. This can be used to create, modify, and delete Linode PostgreSQL Databases.
         For more information, see the [Linode APIv4 docs](https://www.linode.com/docs/api/databases/).
 
         Please keep in mind that Managed Databases can take up to an hour to provision.
 
         ## Example Usage
 
-        Creating a simple MySQL database instance:
+        Creating a simple PostgreSQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMysql("foobar",
-            engine_id="mysql/8.0.26",
+        foobar = linode.DatabasePostgresql("foobar",
+            engine_id="postgresql/13.2",
             label="mydatabase",
             region="us-southeast",
             type="g6-nanode-1")
         ```
 
-        Creating a complex MySQL database instance:
+        Creating a complex PostgreSQL database instance:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabaseMysql("foobar",
+        foobar = linode.DatabasePostgresql("foobar",
             allow_lists=["0.0.0.0/0"],
             cluster_size=3,
             encrypted=True,
-            engine_id="mysql/8.0.26",
+            engine_id="postgresql/13.2",
             label="mydatabase",
             region="us-southeast",
-            replication_type="asynch",
+            replication_commit_type="remote_write",
+            replication_type="semi_synch",
             ssl_connection=True,
             type="g6-nanode-1",
-            updates=linode.DatabaseMysqlUpdatesArgs(
+            updates=linode.DatabasePostgresqlUpdatesArgs(
                 day_of_week="saturday",
                 duration=1,
                 frequency="monthly",
                 hour_of_day=22,
                 week_of_month=2,
             ))
         ```
@@ -664,86 +776,89 @@
 
         * `hour_of_day` - (Required) The hour to begin maintenance based in UTC time. (`0`..`23`)
 
         * `week_of_month` - (Optional) The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
         ## Import
 
-        Linode MySQL Databases can be imported using the `id`, e.g.
+        Linode PostgreSQL Databases can be imported using the `id`, e.g.
 
         ```sh
-         $ pulumi import linode:index/databaseMysql:DatabaseMysql foobar 1234567
+         $ pulumi import linode:index/databasePostgresql:DatabasePostgresql foobar 1234567
         ```
 
         :param str resource_name: The name of the resource.
-        :param DatabaseMysqlArgs args: The arguments to use to populate this resource's properties.
+        :param DatabasePostgresqlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DatabaseMysqlArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DatabasePostgresqlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_size: Optional[pulumi.Input[int]] = None,
                  encrypted: Optional[pulumi.Input[bool]] = None,
                  engine_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 replication_commit_type: Optional[pulumi.Input[str]] = None,
                  replication_type: Optional[pulumi.Input[str]] = None,
                  ssl_connection: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
+                 updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DatabaseMysqlArgs.__new__(DatabaseMysqlArgs)
+            __props__ = DatabasePostgresqlArgs.__new__(DatabasePostgresqlArgs)
 
             __props__.__dict__["allow_lists"] = allow_lists
             __props__.__dict__["cluster_size"] = cluster_size
             __props__.__dict__["encrypted"] = encrypted
             if engine_id is None and not opts.urn:
                 raise TypeError("Missing required property 'engine_id'")
             __props__.__dict__["engine_id"] = engine_id
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
             __props__.__dict__["label"] = label
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
+            __props__.__dict__["replication_commit_type"] = replication_commit_type
             __props__.__dict__["replication_type"] = replication_type
             __props__.__dict__["ssl_connection"] = ssl_connection
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
             __props__.__dict__["updates"] = updates
             __props__.__dict__["ca_cert"] = None
             __props__.__dict__["created"] = None
             __props__.__dict__["engine"] = None
             __props__.__dict__["host_primary"] = None
             __props__.__dict__["host_secondary"] = None
+            __props__.__dict__["port"] = None
             __props__.__dict__["root_password"] = None
             __props__.__dict__["root_username"] = None
             __props__.__dict__["status"] = None
             __props__.__dict__["updated"] = None
             __props__.__dict__["version"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["caCert", "rootPassword", "rootUsername"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(DatabaseMysql, __self__).__init__(
-            'linode:index/databaseMysql:DatabaseMysql',
+        super(DatabasePostgresql, __self__).__init__(
+            'linode:index/databasePostgresql:DatabasePostgresql',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -754,77 +869,95 @@
             created: Optional[pulumi.Input[str]] = None,
             encrypted: Optional[pulumi.Input[bool]] = None,
             engine: Optional[pulumi.Input[str]] = None,
             engine_id: Optional[pulumi.Input[str]] = None,
             host_primary: Optional[pulumi.Input[str]] = None,
             host_secondary: Optional[pulumi.Input[str]] = None,
             label: Optional[pulumi.Input[str]] = None,
+            port: Optional[pulumi.Input[int]] = None,
             region: Optional[pulumi.Input[str]] = None,
+            replication_commit_type: Optional[pulumi.Input[str]] = None,
             replication_type: Optional[pulumi.Input[str]] = None,
             root_password: Optional[pulumi.Input[str]] = None,
             root_username: Optional[pulumi.Input[str]] = None,
             ssl_connection: Optional[pulumi.Input[bool]] = None,
             status: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             updated: Optional[pulumi.Input[str]] = None,
-            updates: Optional[pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']]] = None,
-            version: Optional[pulumi.Input[str]] = None) -> 'DatabaseMysql':
+            updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
+            version: Optional[pulumi.Input[str]] = None) -> 'DatabasePostgresql':
         """
-        Get an existing DatabaseMysql resource's state with the given name, id, and optional extra
+        Get an existing DatabasePostgresql resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         :param pulumi.Input[str] ca_cert: The base64-encoded SSL CA certificate for the Managed Database instance.
         :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
         :param pulumi.Input[str] created: When this Managed Database was created.
         :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `mysql`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `postgresql`)
+        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         :param pulumi.Input[str] host_primary: The primary host for the Managed Database.
         :param pulumi.Input[str] host_secondary: The secondary/private network host for the Managed Database.
         :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
+        :param pulumi.Input[int] port: The access port for this Managed Database.
         :param pulumi.Input[str] region: The region to use for the Managed Database.
+        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+               
+               * Must be `local` or `off` for the `asynch` replication type.
+               
+               * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
         :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+               
+               * Must be `none` for a single node cluster.
+               
+               * Must be `asynch` or `semi_synch` for a high availability cluster.
         :param pulumi.Input[str] root_password: The randomly-generated root password for the Managed Database instance.
         :param pulumi.Input[str] root_username: The root username for the Managed Database instance.
         :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+               
+               * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         :param pulumi.Input[str] status: The operating status of the Managed Database.
         :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
+               
+               - - -
         :param pulumi.Input[str] updated: When this Managed Database was last updated.
-        :param pulumi.Input[pulumi.InputType['DatabaseMysqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
-        :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `v8.0.26`)
+        :param pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `13.2`)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DatabaseMysqlState.__new__(_DatabaseMysqlState)
+        __props__ = _DatabasePostgresqlState.__new__(_DatabasePostgresqlState)
 
         __props__.__dict__["allow_lists"] = allow_lists
         __props__.__dict__["ca_cert"] = ca_cert
         __props__.__dict__["cluster_size"] = cluster_size
         __props__.__dict__["created"] = created
         __props__.__dict__["encrypted"] = encrypted
         __props__.__dict__["engine"] = engine
         __props__.__dict__["engine_id"] = engine_id
         __props__.__dict__["host_primary"] = host_primary
         __props__.__dict__["host_secondary"] = host_secondary
         __props__.__dict__["label"] = label
+        __props__.__dict__["port"] = port
         __props__.__dict__["region"] = region
+        __props__.__dict__["replication_commit_type"] = replication_commit_type
         __props__.__dict__["replication_type"] = replication_type
         __props__.__dict__["root_password"] = root_password
         __props__.__dict__["root_username"] = root_username
         __props__.__dict__["ssl_connection"] = ssl_connection
         __props__.__dict__["status"] = status
         __props__.__dict__["type"] = type
         __props__.__dict__["updated"] = updated
         __props__.__dict__["updates"] = updates
         __props__.__dict__["version"] = version
-        return DatabaseMysql(resource_name, opts=opts, __props__=__props__)
+        return DatabasePostgresql(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="allowLists")
     def allow_lists(self) -> pulumi.Output[Sequence[str]]:
         """
         A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
         """
@@ -862,23 +995,23 @@
         """
         return pulumi.get(self, "encrypted")
 
     @property
     @pulumi.getter
     def engine(self) -> pulumi.Output[str]:
         """
-        The Managed Database engine. (e.g. `mysql`)
+        The Managed Database engine. (e.g. `postgresql`)
         """
         return pulumi.get(self, "engine")
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> pulumi.Output[str]:
         """
-        The Managed Database engine in engine/version format. (e.g. `mysql/8.0.26`)
+        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         """
         return pulumi.get(self, "engine_id")
 
     @property
     @pulumi.getter(name="hostPrimary")
     def host_primary(self) -> pulumi.Output[str]:
         """
@@ -900,25 +1033,49 @@
         """
         A unique, user-defined string referring to the Managed Database.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
+    def port(self) -> pulumi.Output[int]:
+        """
+        The access port for this Managed Database.
+        """
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         The region to use for the Managed Database.
         """
         return pulumi.get(self, "region")
 
     @property
+    @pulumi.getter(name="replicationCommitType")
+    def replication_commit_type(self) -> pulumi.Output[Optional[str]]:
+        """
+        The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+
+        * Must be `local` or `off` for the `asynch` replication type.
+
+        * Must be `on`, `remote_write`, or `remote_apply` for the `semi_synch` replication type.
+        """
+        return pulumi.get(self, "replication_commit_type")
+
+    @property
     @pulumi.getter(name="replicationType")
     def replication_type(self) -> pulumi.Output[Optional[str]]:
         """
         The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+
+        * Must be `none` for a single node cluster.
+
+        * Must be `asynch` or `semi_synch` for a high availability cluster.
         """
         return pulumi.get(self, "replication_type")
 
     @property
     @pulumi.getter(name="rootPassword")
     def root_password(self) -> pulumi.Output[str]:
         """
@@ -935,14 +1092,16 @@
         return pulumi.get(self, "root_username")
 
     @property
     @pulumi.getter(name="sslConnection")
     def ssl_connection(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+
+        * `updates` - (Optional) Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "ssl_connection")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
@@ -951,34 +1110,36 @@
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def updated(self) -> pulumi.Output[str]:
         """
         When this Managed Database was last updated.
         """
         return pulumi.get(self, "updated")
 
     @property
     @pulumi.getter
-    def updates(self) -> pulumi.Output['outputs.DatabaseMysqlUpdates']:
+    def updates(self) -> pulumi.Output['outputs.DatabasePostgresqlUpdates']:
         """
         Configuration settings for automated patch update maintenance for the Managed Database.
         """
         return pulumi.get(self, "updates")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
-        The Managed Database engine version. (e.g. `v8.0.26`)
+        The Managed Database engine version. (e.g. `13.2`)
         """
         return pulumi.get(self, "version")
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/database_postgresql.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/user.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,1055 +7,868 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['DatabasePostgresqlArgs', 'DatabasePostgresql']
+__all__ = ['UserArgs', 'User']
 
 @pulumi.input_type
-class DatabasePostgresqlArgs:
+class UserArgs:
     def __init__(__self__, *,
-                 engine_id: pulumi.Input[str],
-                 label: pulumi.Input[str],
-                 region: pulumi.Input[str],
-                 type: pulumi.Input[str],
-                 allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 cluster_size: Optional[pulumi.Input[int]] = None,
-                 encrypted: Optional[pulumi.Input[bool]] = None,
-                 replication_commit_type: Optional[pulumi.Input[str]] = None,
-                 replication_type: Optional[pulumi.Input[str]] = None,
-                 ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 updates: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']] = None):
-        """
-        The set of arguments for constructing a DatabasePostgresql resource.
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
-        :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
-        :param pulumi.Input[str] region: The region to use for the Managed Database.
-        :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
-        :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
-        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
-        :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input['DatabasePostgresqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
-        """
-        pulumi.set(__self__, "engine_id", engine_id)
-        pulumi.set(__self__, "label", label)
-        pulumi.set(__self__, "region", region)
-        pulumi.set(__self__, "type", type)
-        if allow_lists is not None:
-            pulumi.set(__self__, "allow_lists", allow_lists)
-        if cluster_size is not None:
-            pulumi.set(__self__, "cluster_size", cluster_size)
-        if encrypted is not None:
-            pulumi.set(__self__, "encrypted", encrypted)
-        if replication_commit_type is not None:
-            pulumi.set(__self__, "replication_commit_type", replication_commit_type)
-        if replication_type is not None:
-            pulumi.set(__self__, "replication_type", replication_type)
-        if ssl_connection is not None:
-            pulumi.set(__self__, "ssl_connection", ssl_connection)
-        if updates is not None:
-            pulumi.set(__self__, "updates", updates)
-
-    @property
-    @pulumi.getter(name="engineId")
-    def engine_id(self) -> pulumi.Input[str]:
-        """
-        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
-        """
-        return pulumi.get(self, "engine_id")
-
-    @engine_id.setter
-    def engine_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "engine_id", value)
-
-    @property
-    @pulumi.getter
-    def label(self) -> pulumi.Input[str]:
+                 email: pulumi.Input[str],
+                 username: pulumi.Input[str],
+                 domain_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]]] = None,
+                 firewall_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]]] = None,
+                 global_grants: Optional[pulumi.Input['UserGlobalGrantsArgs']] = None,
+                 image_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]]] = None,
+                 linode_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]]] = None,
+                 longview_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]]] = None,
+                 nodebalancer_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]]] = None,
+                 restricted: Optional[pulumi.Input[bool]] = None,
+                 stackscript_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]]] = None,
+                 volume_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]]] = None):
         """
-        A unique, user-defined string referring to the Managed Database.
+        The set of arguments for constructing a User resource.
+        :param pulumi.Input[str] email: The email address of the user.
+        :param pulumi.Input[str] username: The username of the user.
+        :param pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]] domain_grants: The domains the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]] firewall_grants: The firewalls the user has permissions access to.
+        :param pulumi.Input['UserGlobalGrantsArgs'] global_grants: A structure containing the Account-level grants a User has.
+        :param pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]] image_grants: The images the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]] linode_grants: The Linodes the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]] longview_grants: The longview the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]] nodebalancer_grants: The NodeBalancers the user has permissions access to.
+        :param pulumi.Input[bool] restricted: If true, this user will only have explicit permissions granted.
+               
+               * `global_grants` - (optional) A structure containing the Account-level grants a User has.
+               
+               The following arguments are sets of entity grants:
+        :param pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]] stackscript_grants: The StackScripts the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]] volume_grants: The volumes the user has permissions access to.
         """
-        return pulumi.get(self, "label")
-
-    @label.setter
-    def label(self, value: pulumi.Input[str]):
-        pulumi.set(self, "label", value)
+        pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "username", username)
+        if domain_grants is not None:
+            pulumi.set(__self__, "domain_grants", domain_grants)
+        if firewall_grants is not None:
+            pulumi.set(__self__, "firewall_grants", firewall_grants)
+        if global_grants is not None:
+            pulumi.set(__self__, "global_grants", global_grants)
+        if image_grants is not None:
+            pulumi.set(__self__, "image_grants", image_grants)
+        if linode_grants is not None:
+            pulumi.set(__self__, "linode_grants", linode_grants)
+        if longview_grants is not None:
+            pulumi.set(__self__, "longview_grants", longview_grants)
+        if nodebalancer_grants is not None:
+            pulumi.set(__self__, "nodebalancer_grants", nodebalancer_grants)
+        if restricted is not None:
+            pulumi.set(__self__, "restricted", restricted)
+        if stackscript_grants is not None:
+            pulumi.set(__self__, "stackscript_grants", stackscript_grants)
+        if volume_grants is not None:
+            pulumi.set(__self__, "volume_grants", volume_grants)
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Input[str]:
+    def email(self) -> pulumi.Input[str]:
         """
-        The region to use for the Managed Database.
+        The email address of the user.
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "email")
 
-    @region.setter
-    def region(self, value: pulumi.Input[str]):
-        pulumi.set(self, "region", value)
+    @email.setter
+    def email(self, value: pulumi.Input[str]):
+        pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
+    def username(self) -> pulumi.Input[str]:
         """
-        The Linode Instance type used for the nodes of the  Managed Database instance.
+        The username of the user.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "username")
 
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
 
     @property
-    @pulumi.getter(name="allowLists")
-    def allow_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="domainGrants")
+    def domain_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]]]:
         """
-        A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
+        The domains the user has permissions access to.
         """
-        return pulumi.get(self, "allow_lists")
+        return pulumi.get(self, "domain_grants")
 
-    @allow_lists.setter
-    def allow_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "allow_lists", value)
+    @domain_grants.setter
+    def domain_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]]]):
+        pulumi.set(self, "domain_grants", value)
 
     @property
-    @pulumi.getter(name="clusterSize")
-    def cluster_size(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="firewallGrants")
+    def firewall_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]]]:
         """
-        The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
+        The firewalls the user has permissions access to.
         """
-        return pulumi.get(self, "cluster_size")
+        return pulumi.get(self, "firewall_grants")
 
-    @cluster_size.setter
-    def cluster_size(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "cluster_size", value)
+    @firewall_grants.setter
+    def firewall_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]]]):
+        pulumi.set(self, "firewall_grants", value)
 
     @property
-    @pulumi.getter
-    def encrypted(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="globalGrants")
+    def global_grants(self) -> Optional[pulumi.Input['UserGlobalGrantsArgs']]:
         """
-        Whether the Managed Databases is encrypted. (default `false`)
+        A structure containing the Account-level grants a User has.
         """
-        return pulumi.get(self, "encrypted")
+        return pulumi.get(self, "global_grants")
 
-    @encrypted.setter
-    def encrypted(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "encrypted", value)
+    @global_grants.setter
+    def global_grants(self, value: Optional[pulumi.Input['UserGlobalGrantsArgs']]):
+        pulumi.set(self, "global_grants", value)
 
     @property
-    @pulumi.getter(name="replicationCommitType")
-    def replication_commit_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="imageGrants")
+    def image_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]]]:
         """
-        The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+        The images the user has permissions access to.
         """
-        return pulumi.get(self, "replication_commit_type")
+        return pulumi.get(self, "image_grants")
 
-    @replication_commit_type.setter
-    def replication_commit_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "replication_commit_type", value)
+    @image_grants.setter
+    def image_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]]]):
+        pulumi.set(self, "image_grants", value)
 
     @property
-    @pulumi.getter(name="replicationType")
-    def replication_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="linodeGrants")
+    def linode_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]]]:
         """
-        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+        The Linodes the user has permissions access to.
         """
-        return pulumi.get(self, "replication_type")
+        return pulumi.get(self, "linode_grants")
 
-    @replication_type.setter
-    def replication_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "replication_type", value)
+    @linode_grants.setter
+    def linode_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]]]):
+        pulumi.set(self, "linode_grants", value)
 
     @property
-    @pulumi.getter(name="sslConnection")
-    def ssl_connection(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="longviewGrants")
+    def longview_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]]]:
         """
-        Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+        The longview the user has permissions access to.
         """
-        return pulumi.get(self, "ssl_connection")
+        return pulumi.get(self, "longview_grants")
 
-    @ssl_connection.setter
-    def ssl_connection(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "ssl_connection", value)
+    @longview_grants.setter
+    def longview_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]]]):
+        pulumi.set(self, "longview_grants", value)
 
     @property
-    @pulumi.getter
-    def updates(self) -> Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]:
+    @pulumi.getter(name="nodebalancerGrants")
+    def nodebalancer_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]]]:
         """
-        Configuration settings for automated patch update maintenance for the Managed Database.
+        The NodeBalancers the user has permissions access to.
         """
-        return pulumi.get(self, "updates")
+        return pulumi.get(self, "nodebalancer_grants")
 
-    @updates.setter
-    def updates(self, value: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]):
-        pulumi.set(self, "updates", value)
-
-
-@pulumi.input_type
-class _DatabasePostgresqlState:
-    def __init__(__self__, *,
-                 allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 ca_cert: Optional[pulumi.Input[str]] = None,
-                 cluster_size: Optional[pulumi.Input[int]] = None,
-                 created: Optional[pulumi.Input[str]] = None,
-                 encrypted: Optional[pulumi.Input[bool]] = None,
-                 engine: Optional[pulumi.Input[str]] = None,
-                 engine_id: Optional[pulumi.Input[str]] = None,
-                 host_primary: Optional[pulumi.Input[str]] = None,
-                 host_secondary: Optional[pulumi.Input[str]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
-                 port: Optional[pulumi.Input[int]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 replication_commit_type: Optional[pulumi.Input[str]] = None,
-                 replication_type: Optional[pulumi.Input[str]] = None,
-                 root_password: Optional[pulumi.Input[str]] = None,
-                 root_username: Optional[pulumi.Input[str]] = None,
-                 ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updated: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering DatabasePostgresql resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
-        :param pulumi.Input[str] ca_cert: The base64-encoded SSL CA certificate for the Managed Database instance.
-        :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[str] created: When this Managed Database was created.
-        :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `postgresql`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
-        :param pulumi.Input[str] host_primary: The primary host for the Managed Database.
-        :param pulumi.Input[str] host_secondary: The secondary/private network host for the Managed Database.
-        :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
-        :param pulumi.Input[int] port: The access port for this Managed Database.
-        :param pulumi.Input[str] region: The region to use for the Managed Database.
-        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
-        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
-        :param pulumi.Input[str] root_password: The randomly-generated root password for the Managed Database instance.
-        :param pulumi.Input[str] root_username: The root username for the Managed Database instance.
-        :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input[str] status: The operating status of the Managed Database.
-        :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
-        :param pulumi.Input[str] updated: When this Managed Database was last updated.
-        :param pulumi.Input['DatabasePostgresqlUpdatesArgs'] updates: Configuration settings for automated patch update maintenance for the Managed Database.
-        :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `13.2`)
-        """
-        if allow_lists is not None:
-            pulumi.set(__self__, "allow_lists", allow_lists)
-        if ca_cert is not None:
-            pulumi.set(__self__, "ca_cert", ca_cert)
-        if cluster_size is not None:
-            pulumi.set(__self__, "cluster_size", cluster_size)
-        if created is not None:
-            pulumi.set(__self__, "created", created)
-        if encrypted is not None:
-            pulumi.set(__self__, "encrypted", encrypted)
-        if engine is not None:
-            pulumi.set(__self__, "engine", engine)
-        if engine_id is not None:
-            pulumi.set(__self__, "engine_id", engine_id)
-        if host_primary is not None:
-            pulumi.set(__self__, "host_primary", host_primary)
-        if host_secondary is not None:
-            pulumi.set(__self__, "host_secondary", host_secondary)
-        if label is not None:
-            pulumi.set(__self__, "label", label)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if replication_commit_type is not None:
-            pulumi.set(__self__, "replication_commit_type", replication_commit_type)
-        if replication_type is not None:
-            pulumi.set(__self__, "replication_type", replication_type)
-        if root_password is not None:
-            pulumi.set(__self__, "root_password", root_password)
-        if root_username is not None:
-            pulumi.set(__self__, "root_username", root_username)
-        if ssl_connection is not None:
-            pulumi.set(__self__, "ssl_connection", ssl_connection)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if updated is not None:
-            pulumi.set(__self__, "updated", updated)
-        if updates is not None:
-            pulumi.set(__self__, "updates", updates)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter(name="allowLists")
-    def allow_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
-        """
-        return pulumi.get(self, "allow_lists")
-
-    @allow_lists.setter
-    def allow_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "allow_lists", value)
-
-    @property
-    @pulumi.getter(name="caCert")
-    def ca_cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        The base64-encoded SSL CA certificate for the Managed Database instance.
-        """
-        return pulumi.get(self, "ca_cert")
-
-    @ca_cert.setter
-    def ca_cert(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ca_cert", value)
-
-    @property
-    @pulumi.getter(name="clusterSize")
-    def cluster_size(self) -> Optional[pulumi.Input[int]]:
-        """
-        The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        """
-        return pulumi.get(self, "cluster_size")
-
-    @cluster_size.setter
-    def cluster_size(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "cluster_size", value)
+    @nodebalancer_grants.setter
+    def nodebalancer_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]]]):
+        pulumi.set(self, "nodebalancer_grants", value)
 
     @property
     @pulumi.getter
-    def created(self) -> Optional[pulumi.Input[str]]:
-        """
-        When this Managed Database was created.
+    def restricted(self) -> Optional[pulumi.Input[bool]]:
         """
-        return pulumi.get(self, "created")
+        If true, this user will only have explicit permissions granted.
 
-    @created.setter
-    def created(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created", value)
+        * `global_grants` - (optional) A structure containing the Account-level grants a User has.
 
-    @property
-    @pulumi.getter
-    def encrypted(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether the Managed Databases is encrypted. (default `false`)
+        The following arguments are sets of entity grants:
         """
-        return pulumi.get(self, "encrypted")
+        return pulumi.get(self, "restricted")
 
-    @encrypted.setter
-    def encrypted(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "encrypted", value)
+    @restricted.setter
+    def restricted(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "restricted", value)
 
     @property
-    @pulumi.getter
-    def engine(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="stackscriptGrants")
+    def stackscript_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]]]:
         """
-        The Managed Database engine. (e.g. `postgresql`)
+        The StackScripts the user has permissions access to.
         """
-        return pulumi.get(self, "engine")
+        return pulumi.get(self, "stackscript_grants")
 
-    @engine.setter
-    def engine(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "engine", value)
+    @stackscript_grants.setter
+    def stackscript_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]]]):
+        pulumi.set(self, "stackscript_grants", value)
 
     @property
-    @pulumi.getter(name="engineId")
-    def engine_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="volumeGrants")
+    def volume_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]]]:
         """
-        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
+        The volumes the user has permissions access to.
         """
-        return pulumi.get(self, "engine_id")
+        return pulumi.get(self, "volume_grants")
 
-    @engine_id.setter
-    def engine_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "engine_id", value)
+    @volume_grants.setter
+    def volume_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]]]):
+        pulumi.set(self, "volume_grants", value)
 
-    @property
-    @pulumi.getter(name="hostPrimary")
-    def host_primary(self) -> Optional[pulumi.Input[str]]:
+
+@pulumi.input_type
+class _UserState:
+    def __init__(__self__, *,
+                 domain_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 firewall_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]]] = None,
+                 global_grants: Optional[pulumi.Input['UserGlobalGrantsArgs']] = None,
+                 image_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]]] = None,
+                 linode_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]]] = None,
+                 longview_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]]] = None,
+                 nodebalancer_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]]] = None,
+                 restricted: Optional[pulumi.Input[bool]] = None,
+                 ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 stackscript_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]]] = None,
+                 tfa_enabled: Optional[pulumi.Input[bool]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
+                 volume_grants: Optional[pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]]] = None):
         """
-        The primary host for the Managed Database.
+        Input properties used for looking up and filtering User resources.
+        :param pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]] domain_grants: The domains the user has permissions access to.
+        :param pulumi.Input[str] email: The email address of the user.
+        :param pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]] firewall_grants: The firewalls the user has permissions access to.
+        :param pulumi.Input['UserGlobalGrantsArgs'] global_grants: A structure containing the Account-level grants a User has.
+        :param pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]] image_grants: The images the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]] linode_grants: The Linodes the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]] longview_grants: The longview the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]] nodebalancer_grants: The NodeBalancers the user has permissions access to.
+        :param pulumi.Input[bool] restricted: If true, this user will only have explicit permissions granted.
+               
+               * `global_grants` - (optional) A structure containing the Account-level grants a User has.
+               
+               The following arguments are sets of entity grants:
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_keys: A list of the User's SSH keys.
+        :param pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]] stackscript_grants: The StackScripts the user has permissions access to.
+        :param pulumi.Input[bool] tfa_enabled: Whether the user has two-factor-authentication enabled.
+        :param pulumi.Input[str] username: The username of the user.
+        :param pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]] volume_grants: The volumes the user has permissions access to.
         """
-        return pulumi.get(self, "host_primary")
-
-    @host_primary.setter
-    def host_primary(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "host_primary", value)
+        if domain_grants is not None:
+            pulumi.set(__self__, "domain_grants", domain_grants)
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+        if firewall_grants is not None:
+            pulumi.set(__self__, "firewall_grants", firewall_grants)
+        if global_grants is not None:
+            pulumi.set(__self__, "global_grants", global_grants)
+        if image_grants is not None:
+            pulumi.set(__self__, "image_grants", image_grants)
+        if linode_grants is not None:
+            pulumi.set(__self__, "linode_grants", linode_grants)
+        if longview_grants is not None:
+            pulumi.set(__self__, "longview_grants", longview_grants)
+        if nodebalancer_grants is not None:
+            pulumi.set(__self__, "nodebalancer_grants", nodebalancer_grants)
+        if restricted is not None:
+            pulumi.set(__self__, "restricted", restricted)
+        if ssh_keys is not None:
+            pulumi.set(__self__, "ssh_keys", ssh_keys)
+        if stackscript_grants is not None:
+            pulumi.set(__self__, "stackscript_grants", stackscript_grants)
+        if tfa_enabled is not None:
+            pulumi.set(__self__, "tfa_enabled", tfa_enabled)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+        if volume_grants is not None:
+            pulumi.set(__self__, "volume_grants", volume_grants)
 
     @property
-    @pulumi.getter(name="hostSecondary")
-    def host_secondary(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="domainGrants")
+    def domain_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]]]:
         """
-        The secondary/private network host for the Managed Database.
+        The domains the user has permissions access to.
         """
-        return pulumi.get(self, "host_secondary")
+        return pulumi.get(self, "domain_grants")
 
-    @host_secondary.setter
-    def host_secondary(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "host_secondary", value)
+    @domain_grants.setter
+    def domain_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserDomainGrantArgs']]]]):
+        pulumi.set(self, "domain_grants", value)
 
     @property
     @pulumi.getter
-    def label(self) -> Optional[pulumi.Input[str]]:
+    def email(self) -> Optional[pulumi.Input[str]]:
         """
-        A unique, user-defined string referring to the Managed Database.
+        The email address of the user.
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "email")
 
-    @label.setter
-    def label(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "label", value)
+    @email.setter
+    def email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "email", value)
 
     @property
-    @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="firewallGrants")
+    def firewall_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]]]:
         """
-        The access port for this Managed Database.
+        The firewalls the user has permissions access to.
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "firewall_grants")
 
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
+    @firewall_grants.setter
+    def firewall_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserFirewallGrantArgs']]]]):
+        pulumi.set(self, "firewall_grants", value)
 
     @property
-    @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="globalGrants")
+    def global_grants(self) -> Optional[pulumi.Input['UserGlobalGrantsArgs']]:
         """
-        The region to use for the Managed Database.
+        A structure containing the Account-level grants a User has.
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "global_grants")
 
-    @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "region", value)
+    @global_grants.setter
+    def global_grants(self, value: Optional[pulumi.Input['UserGlobalGrantsArgs']]):
+        pulumi.set(self, "global_grants", value)
 
     @property
-    @pulumi.getter(name="replicationCommitType")
-    def replication_commit_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="imageGrants")
+    def image_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]]]:
         """
-        The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
+        The images the user has permissions access to.
         """
-        return pulumi.get(self, "replication_commit_type")
+        return pulumi.get(self, "image_grants")
 
-    @replication_commit_type.setter
-    def replication_commit_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "replication_commit_type", value)
+    @image_grants.setter
+    def image_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserImageGrantArgs']]]]):
+        pulumi.set(self, "image_grants", value)
 
     @property
-    @pulumi.getter(name="replicationType")
-    def replication_type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="linodeGrants")
+    def linode_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]]]:
         """
-        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
+        The Linodes the user has permissions access to.
         """
-        return pulumi.get(self, "replication_type")
+        return pulumi.get(self, "linode_grants")
 
-    @replication_type.setter
-    def replication_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "replication_type", value)
+    @linode_grants.setter
+    def linode_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserLinodeGrantArgs']]]]):
+        pulumi.set(self, "linode_grants", value)
 
     @property
-    @pulumi.getter(name="rootPassword")
-    def root_password(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="longviewGrants")
+    def longview_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]]]:
         """
-        The randomly-generated root password for the Managed Database instance.
+        The longview the user has permissions access to.
         """
-        return pulumi.get(self, "root_password")
+        return pulumi.get(self, "longview_grants")
 
-    @root_password.setter
-    def root_password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "root_password", value)
+    @longview_grants.setter
+    def longview_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserLongviewGrantArgs']]]]):
+        pulumi.set(self, "longview_grants", value)
 
     @property
-    @pulumi.getter(name="rootUsername")
-    def root_username(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="nodebalancerGrants")
+    def nodebalancer_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]]]:
         """
-        The root username for the Managed Database instance.
+        The NodeBalancers the user has permissions access to.
         """
-        return pulumi.get(self, "root_username")
+        return pulumi.get(self, "nodebalancer_grants")
 
-    @root_username.setter
-    def root_username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "root_username", value)
+    @nodebalancer_grants.setter
+    def nodebalancer_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserNodebalancerGrantArgs']]]]):
+        pulumi.set(self, "nodebalancer_grants", value)
 
     @property
-    @pulumi.getter(name="sslConnection")
-    def ssl_connection(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def restricted(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
+        If true, this user will only have explicit permissions granted.
+
+        * `global_grants` - (optional) A structure containing the Account-level grants a User has.
+
+        The following arguments are sets of entity grants:
         """
-        return pulumi.get(self, "ssl_connection")
+        return pulumi.get(self, "restricted")
 
-    @ssl_connection.setter
-    def ssl_connection(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "ssl_connection", value)
+    @restricted.setter
+    def restricted(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "restricted", value)
 
     @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="sshKeys")
+    def ssh_keys(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The operating status of the Managed Database.
+        A list of the User's SSH keys.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "ssh_keys")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @ssh_keys.setter
+    def ssh_keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "ssh_keys", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="stackscriptGrants")
+    def stackscript_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]]]:
         """
-        The Linode Instance type used for the nodes of the  Managed Database instance.
+        The StackScripts the user has permissions access to.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "stackscript_grants")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @stackscript_grants.setter
+    def stackscript_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserStackscriptGrantArgs']]]]):
+        pulumi.set(self, "stackscript_grants", value)
 
     @property
-    @pulumi.getter
-    def updated(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="tfaEnabled")
+    def tfa_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        When this Managed Database was last updated.
+        Whether the user has two-factor-authentication enabled.
         """
-        return pulumi.get(self, "updated")
+        return pulumi.get(self, "tfa_enabled")
 
-    @updated.setter
-    def updated(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "updated", value)
+    @tfa_enabled.setter
+    def tfa_enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "tfa_enabled", value)
 
     @property
     @pulumi.getter
-    def updates(self) -> Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]:
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        Configuration settings for automated patch update maintenance for the Managed Database.
+        The username of the user.
         """
-        return pulumi.get(self, "updates")
+        return pulumi.get(self, "username")
 
-    @updates.setter
-    def updates(self, value: Optional[pulumi.Input['DatabasePostgresqlUpdatesArgs']]):
-        pulumi.set(self, "updates", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
     @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="volumeGrants")
+    def volume_grants(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]]]:
         """
-        The Managed Database engine version. (e.g. `13.2`)
+        The volumes the user has permissions access to.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "volume_grants")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
+    @volume_grants.setter
+    def volume_grants(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserVolumeGrantArgs']]]]):
+        pulumi.set(self, "volume_grants", value)
 
 
-class DatabasePostgresql(pulumi.CustomResource):
+class User(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 cluster_size: Optional[pulumi.Input[int]] = None,
-                 encrypted: Optional[pulumi.Input[bool]] = None,
-                 engine_id: Optional[pulumi.Input[str]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 replication_commit_type: Optional[pulumi.Input[str]] = None,
-                 replication_type: Optional[pulumi.Input[str]] = None,
-                 ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
+                 domain_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserDomainGrantArgs']]]]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 firewall_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserFirewallGrantArgs']]]]] = None,
+                 global_grants: Optional[pulumi.Input[pulumi.InputType['UserGlobalGrantsArgs']]] = None,
+                 image_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserImageGrantArgs']]]]] = None,
+                 linode_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLinodeGrantArgs']]]]] = None,
+                 longview_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLongviewGrantArgs']]]]] = None,
+                 nodebalancer_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserNodebalancerGrantArgs']]]]] = None,
+                 restricted: Optional[pulumi.Input[bool]] = None,
+                 stackscript_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserStackscriptGrantArgs']]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
+                 volume_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserVolumeGrantArgs']]]]] = None,
                  __props__=None):
         """
-        Provides a Linode PostgreSQL Database resource. This can be used to create, modify, and delete Linode PostgreSQL Databases.
-        For more information, see the [Linode APIv4 docs](https://www.linode.com/docs/api/databases/).
-
-        Please keep in mind that Managed Databases can take up to an hour to provision.
+        Manages a Linode User.
 
         ## Example Usage
 
-        Creating a simple PostgreSQL database instance:
+        Create an unrestricted user:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabasePostgresql("foobar",
-            engine_id="postgresql/13.2",
-            label="mydatabase",
-            region="us-southeast",
-            type="g6-nanode-1")
+        john = linode.User("john",
+            email="john@acme.io",
+            username="john123")
         ```
 
-        Creating a complex PostgreSQL database instance:
+        Create a restricted user with grants:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabasePostgresql("foobar",
-            allow_lists=["0.0.0.0/0"],
-            cluster_size=3,
-            encrypted=True,
-            engine_id="postgresql/13.2",
-            label="mydatabase",
-            region="us-southeast",
-            replication_commit_type="remote_write",
-            replication_type="semi_synch",
-            ssl_connection=True,
-            type="g6-nanode-1",
-            updates=linode.DatabasePostgresqlUpdatesArgs(
-                day_of_week="saturday",
-                duration=1,
-                frequency="monthly",
-                hour_of_day=22,
-                week_of_month=2,
-            ))
+        fooser = linode.User("fooser",
+            email="cool@acme.io",
+            global_grants=linode.UserGlobalGrantsArgs(
+                add_images=True,
+                add_linodes=True,
+            ),
+            linode_grants=[linode.UserLinodeGrantArgs(
+                id=12345,
+                permissions="read_write",
+            )],
+            restricted=True,
+            username="cooluser123")
         ```
-        ## updates
+        ## Global Grants
 
-        The following arguments are supported in the `updates` specification block:
+        * `account-access` - (optional) The level of access this User has to Account-level actions, like billing information. (`read_only`, `read_write`)
 
-        * `day_of_week` - (Required) The day to perform maintenance. (`monday`, `tuesday`, ...)
+        * `add_domains` - (optional) If true, this User may add Domains.
 
-        * `duration` - (Required) The maximum maintenance window time in hours. (`1`..`3`)
+        * `add_databases` - (optional) If true, this User may add Databases.
 
-        * `frequency` - (Required) Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
+        * `add_firewalls` - (optional) If true, this User may add Firewalls.
 
-        * `hour_of_day` - (Required) The hour to begin maintenance based in UTC time. (`0`..`23`)
+        * `add_images` - (optional) If true, this User may add Images.
 
-        * `week_of_month` - (Optional) The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
+        * `add_linodes` - (optional) If true, this User may create Linodes.
 
-        ## Import
+        * `add_longview` - (optional) If true, this User may create Longview clients and view the current plan.
 
-        Linode PostgreSQL Databases can be imported using the `id`, e.g.
+        * `add_nodebalancers` - (optional) If true, this User may add NodeBalancers.
 
-        ```sh
-         $ pulumi import linode:index/databasePostgresql:DatabasePostgresql foobar 1234567
-        ```
+        * `add_stackscripts` - (optional) If true, this User may add StackScripts.
+
+        * `cancel_account` - (optional) If true, this User may cancel the entire Account.
+
+        * `longview_subscription` - (optional) If true, this User may manage the Account’s Longview subscription.
+
+        ## Entity Grants
+
+        * `id` - (required) The ID of the entity this grant applies to.
+
+        * `permissions` - (required) The level of access this User has to this entity. (`read_only`, `read_write`)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
-        :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
-        :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
-        :param pulumi.Input[str] region: The region to use for the Managed Database.
-        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
-        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
-        :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
-        :param pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserDomainGrantArgs']]]] domain_grants: The domains the user has permissions access to.
+        :param pulumi.Input[str] email: The email address of the user.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserFirewallGrantArgs']]]] firewall_grants: The firewalls the user has permissions access to.
+        :param pulumi.Input[pulumi.InputType['UserGlobalGrantsArgs']] global_grants: A structure containing the Account-level grants a User has.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserImageGrantArgs']]]] image_grants: The images the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLinodeGrantArgs']]]] linode_grants: The Linodes the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLongviewGrantArgs']]]] longview_grants: The longview the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserNodebalancerGrantArgs']]]] nodebalancer_grants: The NodeBalancers the user has permissions access to.
+        :param pulumi.Input[bool] restricted: If true, this user will only have explicit permissions granted.
+               
+               * `global_grants` - (optional) A structure containing the Account-level grants a User has.
+               
+               The following arguments are sets of entity grants:
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserStackscriptGrantArgs']]]] stackscript_grants: The StackScripts the user has permissions access to.
+        :param pulumi.Input[str] username: The username of the user.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserVolumeGrantArgs']]]] volume_grants: The volumes the user has permissions access to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DatabasePostgresqlArgs,
+                 args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Linode PostgreSQL Database resource. This can be used to create, modify, and delete Linode PostgreSQL Databases.
-        For more information, see the [Linode APIv4 docs](https://www.linode.com/docs/api/databases/).
-
-        Please keep in mind that Managed Databases can take up to an hour to provision.
+        Manages a Linode User.
 
         ## Example Usage
 
-        Creating a simple PostgreSQL database instance:
+        Create an unrestricted user:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabasePostgresql("foobar",
-            engine_id="postgresql/13.2",
-            label="mydatabase",
-            region="us-southeast",
-            type="g6-nanode-1")
+        john = linode.User("john",
+            email="john@acme.io",
+            username="john123")
         ```
 
-        Creating a complex PostgreSQL database instance:
+        Create a restricted user with grants:
 
         ```python
         import pulumi
         import pulumi_linode as linode
 
-        foobar = linode.DatabasePostgresql("foobar",
-            allow_lists=["0.0.0.0/0"],
-            cluster_size=3,
-            encrypted=True,
-            engine_id="postgresql/13.2",
-            label="mydatabase",
-            region="us-southeast",
-            replication_commit_type="remote_write",
-            replication_type="semi_synch",
-            ssl_connection=True,
-            type="g6-nanode-1",
-            updates=linode.DatabasePostgresqlUpdatesArgs(
-                day_of_week="saturday",
-                duration=1,
-                frequency="monthly",
-                hour_of_day=22,
-                week_of_month=2,
-            ))
+        fooser = linode.User("fooser",
+            email="cool@acme.io",
+            global_grants=linode.UserGlobalGrantsArgs(
+                add_images=True,
+                add_linodes=True,
+            ),
+            linode_grants=[linode.UserLinodeGrantArgs(
+                id=12345,
+                permissions="read_write",
+            )],
+            restricted=True,
+            username="cooluser123")
         ```
-        ## updates
+        ## Global Grants
 
-        The following arguments are supported in the `updates` specification block:
+        * `account-access` - (optional) The level of access this User has to Account-level actions, like billing information. (`read_only`, `read_write`)
 
-        * `day_of_week` - (Required) The day to perform maintenance. (`monday`, `tuesday`, ...)
+        * `add_domains` - (optional) If true, this User may add Domains.
 
-        * `duration` - (Required) The maximum maintenance window time in hours. (`1`..`3`)
+        * `add_databases` - (optional) If true, this User may add Databases.
 
-        * `frequency` - (Required) Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
+        * `add_firewalls` - (optional) If true, this User may add Firewalls.
 
-        * `hour_of_day` - (Required) The hour to begin maintenance based in UTC time. (`0`..`23`)
+        * `add_images` - (optional) If true, this User may add Images.
 
-        * `week_of_month` - (Optional) The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
+        * `add_linodes` - (optional) If true, this User may create Linodes.
 
-        ## Import
+        * `add_longview` - (optional) If true, this User may create Longview clients and view the current plan.
 
-        Linode PostgreSQL Databases can be imported using the `id`, e.g.
+        * `add_nodebalancers` - (optional) If true, this User may add NodeBalancers.
 
-        ```sh
-         $ pulumi import linode:index/databasePostgresql:DatabasePostgresql foobar 1234567
-        ```
+        * `add_stackscripts` - (optional) If true, this User may add StackScripts.
+
+        * `cancel_account` - (optional) If true, this User may cancel the entire Account.
+
+        * `longview_subscription` - (optional) If true, this User may manage the Account’s Longview subscription.
+
+        ## Entity Grants
+
+        * `id` - (required) The ID of the entity this grant applies to.
+
+        * `permissions` - (required) The level of access this User has to this entity. (`read_only`, `read_write`)
 
         :param str resource_name: The name of the resource.
-        :param DatabasePostgresqlArgs args: The arguments to use to populate this resource's properties.
+        :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DatabasePostgresqlArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 cluster_size: Optional[pulumi.Input[int]] = None,
-                 encrypted: Optional[pulumi.Input[bool]] = None,
-                 engine_id: Optional[pulumi.Input[str]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 replication_commit_type: Optional[pulumi.Input[str]] = None,
-                 replication_type: Optional[pulumi.Input[str]] = None,
-                 ssl_connection: Optional[pulumi.Input[bool]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
+                 domain_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserDomainGrantArgs']]]]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 firewall_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserFirewallGrantArgs']]]]] = None,
+                 global_grants: Optional[pulumi.Input[pulumi.InputType['UserGlobalGrantsArgs']]] = None,
+                 image_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserImageGrantArgs']]]]] = None,
+                 linode_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLinodeGrantArgs']]]]] = None,
+                 longview_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLongviewGrantArgs']]]]] = None,
+                 nodebalancer_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserNodebalancerGrantArgs']]]]] = None,
+                 restricted: Optional[pulumi.Input[bool]] = None,
+                 stackscript_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserStackscriptGrantArgs']]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
+                 volume_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserVolumeGrantArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DatabasePostgresqlArgs.__new__(DatabasePostgresqlArgs)
+            __props__ = UserArgs.__new__(UserArgs)
 
-            __props__.__dict__["allow_lists"] = allow_lists
-            __props__.__dict__["cluster_size"] = cluster_size
-            __props__.__dict__["encrypted"] = encrypted
-            if engine_id is None and not opts.urn:
-                raise TypeError("Missing required property 'engine_id'")
-            __props__.__dict__["engine_id"] = engine_id
-            if label is None and not opts.urn:
-                raise TypeError("Missing required property 'label'")
-            __props__.__dict__["label"] = label
-            if region is None and not opts.urn:
-                raise TypeError("Missing required property 'region'")
-            __props__.__dict__["region"] = region
-            __props__.__dict__["replication_commit_type"] = replication_commit_type
-            __props__.__dict__["replication_type"] = replication_type
-            __props__.__dict__["ssl_connection"] = ssl_connection
-            if type is None and not opts.urn:
-                raise TypeError("Missing required property 'type'")
-            __props__.__dict__["type"] = type
-            __props__.__dict__["updates"] = updates
-            __props__.__dict__["ca_cert"] = None
-            __props__.__dict__["created"] = None
-            __props__.__dict__["engine"] = None
-            __props__.__dict__["host_primary"] = None
-            __props__.__dict__["host_secondary"] = None
-            __props__.__dict__["port"] = None
-            __props__.__dict__["root_password"] = None
-            __props__.__dict__["root_username"] = None
-            __props__.__dict__["status"] = None
-            __props__.__dict__["updated"] = None
-            __props__.__dict__["version"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["caCert", "rootPassword", "rootUsername"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(DatabasePostgresql, __self__).__init__(
-            'linode:index/databasePostgresql:DatabasePostgresql',
+            __props__.__dict__["domain_grants"] = domain_grants
+            if email is None and not opts.urn:
+                raise TypeError("Missing required property 'email'")
+            __props__.__dict__["email"] = email
+            __props__.__dict__["firewall_grants"] = firewall_grants
+            __props__.__dict__["global_grants"] = global_grants
+            __props__.__dict__["image_grants"] = image_grants
+            __props__.__dict__["linode_grants"] = linode_grants
+            __props__.__dict__["longview_grants"] = longview_grants
+            __props__.__dict__["nodebalancer_grants"] = nodebalancer_grants
+            __props__.__dict__["restricted"] = restricted
+            __props__.__dict__["stackscript_grants"] = stackscript_grants
+            if username is None and not opts.urn:
+                raise TypeError("Missing required property 'username'")
+            __props__.__dict__["username"] = username
+            __props__.__dict__["volume_grants"] = volume_grants
+            __props__.__dict__["ssh_keys"] = None
+            __props__.__dict__["tfa_enabled"] = None
+        super(User, __self__).__init__(
+            'linode:index/user:User',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            allow_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            ca_cert: Optional[pulumi.Input[str]] = None,
-            cluster_size: Optional[pulumi.Input[int]] = None,
-            created: Optional[pulumi.Input[str]] = None,
-            encrypted: Optional[pulumi.Input[bool]] = None,
-            engine: Optional[pulumi.Input[str]] = None,
-            engine_id: Optional[pulumi.Input[str]] = None,
-            host_primary: Optional[pulumi.Input[str]] = None,
-            host_secondary: Optional[pulumi.Input[str]] = None,
-            label: Optional[pulumi.Input[str]] = None,
-            port: Optional[pulumi.Input[int]] = None,
-            region: Optional[pulumi.Input[str]] = None,
-            replication_commit_type: Optional[pulumi.Input[str]] = None,
-            replication_type: Optional[pulumi.Input[str]] = None,
-            root_password: Optional[pulumi.Input[str]] = None,
-            root_username: Optional[pulumi.Input[str]] = None,
-            ssl_connection: Optional[pulumi.Input[bool]] = None,
-            status: Optional[pulumi.Input[str]] = None,
-            type: Optional[pulumi.Input[str]] = None,
-            updated: Optional[pulumi.Input[str]] = None,
-            updates: Optional[pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']]] = None,
-            version: Optional[pulumi.Input[str]] = None) -> 'DatabasePostgresql':
+            domain_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserDomainGrantArgs']]]]] = None,
+            email: Optional[pulumi.Input[str]] = None,
+            firewall_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserFirewallGrantArgs']]]]] = None,
+            global_grants: Optional[pulumi.Input[pulumi.InputType['UserGlobalGrantsArgs']]] = None,
+            image_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserImageGrantArgs']]]]] = None,
+            linode_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLinodeGrantArgs']]]]] = None,
+            longview_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLongviewGrantArgs']]]]] = None,
+            nodebalancer_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserNodebalancerGrantArgs']]]]] = None,
+            restricted: Optional[pulumi.Input[bool]] = None,
+            ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            stackscript_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserStackscriptGrantArgs']]]]] = None,
+            tfa_enabled: Optional[pulumi.Input[bool]] = None,
+            username: Optional[pulumi.Input[str]] = None,
+            volume_grants: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserVolumeGrantArgs']]]]] = None) -> 'User':
         """
-        Get an existing DatabasePostgresql resource's state with the given name, id, and optional extra
+        Get an existing User resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] allow_lists: A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
-        :param pulumi.Input[str] ca_cert: The base64-encoded SSL CA certificate for the Managed Database instance.
-        :param pulumi.Input[int] cluster_size: The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        :param pulumi.Input[str] created: When this Managed Database was created.
-        :param pulumi.Input[bool] encrypted: Whether the Managed Databases is encrypted. (default `false`)
-        :param pulumi.Input[str] engine: The Managed Database engine. (e.g. `postgresql`)
-        :param pulumi.Input[str] engine_id: The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
-        :param pulumi.Input[str] host_primary: The primary host for the Managed Database.
-        :param pulumi.Input[str] host_secondary: The secondary/private network host for the Managed Database.
-        :param pulumi.Input[str] label: A unique, user-defined string referring to the Managed Database.
-        :param pulumi.Input[int] port: The access port for this Managed Database.
-        :param pulumi.Input[str] region: The region to use for the Managed Database.
-        :param pulumi.Input[str] replication_commit_type: The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
-        :param pulumi.Input[str] replication_type: The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
-        :param pulumi.Input[str] root_password: The randomly-generated root password for the Managed Database instance.
-        :param pulumi.Input[str] root_username: The root username for the Managed Database instance.
-        :param pulumi.Input[bool] ssl_connection: Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        :param pulumi.Input[str] status: The operating status of the Managed Database.
-        :param pulumi.Input[str] type: The Linode Instance type used for the nodes of the  Managed Database instance.
-        :param pulumi.Input[str] updated: When this Managed Database was last updated.
-        :param pulumi.Input[pulumi.InputType['DatabasePostgresqlUpdatesArgs']] updates: Configuration settings for automated patch update maintenance for the Managed Database.
-        :param pulumi.Input[str] version: The Managed Database engine version. (e.g. `13.2`)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserDomainGrantArgs']]]] domain_grants: The domains the user has permissions access to.
+        :param pulumi.Input[str] email: The email address of the user.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserFirewallGrantArgs']]]] firewall_grants: The firewalls the user has permissions access to.
+        :param pulumi.Input[pulumi.InputType['UserGlobalGrantsArgs']] global_grants: A structure containing the Account-level grants a User has.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserImageGrantArgs']]]] image_grants: The images the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLinodeGrantArgs']]]] linode_grants: The Linodes the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserLongviewGrantArgs']]]] longview_grants: The longview the user has permissions access to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserNodebalancerGrantArgs']]]] nodebalancer_grants: The NodeBalancers the user has permissions access to.
+        :param pulumi.Input[bool] restricted: If true, this user will only have explicit permissions granted.
+               
+               * `global_grants` - (optional) A structure containing the Account-level grants a User has.
+               
+               The following arguments are sets of entity grants:
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_keys: A list of the User's SSH keys.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserStackscriptGrantArgs']]]] stackscript_grants: The StackScripts the user has permissions access to.
+        :param pulumi.Input[bool] tfa_enabled: Whether the user has two-factor-authentication enabled.
+        :param pulumi.Input[str] username: The username of the user.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserVolumeGrantArgs']]]] volume_grants: The volumes the user has permissions access to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DatabasePostgresqlState.__new__(_DatabasePostgresqlState)
-
-        __props__.__dict__["allow_lists"] = allow_lists
-        __props__.__dict__["ca_cert"] = ca_cert
-        __props__.__dict__["cluster_size"] = cluster_size
-        __props__.__dict__["created"] = created
-        __props__.__dict__["encrypted"] = encrypted
-        __props__.__dict__["engine"] = engine
-        __props__.__dict__["engine_id"] = engine_id
-        __props__.__dict__["host_primary"] = host_primary
-        __props__.__dict__["host_secondary"] = host_secondary
-        __props__.__dict__["label"] = label
-        __props__.__dict__["port"] = port
-        __props__.__dict__["region"] = region
-        __props__.__dict__["replication_commit_type"] = replication_commit_type
-        __props__.__dict__["replication_type"] = replication_type
-        __props__.__dict__["root_password"] = root_password
-        __props__.__dict__["root_username"] = root_username
-        __props__.__dict__["ssl_connection"] = ssl_connection
-        __props__.__dict__["status"] = status
-        __props__.__dict__["type"] = type
-        __props__.__dict__["updated"] = updated
-        __props__.__dict__["updates"] = updates
-        __props__.__dict__["version"] = version
-        return DatabasePostgresql(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="allowLists")
-    def allow_lists(self) -> pulumi.Output[Sequence[str]]:
-        """
-        A list of IP addresses that can access the Managed Database. Each item can be a single IP address or a range in CIDR format. Use `DatabaseAccessControls` to manage your allow list separately.
-        """
-        return pulumi.get(self, "allow_lists")
-
-    @property
-    @pulumi.getter(name="caCert")
-    def ca_cert(self) -> pulumi.Output[str]:
-        """
-        The base64-encoded SSL CA certificate for the Managed Database instance.
-        """
-        return pulumi.get(self, "ca_cert")
+        __props__ = _UserState.__new__(_UserState)
 
-    @property
-    @pulumi.getter(name="clusterSize")
-    def cluster_size(self) -> pulumi.Output[Optional[int]]:
-        """
-        The number of Linode Instance nodes deployed to the Managed Database. (default `1`)
-        """
-        return pulumi.get(self, "cluster_size")
+        __props__.__dict__["domain_grants"] = domain_grants
+        __props__.__dict__["email"] = email
+        __props__.__dict__["firewall_grants"] = firewall_grants
+        __props__.__dict__["global_grants"] = global_grants
+        __props__.__dict__["image_grants"] = image_grants
+        __props__.__dict__["linode_grants"] = linode_grants
+        __props__.__dict__["longview_grants"] = longview_grants
+        __props__.__dict__["nodebalancer_grants"] = nodebalancer_grants
+        __props__.__dict__["restricted"] = restricted
+        __props__.__dict__["ssh_keys"] = ssh_keys
+        __props__.__dict__["stackscript_grants"] = stackscript_grants
+        __props__.__dict__["tfa_enabled"] = tfa_enabled
+        __props__.__dict__["username"] = username
+        __props__.__dict__["volume_grants"] = volume_grants
+        return User(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def created(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="domainGrants")
+    def domain_grants(self) -> pulumi.Output[Sequence['outputs.UserDomainGrant']]:
         """
-        When this Managed Database was created.
+        The domains the user has permissions access to.
         """
-        return pulumi.get(self, "created")
+        return pulumi.get(self, "domain_grants")
 
     @property
     @pulumi.getter
-    def encrypted(self) -> pulumi.Output[Optional[bool]]:
+    def email(self) -> pulumi.Output[str]:
         """
-        Whether the Managed Databases is encrypted. (default `false`)
+        The email address of the user.
         """
-        return pulumi.get(self, "encrypted")
+        return pulumi.get(self, "email")
 
     @property
-    @pulumi.getter
-    def engine(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="firewallGrants")
+    def firewall_grants(self) -> pulumi.Output[Sequence['outputs.UserFirewallGrant']]:
         """
-        The Managed Database engine. (e.g. `postgresql`)
+        The firewalls the user has permissions access to.
         """
-        return pulumi.get(self, "engine")
+        return pulumi.get(self, "firewall_grants")
 
     @property
-    @pulumi.getter(name="engineId")
-    def engine_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="globalGrants")
+    def global_grants(self) -> pulumi.Output['outputs.UserGlobalGrants']:
         """
-        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
+        A structure containing the Account-level grants a User has.
         """
-        return pulumi.get(self, "engine_id")
+        return pulumi.get(self, "global_grants")
 
     @property
-    @pulumi.getter(name="hostPrimary")
-    def host_primary(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="imageGrants")
+    def image_grants(self) -> pulumi.Output[Sequence['outputs.UserImageGrant']]:
         """
-        The primary host for the Managed Database.
+        The images the user has permissions access to.
         """
-        return pulumi.get(self, "host_primary")
+        return pulumi.get(self, "image_grants")
 
     @property
-    @pulumi.getter(name="hostSecondary")
-    def host_secondary(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="linodeGrants")
+    def linode_grants(self) -> pulumi.Output[Sequence['outputs.UserLinodeGrant']]:
         """
-        The secondary/private network host for the Managed Database.
+        The Linodes the user has permissions access to.
         """
-        return pulumi.get(self, "host_secondary")
+        return pulumi.get(self, "linode_grants")
 
     @property
-    @pulumi.getter
-    def label(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="longviewGrants")
+    def longview_grants(self) -> pulumi.Output[Sequence['outputs.UserLongviewGrant']]:
         """
-        A unique, user-defined string referring to the Managed Database.
+        The longview the user has permissions access to.
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "longview_grants")
 
     @property
-    @pulumi.getter
-    def port(self) -> pulumi.Output[int]:
+    @pulumi.getter(name="nodebalancerGrants")
+    def nodebalancer_grants(self) -> pulumi.Output[Sequence['outputs.UserNodebalancerGrant']]:
         """
-        The access port for this Managed Database.
+        The NodeBalancers the user has permissions access to.
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "nodebalancer_grants")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[str]:
-        """
-        The region to use for the Managed Database.
-        """
-        return pulumi.get(self, "region")
-
-    @property
-    @pulumi.getter(name="replicationCommitType")
-    def replication_commit_type(self) -> pulumi.Output[Optional[str]]:
-        """
-        The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`; default `off`)
-        """
-        return pulumi.get(self, "replication_commit_type")
-
-    @property
-    @pulumi.getter(name="replicationType")
-    def replication_type(self) -> pulumi.Output[Optional[str]]:
-        """
-        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`; default `none`)
-        """
-        return pulumi.get(self, "replication_type")
-
-    @property
-    @pulumi.getter(name="rootPassword")
-    def root_password(self) -> pulumi.Output[str]:
+    def restricted(self) -> pulumi.Output[Optional[bool]]:
         """
-        The randomly-generated root password for the Managed Database instance.
-        """
-        return pulumi.get(self, "root_password")
+        If true, this user will only have explicit permissions granted.
 
-    @property
-    @pulumi.getter(name="rootUsername")
-    def root_username(self) -> pulumi.Output[str]:
-        """
-        The root username for the Managed Database instance.
-        """
-        return pulumi.get(self, "root_username")
+        * `global_grants` - (optional) A structure containing the Account-level grants a User has.
 
-    @property
-    @pulumi.getter(name="sslConnection")
-    def ssl_connection(self) -> pulumi.Output[Optional[bool]]:
+        The following arguments are sets of entity grants:
         """
-        Whether to require SSL credentials to establish a connection to the Managed Database. (default `false`)
-        """
-        return pulumi.get(self, "ssl_connection")
+        return pulumi.get(self, "restricted")
 
     @property
-    @pulumi.getter
-    def status(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="sshKeys")
+    def ssh_keys(self) -> pulumi.Output[Sequence[str]]:
         """
-        The operating status of the Managed Database.
+        A list of the User's SSH keys.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "ssh_keys")
 
     @property
-    @pulumi.getter
-    def type(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="stackscriptGrants")
+    def stackscript_grants(self) -> pulumi.Output[Sequence['outputs.UserStackscriptGrant']]:
         """
-        The Linode Instance type used for the nodes of the  Managed Database instance.
+        The StackScripts the user has permissions access to.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "stackscript_grants")
 
     @property
-    @pulumi.getter
-    def updated(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="tfaEnabled")
+    def tfa_enabled(self) -> pulumi.Output[bool]:
         """
-        When this Managed Database was last updated.
+        Whether the user has two-factor-authentication enabled.
         """
-        return pulumi.get(self, "updated")
+        return pulumi.get(self, "tfa_enabled")
 
     @property
     @pulumi.getter
-    def updates(self) -> pulumi.Output['outputs.DatabasePostgresqlUpdates']:
+    def username(self) -> pulumi.Output[str]:
         """
-        Configuration settings for automated patch update maintenance for the Managed Database.
+        The username of the user.
         """
-        return pulumi.get(self, "updates")
+        return pulumi.get(self, "username")
 
     @property
-    @pulumi.getter
-    def version(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="volumeGrants")
+    def volume_grants(self) -> pulumi.Output[Sequence['outputs.UserVolumeGrant']]:
         """
-        The Managed Database engine version. (e.g. `13.2`)
+        The volumes the user has permissions access to.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "volume_grants")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/domain.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         :param pulumi.Input[str] domain: The domain this Domain represents. These must be unique in our system; you cannot have two Domains representing the same domain.
         :param pulumi.Input[str] type: If this Domain represents the authoritative source of information for the domain it describes, or if it is a read-only copy of a master (also called a slave).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] axfr_ips: The list of IPs that may perform a zone transfer for this Domain. This is potentially dangerous, and should be set to an empty list unless you intend to use it.
         :param pulumi.Input[str] description: A description for this Domain. This is for display purposes only.
         :param pulumi.Input[int] expire_sec: The amount of time in seconds that may pass before this Domain is no longer authoritative. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] group: The group this Domain belongs to. This is for display purposes only.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] master_ips: The IP addresses representing the master DNS for this Domain.
+               
+               - - -
         :param pulumi.Input[int] refresh_sec: The amount of time in seconds before this Domain should be refreshed. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] retry_sec: The interval, in seconds, at which a failed refresh should be retried. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] soa_email: Start of Authority email address. This is required for master Domains.
         :param pulumi.Input[str] status: Used to control whether this Domain is currently being rendered (defaults to "active").
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         """
@@ -141,14 +143,16 @@
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter(name="masterIps")
     def master_ips(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IP addresses representing the master DNS for this Domain.
+
+        - - -
         """
         return pulumi.get(self, "master_ips")
 
     @master_ips.setter
     def master_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "master_ips", value)
 
@@ -245,14 +249,16 @@
         Input properties used for looking up and filtering Domain resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] axfr_ips: The list of IPs that may perform a zone transfer for this Domain. This is potentially dangerous, and should be set to an empty list unless you intend to use it.
         :param pulumi.Input[str] description: A description for this Domain. This is for display purposes only.
         :param pulumi.Input[str] domain: The domain this Domain represents. These must be unique in our system; you cannot have two Domains representing the same domain.
         :param pulumi.Input[int] expire_sec: The amount of time in seconds that may pass before this Domain is no longer authoritative. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] group: The group this Domain belongs to. This is for display purposes only.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] master_ips: The IP addresses representing the master DNS for this Domain.
+               
+               - - -
         :param pulumi.Input[int] refresh_sec: The amount of time in seconds before this Domain should be refreshed. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] retry_sec: The interval, in seconds, at which a failed refresh should be retried. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] soa_email: Start of Authority email address. This is required for master Domains.
         :param pulumi.Input[str] status: Used to control whether this Domain is currently being rendered (defaults to "active").
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] type: If this Domain represents the authoritative source of information for the domain it describes, or if it is a read-only copy of a master (also called a slave).
@@ -345,14 +351,16 @@
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter(name="masterIps")
     def master_ips(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IP addresses representing the master DNS for this Domain.
+
+        - - -
         """
         return pulumi.get(self, "master_ips")
 
     @master_ips.setter
     def master_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "master_ips", value)
 
@@ -501,14 +509,16 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] axfr_ips: The list of IPs that may perform a zone transfer for this Domain. This is potentially dangerous, and should be set to an empty list unless you intend to use it.
         :param pulumi.Input[str] description: A description for this Domain. This is for display purposes only.
         :param pulumi.Input[str] domain: The domain this Domain represents. These must be unique in our system; you cannot have two Domains representing the same domain.
         :param pulumi.Input[int] expire_sec: The amount of time in seconds that may pass before this Domain is no longer authoritative. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] group: The group this Domain belongs to. This is for display purposes only.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] master_ips: The IP addresses representing the master DNS for this Domain.
+               
+               - - -
         :param pulumi.Input[int] refresh_sec: The amount of time in seconds before this Domain should be refreshed. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] retry_sec: The interval, in seconds, at which a failed refresh should be retried. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] soa_email: Start of Authority email address. This is required for master Domains.
         :param pulumi.Input[str] status: Used to control whether this Domain is currently being rendered (defaults to "active").
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] type: If this Domain represents the authoritative source of information for the domain it describes, or if it is a read-only copy of a master (also called a slave).
@@ -642,14 +652,16 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] axfr_ips: The list of IPs that may perform a zone transfer for this Domain. This is potentially dangerous, and should be set to an empty list unless you intend to use it.
         :param pulumi.Input[str] description: A description for this Domain. This is for display purposes only.
         :param pulumi.Input[str] domain: The domain this Domain represents. These must be unique in our system; you cannot have two Domains representing the same domain.
         :param pulumi.Input[int] expire_sec: The amount of time in seconds that may pass before this Domain is no longer authoritative. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] group: The group this Domain belongs to. This is for display purposes only.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] master_ips: The IP addresses representing the master DNS for this Domain.
+               
+               - - -
         :param pulumi.Input[int] refresh_sec: The amount of time in seconds before this Domain should be refreshed. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] retry_sec: The interval, in seconds, at which a failed refresh should be retried. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] soa_email: Start of Authority email address. This is required for master Domains.
         :param pulumi.Input[str] status: Used to control whether this Domain is currently being rendered (defaults to "active").
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 0, 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[str] type: If this Domain represents the authoritative source of information for the domain it describes, or if it is a read-only copy of a master (also called a slave).
@@ -714,14 +726,16 @@
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="masterIps")
     def master_ips(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IP addresses representing the master DNS for this Domain.
+
+        - - -
         """
         return pulumi.get(self, "master_ips")
 
     @property
     @pulumi.getter(name="refreshSec")
     def refresh_sec(self) -> pulumi.Output[Optional[int]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/domain_record.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/domain_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
                  ttl_sec: Optional[pulumi.Input[int]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a DomainRecord resource.
         :param pulumi.Input[int] domain_id: The ID of the Domain to access.  *Changing `domain_id` forces the creation of a new Linode Domain Record.*.
         :param pulumi.Input[str] record_type: The type of Record this is in the DNS system. For example, A records associate a domain name with an IPv4 address, and AAAA records associate a domain name with an IPv6 address. See all supported record types [here](https://www.linode.com/docs/api/domains/#domain-record-create__request-body-schema). *Changing `record_type` forces the creation of a new Linode Domain Record.*.
         :param pulumi.Input[str] target: The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+               
+               - - -
         :param pulumi.Input[str] name: The name of this Record. Setting this is invalid for `SRV` records as it is generated by the API. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the subdomain being associated with an IP address.
         :param pulumi.Input[int] port: The port this Record points to.
         :param pulumi.Input[int] priority: The priority of the target host. Lower values are preferred.
         :param pulumi.Input[str] protocol: The protocol this Record's service communicates with. Only valid for SRV records.
         :param pulumi.Input[str] service: The service this Record identified. Only valid for SRV records.
         :param pulumi.Input[str] tag: The tag portion of a CAA record. It is invalid to set this on other record types.
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
@@ -84,14 +86,16 @@
         pulumi.set(self, "record_type", value)
 
     @property
     @pulumi.getter
     def target(self) -> pulumi.Input[str]:
         """
         The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+
+        - - -
         """
         return pulumi.get(self, "target")
 
     @target.setter
     def target(self, value: pulumi.Input[str]):
         pulumi.set(self, "target", value)
 
@@ -213,14 +217,16 @@
         :param pulumi.Input[int] port: The port this Record points to.
         :param pulumi.Input[int] priority: The priority of the target host. Lower values are preferred.
         :param pulumi.Input[str] protocol: The protocol this Record's service communicates with. Only valid for SRV records.
         :param pulumi.Input[str] record_type: The type of Record this is in the DNS system. For example, A records associate a domain name with an IPv4 address, and AAAA records associate a domain name with an IPv6 address. See all supported record types [here](https://www.linode.com/docs/api/domains/#domain-record-create__request-body-schema). *Changing `record_type` forces the creation of a new Linode Domain Record.*.
         :param pulumi.Input[str] service: The service this Record identified. Only valid for SRV records.
         :param pulumi.Input[str] tag: The tag portion of a CAA record. It is invalid to set this on other record types.
         :param pulumi.Input[str] target: The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+               
+               - - -
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] weight: The relative weight of this Record. Higher values are preferred.
         """
         if domain_id is not None:
             pulumi.set(__self__, "domain_id", domain_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -340,14 +346,16 @@
         pulumi.set(self, "tag", value)
 
     @property
     @pulumi.getter
     def target(self) -> Optional[pulumi.Input[str]]:
         """
         The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+
+        - - -
         """
         return pulumi.get(self, "target")
 
     @target.setter
     def target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target", value)
 
@@ -433,14 +441,16 @@
         :param pulumi.Input[int] port: The port this Record points to.
         :param pulumi.Input[int] priority: The priority of the target host. Lower values are preferred.
         :param pulumi.Input[str] protocol: The protocol this Record's service communicates with. Only valid for SRV records.
         :param pulumi.Input[str] record_type: The type of Record this is in the DNS system. For example, A records associate a domain name with an IPv4 address, and AAAA records associate a domain name with an IPv6 address. See all supported record types [here](https://www.linode.com/docs/api/domains/#domain-record-create__request-body-schema). *Changing `record_type` forces the creation of a new Linode Domain Record.*.
         :param pulumi.Input[str] service: The service this Record identified. Only valid for SRV records.
         :param pulumi.Input[str] tag: The tag portion of a CAA record. It is invalid to set this on other record types.
         :param pulumi.Input[str] target: The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+               
+               - - -
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] weight: The relative weight of this Record. Higher values are preferred.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -564,14 +574,16 @@
         :param pulumi.Input[int] port: The port this Record points to.
         :param pulumi.Input[int] priority: The priority of the target host. Lower values are preferred.
         :param pulumi.Input[str] protocol: The protocol this Record's service communicates with. Only valid for SRV records.
         :param pulumi.Input[str] record_type: The type of Record this is in the DNS system. For example, A records associate a domain name with an IPv4 address, and AAAA records associate a domain name with an IPv6 address. See all supported record types [here](https://www.linode.com/docs/api/domains/#domain-record-create__request-body-schema). *Changing `record_type` forces the creation of a new Linode Domain Record.*.
         :param pulumi.Input[str] service: The service this Record identified. Only valid for SRV records.
         :param pulumi.Input[str] tag: The tag portion of a CAA record. It is invalid to set this on other record types.
         :param pulumi.Input[str] target: The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+               
+               - - -
         :param pulumi.Input[int] ttl_sec: 'Time to Live' - the amount of time in seconds that this Domain's records may be cached by resolvers or other domain servers. Valid values are 30, 120, 300, 3600, 7200, 14400, 28800, 57600, 86400, 172800, 345600, 604800, 1209600, and 2419200 - any other value will be rounded to the nearest valid value.
         :param pulumi.Input[int] weight: The relative weight of this Record. Higher values are preferred.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DomainRecordState.__new__(_DomainRecordState)
 
@@ -653,14 +665,16 @@
         return pulumi.get(self, "tag")
 
     @property
     @pulumi.getter
     def target(self) -> pulumi.Output[str]:
         """
         The target for this Record. This field's actual usage depends on the type of record this represents. For A and AAAA records, this is the address the named Domain should resolve to.
+
+        - - -
         """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter(name="ttlSec")
     def ttl_sec(self) -> pulumi.Output[Optional[int]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/firewall.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/firewall.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,21 @@
                  inbounds: Optional[pulumi.Input[Sequence[pulumi.Input['FirewallInboundArgs']]]] = None,
                  linodes: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  outbounds: Optional[pulumi.Input[Sequence[pulumi.Input['FirewallOutboundArgs']]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Firewall resource.
         :param pulumi.Input[str] inbound_policy: The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+               
+               * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[str] label: This Firewall's unique label.
         :param pulumi.Input[str] outbound_policy: The default behavior for outbound traffic. This setting can be overridden by updating the outbound.action property for an individual Firewall Rule. (`ACCEPT`, `DROP`)
         :param pulumi.Input[bool] disabled: If `true`, the Firewall's rules are not enforced (defaults to `false`).
+               
+               * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallInboundArgs']]] inbounds: A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] linodes: A list of IDs of Linodes this Firewall should govern it's network traffic for.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallOutboundArgs']]] outbounds: A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
         """
         pulumi.set(__self__, "inbound_policy", inbound_policy)
         pulumi.set(__self__, "label", label)
@@ -50,14 +54,16 @@
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="inboundPolicy")
     def inbound_policy(self) -> pulumi.Input[str]:
         """
         The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+
+        * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         """
         return pulumi.get(self, "inbound_policy")
 
     @inbound_policy.setter
     def inbound_policy(self, value: pulumi.Input[str]):
         pulumi.set(self, "inbound_policy", value)
 
@@ -86,14 +92,16 @@
         pulumi.set(self, "outbound_policy", value)
 
     @property
     @pulumi.getter
     def disabled(self) -> Optional[pulumi.Input[bool]]:
         """
         If `true`, the Firewall's rules are not enforced (defaults to `false`).
+
+        * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         """
         return pulumi.get(self, "disabled")
 
     @disabled.setter
     def disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disabled", value)
 
@@ -159,15 +167,19 @@
                  outbounds: Optional[pulumi.Input[Sequence[pulumi.Input['FirewallOutboundArgs']]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Firewall resources.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallDeviceArgs']]] devices: The devices associated with this firewall.
         :param pulumi.Input[bool] disabled: If `true`, the Firewall's rules are not enforced (defaults to `false`).
+               
+               * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[str] inbound_policy: The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+               
+               * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input['FirewallInboundArgs']]] inbounds: A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[str] label: This Firewall's unique label.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] linodes: A list of IDs of Linodes this Firewall should govern it's network traffic for.
         :param pulumi.Input[str] outbound_policy: The default behavior for outbound traffic. This setting can be overridden by updating the outbound.action property for an individual Firewall Rule. (`ACCEPT`, `DROP`)
         :param pulumi.Input[Sequence[pulumi.Input['FirewallOutboundArgs']]] outbounds: A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[str] status: The status of the Firewall.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
@@ -206,26 +218,30 @@
         pulumi.set(self, "devices", value)
 
     @property
     @pulumi.getter
     def disabled(self) -> Optional[pulumi.Input[bool]]:
         """
         If `true`, the Firewall's rules are not enforced (defaults to `false`).
+
+        * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         """
         return pulumi.get(self, "disabled")
 
     @disabled.setter
     def disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disabled", value)
 
     @property
     @pulumi.getter(name="inboundPolicy")
     def inbound_policy(self) -> Optional[pulumi.Input[str]]:
         """
         The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+
+        * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         """
         return pulumi.get(self, "inbound_policy")
 
     @inbound_policy.setter
     def inbound_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "inbound_policy", value)
 
@@ -396,15 +412,19 @@
         ```sh
          $ pulumi import linode:index/firewall:Firewall my_firewall 12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disabled: If `true`, the Firewall's rules are not enforced (defaults to `false`).
+               
+               * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[str] inbound_policy: The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+               
+               * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallInboundArgs']]]] inbounds: A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[str] label: This Firewall's unique label.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] linodes: A list of IDs of Linodes this Firewall should govern it's network traffic for.
         :param pulumi.Input[str] outbound_policy: The default behavior for outbound traffic. This setting can be overridden by updating the outbound.action property for an individual Firewall Rule. (`ACCEPT`, `DROP`)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallOutboundArgs']]]] outbounds: A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
         """
@@ -556,15 +576,19 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallDeviceArgs']]]] devices: The devices associated with this firewall.
         :param pulumi.Input[bool] disabled: If `true`, the Firewall's rules are not enforced (defaults to `false`).
+               
+               * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[str] inbound_policy: The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+               
+               * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallInboundArgs']]]] inbounds: A firewall rule that specifies what inbound network traffic is allowed.
         :param pulumi.Input[str] label: This Firewall's unique label.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] linodes: A list of IDs of Linodes this Firewall should govern it's network traffic for.
         :param pulumi.Input[str] outbound_policy: The default behavior for outbound traffic. This setting can be overridden by updating the outbound.action property for an individual Firewall Rule. (`ACCEPT`, `DROP`)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['FirewallOutboundArgs']]]] outbounds: A firewall rule that specifies what outbound network traffic is allowed.
         :param pulumi.Input[str] status: The status of the Firewall.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
@@ -594,22 +618,26 @@
         return pulumi.get(self, "devices")
 
     @property
     @pulumi.getter
     def disabled(self) -> pulumi.Output[Optional[bool]]:
         """
         If `true`, the Firewall's rules are not enforced (defaults to `false`).
+
+        * `inbound` - (Optional) A firewall rule that specifies what inbound network traffic is allowed.
         """
         return pulumi.get(self, "disabled")
 
     @property
     @pulumi.getter(name="inboundPolicy")
     def inbound_policy(self) -> pulumi.Output[str]:
         """
         The default behavior for inbound traffic. This setting can be overridden by updating the inbound.action property of the Firewall Rule. (`ACCEPT`, `DROP`)
+
+        * `outbound` - (Optional) A firewall rule that specifies what outbound network traffic is allowed.
         """
         return pulumi.get(self, "inbound_policy")
 
     @property
     @pulumi.getter
     def inbounds(self) -> pulumi.Output[Optional[Sequence['outputs.FirewallInbound']]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/firewall_device.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/firewall_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def __init__(__self__, address1=None, address2=None, balance=None, city=None, company=None, country=None, email=None, first_name=None, id=None, last_name=None, phone=None, state=None, zip=None):
         if address1 and not isinstance(address1, str):
             raise TypeError("Expected argument 'address1' to be a str")
         pulumi.set(__self__, "address1", address1)
         if address2 and not isinstance(address2, str):
             raise TypeError("Expected argument 'address2' to be a str")
         pulumi.set(__self__, "address2", address2)
-        if balance and not isinstance(balance, int):
-            raise TypeError("Expected argument 'balance' to be a int")
+        if balance and not isinstance(balance, float):
+            raise TypeError("Expected argument 'balance' to be a float")
         pulumi.set(__self__, "balance", balance)
         if city and not isinstance(city, str):
             raise TypeError("Expected argument 'city' to be a str")
         pulumi.set(__self__, "city", city)
         if company and not isinstance(company, str):
             raise TypeError("Expected argument 'company' to be a str")
         pulumi.set(__self__, "company", company)
@@ -75,15 +75,15 @@
         """
         Second line of this Account's billing address.
         """
         return pulumi.get(self, "address2")
 
     @property
     @pulumi.getter
-    def balance(self) -> int:
+    def balance(self) -> float:
         """
         This Account's balance, in US dollars.
         """
         return pulumi.get(self, "balance")
 
     @property
     @pulumi.getter
@@ -124,17 +124,14 @@
         The first name of the person associated with this Account.
         """
         return pulumi.get(self, "first_name")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="lastName")
     def last_name(self) -> str:
         """
         The last name of the person associated with this Account.
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account_login.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account_logins.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account_logins.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             values=["true"],
         ),
         linode.GetAccountLoginsFilterArgs(
             name="username",
             values=["myUsername"],
         ),
     ])
-    pulumi.export("loginIds", [__item.id for __item in [filtered_account_logins.logins]])
+    pulumi.export("loginIds", [__item.id for __item in filtered_account_logins.logins])
     ```
     ## Filterable Fields
 
     * `ip`
 
     * `restricted`
 
@@ -128,15 +128,15 @@
             values=["true"],
         ),
         linode.GetAccountLoginsFilterArgs(
             name="username",
             values=["myUsername"],
         ),
     ])
-    pulumi.export("loginIds", [__item.id for __item in [filtered_account_logins.logins]])
+    pulumi.export("loginIds", [__item.id for __item in filtered_account_logins.logins])
     ```
     ## Filterable Fields
 
     * `ip`
 
     * `restricted`
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_account_settings.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_backups.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,32 +127,34 @@
     import pulumi
     import pulumi_linode as linode
 
     all_backups = linode.get_database_backups(database_id=12345,
         database_type="mysql")
     ```
 
-    Get information about all automatic MongoDB Database Backups:
+    Get information about all automatic PostgreSQL Database Backups:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     auto_backups = linode.get_database_backups(database_id=12345,
-        database_type="mongodb",
+        database_type="postgresql",
         filters=[linode.GetDatabaseBackupsFilterArgs(
             name="type",
             values=["auto"],
         )])
     ```
 
 
     :param int database_id: The ID of the database to retrieve backups for.
-    :param str database_type: The type of the database to retrieve backups for. (`mysql`, `mongodb`, `postgresql`)
+    :param str database_type: The type of the database to retrieve backups for. (`mysql`, `postgresql`)
     :param bool latest: If true, only the latest backup will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select database backups that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`created`)
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['databaseType'] = database_type
     __args__['filters'] = filters
@@ -192,29 +194,31 @@
     import pulumi
     import pulumi_linode as linode
 
     all_backups = linode.get_database_backups(database_id=12345,
         database_type="mysql")
     ```
 
-    Get information about all automatic MongoDB Database Backups:
+    Get information about all automatic PostgreSQL Database Backups:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     auto_backups = linode.get_database_backups(database_id=12345,
-        database_type="mongodb",
+        database_type="postgresql",
         filters=[linode.GetDatabaseBackupsFilterArgs(
             name="type",
             values=["auto"],
         )])
     ```
 
 
     :param int database_id: The ID of the database to retrieve backups for.
-    :param str database_type: The type of the database to retrieve backups for. (`mysql`, `mongodb`, `postgresql`)
+    :param str database_type: The type of the database to retrieve backups for. (`mysql`, `postgresql`)
     :param bool latest: If true, only the latest backup will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select database backups that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`created`)
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_engines.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,28 +104,28 @@
     Get information about all Linode Managed Database engines:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all = linode.get_database_engines()
-    pulumi.export("engineIds", [__item.id for __item in [all.engines]])
+    pulumi.export("engineIds", [__item.id for __item in all.engines])
     ```
 
     Get information about all Linode MySQL Database engines:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     mysql = linode.get_database_engines(filters=[linode.GetDatabaseEnginesFilterArgs(
         name="engine",
         values=["mysql"],
     )])
-    pulumi.export("engineIds", [__item.id for __item in [mysql.engines]])
+    pulumi.export("engineIds", [__item.id for __item in mysql.engines])
     ```
 
     Create a Linode MySQL Database using the latest support MySQL version:
 
     ```python
     import pulumi
     import pulumi_linode as linode
@@ -140,14 +140,16 @@
         engine_id=mysql.engines[0].id,
         region="us-southeast",
         type="g6-nanode-1")
     ```
 
 
     :param bool latest: If true, only the latest engine version will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select engines that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
@@ -178,28 +180,28 @@
     Get information about all Linode Managed Database engines:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all = linode.get_database_engines()
-    pulumi.export("engineIds", [__item.id for __item in [all.engines]])
+    pulumi.export("engineIds", [__item.id for __item in all.engines])
     ```
 
     Get information about all Linode MySQL Database engines:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     mysql = linode.get_database_engines(filters=[linode.GetDatabaseEnginesFilterArgs(
         name="engine",
         values=["mysql"],
     )])
-    pulumi.export("engineIds", [__item.id for __item in [mysql.engines]])
+    pulumi.export("engineIds", [__item.id for __item in mysql.engines])
     ```
 
     Create a Linode MySQL Database using the latest support MySQL version:
 
     ```python
     import pulumi
     import pulumi_linode as linode
@@ -214,11 +216,13 @@
         engine_id=mysql.engines[0].id,
         region="us-southeast",
         type="g6-nanode-1")
     ```
 
 
     :param bool latest: If true, only the latest engine version will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select engines that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_mongodb.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_postgresql.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,38 +7,35 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'GetDatabaseMongodbResult',
-    'AwaitableGetDatabaseMongodbResult',
-    'get_database_mongodb',
-    'get_database_mongodb_output',
+    'GetDatabasePostgresqlResult',
+    'AwaitableGetDatabasePostgresqlResult',
+    'get_database_postgresql',
+    'get_database_postgresql_output',
 ]
 
 @pulumi.output_type
-class GetDatabaseMongodbResult:
+class GetDatabasePostgresqlResult:
     """
-    A collection of values returned by getDatabaseMongodb.
+    A collection of values returned by getDatabasePostgresql.
     """
-    def __init__(__self__, allow_lists=None, ca_cert=None, cluster_size=None, compression_type=None, created=None, database_id=None, encrypted=None, engine=None, engine_id=None, host_primary=None, host_secondary=None, id=None, label=None, peers=None, port=None, region=None, replica_set=None, root_password=None, root_username=None, ssl_connection=None, status=None, storage_engine=None, type=None, updated=None, updates=None, version=None):
+    def __init__(__self__, allow_lists=None, ca_cert=None, cluster_size=None, created=None, database_id=None, encrypted=None, engine=None, engine_id=None, host_primary=None, host_secondary=None, id=None, label=None, port=None, region=None, replication_commit_type=None, replication_type=None, root_password=None, root_username=None, ssl_connection=None, status=None, type=None, updated=None, updates=None, version=None):
         if allow_lists and not isinstance(allow_lists, list):
             raise TypeError("Expected argument 'allow_lists' to be a list")
         pulumi.set(__self__, "allow_lists", allow_lists)
         if ca_cert and not isinstance(ca_cert, str):
             raise TypeError("Expected argument 'ca_cert' to be a str")
         pulumi.set(__self__, "ca_cert", ca_cert)
         if cluster_size and not isinstance(cluster_size, int):
             raise TypeError("Expected argument 'cluster_size' to be a int")
         pulumi.set(__self__, "cluster_size", cluster_size)
-        if compression_type and not isinstance(compression_type, str):
-            raise TypeError("Expected argument 'compression_type' to be a str")
-        pulumi.set(__self__, "compression_type", compression_type)
         if created and not isinstance(created, str):
             raise TypeError("Expected argument 'created' to be a str")
         pulumi.set(__self__, "created", created)
         if database_id and not isinstance(database_id, int):
             raise TypeError("Expected argument 'database_id' to be a int")
         pulumi.set(__self__, "database_id", database_id)
         if encrypted and not isinstance(encrypted, bool):
@@ -58,41 +55,38 @@
         pulumi.set(__self__, "host_secondary", host_secondary)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if label and not isinstance(label, str):
             raise TypeError("Expected argument 'label' to be a str")
         pulumi.set(__self__, "label", label)
-        if peers and not isinstance(peers, list):
-            raise TypeError("Expected argument 'peers' to be a list")
-        pulumi.set(__self__, "peers", peers)
         if port and not isinstance(port, int):
             raise TypeError("Expected argument 'port' to be a int")
         pulumi.set(__self__, "port", port)
         if region and not isinstance(region, str):
             raise TypeError("Expected argument 'region' to be a str")
         pulumi.set(__self__, "region", region)
-        if replica_set and not isinstance(replica_set, str):
-            raise TypeError("Expected argument 'replica_set' to be a str")
-        pulumi.set(__self__, "replica_set", replica_set)
+        if replication_commit_type and not isinstance(replication_commit_type, str):
+            raise TypeError("Expected argument 'replication_commit_type' to be a str")
+        pulumi.set(__self__, "replication_commit_type", replication_commit_type)
+        if replication_type and not isinstance(replication_type, str):
+            raise TypeError("Expected argument 'replication_type' to be a str")
+        pulumi.set(__self__, "replication_type", replication_type)
         if root_password and not isinstance(root_password, str):
             raise TypeError("Expected argument 'root_password' to be a str")
         pulumi.set(__self__, "root_password", root_password)
         if root_username and not isinstance(root_username, str):
             raise TypeError("Expected argument 'root_username' to be a str")
         pulumi.set(__self__, "root_username", root_username)
         if ssl_connection and not isinstance(ssl_connection, bool):
             raise TypeError("Expected argument 'ssl_connection' to be a bool")
         pulumi.set(__self__, "ssl_connection", ssl_connection)
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
-        if storage_engine and not isinstance(storage_engine, str):
-            raise TypeError("Expected argument 'storage_engine' to be a str")
-        pulumi.set(__self__, "storage_engine", storage_engine)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if updated and not isinstance(updated, str):
             raise TypeError("Expected argument 'updated' to be a str")
         pulumi.set(__self__, "updated", updated)
         if updates and not isinstance(updates, list):
@@ -123,22 +117,14 @@
     def cluster_size(self) -> int:
         """
         The number of Linode Instance nodes deployed to the Managed Database.
         """
         return pulumi.get(self, "cluster_size")
 
     @property
-    @pulumi.getter(name="compressionType")
-    def compression_type(self) -> str:
-        """
-        The type of data compression for this Database. (`none`, `snappy`, `zlib`)
-        """
-        return pulumi.get(self, "compression_type")
-
-    @property
     @pulumi.getter
     def created(self) -> str:
         """
         When this Managed Database was created.
         """
         return pulumi.get(self, "created")
 
@@ -155,23 +141,23 @@
         """
         return pulumi.get(self, "encrypted")
 
     @property
     @pulumi.getter
     def engine(self) -> str:
         """
-        The Managed Database engine. (e.g. `mongodb`)
+        The Managed Database engine. (e.g. `postgresql`)
         """
         return pulumi.get(self, "engine")
 
     @property
     @pulumi.getter(name="engineId")
     def engine_id(self) -> str:
         """
-        The Managed Database engine in engine/version format. (e.g. `mongodb/4.4.10`)
+        The Managed Database engine in engine/version format. (e.g. `postgresql/13.2`)
         """
         return pulumi.get(self, "engine_id")
 
     @property
     @pulumi.getter(name="hostPrimary")
     def host_primary(self) -> str:
         """
@@ -201,43 +187,40 @@
         """
         A unique, user-defined string referring to the Managed Database.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
-    def peers(self) -> Sequence[str]:
-        """
-        A set of peer addresses for this Database.
-        """
-        return pulumi.get(self, "peers")
-
-    @property
-    @pulumi.getter
     def port(self) -> int:
-        """
-        The access port for this Managed Database.
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def region(self) -> str:
         """
         The region that hosts this Linode Managed Database.
         """
         return pulumi.get(self, "region")
 
     @property
-    @pulumi.getter(name="replicaSet")
-    def replica_set(self) -> str:
+    @pulumi.getter(name="replicationCommitType")
+    def replication_commit_type(self) -> str:
+        """
+        (Optional) The synchronization level of the replicating server. (`on`, `local`, `remote_write`, `remote_apply`, `off`)
+        """
+        return pulumi.get(self, "replication_commit_type")
+
+    @property
+    @pulumi.getter(name="replicationType")
+    def replication_type(self) -> str:
         """
-        Label for configuring a MongoDB replica set. Choose the same label on multiple Databases to include them in the same replica set.
+        The replication method used for the Managed Database. (`none`, `asynch`, `semi_synch`)
         """
-        return pulumi.get(self, "replica_set")
+        return pulumi.get(self, "replication_type")
 
     @property
     @pulumi.getter(name="rootPassword")
     def root_password(self) -> str:
         """
         The randomly-generated root password for the Managed Database instance.
         """
@@ -264,22 +247,14 @@
     def status(self) -> str:
         """
         The operating status of the Managed Database.
         """
         return pulumi.get(self, "status")
 
     @property
-    @pulumi.getter(name="storageEngine")
-    def storage_engine(self) -> str:
-        """
-        The type of storage engine for this Database. (`mmapv1`, `wiredtiger`)
-        """
-        return pulumi.get(self, "storage_engine")
-
-    @property
     @pulumi.getter
     def type(self) -> str:
         """
         The Linode Instance type used for the nodes of the  Managed Database instance.
         """
         return pulumi.get(self, "type")
 
@@ -289,74 +264,72 @@
         """
         When this Managed Database was last updated.
         """
         return pulumi.get(self, "updated")
 
     @property
     @pulumi.getter
-    def updates(self) -> Sequence['outputs.GetDatabaseMongodbUpdateResult']:
+    def updates(self) -> Sequence['outputs.GetDatabasePostgresqlUpdateResult']:
         return pulumi.get(self, "updates")
 
     @property
     @pulumi.getter
     def version(self) -> str:
         """
         The Managed Database engine version. (e.g. `v8.0.26`)
         """
         return pulumi.get(self, "version")
 
 
-class AwaitableGetDatabaseMongodbResult(GetDatabaseMongodbResult):
+class AwaitableGetDatabasePostgresqlResult(GetDatabasePostgresqlResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetDatabaseMongodbResult(
+        return GetDatabasePostgresqlResult(
             allow_lists=self.allow_lists,
             ca_cert=self.ca_cert,
             cluster_size=self.cluster_size,
-            compression_type=self.compression_type,
             created=self.created,
             database_id=self.database_id,
             encrypted=self.encrypted,
             engine=self.engine,
             engine_id=self.engine_id,
             host_primary=self.host_primary,
             host_secondary=self.host_secondary,
             id=self.id,
             label=self.label,
-            peers=self.peers,
             port=self.port,
             region=self.region,
-            replica_set=self.replica_set,
+            replication_commit_type=self.replication_commit_type,
+            replication_type=self.replication_type,
             root_password=self.root_password,
             root_username=self.root_username,
             ssl_connection=self.ssl_connection,
             status=self.status,
-            storage_engine=self.storage_engine,
             type=self.type,
             updated=self.updated,
             updates=self.updates,
             version=self.version)
 
 
-def get_database_mongodb(database_id: Optional[int] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseMongodbResult:
+def get_database_postgresql(database_id: Optional[int] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabasePostgresqlResult:
     """
-    Provides information about a Linode MongoDB Database.
+    Provides information about a Linode PostgreSQL Database.
 
     ## Example Usage
 
-    Get information about a MongoDB database:
+    Get information about a PostgreSQL database:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_db = linode.get_database_mongodb(database_id=12345)
+    my_db = linode.get_database_postgresql(database_id=12345)
     ```
     ## updates
 
     The following arguments are exported by the `updates` specification block:
 
     * `day_of_week` - The day to perform maintenance. (`monday`, `tuesday`, ...)
 
@@ -365,65 +338,63 @@
     * `frequency` - Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
 
     * `hour_of_day` - The hour to begin maintenance based in UTC time. (`0`..`23`)
 
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
-    :param int database_id: The ID of the MongoDB database.
+    :param int database_id: The ID of the PostgreSQL database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMongodb:getDatabaseMongodb', __args__, opts=opts, typ=GetDatabaseMongodbResult).value
+    __ret__ = pulumi.runtime.invoke('linode:index/getDatabasePostgresql:getDatabasePostgresql', __args__, opts=opts, typ=GetDatabasePostgresqlResult).value
 
-    return AwaitableGetDatabaseMongodbResult(
+    return AwaitableGetDatabasePostgresqlResult(
         allow_lists=__ret__.allow_lists,
         ca_cert=__ret__.ca_cert,
         cluster_size=__ret__.cluster_size,
-        compression_type=__ret__.compression_type,
         created=__ret__.created,
         database_id=__ret__.database_id,
         encrypted=__ret__.encrypted,
         engine=__ret__.engine,
         engine_id=__ret__.engine_id,
         host_primary=__ret__.host_primary,
         host_secondary=__ret__.host_secondary,
         id=__ret__.id,
         label=__ret__.label,
-        peers=__ret__.peers,
         port=__ret__.port,
         region=__ret__.region,
-        replica_set=__ret__.replica_set,
+        replication_commit_type=__ret__.replication_commit_type,
+        replication_type=__ret__.replication_type,
         root_password=__ret__.root_password,
         root_username=__ret__.root_username,
         ssl_connection=__ret__.ssl_connection,
         status=__ret__.status,
-        storage_engine=__ret__.storage_engine,
         type=__ret__.type,
         updated=__ret__.updated,
         updates=__ret__.updates,
         version=__ret__.version)
 
 
-@_utilities.lift_output_func(get_database_mongodb)
-def get_database_mongodb_output(database_id: Optional[pulumi.Input[int]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseMongodbResult]:
+@_utilities.lift_output_func(get_database_postgresql)
+def get_database_postgresql_output(database_id: Optional[pulumi.Input[int]] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabasePostgresqlResult]:
     """
-    Provides information about a Linode MongoDB Database.
+    Provides information about a Linode PostgreSQL Database.
 
     ## Example Usage
 
-    Get information about a MongoDB database:
+    Get information about a PostgreSQL database:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_db = linode.get_database_mongodb(database_id=12345)
+    my_db = linode.get_database_postgresql(database_id=12345)
     ```
     ## updates
 
     The following arguments are exported by the `updates` specification block:
 
     * `day_of_week` - The day to perform maintenance. (`monday`, `tuesday`, ...)
 
@@ -432,10 +403,10 @@
     * `frequency` - Whether maintenance occurs on a weekly or monthly basis. (`weekly`, `monthly`)
 
     * `hour_of_day` - The hour to begin maintenance based in UTC time. (`0`..`23`)
 
     * `week_of_month` - The week of the month to perform monthly frequency updates. Required for `monthly` frequency updates. (`1`..`4`)
 
 
-    :param int database_id: The ID of the MongoDB database.
+    :param int database_id: The ID of the PostgreSQL database.
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_mysql.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_database_mysql_backups.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_database_mysql_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
             values=["auto"],
         )])
     ```
 
 
     :param int database_id: The ID of the database to retrieve backups for.
     :param bool latest: If true, only the latest backup will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select database backups that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`created`)
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['filters'] = filters
     __args__['latest'] = latest
@@ -195,11 +197,13 @@
             values=["auto"],
         )])
     ```
 
 
     :param int database_id: The ID of the database to retrieve backups for.
     :param bool latest: If true, only the latest backup will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select database backups that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`created`)
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_databases.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_databases.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,32 +104,34 @@
     Get information about all Linode Managed Databases:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all = linode.get_databases()
-    pulumi.export("databaseIds", [__item.id for __item in [all.databases]])
+    pulumi.export("databaseIds", [__item.id for __item in all.databases])
     ```
 
     Get information about all Linode MySQL Databases:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     mysql = linode.get_databases(filters=[linode.GetDatabasesFilterArgs(
         name="engine",
         values=["mysql"],
     )])
-    pulumi.export("databaseIds", [__item.id for __item in [mysql.databases]])
+    pulumi.export("databaseIds", [__item.id for __item in mysql.databases])
     ```
 
 
     :param bool latest: If true, only the latest create database will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select databases that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
@@ -160,29 +162,31 @@
     Get information about all Linode Managed Databases:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all = linode.get_databases()
-    pulumi.export("databaseIds", [__item.id for __item in [all.databases]])
+    pulumi.export("databaseIds", [__item.id for __item in all.databases])
     ```
 
     Get information about all Linode MySQL Databases:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     mysql = linode.get_databases(filters=[linode.GetDatabasesFilterArgs(
         name="engine",
         values=["mysql"],
     )])
-    pulumi.export("databaseIds", [__item.id for __item in [mysql.databases]])
+    pulumi.export("databaseIds", [__item.id for __item in mysql.databases])
     ```
 
 
     :param bool latest: If true, only the latest create database will be returned.
+           
+           * `filter` - (Optional) A set of filters used to select databases that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. (`version`)
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_domain.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_domain_record.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_domain_zonefile.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_domain_zonefile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_firewall.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_image.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_images.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_images.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     Get information about all Linode images associated with the current token:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all_images = linode.get_images()
-    pulumi.export("imageIds", [__item.id for __item in [all_images.images]])
+    pulumi.export("imageIds", [__item.id for __item in all_images.images])
     ```
     ## Filterable Fields
 
     * `created_by`
 
     * `deprecated`
 
@@ -147,14 +147,16 @@
 
     * `status`
 
     * `vendor`
 
 
     :param bool latest: If true, only the latest image will be returned. Images without a valid `created` field are not included in the result.
+           
+           * `filter` - (Optional) A set of filters used to select Linode images that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
@@ -204,15 +206,15 @@
     Get information about all Linode images associated with the current token:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all_images = linode.get_images()
-    pulumi.export("imageIds", [__item.id for __item in [all_images.images]])
+    pulumi.export("imageIds", [__item.id for __item in all_images.images])
     ```
     ## Filterable Fields
 
     * `created_by`
 
     * `deprecated`
 
@@ -228,11 +230,13 @@
 
     * `status`
 
     * `vendor`
 
 
     :param bool latest: If true, only the latest image will be returned. Images without a valid `created` field are not included in the result.
+           
+           * `filter` - (Optional) A set of filters used to select Linode images that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_backups.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_backups.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     def __init__(__self__, automatics=None, currents=None, id=None, in_progresses=None, linode_id=None):
         if automatics and not isinstance(automatics, list):
             raise TypeError("Expected argument 'automatics' to be a list")
         pulumi.set(__self__, "automatics", automatics)
         if currents and not isinstance(currents, list):
             raise TypeError("Expected argument 'currents' to be a list")
         pulumi.set(__self__, "currents", currents)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
+        if id and not isinstance(id, int):
+            raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if in_progresses and not isinstance(in_progresses, list):
             raise TypeError("Expected argument 'in_progresses' to be a list")
         pulumi.set(__self__, "in_progresses", in_progresses)
         if linode_id and not isinstance(linode_id, int):
             raise TypeError("Expected argument 'linode_id' to be a int")
         pulumi.set(__self__, "linode_id", linode_id)
@@ -47,17 +47,17 @@
     @property
     @pulumi.getter
     def currents(self) -> Sequence['outputs.GetInstanceBackupsCurrentResult']:
         return pulumi.get(self, "currents")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def id(self) -> int:
         """
-        The provider-assigned unique ID for this managed resource.
+        The unique ID of this Backup.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="inProgresses")
     def in_progresses(self) -> Sequence['outputs.GetInstanceBackupsInProgressResult']:
         return pulumi.get(self, "in_progresses")
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_networking.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_networking.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_type.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instance_types.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instance_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,25 +97,25 @@
     import pulumi
     import pulumi_linode as linode
 
     specific_types = linode.get_instance_types(filters=[linode.GetInstanceTypesFilterArgs(
         name="vcpus",
         values=["2"],
     )])
-    pulumi.export("typeIds", [__item.id for __item in [specific_types.types]])
+    pulumi.export("typeIds", [__item.id for __item in specific_types.types])
     ```
 
     Get information about all Linode Instance types:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all_types = linode.get_instance_types()
-    pulumi.export("typeIds", [__item.id for __item in [all_types.types]])
+    pulumi.export("typeIds", [__item.id for __item in all_types.types])
     ```
     ## Filterable Fields
 
     * `class`
 
     * `disk`
 
@@ -166,25 +166,25 @@
     import pulumi
     import pulumi_linode as linode
 
     specific_types = linode.get_instance_types(filters=[linode.GetInstanceTypesFilterArgs(
         name="vcpus",
         values=["2"],
     )])
-    pulumi.export("typeIds", [__item.id for __item in [specific_types.types]])
+    pulumi.export("typeIds", [__item.id for __item in specific_types.types])
     ```
 
     Get information about all Linode Instance types:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all_types = linode.get_instance_types()
-    pulumi.export("typeIds", [__item.id for __item in [all_types.types]])
+    pulumi.export("typeIds", [__item.id for __item in all_types.types])
     ```
     ## Filterable Fields
 
     * `class`
 
     * `disk`
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_instances.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     Get information about all Linode instances associated with the current token:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all_instances = linode.get_instances()
-    pulumi.export("instanceIds", [__item.id for __item in [all_instances.instances]])
+    pulumi.export("instanceIds", [__item.id for __item in all_instances.instances])
     ```
     ## Filterable Fields
 
     * `group`
 
     * `id`
 
@@ -196,15 +196,15 @@
     Get information about all Linode instances associated with the current token:
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
     all_instances = linode.get_instances()
-    pulumi.export("instanceIds", [__item.id for __item in [all_instances.instances]])
+    pulumi.export("instanceIds", [__item.id for __item in all_instances.instances])
     ```
     ## Filterable Fields
 
     * `group`
 
     * `id`
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_ipv6_range.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_kernel.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_kernel.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_linode_object_storage_bucket.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_linode_object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_lke_cluster.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_lke_versions.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_lke_versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             raise TypeError("Expected argument 'versions' to be a list")
         pulumi.set(__self__, "versions", versions)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The Kubernetes version numbers available for deployment to a Kubernetes cluster in the format of [major].[minor], and the latest supported patch version.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def versions(self) -> Sequence['outputs.GetLkeVersionsVersionResult']:
         return pulumi.get(self, "versions")
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_networking_ip.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_networking_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,14 @@
         The default gateway for this address.
         """
         return pulumi.get(self, "gateway")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="linodeId")
     def linode_id(self) -> int:
         """
         The ID of the Linode this address currently belongs to.
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_node_balancer.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_node_balancer_config.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_node_balancer_node.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_object_storage_cluster.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_object_storage_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_profile.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_region.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_regions.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_ssh_key.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_stack_script.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_stack_script.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
-from ._inputs import *
 
 __all__ = [
     'GetStackScriptResult',
     'AwaitableGetStackScriptResult',
     'get_stack_script',
     'get_stack_script_output',
 ]
@@ -32,16 +31,16 @@
         pulumi.set(__self__, "deployments_active", deployments_active)
         if deployments_total and not isinstance(deployments_total, int):
             raise TypeError("Expected argument 'deployments_total' to be a int")
         pulumi.set(__self__, "deployments_total", deployments_total)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
-        if id and not isinstance(id, int):
-            raise TypeError("Expected argument 'id' to be a int")
+        if id and not isinstance(id, str):
+            raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if images and not isinstance(images, list):
             raise TypeError("Expected argument 'images' to be a list")
         pulumi.set(__self__, "images", images)
         if is_public and not isinstance(is_public, bool):
             raise TypeError("Expected argument 'is_public' to be a bool")
         pulumi.set(__self__, "is_public", is_public)
@@ -97,22 +96,22 @@
         """
         A description for the StackScript.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def id(self) -> int:
+    def id(self) -> str:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def images(self) -> Sequence[str]:
         """
-        An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted.
+        A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted.
         """
         return pulumi.get(self, "images")
 
     @property
     @pulumi.getter(name="isPublic")
     def is_public(self) -> bool:
         """
@@ -195,38 +194,35 @@
             script=self.script,
             updated=self.updated,
             user_defined_fields=self.user_defined_fields,
             user_gravatar_id=self.user_gravatar_id,
             username=self.username)
 
 
-def get_stack_script(id: Optional[int] = None,
-                     user_defined_fields: Optional[Sequence[pulumi.InputType['GetStackScriptUserDefinedFieldArgs']]] = None,
+def get_stack_script(id: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetStackScriptResult:
     """
     Provides details about a specific Linode StackScript.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode StackScript.
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_stackscript = linode.get_stack_script(id=355872)
+    my_stackscript = linode.get_stack_script(id="355872")
     ```
 
 
-    :param int id: The unique numeric ID of the StackScript to query.
-    :param Sequence[pulumi.InputType['GetStackScriptUserDefinedFieldArgs']] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
+    :param str id: The unique numeric ID of the StackScript to query.
     """
     __args__ = dict()
     __args__['id'] = id
-    __args__['userDefinedFields'] = user_defined_fields
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getStackScript:getStackScript', __args__, opts=opts, typ=GetStackScriptResult).value
 
     return AwaitableGetStackScriptResult(
         created=__ret__.created,
         deployments_active=__ret__.deployments_active,
         deployments_total=__ret__.deployments_total,
@@ -240,29 +236,27 @@
         updated=__ret__.updated,
         user_defined_fields=__ret__.user_defined_fields,
         user_gravatar_id=__ret__.user_gravatar_id,
         username=__ret__.username)
 
 
 @_utilities.lift_output_func(get_stack_script)
-def get_stack_script_output(id: Optional[pulumi.Input[int]] = None,
-                            user_defined_fields: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetStackScriptUserDefinedFieldArgs']]]]] = None,
+def get_stack_script_output(id: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetStackScriptResult]:
     """
     Provides details about a specific Linode StackScript.
 
     ## Example Usage
 
     The following example shows how one might use this data source to access information about a Linode StackScript.
 
     ```python
     import pulumi
     import pulumi_linode as linode
 
-    my_stackscript = linode.get_stack_script(id=355872)
+    my_stackscript = linode.get_stack_script(id="355872")
     ```
 
 
-    :param int id: The unique numeric ID of the StackScript to query.
-    :param Sequence[pulumi.InputType['GetStackScriptUserDefinedFieldArgs']] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
+    :param str id: The unique numeric ID of the StackScript to query.
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_stack_scripts.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_stack_scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,16 @@
 
     * `rev_note`
 
     * `username`
 
 
     :param bool latest: If true, only the latest StackScript will be returned. StackScripts without a valid `created` field are not included in the result.
+           
+           * `filter` - (Optional) A set of filters used to select Linode StackScripts that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['latest'] = latest
     __args__['order'] = order
@@ -212,11 +214,13 @@
 
     * `rev_note`
 
     * `username`
 
 
     :param bool latest: If true, only the latest StackScript will be returned. StackScripts without a valid `created` field are not included in the result.
+           
+           * `filter` - (Optional) A set of filters used to select Linode StackScripts that meet certain requirements.
     :param str order: The order in which results should be returned. (`asc`, `desc`; default `asc`)
     :param str order_by: The attribute to order the results by. See the Filterable Fields section for a list of valid fields.
     """
     ...
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_user.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_vlans.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_vlans.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/get_volume.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/image.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,28 @@
                  file_path: Optional[pulumi.Input[str]] = None,
                  linode_id: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Image resource.
         :param pulumi.Input[str] label: A short description of the Image. Labels cannot contain special characters.
         :param pulumi.Input[str] description: A detailed description of this Image.
+               
+               - - -
+               
+               The following arguments apply to creating an image from an existing Linode Instance:
         :param pulumi.Input[int] disk_id: The ID of the Linode Disk that this Image will be created from.
         :param pulumi.Input[str] file_hash: The MD5 hash of the file to be uploaded. This is used to trigger file updates.
         :param pulumi.Input[str] file_path: The path of the image file to be uploaded.
         :param pulumi.Input[int] linode_id: The ID of the Linode that this Image will be created from.
+               
+               - - -
+               
+               > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+               
+               The following arguments apply to uploading an image:
         :param pulumi.Input[str] region: The region of the image. See all regions [here](https://api.linode.com/v4/regions).
         """
         pulumi.set(__self__, "label", label)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disk_id is not None:
             pulumi.set(__self__, "disk_id", disk_id)
@@ -58,14 +68,18 @@
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         A detailed description of this Image.
+
+        - - -
+
+        The following arguments apply to creating an image from an existing Linode Instance:
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -106,14 +120,20 @@
         pulumi.set(self, "file_path", value)
 
     @property
     @pulumi.getter(name="linodeId")
     def linode_id(self) -> Optional[pulumi.Input[int]]:
         """
         The ID of the Linode that this Image will be created from.
+
+        - - -
+
+        > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+
+        The following arguments apply to uploading an image:
         """
         return pulumi.get(self, "linode_id")
 
     @linode_id.setter
     def linode_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "linode_id", value)
 
@@ -151,21 +171,31 @@
                  vendor: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Image resources.
         :param pulumi.Input[str] created: When this Image was created.
         :param pulumi.Input[str] created_by: The name of the User who created this Image.
         :param pulumi.Input[bool] deprecated: Whether or not this Image is deprecated. Will only be True for deprecated public Images.
         :param pulumi.Input[str] description: A detailed description of this Image.
+               
+               - - -
+               
+               The following arguments apply to creating an image from an existing Linode Instance:
         :param pulumi.Input[int] disk_id: The ID of the Linode Disk that this Image will be created from.
         :param pulumi.Input[str] expiry: Only Images created automatically (from a deleted Linode; type=automatic) will expire.
         :param pulumi.Input[str] file_hash: The MD5 hash of the file to be uploaded. This is used to trigger file updates.
         :param pulumi.Input[str] file_path: The path of the image file to be uploaded.
         :param pulumi.Input[bool] is_public: True if the Image is public.
         :param pulumi.Input[str] label: A short description of the Image. Labels cannot contain special characters.
         :param pulumi.Input[int] linode_id: The ID of the Linode that this Image will be created from.
+               
+               - - -
+               
+               > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+               
+               The following arguments apply to uploading an image:
         :param pulumi.Input[str] region: The region of the image. See all regions [here](https://api.linode.com/v4/regions).
         :param pulumi.Input[int] size: The minimum size this Image needs to deploy. Size is in MB.
         :param pulumi.Input[str] status: The current status of this Image.
         :param pulumi.Input[str] type: How the Image was created. 'Manual' Images can be created at any time. 'Automatic' images are created automatically from a deleted Linode.
         :param pulumi.Input[str] vendor: The upstream distribution vendor. Nil for private Images.
         """
         if created is not None:
@@ -238,14 +268,18 @@
         pulumi.set(self, "deprecated", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         A detailed description of this Image.
+
+        - - -
+
+        The following arguments apply to creating an image from an existing Linode Instance:
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -322,14 +356,20 @@
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter(name="linodeId")
     def linode_id(self) -> Optional[pulumi.Input[int]]:
         """
         The ID of the Linode that this Image will be created from.
+
+        - - -
+
+        > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+
+        The following arguments apply to uploading an image:
         """
         return pulumi.get(self, "linode_id")
 
     @linode_id.setter
     def linode_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "linode_id", value)
 
@@ -419,19 +459,29 @@
         ```sh
          $ pulumi import linode:index/image:Image myimage 1234567
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A detailed description of this Image.
+               
+               - - -
+               
+               The following arguments apply to creating an image from an existing Linode Instance:
         :param pulumi.Input[int] disk_id: The ID of the Linode Disk that this Image will be created from.
         :param pulumi.Input[str] file_hash: The MD5 hash of the file to be uploaded. This is used to trigger file updates.
         :param pulumi.Input[str] file_path: The path of the image file to be uploaded.
         :param pulumi.Input[str] label: A short description of the Image. Labels cannot contain special characters.
         :param pulumi.Input[int] linode_id: The ID of the Linode that this Image will be created from.
+               
+               - - -
+               
+               > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+               
+               The following arguments apply to uploading an image:
         :param pulumi.Input[str] region: The region of the image. See all regions [here](https://api.linode.com/v4/regions).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ImageArgs,
@@ -531,21 +581,31 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created: When this Image was created.
         :param pulumi.Input[str] created_by: The name of the User who created this Image.
         :param pulumi.Input[bool] deprecated: Whether or not this Image is deprecated. Will only be True for deprecated public Images.
         :param pulumi.Input[str] description: A detailed description of this Image.
+               
+               - - -
+               
+               The following arguments apply to creating an image from an existing Linode Instance:
         :param pulumi.Input[int] disk_id: The ID of the Linode Disk that this Image will be created from.
         :param pulumi.Input[str] expiry: Only Images created automatically (from a deleted Linode; type=automatic) will expire.
         :param pulumi.Input[str] file_hash: The MD5 hash of the file to be uploaded. This is used to trigger file updates.
         :param pulumi.Input[str] file_path: The path of the image file to be uploaded.
         :param pulumi.Input[bool] is_public: True if the Image is public.
         :param pulumi.Input[str] label: A short description of the Image. Labels cannot contain special characters.
         :param pulumi.Input[int] linode_id: The ID of the Linode that this Image will be created from.
+               
+               - - -
+               
+               > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+               
+               The following arguments apply to uploading an image:
         :param pulumi.Input[str] region: The region of the image. See all regions [here](https://api.linode.com/v4/regions).
         :param pulumi.Input[int] size: The minimum size this Image needs to deploy. Size is in MB.
         :param pulumi.Input[str] status: The current status of this Image.
         :param pulumi.Input[str] type: How the Image was created. 'Manual' Images can be created at any time. 'Automatic' images are created automatically from a deleted Linode.
         :param pulumi.Input[str] vendor: The upstream distribution vendor. Nil for private Images.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -595,14 +655,18 @@
         return pulumi.get(self, "deprecated")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         A detailed description of this Image.
+
+        - - -
+
+        The following arguments apply to creating an image from an existing Linode Instance:
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="diskId")
     def disk_id(self) -> pulumi.Output[Optional[int]]:
         """
@@ -651,14 +715,20 @@
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter(name="linodeId")
     def linode_id(self) -> pulumi.Output[Optional[int]]:
         """
         The ID of the Linode that this Image will be created from.
+
+        - - -
+
+        > **NOTICE:** Uploading images is currently in beta. Ensure `LINODE_API_VERSION` is set to `v4beta` in order to use this functionality.
+
+        The following arguments apply to uploading an image:
         """
         return pulumi.get(self, "linode_id")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/instance.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,29 +46,43 @@
         :param pulumi.Input['InstanceAlertsArgs'] alerts: Configuration options for alert triggers on this Linode.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_keys: A list of SSH public keys to deploy for the root user on the newly created Linode. *This value can not be imported.* *Changing `authorized_keys` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_users: A list of Linode usernames. If the usernames have associated SSH keys, the keys will be appended to the `root` user's `~/.ssh/authorized_keys` file automatically. *This value can not be imported.* *Changing `authorized_users` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] backup_id: A Backup ID from another Linode's available backups. Your User must have read_write access to that Linode, the Backup must have a status of successful, and the Linode must be deployed to the same region as the Backup. See /linode/instances/{linodeId}/backups for a Linode's available backups. This field and the image field are mutually exclusive. *This value can not be imported.* *Changing `backup_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[bool] backups_enabled: If this field is set to true, the created Linode will automatically be enrolled in the Linode Backup service. This will incur an additional charge. The cost for the Backup service is dependent on the Type of Linode deployed.
         :param pulumi.Input[str] boot_config_label: The Label of the Instance Config that should be used to boot the Linode instance.  If there is only one `config`, the `label` of that `config` will be used as the `boot_config_label`. *This value can not be imported.*
         :param pulumi.Input[bool] booted: If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+               
+               * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         :param pulumi.Input[Sequence[pulumi.Input['InstanceConfigArgs']]] configs: Configuration profiles define the VM settings and boot behavior of the Linode Instance.
         :param pulumi.Input[str] group: The display group of the Linode instance.
         :param pulumi.Input[str] image: An Image ID to deploy the Disk from. Official Linode Images start with linode/, while your Images start with `private/`. See [images](https://api.linode.com/v4/images) for more information on the Images available for you to use. Examples are `linode/debian9`, `linode/fedora28`, `linode/ubuntu16.04lts`, `linode/arch`, and `private/12345`. See all images [here](https://api.linode.com/v4/linode/images) (Requires a personal access token; docs [here](https://developers.linode.com/api/v4/images)). *This value can not be imported.* *Changing `image` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input['InstanceInterfaceArgs']]] interfaces: An array of Network Interfaces for this Linode to be created with. If an explicit config or disk is defined, interfaces
                must be declared in the config block.
         :param pulumi.Input[str] label: The Linode's label is for display purposes only. If no label is provided for a Linode, a default will be assigned.
         :param pulumi.Input[bool] private_ip: If true, the created Linode will have private networking enabled, allowing use of the 192.168.128.0/17 network within the Linode's region. It can be enabled on an existing Linode but it can't be disabled.
         :param pulumi.Input[bool] resize_disk: If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+               
+               * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+               
+               * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         :param pulumi.Input[str] root_pass: The initial password for the `root` user account. *This value can not be imported.* *Changing `root_pass` forces the creation of a new Linode Instance.* *If omitted, a random password will be generated but will not be stored in the state.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] shared_ipv4s: A set of IPv4 addresses to be shared with the Instance. These IP addresses can be both private and public, but must be in the same region as the instance.
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Linode. Only accepted if 'stackscript_id' is given. The required values depend on the StackScript being deployed.  *This value can not be imported.* *Changing `stackscript_data` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] stackscript_id: The StackScript to deploy to the newly created Linode. If provided, 'image' must also be provided, and must be an Image that is compatible with this StackScript. *This value can not be imported.* *Changing `stackscript_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] swap_size: When deploying from an Image, this field is optional with a Linode API default of 512mb, otherwise it is ignored. This is used to set the swap disk size for the newly-created Linode.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[str] type: The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+               
+               - - -
         :param pulumi.Input[bool] watchdog_enabled: The watchdog, named Lassie, is a Shutdown Watchdog that monitors your Linode and will reboot it if it powers off unexpectedly. It works by issuing a boot job when your Linode powers off without a shutdown job being responsible. To prevent a loop, Lassie will give up if there have been more than 5 boot jobs issued within 15 minutes.
         """
         pulumi.set(__self__, "region", region)
         if alerts is not None:
             pulumi.set(__self__, "alerts", alerts)
         if authorized_keys is not None:
             pulumi.set(__self__, "authorized_keys", authorized_keys)
@@ -200,14 +214,16 @@
         pulumi.set(self, "boot_config_label", value)
 
     @property
     @pulumi.getter
     def booted(self) -> Optional[pulumi.Input[bool]]:
         """
         If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+
+        * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         """
         return pulumi.get(self, "booted")
 
     @booted.setter
     def booted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "booted", value)
 
@@ -294,14 +310,24 @@
         pulumi.set(self, "private_ip", value)
 
     @property
     @pulumi.getter(name="resizeDisk")
     def resize_disk(self) -> Optional[pulumi.Input[bool]]:
         """
         If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+
+        * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+
+        * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         """
         return pulumi.get(self, "resize_disk")
 
     @resize_disk.setter
     def resize_disk(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "resize_disk", value)
 
@@ -378,14 +404,16 @@
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -443,37 +471,51 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_keys: A list of SSH public keys to deploy for the root user on the newly created Linode. *This value can not be imported.* *Changing `authorized_keys` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_users: A list of Linode usernames. If the usernames have associated SSH keys, the keys will be appended to the `root` user's `~/.ssh/authorized_keys` file automatically. *This value can not be imported.* *Changing `authorized_users` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] backup_id: A Backup ID from another Linode's available backups. Your User must have read_write access to that Linode, the Backup must have a status of successful, and the Linode must be deployed to the same region as the Backup. See /linode/instances/{linodeId}/backups for a Linode's available backups. This field and the image field are mutually exclusive. *This value can not be imported.* *Changing `backup_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input['InstanceBackupsArgs'] backups: Information about this Linode's backups status.
         :param pulumi.Input[bool] backups_enabled: If this field is set to true, the created Linode will automatically be enrolled in the Linode Backup service. This will incur an additional charge. The cost for the Backup service is dependent on the Type of Linode deployed.
         :param pulumi.Input[str] boot_config_label: The Label of the Instance Config that should be used to boot the Linode instance.  If there is only one `config`, the `label` of that `config` will be used as the `boot_config_label`. *This value can not be imported.*
         :param pulumi.Input[bool] booted: If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+               
+               * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         :param pulumi.Input[Sequence[pulumi.Input['InstanceConfigArgs']]] configs: Configuration profiles define the VM settings and boot behavior of the Linode Instance.
         :param pulumi.Input[str] group: The display group of the Linode instance.
         :param pulumi.Input[str] host_uuid: The Linode’s host machine, as a UUID.
         :param pulumi.Input[str] image: An Image ID to deploy the Disk from. Official Linode Images start with linode/, while your Images start with `private/`. See [images](https://api.linode.com/v4/images) for more information on the Images available for you to use. Examples are `linode/debian9`, `linode/fedora28`, `linode/ubuntu16.04lts`, `linode/arch`, and `private/12345`. See all images [here](https://api.linode.com/v4/linode/images) (Requires a personal access token; docs [here](https://developers.linode.com/api/v4/images)). *This value can not be imported.* *Changing `image` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input['InstanceInterfaceArgs']]] interfaces: An array of Network Interfaces for this Linode to be created with. If an explicit config or disk is defined, interfaces
                must be declared in the config block.
         :param pulumi.Input[str] ip_address: A string containing the Linode's public IP address.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ipv4s: This Linode's IPv4 Addresses. Each Linode is assigned a single public IPv4 address upon creation, and may get a single private IPv4 address if needed. You may need to open a support ticket to get additional IPv4 addresses.
         :param pulumi.Input[str] ipv6: This Linode's IPv6 SLAAC addresses. This address is specific to a Linode, and may not be shared.  The prefix (`/64`) is included in this attribute.
         :param pulumi.Input[str] label: The Linode's label is for display purposes only. If no label is provided for a Linode, a default will be assigned.
         :param pulumi.Input[bool] private_ip: If true, the created Linode will have private networking enabled, allowing use of the 192.168.128.0/17 network within the Linode's region. It can be enabled on an existing Linode but it can't be disabled.
         :param pulumi.Input[str] private_ip_address: This Linode's Private IPv4 Address, if enabled.  The regional private IP address range, 192.168.128.0/17, is shared by all Linode Instances in a region.
         :param pulumi.Input[str] region: This is the location where the Linode is deployed. Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Instance.*.
         :param pulumi.Input[bool] resize_disk: If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+               
+               * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+               
+               * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         :param pulumi.Input[str] root_pass: The initial password for the `root` user account. *This value can not be imported.* *Changing `root_pass` forces the creation of a new Linode Instance.* *If omitted, a random password will be generated but will not be stored in the state.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] shared_ipv4s: A set of IPv4 addresses to be shared with the Instance. These IP addresses can be both private and public, but must be in the same region as the instance.
         :param pulumi.Input['InstanceSpecsArgs'] specs: Information about the resources available to this Linode.
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Linode. Only accepted if 'stackscript_id' is given. The required values depend on the StackScript being deployed.  *This value can not be imported.* *Changing `stackscript_data` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] stackscript_id: The StackScript to deploy to the newly created Linode. If provided, 'image' must also be provided, and must be an Image that is compatible with this StackScript. *This value can not be imported.* *Changing `stackscript_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[str] status: The status of the instance, indicating the current readiness state. (`running`, `offline`, ...)
         :param pulumi.Input[int] swap_size: When deploying from an Image, this field is optional with a Linode API default of 512mb, otherwise it is ignored. This is used to set the swap disk size for the newly-created Linode.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[str] type: The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+               
+               - - -
         :param pulumi.Input[bool] watchdog_enabled: The watchdog, named Lassie, is a Shutdown Watchdog that monitors your Linode and will reboot it if it powers off unexpectedly. It works by issuing a boot job when your Linode powers off without a shutdown job being responsible. To prevent a loop, Lassie will give up if there have been more than 5 boot jobs issued within 15 minutes.
         """
         if alerts is not None:
             pulumi.set(__self__, "alerts", alerts)
         if authorized_keys is not None:
             pulumi.set(__self__, "authorized_keys", authorized_keys)
         if authorized_users is not None:
@@ -622,14 +664,16 @@
         pulumi.set(self, "boot_config_label", value)
 
     @property
     @pulumi.getter
     def booted(self) -> Optional[pulumi.Input[bool]]:
         """
         If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+
+        * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         """
         return pulumi.get(self, "booted")
 
     @booted.setter
     def booted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "booted", value)
 
@@ -788,14 +832,24 @@
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="resizeDisk")
     def resize_disk(self) -> Optional[pulumi.Input[bool]]:
         """
         If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+
+        * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+
+        * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         """
         return pulumi.get(self, "resize_disk")
 
     @resize_disk.setter
     def resize_disk(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "resize_disk", value)
 
@@ -896,14 +950,16 @@
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -995,30 +1051,44 @@
         :param pulumi.Input[pulumi.InputType['InstanceAlertsArgs']] alerts: Configuration options for alert triggers on this Linode.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_keys: A list of SSH public keys to deploy for the root user on the newly created Linode. *This value can not be imported.* *Changing `authorized_keys` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_users: A list of Linode usernames. If the usernames have associated SSH keys, the keys will be appended to the `root` user's `~/.ssh/authorized_keys` file automatically. *This value can not be imported.* *Changing `authorized_users` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] backup_id: A Backup ID from another Linode's available backups. Your User must have read_write access to that Linode, the Backup must have a status of successful, and the Linode must be deployed to the same region as the Backup. See /linode/instances/{linodeId}/backups for a Linode's available backups. This field and the image field are mutually exclusive. *This value can not be imported.* *Changing `backup_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[bool] backups_enabled: If this field is set to true, the created Linode will automatically be enrolled in the Linode Backup service. This will incur an additional charge. The cost for the Backup service is dependent on the Type of Linode deployed.
         :param pulumi.Input[str] boot_config_label: The Label of the Instance Config that should be used to boot the Linode instance.  If there is only one `config`, the `label` of that `config` will be used as the `boot_config_label`. *This value can not be imported.*
         :param pulumi.Input[bool] booted: If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+               
+               * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceConfigArgs']]]] configs: Configuration profiles define the VM settings and boot behavior of the Linode Instance.
         :param pulumi.Input[str] group: The display group of the Linode instance.
         :param pulumi.Input[str] image: An Image ID to deploy the Disk from. Official Linode Images start with linode/, while your Images start with `private/`. See [images](https://api.linode.com/v4/images) for more information on the Images available for you to use. Examples are `linode/debian9`, `linode/fedora28`, `linode/ubuntu16.04lts`, `linode/arch`, and `private/12345`. See all images [here](https://api.linode.com/v4/linode/images) (Requires a personal access token; docs [here](https://developers.linode.com/api/v4/images)). *This value can not be imported.* *Changing `image` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceInterfaceArgs']]]] interfaces: An array of Network Interfaces for this Linode to be created with. If an explicit config or disk is defined, interfaces
                must be declared in the config block.
         :param pulumi.Input[str] label: The Linode's label is for display purposes only. If no label is provided for a Linode, a default will be assigned.
         :param pulumi.Input[bool] private_ip: If true, the created Linode will have private networking enabled, allowing use of the 192.168.128.0/17 network within the Linode's region. It can be enabled on an existing Linode but it can't be disabled.
         :param pulumi.Input[str] region: This is the location where the Linode is deployed. Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Instance.*.
         :param pulumi.Input[bool] resize_disk: If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+               
+               * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+               
+               * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         :param pulumi.Input[str] root_pass: The initial password for the `root` user account. *This value can not be imported.* *Changing `root_pass` forces the creation of a new Linode Instance.* *If omitted, a random password will be generated but will not be stored in the state.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] shared_ipv4s: A set of IPv4 addresses to be shared with the Instance. These IP addresses can be both private and public, but must be in the same region as the instance.
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Linode. Only accepted if 'stackscript_id' is given. The required values depend on the StackScript being deployed.  *This value can not be imported.* *Changing `stackscript_data` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] stackscript_id: The StackScript to deploy to the newly created Linode. If provided, 'image' must also be provided, and must be an Image that is compatible with this StackScript. *This value can not be imported.* *Changing `stackscript_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] swap_size: When deploying from an Image, this field is optional with a Linode API default of 512mb, otherwise it is ignored. This is used to set the swap disk size for the newly-created Linode.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[str] type: The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+               
+               - - -
         :param pulumi.Input[bool] watchdog_enabled: The watchdog, named Lassie, is a Shutdown Watchdog that monitors your Linode and will reboot it if it powers off unexpectedly. It works by issuing a boot job when your Linode powers off without a shutdown job being responsible. To prevent a loop, Lassie will give up if there have been more than 5 boot jobs issued within 15 minutes.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: InstanceArgs,
@@ -1200,37 +1270,51 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_keys: A list of SSH public keys to deploy for the root user on the newly created Linode. *This value can not be imported.* *Changing `authorized_keys` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_users: A list of Linode usernames. If the usernames have associated SSH keys, the keys will be appended to the `root` user's `~/.ssh/authorized_keys` file automatically. *This value can not be imported.* *Changing `authorized_users` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] backup_id: A Backup ID from another Linode's available backups. Your User must have read_write access to that Linode, the Backup must have a status of successful, and the Linode must be deployed to the same region as the Backup. See /linode/instances/{linodeId}/backups for a Linode's available backups. This field and the image field are mutually exclusive. *This value can not be imported.* *Changing `backup_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[pulumi.InputType['InstanceBackupsArgs']] backups: Information about this Linode's backups status.
         :param pulumi.Input[bool] backups_enabled: If this field is set to true, the created Linode will automatically be enrolled in the Linode Backup service. This will incur an additional charge. The cost for the Backup service is dependent on the Type of Linode deployed.
         :param pulumi.Input[str] boot_config_label: The Label of the Instance Config that should be used to boot the Linode instance.  If there is only one `config`, the `label` of that `config` will be used as the `boot_config_label`. *This value can not be imported.*
         :param pulumi.Input[bool] booted: If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+               
+               * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceConfigArgs']]]] configs: Configuration profiles define the VM settings and boot behavior of the Linode Instance.
         :param pulumi.Input[str] group: The display group of the Linode instance.
         :param pulumi.Input[str] host_uuid: The Linode’s host machine, as a UUID.
         :param pulumi.Input[str] image: An Image ID to deploy the Disk from. Official Linode Images start with linode/, while your Images start with `private/`. See [images](https://api.linode.com/v4/images) for more information on the Images available for you to use. Examples are `linode/debian9`, `linode/fedora28`, `linode/ubuntu16.04lts`, `linode/arch`, and `private/12345`. See all images [here](https://api.linode.com/v4/linode/images) (Requires a personal access token; docs [here](https://developers.linode.com/api/v4/images)). *This value can not be imported.* *Changing `image` forces the creation of a new Linode Instance.*
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstanceInterfaceArgs']]]] interfaces: An array of Network Interfaces for this Linode to be created with. If an explicit config or disk is defined, interfaces
                must be declared in the config block.
         :param pulumi.Input[str] ip_address: A string containing the Linode's public IP address.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ipv4s: This Linode's IPv4 Addresses. Each Linode is assigned a single public IPv4 address upon creation, and may get a single private IPv4 address if needed. You may need to open a support ticket to get additional IPv4 addresses.
         :param pulumi.Input[str] ipv6: This Linode's IPv6 SLAAC addresses. This address is specific to a Linode, and may not be shared.  The prefix (`/64`) is included in this attribute.
         :param pulumi.Input[str] label: The Linode's label is for display purposes only. If no label is provided for a Linode, a default will be assigned.
         :param pulumi.Input[bool] private_ip: If true, the created Linode will have private networking enabled, allowing use of the 192.168.128.0/17 network within the Linode's region. It can be enabled on an existing Linode but it can't be disabled.
         :param pulumi.Input[str] private_ip_address: This Linode's Private IPv4 Address, if enabled.  The regional private IP address range, 192.168.128.0/17, is shared by all Linode Instances in a region.
         :param pulumi.Input[str] region: This is the location where the Linode is deployed. Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). *Changing `region` forces the creation of a new Linode Instance.*.
         :param pulumi.Input[bool] resize_disk: If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+               
+               * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+               
+               * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+               
+               * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         :param pulumi.Input[str] root_pass: The initial password for the `root` user account. *This value can not be imported.* *Changing `root_pass` forces the creation of a new Linode Instance.* *If omitted, a random password will be generated but will not be stored in the state.*
         :param pulumi.Input[Sequence[pulumi.Input[str]]] shared_ipv4s: A set of IPv4 addresses to be shared with the Instance. These IP addresses can be both private and public, but must be in the same region as the instance.
         :param pulumi.Input[pulumi.InputType['InstanceSpecsArgs']] specs: Information about the resources available to this Linode.
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Linode. Only accepted if 'stackscript_id' is given. The required values depend on the StackScript being deployed.  *This value can not be imported.* *Changing `stackscript_data` forces the creation of a new Linode Instance.*
         :param pulumi.Input[int] stackscript_id: The StackScript to deploy to the newly created Linode. If provided, 'image' must also be provided, and must be an Image that is compatible with this StackScript. *This value can not be imported.* *Changing `stackscript_id` forces the creation of a new Linode Instance.*
         :param pulumi.Input[str] status: The status of the instance, indicating the current readiness state. (`running`, `offline`, ...)
         :param pulumi.Input[int] swap_size: When deploying from an Image, this field is optional with a Linode API default of 512mb, otherwise it is ignored. This is used to set the swap disk size for the newly-created Linode.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[str] type: The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+               
+               - - -
         :param pulumi.Input[bool] watchdog_enabled: The watchdog, named Lassie, is a Shutdown Watchdog that monitors your Linode and will reboot it if it powers off unexpectedly. It works by issuing a boot job when your Linode powers off without a shutdown job being responsible. To prevent a loop, Lassie will give up if there have been more than 5 boot jobs issued within 15 minutes.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstanceState.__new__(_InstanceState)
 
         __props__.__dict__["alerts"] = alerts
@@ -1324,14 +1408,16 @@
         return pulumi.get(self, "boot_config_label")
 
     @property
     @pulumi.getter
     def booted(self) -> pulumi.Output[bool]:
         """
         If true, then the instance is kept or converted into in a running state. If false, the instance will be shutdown. If unspecified, the Linode's power status will not be managed by the Provider.
+
+        * `interface` - (Optional) A list of network interfaces to be assigned to the Linode on creation. If an explicit config or disk is defined, interfaces must be declared in the `config` block.
         """
         return pulumi.get(self, "booted")
 
     @property
     @pulumi.getter
     def configs(self) -> pulumi.Output[Sequence['outputs.InstanceConfig']]:
         """
@@ -1434,14 +1520,24 @@
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="resizeDisk")
     def resize_disk(self) -> pulumi.Output[Optional[bool]]:
         """
         If true, changes in Linode type will attempt to upsize or downsize implicitly created disks. This must be false if explicit disks are defined. *This is an irreversible action as Linode disks cannot be automatically downsized.*
+
+        * `alerts.0.cpu` - (Optional) The percentage of CPU usage required to trigger an alert. If the average CPU usage over two hours exceeds this value, we'll send you an alert. If this is set to 0, the alert is disabled.
+
+        * `alerts.0.network_in` - (Optional) The amount of incoming traffic, in Mbit/s, required to trigger an alert. If the average incoming traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.network_out` - (Optional) The amount of outbound traffic, in Mbit/s, required to trigger an alert. If the average outbound traffic over two hours exceeds this value, we'll send you an alert. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.transfer_quota` - (Optional) The percentage of network transfer that may be used before an alert is triggered. When this value is exceeded, we'll alert you. If this is set to 0 (zero), the alert is disabled.
+
+        * `alerts.0.io` - (Optional) The amount of disk IO operation per second required to trigger an alert. If the average disk IO over two hours exceeds this value, we'll send you an alert. If set to 0, this alert is disabled.
         """
         return pulumi.get(self, "resize_disk")
 
     @property
     @pulumi.getter(name="rootPass")
     def root_pass(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1506,14 +1602,16 @@
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         """
         The Linode type defines the pricing, CPU, disk, and RAM specs of the instance. Examples are `"g6-nanode-1"`, `"g6-standard-2"`, `"g6-highmem-16"`, `"g6-dedicated-16"`, etc. See all types [here](https://api.linode.com/v4/linode/types).
+
+        - - -
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="watchdogEnabled")
     def watchdog_enabled(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/instance_disk.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/instance_disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
                  stackscript_data: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  stackscript_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a InstanceDisk resource.
         :param pulumi.Input[str] label: The Disk's label for display purposes only.
         :param pulumi.Input[int] linode_id: The ID of the Linode to create this Disk under.
         :param pulumi.Input[int] size: The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_keys: A list of public SSH keys that will be automatically appended to the root user’s ~/.ssh/authorized_keys file when deploying from an Image.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_users: A list of usernames. If the usernames have associated SSH keys, the keys will be appended to the
         :param pulumi.Input[str] filesystem: The filesystem of this disk. (`raw`, `swap`, `ext3`, `ext4`, `initrd`)
         :param pulumi.Input[str] image: An Image ID to deploy the Linode Disk from.
         :param pulumi.Input[str] root_pass: The root user’s password on a newly-created Linode Disk when deploying from an Image.
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Disk. Only accepted if `stackscript_id` is given.
         :param pulumi.Input[int] stackscript_id: A StackScript ID that will cause the referenced StackScript to be run during deployment of this Disk.
@@ -80,14 +82,16 @@
         pulumi.set(self, "linode_id", value)
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Input[int]:
         """
         The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+
+        - - -
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: pulumi.Input[int]):
         pulumi.set(self, "size", value)
 
@@ -199,14 +203,16 @@
         :param pulumi.Input[str] created: When this disk was created.
         :param pulumi.Input[str] filesystem: The filesystem of this disk. (`raw`, `swap`, `ext3`, `ext4`, `initrd`)
         :param pulumi.Input[str] image: An Image ID to deploy the Linode Disk from.
         :param pulumi.Input[str] label: The Disk's label for display purposes only.
         :param pulumi.Input[int] linode_id: The ID of the Linode to create this Disk under.
         :param pulumi.Input[str] root_pass: The root user’s password on a newly-created Linode Disk when deploying from an Image.
         :param pulumi.Input[int] size: The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+               
+               - - -
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Disk. Only accepted if `stackscript_id` is given.
         :param pulumi.Input[int] stackscript_id: A StackScript ID that will cause the referenced StackScript to be run during deployment of this Disk.
         :param pulumi.Input[str] status: A brief description of this Disk's current state.
         :param pulumi.Input[str] updated: When this disk was last updated.
         """
         if authorized_keys is not None:
             pulumi.set(__self__, "authorized_keys", authorized_keys)
@@ -332,14 +338,16 @@
         pulumi.set(self, "root_pass", value)
 
     @property
     @pulumi.getter
     def size(self) -> Optional[pulumi.Input[int]]:
         """
         The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+
+        - - -
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "size", value)
 
@@ -471,14 +479,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] authorized_users: A list of usernames. If the usernames have associated SSH keys, the keys will be appended to the
         :param pulumi.Input[str] filesystem: The filesystem of this disk. (`raw`, `swap`, `ext3`, `ext4`, `initrd`)
         :param pulumi.Input[str] image: An Image ID to deploy the Linode Disk from.
         :param pulumi.Input[str] label: The Disk's label for display purposes only.
         :param pulumi.Input[int] linode_id: The ID of the Linode to create this Disk under.
         :param pulumi.Input[str] root_pass: The root user’s password on a newly-created Linode Disk when deploying from an Image.
         :param pulumi.Input[int] size: The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+               
+               - - -
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Disk. Only accepted if `stackscript_id` is given.
         :param pulumi.Input[int] stackscript_id: A StackScript ID that will cause the referenced StackScript to be run during deployment of this Disk.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -631,14 +641,16 @@
         :param pulumi.Input[str] created: When this disk was created.
         :param pulumi.Input[str] filesystem: The filesystem of this disk. (`raw`, `swap`, `ext3`, `ext4`, `initrd`)
         :param pulumi.Input[str] image: An Image ID to deploy the Linode Disk from.
         :param pulumi.Input[str] label: The Disk's label for display purposes only.
         :param pulumi.Input[int] linode_id: The ID of the Linode to create this Disk under.
         :param pulumi.Input[str] root_pass: The root user’s password on a newly-created Linode Disk when deploying from an Image.
         :param pulumi.Input[int] size: The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+               
+               - - -
         :param pulumi.Input[Mapping[str, Any]] stackscript_data: An object containing responses to any User Defined Fields present in the StackScript being deployed to this Disk. Only accepted if `stackscript_id` is given.
         :param pulumi.Input[int] stackscript_id: A StackScript ID that will cause the referenced StackScript to be run during deployment of this Disk.
         :param pulumi.Input[str] status: A brief description of this Disk's current state.
         :param pulumi.Input[str] updated: When this disk was last updated.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -724,14 +736,16 @@
         return pulumi.get(self, "root_pass")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
         """
         The size of the Disk in MB. **NOTE:** Resizing a disk will trigger a Linode reboot.
+
+        - - -
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter(name="stackscriptData")
     def stackscript_data(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/instance_ip.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/instance_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/instance_shared_ips.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/instance_shared_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/ipv6_range.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/lke_cluster.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/lke_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a LkeCluster resource.
         :param pulumi.Input[str] k8s_version: The desired Kubernetes version for this Kubernetes cluster in the format of `major.minor` (e.g. `1.21`), and the latest supported patch version will be deployed.
         :param pulumi.Input[str] label: This Kubernetes cluster's unique label.
         :param pulumi.Input[Sequence[pulumi.Input['LkeClusterPoolArgs']]] pools: Additional nested attributes:
         :param pulumi.Input[str] region: This Kubernetes cluster's location.
+               
+               * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+               
+               * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input['LkeClusterControlPlaneArgs'] control_plane: Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: An array of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
         """
         pulumi.set(__self__, "k8s_version", k8s_version)
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "pools", pools)
         pulumi.set(__self__, "region", region)
@@ -77,14 +81,18 @@
         pulumi.set(self, "pools", value)
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Input[str]:
         """
         This Kubernetes cluster's location.
+
+        * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+
+        * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
@@ -132,14 +140,18 @@
         :param pulumi.Input['LkeClusterControlPlaneArgs'] control_plane: Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[str] dashboard_url: The Kubernetes Dashboard access URL for this cluster.
         :param pulumi.Input[str] k8s_version: The desired Kubernetes version for this Kubernetes cluster in the format of `major.minor` (e.g. `1.21`), and the latest supported patch version will be deployed.
         :param pulumi.Input[str] kubeconfig: The base64 encoded kubeconfig for the Kubernetes cluster.
         :param pulumi.Input[str] label: This Kubernetes cluster's unique label.
         :param pulumi.Input[Sequence[pulumi.Input['LkeClusterPoolArgs']]] pools: Additional nested attributes:
         :param pulumi.Input[str] region: This Kubernetes cluster's location.
+               
+               * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+               
+               * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[str] status: The status of the node. (`ready`, `not_ready`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: An array of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
         """
         if api_endpoints is not None:
             pulumi.set(__self__, "api_endpoints", api_endpoints)
         if control_plane is not None:
             pulumi.set(__self__, "control_plane", control_plane)
@@ -245,14 +257,18 @@
         pulumi.set(self, "pools", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         This Kubernetes cluster's location.
+
+        * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+
+        * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
@@ -347,14 +363,18 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['LkeClusterControlPlaneArgs']] control_plane: Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[str] k8s_version: The desired Kubernetes version for this Kubernetes cluster in the format of `major.minor` (e.g. `1.21`), and the latest supported patch version will be deployed.
         :param pulumi.Input[str] label: This Kubernetes cluster's unique label.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LkeClusterPoolArgs']]]] pools: Additional nested attributes:
         :param pulumi.Input[str] region: This Kubernetes cluster's location.
+               
+               * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+               
+               * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: An array of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: LkeClusterArgs,
@@ -491,14 +511,18 @@
         :param pulumi.Input[pulumi.InputType['LkeClusterControlPlaneArgs']] control_plane: Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[str] dashboard_url: The Kubernetes Dashboard access URL for this cluster.
         :param pulumi.Input[str] k8s_version: The desired Kubernetes version for this Kubernetes cluster in the format of `major.minor` (e.g. `1.21`), and the latest supported patch version will be deployed.
         :param pulumi.Input[str] kubeconfig: The base64 encoded kubeconfig for the Kubernetes cluster.
         :param pulumi.Input[str] label: This Kubernetes cluster's unique label.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LkeClusterPoolArgs']]]] pools: Additional nested attributes:
         :param pulumi.Input[str] region: This Kubernetes cluster's location.
+               
+               * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+               
+               * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         :param pulumi.Input[str] status: The status of the node. (`ready`, `not_ready`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: An array of tags applied to the Kubernetes cluster. Tags are for organizational purposes only.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LkeClusterState.__new__(_LkeClusterState)
 
@@ -571,14 +595,18 @@
         return pulumi.get(self, "pools")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         This Kubernetes cluster's location.
+
+        * `pool` - (Required) The Node Pool specifications for the Kubernetes cluster. At least one Node Pool is required.
+
+        * `control_plane` (Optional) Defines settings for the Kubernetes Control Plane.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/node_balancer.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/node_balancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
                  region: pulumi.Input[str],
                  client_conn_throttle: Optional[pulumi.Input[int]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a NodeBalancer resource.
         :param pulumi.Input[str] region: The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+               
+               - - -
         :param pulumi.Input[int] client_conn_throttle: Throttle connections per second (0-20). Set to 0 (default) to disable throttling.
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         pulumi.set(__self__, "region", region)
         if client_conn_throttle is not None:
             pulumi.set(__self__, "client_conn_throttle", client_conn_throttle)
@@ -36,14 +38,16 @@
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Input[str]:
         """
         The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+
+        - - -
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
@@ -102,14 +106,16 @@
         :param pulumi.Input[int] client_conn_throttle: Throttle connections per second (0-20). Set to 0 (default) to disable throttling.
         :param pulumi.Input[str] created: When this NodeBalancer was created
         :param pulumi.Input[str] hostname: This NodeBalancer's hostname, ending with .nodebalancer.linode.com
         :param pulumi.Input[str] ipv4: The Public IPv4 Address of this NodeBalancer
         :param pulumi.Input[str] ipv6: The Public IPv6 Address of this NodeBalancer
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer
         :param pulumi.Input[str] region: The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[Sequence[pulumi.Input['NodeBalancerTransferArgs']]] transfers: Information about the amount of transfer this NodeBalancer has had so far this month.
         :param pulumi.Input[str] updated: When this NodeBalancer was last updated.
         """
         if client_conn_throttle is not None:
             pulumi.set(__self__, "client_conn_throttle", client_conn_throttle)
         if created is not None:
@@ -204,14 +210,16 @@
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+
+        - - -
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
@@ -292,14 +300,16 @@
          The Linode Guide, [Import Existing Infrastructure to Terraform](https://www.linode.com/docs/applications/configuration-management/import-existing-infrastructure-to-terraform/), offers resource importing examples for NodeBalancers and other Linode resource types.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] client_conn_throttle: Throttle connections per second (0-20). Set to 0 (default) to disable throttling.
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer
         :param pulumi.Input[str] region: The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NodeBalancerArgs,
@@ -403,14 +413,16 @@
         :param pulumi.Input[int] client_conn_throttle: Throttle connections per second (0-20). Set to 0 (default) to disable throttling.
         :param pulumi.Input[str] created: When this NodeBalancer was created
         :param pulumi.Input[str] hostname: This NodeBalancer's hostname, ending with .nodebalancer.linode.com
         :param pulumi.Input[str] ipv4: The Public IPv4 Address of this NodeBalancer
         :param pulumi.Input[str] ipv6: The Public IPv6 Address of this NodeBalancer
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer
         :param pulumi.Input[str] region: The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NodeBalancerTransferArgs']]]] transfers: Information about the amount of transfer this NodeBalancer has had so far this month.
         :param pulumi.Input[str] updated: When this NodeBalancer was last updated.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NodeBalancerState.__new__(_NodeBalancerState)
@@ -476,14 +488,16 @@
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         The region where this NodeBalancer will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions).  *Changing `region` forces the creation of a new Linode NodeBalancer.*.
+
+        - - -
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/node_balancer_config.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/node_balancer_node.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/node_balancer_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
                  label: pulumi.Input[str],
                  nodebalancer_id: pulumi.Input[int],
                  mode: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a NodeBalancerNode resource.
         :param pulumi.Input[str] address: The private IP Address where this backend can be reached. This must be a private IP address.
+               
+               - - -
         :param pulumi.Input[int] config_id: The ID of the NodeBalancerConfig to access.
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer Node. This is for display purposes only.
         :param pulumi.Input[int] nodebalancer_id: The ID of the NodeBalancer to access.
         :param pulumi.Input[str] mode: The mode this NodeBalancer should use when sending traffic to this backend. If set to `accept` this backend is accepting traffic. If set to `reject` this backend will not receive traffic. If set to `drain` this backend will not receive new traffic, but connections already pinned to it will continue to be routed to it. (`accept`, `reject`, `drain`, `backup`)
         :param pulumi.Input[int] weight: Used when picking a backend to serve a request and is not pinned to a single backend yet. Nodes with a higher weight will receive more traffic. (1-255).
         """
         pulumi.set(__self__, "address", address)
@@ -39,14 +41,16 @@
             pulumi.set(__self__, "weight", weight)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Input[str]:
         """
         The private IP Address where this backend can be reached. This must be a private IP address.
+
+        - - -
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: pulumi.Input[str]):
         pulumi.set(self, "address", value)
 
@@ -120,14 +124,16 @@
                  mode: Optional[pulumi.Input[str]] = None,
                  nodebalancer_id: Optional[pulumi.Input[int]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering NodeBalancerNode resources.
         :param pulumi.Input[str] address: The private IP Address where this backend can be reached. This must be a private IP address.
+               
+               - - -
         :param pulumi.Input[int] config_id: The ID of the NodeBalancerConfig to access.
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer Node. This is for display purposes only.
         :param pulumi.Input[str] mode: The mode this NodeBalancer should use when sending traffic to this backend. If set to `accept` this backend is accepting traffic. If set to `reject` this backend will not receive traffic. If set to `drain` this backend will not receive new traffic, but connections already pinned to it will continue to be routed to it. (`accept`, `reject`, `drain`, `backup`)
         :param pulumi.Input[int] nodebalancer_id: The ID of the NodeBalancer to access.
         :param pulumi.Input[str] status: The current status of this node, based on the configured checks of its NodeBalancer Config. (`unknown`, `UP`, `DOWN`).
         :param pulumi.Input[int] weight: Used when picking a backend to serve a request and is not pinned to a single backend yet. Nodes with a higher weight will receive more traffic. (1-255).
         """
@@ -147,14 +153,16 @@
             pulumi.set(__self__, "weight", weight)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
         The private IP Address where this backend can be reached. This must be a private IP address.
+
+        - - -
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
@@ -298,14 +306,16 @@
         ```
 
          The Linode Guide, [Import Existing Infrastructure to Terraform](https://www.linode.com/docs/applications/configuration-management/import-existing-infrastructure-to-terraform/), offers resource importing examples for NodeBalancer Nodes and other Linode resource types.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The private IP Address where this backend can be reached. This must be a private IP address.
+               
+               - - -
         :param pulumi.Input[int] config_id: The ID of the NodeBalancerConfig to access.
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer Node. This is for display purposes only.
         :param pulumi.Input[str] mode: The mode this NodeBalancer should use when sending traffic to this backend. If set to `accept` this backend is accepting traffic. If set to `reject` this backend will not receive traffic. If set to `drain` this backend will not receive new traffic, but connections already pinned to it will continue to be routed to it. (`accept`, `reject`, `drain`, `backup`)
         :param pulumi.Input[int] nodebalancer_id: The ID of the NodeBalancer to access.
         :param pulumi.Input[int] weight: Used when picking a backend to serve a request and is not pinned to a single backend yet. Nodes with a higher weight will receive more traffic. (1-255).
         """
         ...
@@ -436,14 +446,16 @@
         Get an existing NodeBalancerNode resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The private IP Address where this backend can be reached. This must be a private IP address.
+               
+               - - -
         :param pulumi.Input[int] config_id: The ID of the NodeBalancerConfig to access.
         :param pulumi.Input[str] label: The label of the Linode NodeBalancer Node. This is for display purposes only.
         :param pulumi.Input[str] mode: The mode this NodeBalancer should use when sending traffic to this backend. If set to `accept` this backend is accepting traffic. If set to `reject` this backend will not receive traffic. If set to `drain` this backend will not receive new traffic, but connections already pinned to it will continue to be routed to it. (`accept`, `reject`, `drain`, `backup`)
         :param pulumi.Input[int] nodebalancer_id: The ID of the NodeBalancer to access.
         :param pulumi.Input[str] status: The current status of this node, based on the configured checks of its NodeBalancer Config. (`unknown`, `UP`, `DOWN`).
         :param pulumi.Input[int] weight: Used when picking a backend to serve a request and is not pinned to a single backend yet. Nodes with a higher weight will receive more traffic. (1-255).
         """
@@ -461,14 +473,16 @@
         return NodeBalancerNode(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Output[str]:
         """
         The private IP Address where this backend can be reached. This must be a private IP address.
+
+        - - -
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/object_storage_bucket.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/object_storage_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         :param pulumi.Input[str] access_key: The access key to authenticate with.
         :param pulumi.Input[str] acl: The Access Control Level of the bucket using a canned ACL string. See all ACL strings [in the Linode API v4 documentation](https://linode.com/docs/api/object-storage/#object-storage-bucket-access-update__request-body-schema).
         :param pulumi.Input['ObjectStorageBucketCertArgs'] cert: The cert used by this Object Storage Bucket.
         :param pulumi.Input[bool] cors_enabled: If true, the bucket will have CORS enabled for all origins.
         :param pulumi.Input[Sequence[pulumi.Input['ObjectStorageBucketLifecycleRuleArgs']]] lifecycle_rules: Lifecycle rules to be applied to the bucket.
         :param pulumi.Input[str] secret_key: The secret key to authenticate with.
         :param pulumi.Input[bool] versioning: Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+               
+               * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+               
+               * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         pulumi.set(__self__, "cluster", cluster)
         pulumi.set(__self__, "label", label)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
@@ -151,14 +155,18 @@
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter
     def versioning(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+
+        * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+
+        * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         return pulumi.get(self, "versioning")
 
     @versioning.setter
     def versioning(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "versioning", value)
 
@@ -185,14 +193,18 @@
         :param pulumi.Input[bool] cors_enabled: If true, the bucket will have CORS enabled for all origins.
         :param pulumi.Input[str] hostname: The hostname where this bucket can be accessed. This hostname can be accessed through a browser if the bucket is made
                public.
         :param pulumi.Input[str] label: The label of the Linode Object Storage Bucket.
         :param pulumi.Input[Sequence[pulumi.Input['ObjectStorageBucketLifecycleRuleArgs']]] lifecycle_rules: Lifecycle rules to be applied to the bucket.
         :param pulumi.Input[str] secret_key: The secret key to authenticate with.
         :param pulumi.Input[bool] versioning: Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+               
+               * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+               
+               * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
@@ -321,14 +333,18 @@
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter
     def versioning(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+
+        * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+
+        * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         return pulumi.get(self, "versioning")
 
     @versioning.setter
     def versioning(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "versioning", value)
 
@@ -402,14 +418,18 @@
         :param pulumi.Input[pulumi.InputType['ObjectStorageBucketCertArgs']] cert: The cert used by this Object Storage Bucket.
         :param pulumi.Input[str] cluster: The cluster of the Linode Object Storage Bucket.
         :param pulumi.Input[bool] cors_enabled: If true, the bucket will have CORS enabled for all origins.
         :param pulumi.Input[str] label: The label of the Linode Object Storage Bucket.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageBucketLifecycleRuleArgs']]]] lifecycle_rules: Lifecycle rules to be applied to the bucket.
         :param pulumi.Input[str] secret_key: The secret key to authenticate with.
         :param pulumi.Input[bool] versioning: Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+               
+               * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+               
+               * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ObjectStorageBucketArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -541,14 +561,18 @@
         :param pulumi.Input[bool] cors_enabled: If true, the bucket will have CORS enabled for all origins.
         :param pulumi.Input[str] hostname: The hostname where this bucket can be accessed. This hostname can be accessed through a browser if the bucket is made
                public.
         :param pulumi.Input[str] label: The label of the Linode Object Storage Bucket.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageBucketLifecycleRuleArgs']]]] lifecycle_rules: Lifecycle rules to be applied to the bucket.
         :param pulumi.Input[str] secret_key: The secret key to authenticate with.
         :param pulumi.Input[bool] versioning: Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+               
+               * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+               
+               * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ObjectStorageBucketState.__new__(_ObjectStorageBucketState)
 
         __props__.__dict__["access_key"] = access_key
         __props__.__dict__["acl"] = acl
@@ -636,10 +660,14 @@
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter
     def versioning(self) -> pulumi.Output[bool]:
         """
         Whether to enable versioning. Once you version-enable a bucket, it can never return to an unversioned state. You can, however, suspend versioning on that bucket. (Requires `access_key` and `secret_key`)
+
+        * `lifecycle_rule` - (Optional) Lifecycle rules to be applied to the bucket. (Requires `access_key` and `secret_key`)
+
+        * `cert` - (Optional) The bucket's TLS/SSL certificate.
         """
         return pulumi.get(self, "versioning")
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/object_storage_key.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/object_storage_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 class ObjectStorageKeyArgs:
     def __init__(__self__, *,
                  label: pulumi.Input[str],
                  bucket_accesses: Optional[pulumi.Input[Sequence[pulumi.Input['ObjectStorageKeyBucketAccessArgs']]]] = None):
         """
         The set of arguments for constructing a ObjectStorageKey resource.
         :param pulumi.Input[str] label: The label given to this key. For display purposes only.
+               
+               - - -
         :param pulumi.Input[Sequence[pulumi.Input['ObjectStorageKeyBucketAccessArgs']]] bucket_accesses: Defines this key as a Limited Access Key. Limited Access Keys restrict this Object Storage key’s access to only the bucket(s) declared in this array and define their bucket-level permissions. Not providing this block will not limit this Object Storage Key.
         """
         pulumi.set(__self__, "label", label)
         if bucket_accesses is not None:
             pulumi.set(__self__, "bucket_accesses", bucket_accesses)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
         """
         The label given to this key. For display purposes only.
+
+        - - -
         """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
@@ -61,14 +65,16 @@
                  limited: Optional[pulumi.Input[bool]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ObjectStorageKey resources.
         :param pulumi.Input[str] access_key: This keypair's access key. This is not secret.
         :param pulumi.Input[Sequence[pulumi.Input['ObjectStorageKeyBucketAccessArgs']]] bucket_accesses: Defines this key as a Limited Access Key. Limited Access Keys restrict this Object Storage key’s access to only the bucket(s) declared in this array and define their bucket-level permissions. Not providing this block will not limit this Object Storage Key.
         :param pulumi.Input[str] label: The label given to this key. For display purposes only.
+               
+               - - -
         :param pulumi.Input[bool] limited: Whether or not this key is a limited access key.
         :param pulumi.Input[str] secret_key: This keypair's secret key.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bucket_accesses is not None:
             pulumi.set(__self__, "bucket_accesses", bucket_accesses)
@@ -104,14 +110,16 @@
         pulumi.set(self, "bucket_accesses", value)
 
     @property
     @pulumi.getter
     def label(self) -> Optional[pulumi.Input[str]]:
         """
         The label given to this key. For display purposes only.
+
+        - - -
         """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "label", value)
 
@@ -162,14 +170,16 @@
         foo = linode.ObjectStorageKey("foo", label="image-access")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageKeyBucketAccessArgs']]]] bucket_accesses: Defines this key as a Limited Access Key. Limited Access Keys restrict this Object Storage key’s access to only the bucket(s) declared in this array and define their bucket-level permissions. Not providing this block will not limit this Object Storage Key.
         :param pulumi.Input[str] label: The label given to this key. For display purposes only.
+               
+               - - -
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ObjectStorageKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -243,14 +253,16 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_key: This keypair's access key. This is not secret.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ObjectStorageKeyBucketAccessArgs']]]] bucket_accesses: Defines this key as a Limited Access Key. Limited Access Keys restrict this Object Storage key’s access to only the bucket(s) declared in this array and define their bucket-level permissions. Not providing this block will not limit this Object Storage Key.
         :param pulumi.Input[str] label: The label given to this key. For display purposes only.
+               
+               - - -
         :param pulumi.Input[bool] limited: Whether or not this key is a limited access key.
         :param pulumi.Input[str] secret_key: This keypair's secret key.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ObjectStorageKeyState.__new__(_ObjectStorageKeyState)
 
@@ -278,14 +290,16 @@
         return pulumi.get(self, "bucket_accesses")
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Output[str]:
         """
         The label given to this key. For display purposes only.
+
+        - - -
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def limited(self) -> pulumi.Output[bool]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/object_storage_object.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/object_storage_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/outputs.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'DatabaseMongodbUpdates',
     'DatabaseMysqlUpdates',
     'DatabasePostgresqlUpdates',
     'FirewallDevice',
     'FirewallInbound',
     'FirewallOutbound',
     'InstanceAlerts',
     'InstanceBackups',
@@ -58,15 +57,14 @@
     'UserVolumeGrant',
     'GetAccountLoginsFilterResult',
     'GetAccountLoginsLoginResult',
     'GetDatabaseBackupsBackupResult',
     'GetDatabaseBackupsFilterResult',
     'GetDatabaseEnginesEngineResult',
     'GetDatabaseEnginesFilterResult',
-    'GetDatabaseMongodbUpdateResult',
     'GetDatabaseMysqlBackupsBackupResult',
     'GetDatabaseMysqlBackupsFilterResult',
     'GetDatabaseMysqlUpdateResult',
     'GetDatabasePostgresqlUpdateResult',
     'GetDatabasesDatabaseResult',
     'GetDatabasesFilterResult',
     'GetFirewallDeviceResult',
@@ -144,76 +142,14 @@
     'GetUserStackscriptGrantResult',
     'GetUserVolumeGrantResult',
     'GetVlansFilterResult',
     'GetVlansVlanResult',
 ]
 
 @pulumi.output_type
-class DatabaseMongodbUpdates(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "dayOfWeek":
-            suggest = "day_of_week"
-        elif key == "hourOfDay":
-            suggest = "hour_of_day"
-        elif key == "weekOfMonth":
-            suggest = "week_of_month"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in DatabaseMongodbUpdates. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        DatabaseMongodbUpdates.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        DatabaseMongodbUpdates.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 day_of_week: str,
-                 duration: int,
-                 frequency: str,
-                 hour_of_day: int,
-                 week_of_month: Optional[int] = None):
-        pulumi.set(__self__, "day_of_week", day_of_week)
-        pulumi.set(__self__, "duration", duration)
-        pulumi.set(__self__, "frequency", frequency)
-        pulumi.set(__self__, "hour_of_day", hour_of_day)
-        if week_of_month is not None:
-            pulumi.set(__self__, "week_of_month", week_of_month)
-
-    @property
-    @pulumi.getter(name="dayOfWeek")
-    def day_of_week(self) -> str:
-        return pulumi.get(self, "day_of_week")
-
-    @property
-    @pulumi.getter
-    def duration(self) -> int:
-        return pulumi.get(self, "duration")
-
-    @property
-    @pulumi.getter
-    def frequency(self) -> str:
-        return pulumi.get(self, "frequency")
-
-    @property
-    @pulumi.getter(name="hourOfDay")
-    def hour_of_day(self) -> int:
-        return pulumi.get(self, "hour_of_day")
-
-    @property
-    @pulumi.getter(name="weekOfMonth")
-    def week_of_month(self) -> Optional[int]:
-        return pulumi.get(self, "week_of_month")
-
-
-@pulumi.output_type
 class DatabaseMysqlUpdates(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "dayOfWeek":
             suggest = "day_of_week"
         elif key == "hourOfDay":
@@ -740,14 +676,16 @@
         """
         :param str label: The Linode's label is for display purposes only. If no label is provided for a Linode, a default will be assigned.
         :param str comments: Arbitrary user comments about this `config`.
         :param 'InstanceConfigDevicesArgs' devices: A list of `disk` or `volume` attachments for this `config`.  If the `boot_config_label` omits a `devices` block, the Linode will not be booted.
         :param 'InstanceConfigHelpersArgs' helpers: Helpers enabled when booting to this Linode Config.
         :param str kernel: A Kernel ID to boot a Linode with. Default is based on image choice. Examples are `linode/latest-64bit`, `linode/grub2`, `linode/direct-disk`, etc. See all kernels [here](https://api.linode.com/v4/linode/kernels). Note that this is a paginated API endpoint ([docs](https://developers.linode.com/api/v4/linode-kernels)).
         :param int memory_limit: Defaults to the total RAM of the Linode
+               
+               * `interface` - (Optional) A list of network interfaces to be assigned to the Linode.
         :param str root_device: The root device to boot. The corresponding disk must be attached to a `device` slot.  Example: `"/dev/sda"`
         :param str run_level: Defines the state of your Linode after booting. Defaults to `"default"`.
         :param str virt_mode: Controls the virtualization mode. Defaults to `"paravirt"`.
         """
         pulumi.set(__self__, "label", label)
         if comments is not None:
             pulumi.set(__self__, "comments", comments)
@@ -814,14 +752,16 @@
         return pulumi.get(self, "kernel")
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> Optional[int]:
         """
         Defaults to the total RAM of the Linode
+
+        * `interface` - (Optional) A list of network interfaces to be assigned to the Linode.
         """
         return pulumi.get(self, "memory_limit")
 
     @property
     @pulumi.getter(name="rootDevice")
     def root_device(self) -> Optional[str]:
         """
@@ -1880,14 +1820,16 @@
                  count: int,
                  type: str,
                  autoscaler: Optional['outputs.LkeClusterPoolAutoscaler'] = None,
                  id: Optional[int] = None,
                  nodes: Optional[Sequence['outputs.LkeClusterPoolNode']] = None):
         """
         :param int count: The number of nodes in the Node Pool.
+               
+               * `autoscaler` - (Optional) If defined, an autoscaler will be enabled with the given configuration.
         :param str type: A Linode Type for all of the nodes in the Node Pool. See all node types [here](https://api.linode.com/v4/linode/types).
         :param int id: The ID of the node.
         """
         pulumi.set(__self__, "count", count)
         pulumi.set(__self__, "type", type)
         if autoscaler is not None:
             pulumi.set(__self__, "autoscaler", autoscaler)
@@ -1897,14 +1839,16 @@
             pulumi.set(__self__, "nodes", nodes)
 
     @property
     @pulumi.getter
     def count(self) -> int:
         """
         The number of nodes in the Node Pool.
+
+        * `autoscaler` - (Optional) If defined, an autoscaler will be enabled with the given configuration.
         """
         return pulumi.get(self, "count")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
@@ -2184,14 +2128,18 @@
                  expiration: Optional['outputs.ObjectStorageBucketLifecycleRuleExpiration'] = None,
                  id: Optional[str] = None,
                  noncurrent_version_expiration: Optional['outputs.ObjectStorageBucketLifecycleRuleNoncurrentVersionExpiration'] = None,
                  prefix: Optional[str] = None):
         """
         :param bool enabled: Specifies whether the lifecycle rule is active.
         :param int abort_incomplete_multipart_upload_days: Specifies the number of days after initiating a multipart upload when the multipart upload must be completed.
+               
+               * `expiration` - (Optional) Specifies a period in the object's expire.
+               
+               * `noncurrent_version_expiration` - (Optional) Specifies when non-current object versions expire.
         :param str id: The unique identifier for the rule.
         :param str prefix: The object key prefix identifying one or more objects to which the rule applies.
         """
         pulumi.set(__self__, "enabled", enabled)
         if abort_incomplete_multipart_upload_days is not None:
             pulumi.set(__self__, "abort_incomplete_multipart_upload_days", abort_incomplete_multipart_upload_days)
         if expiration is not None:
@@ -2212,14 +2160,18 @@
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="abortIncompleteMultipartUploadDays")
     def abort_incomplete_multipart_upload_days(self) -> Optional[int]:
         """
         Specifies the number of days after initiating a multipart upload when the multipart upload must be completed.
+
+        * `expiration` - (Optional) Specifies a period in the object's expire.
+
+        * `noncurrent_version_expiration` - (Optional) Specifies when non-current object versions expire.
         """
         return pulumi.get(self, "abort_incomplete_multipart_upload_days")
 
     @property
     @pulumi.getter
     def expiration(self) -> Optional['outputs.ObjectStorageBucketLifecycleRuleExpiration']:
         return pulumi.get(self, "expiration")
@@ -2399,84 +2351,78 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         StackScriptUserDefinedField.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 default: Optional[str] = None,
-                 example: Optional[str] = None,
-                 label: Optional[str] = None,
-                 many_of: Optional[str] = None,
-                 name: Optional[str] = None,
-                 one_of: Optional[str] = None):
+                 default: str,
+                 example: str,
+                 label: str,
+                 many_of: str,
+                 name: str,
+                 one_of: str):
         """
         :param str default: The default value. If not specified, this value will be used.
         :param str example: An example value for the field.
         :param str label: The StackScript's label is for display purposes only.
         :param str many_of: A list of acceptable values for the field in any quantity, combination or order.
         :param str name: The name of the field.
         :param str one_of: A list of acceptable single values for the field.
         """
-        if default is not None:
-            pulumi.set(__self__, "default", default)
-        if example is not None:
-            pulumi.set(__self__, "example", example)
-        if label is not None:
-            pulumi.set(__self__, "label", label)
-        if many_of is not None:
-            pulumi.set(__self__, "many_of", many_of)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if one_of is not None:
-            pulumi.set(__self__, "one_of", one_of)
+        pulumi.set(__self__, "default", default)
+        pulumi.set(__self__, "example", example)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "many_of", many_of)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "one_of", one_of)
 
     @property
     @pulumi.getter
-    def default(self) -> Optional[str]:
+    def default(self) -> str:
         """
         The default value. If not specified, this value will be used.
         """
         return pulumi.get(self, "default")
 
     @property
     @pulumi.getter
-    def example(self) -> Optional[str]:
+    def example(self) -> str:
         """
         An example value for the field.
         """
         return pulumi.get(self, "example")
 
     @property
     @pulumi.getter
-    def label(self) -> Optional[str]:
+    def label(self) -> str:
         """
         The StackScript's label is for display purposes only.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter(name="manyOf")
-    def many_of(self) -> Optional[str]:
+    def many_of(self) -> str:
         """
         A list of acceptable values for the field in any quantity, combination or order.
         """
         return pulumi.get(self, "many_of")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[str]:
+    def name(self) -> str:
         """
         The name of the field.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="oneOf")
-    def one_of(self) -> Optional[str]:
+    def one_of(self) -> str:
         """
         A list of acceptable single values for the field.
         """
         return pulumi.get(self, "one_of")
 
 
 @pulumi.output_type
@@ -3051,54 +2997,14 @@
         """
         The method to match the field by. (`exact`, `regex`, `substring`; default `exact`)
         """
         return pulumi.get(self, "match_by")
 
 
 @pulumi.output_type
-class GetDatabaseMongodbUpdateResult(dict):
-    def __init__(__self__, *,
-                 day_of_week: str,
-                 duration: int,
-                 frequency: str,
-                 hour_of_day: int,
-                 week_of_month: int):
-        pulumi.set(__self__, "day_of_week", day_of_week)
-        pulumi.set(__self__, "duration", duration)
-        pulumi.set(__self__, "frequency", frequency)
-        pulumi.set(__self__, "hour_of_day", hour_of_day)
-        pulumi.set(__self__, "week_of_month", week_of_month)
-
-    @property
-    @pulumi.getter(name="dayOfWeek")
-    def day_of_week(self) -> str:
-        return pulumi.get(self, "day_of_week")
-
-    @property
-    @pulumi.getter
-    def duration(self) -> int:
-        return pulumi.get(self, "duration")
-
-    @property
-    @pulumi.getter
-    def frequency(self) -> str:
-        return pulumi.get(self, "frequency")
-
-    @property
-    @pulumi.getter(name="hourOfDay")
-    def hour_of_day(self) -> int:
-        return pulumi.get(self, "hour_of_day")
-
-    @property
-    @pulumi.getter(name="weekOfMonth")
-    def week_of_month(self) -> int:
-        return pulumi.get(self, "week_of_month")
-
-
-@pulumi.output_type
 class GetDatabaseMysqlBackupsBackupResult(dict):
     def __init__(__self__, *,
                  created: str,
                  id: int,
                  label: str,
                  type: str):
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/provider.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/rdns.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/rdns.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/ssh_key.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/stack_script.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/stack_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,36 +17,34 @@
 class StackScriptArgs:
     def __init__(__self__, *,
                  description: pulumi.Input[str],
                  images: pulumi.Input[Sequence[pulumi.Input[str]]],
                  label: pulumi.Input[str],
                  script: pulumi.Input[str],
                  is_public: Optional[pulumi.Input[bool]] = None,
-                 rev_note: Optional[pulumi.Input[str]] = None,
-                 user_defined_fields: Optional[pulumi.Input[Sequence[pulumi.Input['StackScriptUserDefinedFieldArgs']]]] = None):
+                 rev_note: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a StackScript resource.
         :param pulumi.Input[str] description: A description for the StackScript.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+               
+               - - -
         :param pulumi.Input[str] label: The StackScript's label is for display purposes only.
         :param pulumi.Input[str] script: The script to execute when provisioning a new Linode with this StackScript.
         :param pulumi.Input[bool] is_public: This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private. *Changing `is_public` forces the creation of a new StackScript*
         :param pulumi.Input[str] rev_note: This field allows you to add notes for the set of revisions made to this StackScript.
-        :param pulumi.Input[Sequence[pulumi.Input['StackScriptUserDefinedFieldArgs']]] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "images", images)
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "script", script)
         if is_public is not None:
             pulumi.set(__self__, "is_public", is_public)
         if rev_note is not None:
             pulumi.set(__self__, "rev_note", rev_note)
-        if user_defined_fields is not None:
-            pulumi.set(__self__, "user_defined_fields", user_defined_fields)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         """
         A description for the StackScript.
         """
@@ -56,15 +54,17 @@
     def description(self, value: pulumi.Input[str]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def images(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+
+        - - -
         """
         return pulumi.get(self, "images")
 
     @images.setter
     def images(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "images", value)
 
@@ -112,26 +112,14 @@
         """
         return pulumi.get(self, "rev_note")
 
     @rev_note.setter
     def rev_note(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rev_note", value)
 
-    @property
-    @pulumi.getter(name="userDefinedFields")
-    def user_defined_fields(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['StackScriptUserDefinedFieldArgs']]]]:
-        """
-        This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
-        """
-        return pulumi.get(self, "user_defined_fields")
-
-    @user_defined_fields.setter
-    def user_defined_fields(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['StackScriptUserDefinedFieldArgs']]]]):
-        pulumi.set(self, "user_defined_fields", value)
-
 
 @pulumi.input_type
 class _StackScriptState:
     def __init__(__self__, *,
                  created: Optional[pulumi.Input[str]] = None,
                  deployments_active: Optional[pulumi.Input[int]] = None,
                  deployments_total: Optional[pulumi.Input[int]] = None,
@@ -147,15 +135,17 @@
                  username: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering StackScript resources.
         :param pulumi.Input[str] created: The date this StackScript was created.
         :param pulumi.Input[int] deployments_active: Count of currently active, deployed Linodes created from this StackScript.
         :param pulumi.Input[int] deployments_total: The total number of times this StackScript has been deployed.
         :param pulumi.Input[str] description: A description for the StackScript.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+               
+               - - -
         :param pulumi.Input[bool] is_public: This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private. *Changing `is_public` forces the creation of a new StackScript*
         :param pulumi.Input[str] label: The StackScript's label is for display purposes only.
         :param pulumi.Input[str] rev_note: This field allows you to add notes for the set of revisions made to this StackScript.
         :param pulumi.Input[str] script: The script to execute when provisioning a new Linode with this StackScript.
         :param pulumi.Input[str] updated: The date this StackScript was updated.
         :param pulumi.Input[Sequence[pulumi.Input['StackScriptUserDefinedFieldArgs']]] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
         :param pulumi.Input[str] user_gravatar_id: The Gravatar ID for the User who created the StackScript.
@@ -236,15 +226,17 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def images(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+
+        - - -
         """
         return pulumi.get(self, "images")
 
     @images.setter
     def images(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "images", value)
 
@@ -352,15 +344,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  is_public: Optional[pulumi.Input[bool]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  rev_note: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
-                 user_defined_fields: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StackScriptUserDefinedFieldArgs']]]]] = None,
                  __props__=None):
         """
         Provides a Linode StackScript resource.  This can be used to create, modify, and delete Linode StackScripts.  StackScripts are private or public managed scripts which run within an instance during startup.  StackScripts can include variables whose values are specified when the Instance is created.
 
         For more information, see [Automate Deployment with StackScripts](https://www.linode.com/docs/platform/stackscripts/) and the [Linode APIv4 docs](https://developers.linode.com/api/v4#tag/StackScripts).
 
         ## Example Usage
@@ -403,20 +394,21 @@
         ```sh
          $ pulumi import linode:index/stackScript:StackScript mystackscript 1234567
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description for the StackScript.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+               
+               - - -
         :param pulumi.Input[bool] is_public: This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private. *Changing `is_public` forces the creation of a new StackScript*
         :param pulumi.Input[str] label: The StackScript's label is for display purposes only.
         :param pulumi.Input[str] rev_note: This field allows you to add notes for the set of revisions made to this StackScript.
         :param pulumi.Input[str] script: The script to execute when provisioning a new Linode with this StackScript.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StackScriptUserDefinedFieldArgs']]]] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: StackScriptArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -483,15 +475,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  images: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  is_public: Optional[pulumi.Input[bool]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  rev_note: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
-                 user_defined_fields: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StackScriptUserDefinedFieldArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -507,19 +498,19 @@
             if label is None and not opts.urn:
                 raise TypeError("Missing required property 'label'")
             __props__.__dict__["label"] = label
             __props__.__dict__["rev_note"] = rev_note
             if script is None and not opts.urn:
                 raise TypeError("Missing required property 'script'")
             __props__.__dict__["script"] = script
-            __props__.__dict__["user_defined_fields"] = user_defined_fields
             __props__.__dict__["created"] = None
             __props__.__dict__["deployments_active"] = None
             __props__.__dict__["deployments_total"] = None
             __props__.__dict__["updated"] = None
+            __props__.__dict__["user_defined_fields"] = None
             __props__.__dict__["user_gravatar_id"] = None
             __props__.__dict__["username"] = None
         super(StackScript, __self__).__init__(
             'linode:index/stackScript:StackScript',
             resource_name,
             __props__,
             opts)
@@ -548,15 +539,17 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created: The date this StackScript was created.
         :param pulumi.Input[int] deployments_active: Count of currently active, deployed Linodes created from this StackScript.
         :param pulumi.Input[int] deployments_total: The total number of times this StackScript has been deployed.
         :param pulumi.Input[str] description: A description for the StackScript.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] images: A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+               
+               - - -
         :param pulumi.Input[bool] is_public: This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private. *Changing `is_public` forces the creation of a new StackScript*
         :param pulumi.Input[str] label: The StackScript's label is for display purposes only.
         :param pulumi.Input[str] rev_note: This field allows you to add notes for the set of revisions made to this StackScript.
         :param pulumi.Input[str] script: The script to execute when provisioning a new Linode with this StackScript.
         :param pulumi.Input[str] updated: The date this StackScript was updated.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['StackScriptUserDefinedFieldArgs']]]] user_defined_fields: This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
         :param pulumi.Input[str] user_gravatar_id: The Gravatar ID for the User who created the StackScript.
@@ -613,21 +606,23 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def images(self) -> pulumi.Output[Sequence[str]]:
         """
-        An array of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+        A set of Image IDs representing the Images that this StackScript is compatible for deploying with. `any/all` indicates that all available image distributions, including private images, are accepted. Currently private image IDs are not supported.
+
+        - - -
         """
         return pulumi.get(self, "images")
 
     @property
     @pulumi.getter(name="isPublic")
-    def is_public(self) -> pulumi.Output[Optional[bool]]:
+    def is_public(self) -> pulumi.Output[bool]:
         """
         This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private. *Changing `is_public` forces the creation of a new StackScript*
         """
         return pulumi.get(self, "is_public")
 
     @property
     @pulumi.getter
@@ -635,15 +630,15 @@
         """
         The StackScript's label is for display purposes only.
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter(name="revNote")
-    def rev_note(self) -> pulumi.Output[Optional[str]]:
+    def rev_note(self) -> pulumi.Output[str]:
         """
         This field allows you to add notes for the set of revisions made to this StackScript.
         """
         return pulumi.get(self, "rev_note")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode/volume.py` & `pulumi_linode-4.1.0a1684348483/pulumi_linode/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
                  source_volume_id: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Volume resource.
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
         :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+               
+               - - -
         :param pulumi.Input[int] size: Size of the Volume in GB.
         :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         pulumi.set(__self__, "label", label)
         if linode_id is not None:
             pulumi.set(__self__, "linode_id", linode_id)
@@ -66,14 +68,16 @@
         pulumi.set(self, "linode_id", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+
+        - - -
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
@@ -127,14 +131,16 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Volume resources.
         :param pulumi.Input[str] filesystem_path: The full filesystem path for the Volume based on the Volume's label. The path is "/dev/disk/by-id/scsi-0Linode_Volume_" + the Volume label
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
         :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+               
+               - - -
         :param pulumi.Input[int] size: Size of the Volume in GB.
         :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[str] status: The status of the Linode Volume. (`creating`, `active`, `resizing`, `contact_support`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         if filesystem_path is not None:
             pulumi.set(__self__, "filesystem_path", filesystem_path)
@@ -190,14 +196,16 @@
         pulumi.set(self, "linode_id", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+
+        - - -
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
@@ -328,14 +336,16 @@
          The Linode Guide, [Import Existing Infrastructure to Terraform](https://www.linode.com/docs/applications/configuration-management/import-existing-infrastructure-to-terraform/), offers resource importing examples for Block Storage Volumes and other Linode resource types.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
         :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+               
+               - - -
         :param pulumi.Input[int] size: Size of the Volume in GB.
         :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         ...
     @overload
     def __init__(__self__,
@@ -472,14 +482,16 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] filesystem_path: The full filesystem path for the Volume based on the Volume's label. The path is "/dev/disk/by-id/scsi-0Linode_Volume_" + the Volume label
         :param pulumi.Input[str] label: The label of the Linode Volume
         :param pulumi.Input[int] linode_id: The ID of a Linode Instance where the Volume should be attached.
         :param pulumi.Input[str] region: The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+               
+               - - -
         :param pulumi.Input[int] size: Size of the Volume in GB.
         :param pulumi.Input[int] source_volume_id: The ID of a Linode Volume to clone. NOTE: Cloned volumes must be in the same region as the source volume.
         :param pulumi.Input[str] status: The status of the Linode Volume. (`creating`, `active`, `resizing`, `contact_support`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags applied to this object. Tags are for organizational purposes only.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -520,14 +532,16 @@
         return pulumi.get(self, "linode_id")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         The region where this volume will be deployed.  Examples are `"us-east"`, `"us-west"`, `"ap-south"`, etc. See all regions [here](https://api.linode.com/v4/regions). This field is optional for cloned volumes. *Changing `region` forces the creation of a new Linode Volume.*.
+
+        - - -
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/PKG-INFO` & `pulumi_linode-4.1.0a1684348483/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-linode
-Version: 4.1.0a1684215503
+Name: pulumi_linode
+Version: 4.1.0a1684348483
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.1.0a1684215503/pulumi_linode.egg-info/SOURCES.txt` & `pulumi_linode-4.1.0a1684348483/pulumi_linode.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 README.md
 setup.py
 pulumi_linode/__init__.py
 pulumi_linode/_inputs.py
 pulumi_linode/_utilities.py
 pulumi_linode/account_settings.py
 pulumi_linode/database_access_controls.py
-pulumi_linode/database_mongodb.py
 pulumi_linode/database_mysql.py
 pulumi_linode/database_postgresql.py
 pulumi_linode/domain.py
 pulumi_linode/domain_record.py
 pulumi_linode/firewall.py
 pulumi_linode/firewall_device.py
 pulumi_linode/get_account.py
 pulumi_linode/get_account_login.py
 pulumi_linode/get_account_logins.py
 pulumi_linode/get_account_settings.py
 pulumi_linode/get_database_backups.py
 pulumi_linode/get_database_engines.py
-pulumi_linode/get_database_mongodb.py
 pulumi_linode/get_database_mysql.py
 pulumi_linode/get_database_mysql_backups.py
 pulumi_linode/get_database_postgresql.py
 pulumi_linode/get_databases.py
 pulumi_linode/get_domain.py
 pulumi_linode/get_domain_record.py
 pulumi_linode/get_domain_zonefile.py
@@ -69,14 +67,15 @@
 pulumi_linode/outputs.py
 pulumi_linode/provider.py
 pulumi_linode/pulumi-plugin.json
 pulumi_linode/py.typed
 pulumi_linode/rdns.py
 pulumi_linode/ssh_key.py
 pulumi_linode/stack_script.py
+pulumi_linode/token.py
 pulumi_linode/user.py
 pulumi_linode/volume.py
 pulumi_linode.egg-info/PKG-INFO
 pulumi_linode.egg-info/SOURCES.txt
 pulumi_linode.egg-info/dependency_links.txt
 pulumi_linode.egg-info/not-zip-safe
 pulumi_linode.egg-info/requires.txt
```

### Comparing `pulumi_linode-4.1.0a1684215503/setup.py` & `pulumi_linode-4.1.0a1684348483/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.1.0a1684215503"
-PLUGIN_VERSION = "4.1.0-alpha.1684215503+304e9709"
+VERSION = "4.1.0a1684348483"
+PLUGIN_VERSION = "4.1.0-alpha.1684348483+6b8d2a02"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'linode', PLUGIN_VERSION])
         except OSError as error:
```

