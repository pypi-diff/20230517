# Comparing `tmp/ionoscloud-6.1.4.tar.gz` & `tmp/ionoscloud-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ionoscloud-6.1.4.tar", last modified: Thu Sep  8 10:25:30 2022, max compression
+gzip compressed data, was "ionoscloud-6.1.5.tar", last modified: Wed May 17 11:58:47 2023, max compression
```

## Comparing `ionoscloud-6.1.4.tar` & `ionoscloud-6.1.5.tar`

### file list

```diff
@@ -1,234 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:25:30.858807 ionoscloud-6.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-09-08 10:25:30.858807 ionoscloud-6.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:25:30.818807 ionoscloud-6.1.4/ionoscloud/
--rw-r--r--   0 runner    (1001) docker     (121)    15175 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:25:30.826807 ionoscloud-6.1.4/ionoscloud/api/
--rw-r--r--   0 runner    (1001) docker     (121)     8406 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/__api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   213938 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/application_load_balancers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    64006 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/backup_units_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8641 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/contract_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    59467 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/data_centers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    75234 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/firewall_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    70574 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/flow_logs_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    45920 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/images_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    57183 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/ip_blocks_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   160570 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/kubernetes_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   273907 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/labels_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    95948 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/lans_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   108562 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/load_balancers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    27669 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/locations_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   198795 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/nat_gateways_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    68048 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/network_interfaces_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   210828 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/network_load_balancers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    45780 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/private_cross_connects_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    36951 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/requests_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   237445 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/servers_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    46420 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    58443 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/target_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    15744 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/templates_api.py
--rw-r--r--   0 runner    (1001) docker     (121)   226401 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/user_management_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    56915 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/user_s3_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    86469 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api/volumes_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    34764 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    17710 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     5434 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:25:30.858807 ionoscloud-6.1.4/ionoscloud/models/
--rw-r--r--   0 runner    (1001) docker     (121)    13191 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7841 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4062 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7423 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    11827 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rule_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)    13138 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_http_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     9183 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_http_rule_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     8709 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     8405 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/application_load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/attached_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7028 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/backup_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5695 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/backup_unit_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/backup_unit_sso.py
--rw-r--r--   0 runner    (1001) docker     (121)     6157 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/backup_units.py
--rw-r--r--   0 runner    (1001) docker     (121)     7961 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/balanced_nics.py
--rw-r--r--   0 runner    (1001) docker     (121)     7775 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/cdroms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/connectable_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4540 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (121)     7145 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/contract_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/contracts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6329 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/cpu_architecture_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     7592 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/data_center_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (121)    13639 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/datacenter_element_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    10027 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/datacenter_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     7950 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/datacenters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-09-08 09:40:31.000000 ionoscloud-6.1.4/ionoscloud/models/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/error_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     8020 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)    17328 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/firewallrule_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6613 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/flow_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     7470 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/flow_log_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/flow_log_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     7845 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     5825 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_members.py
--rw-r--r--   0 runner    (1001) docker     (121)    16837 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_share.py
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_share_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_shares.py
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/group_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     6559 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    21505 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/image_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5708 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6613 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/ip_block.py
--rw-r--r--   0 runner    (1001) docker     (121)     7403 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/ip_block_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     8053 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/ip_blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9353 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/ip_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/ip_failover.py
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_auto_scaling.py
--rw-r--r--   0 runner    (1001) docker     (121)     7920 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     8137 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_for_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_for_put.py
--rw-r--r--   0 runner    (1001) docker     (121)    11931 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     9547 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_properties_for_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     9523 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_properties_for_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     7077 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     7198 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     7387 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_for_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     7360 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_for_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_lan.py
--rw-r--r--   0 runner    (1001) docker     (121)     4792 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_lan_routes.py
--rw-r--r--   0 runner    (1001) docker     (121)    22787 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    21983 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_properties_for_post.py
--rw-r--r--   0 runner    (1001) docker     (121)    12937 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_properties_for_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7022 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6345 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/kubernetes_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6870 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     7070 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/label_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     7108 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/label_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     4430 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/label_resource_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     8455 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/label_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     6108 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/labels.py
--rw-r--r--   0 runner    (1001) docker     (121)     7161 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lan_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lan_nics.py
--rw-r--r--   0 runner    (1001) docker     (121)     7285 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lan_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     6095 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lan_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6175 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lan_properties_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/lans.py
--rw-r--r--   0 runner    (1001) docker     (121)     7467 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/loadbalancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/loadbalancer_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/loadbalancer_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     8020 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/location.py
--rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/location_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/locations.py
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_lan_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6127 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6028 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     6802 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    10741 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     6120 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     3116 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     5915 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     7950 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7315 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     7839 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    11456 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6557 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     7784 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     8559 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6235 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     8265 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/network_load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7161 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4464 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nic_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)    11679 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nic_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5867 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nic_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/nics.py
--rw-r--r--   0 runner    (1001) docker     (121)     9995 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/no_state_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5530 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/pagination_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     6178 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/peer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/private_cross_connect.py
--rw-r--r--   0 runner    (1001) docker     (121)     6933 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/private_cross_connect_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6030 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/private_cross_connects.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/remote_console_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     6583 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/request_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/request_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5829 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/request_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/request_status_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/request_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     7139 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resource_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     5845 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    28994 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resource_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resource_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resource_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     5745 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     5845 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/resources_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/s3_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/s3_key_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     4572 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/s3_key_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/s3_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/s3_object_storage_sso.py
--rw-r--r--   0 runner    (1001) docker     (121)     7263 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/server_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)    13256 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/server_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     7810 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/servers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)    18679 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/snapshot_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (121)     6721 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     6360 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_group_health_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     8925 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_group_http_health_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     9214 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_group_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_group_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     9110 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_group_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     8193 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     4526 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/target_port_range.py
--rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/template.py
--rw-r--r--   0 runner    (1001) docker     (121)     6615 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/template_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/type.py
--rw-r--r--   0 runner    (1001) docker     (121)     7159 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     5738 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     9979 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     9800 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user_properties_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     9776 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user_properties_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/user_put.py
--rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/users_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     6586 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    27480 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/volume_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     7810 2022-09-08 09:40:32.000000 ionoscloud-6.1.4/ionoscloud/models/volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    13863 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/ionoscloud/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:25:30.818807 ionoscloud-6.1.4/ionoscloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-09-08 10:25:30.000000 ionoscloud-6.1.4/ionoscloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8812 2022-09-08 10:25:30.000000 ionoscloud-6.1.4/ionoscloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 10:25:30.000000 ionoscloud-6.1.4/ionoscloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-08 10:25:30.000000 ionoscloud-6.1.4/ionoscloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-08 10:25:30.000000 ionoscloud-6.1.4/ionoscloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-08 10:25:30.858807 ionoscloud-6.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-09-08 09:40:33.000000 ionoscloud-6.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:58:46.992526 ionoscloud-6.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-05-17 09:59:08.000000 ionoscloud-6.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    67343 2023-05-17 11:58:46.992526 ionoscloud-6.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:58:46.956526 ionoscloud-6.1.5/ionoscloud/
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:58:46.972526 ionoscloud-6.1.5/ionoscloud/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/__api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214360 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/application_load_balancers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64006 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/backup_units_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/contract_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/data_centers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75244 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/firewall_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70578 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/flow_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45940 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/images_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57205 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/ip_blocks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160838 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/kubernetes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   273991 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/labels_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105136 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/lans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108586 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/load_balancers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28903 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/locations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198835 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/nat_gateways_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/network_interfaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/network_load_balancers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45784 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/private_cross_connects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36951 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241017 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/servers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46438 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59171 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/target_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226405 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/user_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/user_s3_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86491 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api/volumes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34764 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:58:46.992526 ionoscloud-6.1.5/ionoscloud/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rule_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_http_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_http_rule_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/application_load_balancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/attached_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/backup_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/backup_unit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/backup_unit_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/backup_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/balanced_nics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/cdroms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/connectable_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/contract_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/cpu_architecture_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/data_center_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-17 09:59:32.000000 ionoscloud-6.1.5/ionoscloud/models/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/datacenter_element_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/datacenter_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/firewallrule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/flow_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/flow_log_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/flow_log_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_share_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/image_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/ip_block_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/ip_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/ip_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/ip_failover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_auto_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_properties_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_properties_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_lan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_lan_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23285 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_properties_for_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_properties_for_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/kubernetes_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/label_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/label_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/label_resource_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/label_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lan_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lan_nics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lan_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lan_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lan_properties_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/lans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/loadbalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/loadbalancer_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/loadbalancer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/location_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_lan_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/network_load_balancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nic_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nic_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nic_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/nics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/no_state_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/pagination_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/private_cross_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/private_cross_connect_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/private_cross_connects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/remote_console_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/request_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/request_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/request_status_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resource_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30562 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resource_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resource_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resource_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/resources_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/s3_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/s3_key_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/s3_key_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/s3_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/s3_object_storage_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/server_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/server_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/snapshot_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_group_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_group_http_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_group_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_group_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_group_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/target_port_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/template_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user_properties_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user_properties_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/user_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/users_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27446 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/volume_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-17 09:59:33.000000 ionoscloud-6.1.5/ionoscloud/models/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/ionoscloud/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:58:46.960526 ionoscloud-6.1.5/ionoscloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67343 2023-05-17 11:58:46.000000 ionoscloud-6.1.5/ionoscloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-17 11:58:46.000000 ionoscloud-6.1.5/ionoscloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:58:46.000000 ionoscloud-6.1.5/ionoscloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 11:58:46.000000 ionoscloud-6.1.5/ionoscloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 11:58:46.000000 ionoscloud-6.1.5/ionoscloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 11:58:46.992526 ionoscloud-6.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-17 09:59:34.000000 ionoscloud-6.1.5/setup.py
```

### Comparing `ionoscloud-6.1.4/ionoscloud/__init__.py` & `ionoscloud-6.1.5/ionoscloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 6.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "6.1.4"
+__version__ = "6.1.5"
 
 # import apis into sdk package
 from ionoscloud.api.application_load_balancers_api import ApplicationLoadBalancersApi
 from ionoscloud.api.backup_units_api import BackupUnitsApi
 from ionoscloud.api.contract_resources_api import ContractResourcesApi
 from ionoscloud.api.data_centers_api import DataCentersApi
 from ionoscloud.api.firewall_rules_api import FirewallRulesApi
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/__api.py` & `ionoscloud-6.1.5/ionoscloud/api/__api.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def api_info_get(self, **kwargs):  # noqa: E501
-        """Display API information  # noqa: E501
+        """Get API information  # noqa: E501
 
-        Display API information  # noqa: E501
+        Retrieves the API information such as API version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_info_get(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -48,17 +48,17 @@
                  returns the request thread.
         :rtype: Info
         """
         kwargs['_return_http_data_only'] = True
         return self.api_info_get_with_http_info(**kwargs)  # noqa: E501
 
     def api_info_get_with_http_info(self, **kwargs):  # noqa: E501
-        """Display API information  # noqa: E501
+        """Get API information  # noqa: E501
 
-        Display API information  # noqa: E501
+        Retrieves the API information such as API version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_info_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/__init__.py` & `ionoscloud-6.1.5/ionoscloud/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/api/application_load_balancers_api.py` & `ionoscloud-6.1.5/ionoscloud/api/application_load_balancers_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def datacenters_applicationloadbalancers_delete(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """Delete Application Load Balancers  # noqa: E501
+        """Delete an Application Load Balancer by ID  # noqa: E501
 
-        Remove the specified Application Load Balancer from the data center..  # noqa: E501
+        Removes the specified Application Load Balancer from the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_delete(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -52,17 +52,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_delete_with_http_info(datacenter_id, application_load_balancer_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_delete_with_http_info(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """Delete Application Load Balancers  # noqa: E501
+        """Delete an Application Load Balancer by ID  # noqa: E501
 
-        Remove the specified Application Load Balancer from the data center..  # noqa: E501
+        Removes the specified Application Load Balancer from the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_delete_with_http_info(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -187,17 +187,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_find_by_application_load_balancer_id(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """Retrieve Application Load Balancers  # noqa: E501
+        """Get an Application Load Balancer by ID  # noqa: E501
 
-        Retrieve the properties of the specified Application Load Balancer within the data center.  # noqa: E501
+        Retrieves the properties of the specified Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_find_by_application_load_balancer_id(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -225,17 +225,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_find_by_application_load_balancer_id_with_http_info(datacenter_id, application_load_balancer_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_find_by_application_load_balancer_id_with_http_info(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """Retrieve Application Load Balancers  # noqa: E501
+        """Get an Application Load Balancer by ID  # noqa: E501
 
-        Retrieve the properties of the specified Application Load Balancer within the data center.  # noqa: E501
+        Retrieves the properties of the specified Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_find_by_application_load_balancer_id_with_http_info(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -360,28 +360,28 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_flowlogs_delete(self, datacenter_id, application_load_balancer_id, flow_log_id, **kwargs):  # noqa: E501
-        """Delete ALB Flow Logs  # noqa: E501
+        """Delete an ALB Flow Log by ID  # noqa: E501
 
-        Delete the specified Application Load Balancer Flow Log.  # noqa: E501
+        Deletes the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_delete(datacenter_id, application_load_balancer_id, flow_log_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -400,28 +400,28 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_flowlogs_delete_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_flowlogs_delete_with_http_info(self, datacenter_id, application_load_balancer_id, flow_log_id, **kwargs):  # noqa: E501
-        """Delete ALB Flow Logs  # noqa: E501
+        """Delete an ALB Flow Log by ID  # noqa: E501
 
-        Delete the specified Application Load Balancer Flow Log.  # noqa: E501
+        Deletes the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_delete_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -544,28 +544,28 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_flowlogs_find_by_flow_log_id(self, datacenter_id, application_load_balancer_id, flow_log_id, **kwargs):  # noqa: E501
-        """Retrieve ALB Flow Logs  # noqa: E501
+        """Get an ALB Flow Log by ID  # noqa: E501
 
-        Retrieve the specified Application Load Balancer Flow Log.  # noqa: E501
+        Retrieves the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_find_by_flow_log_id(datacenter_id, application_load_balancer_id, flow_log_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -584,28 +584,28 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_flowlogs_find_by_flow_log_id_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_flowlogs_find_by_flow_log_id_with_http_info(self, datacenter_id, application_load_balancer_id, flow_log_id, **kwargs):  # noqa: E501
-        """Retrieve ALB Flow Logs  # noqa: E501
+        """Get an ALB Flow Log by ID  # noqa: E501
 
-        Retrieve the specified Application Load Balancer Flow Log.  # noqa: E501
+        Retrieves the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_find_by_flow_log_id_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -728,17 +728,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_flowlogs_get(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """List ALB Flow Logs  # noqa: E501
+        """Get ALB Flow Logs  # noqa: E501
 
-        List the Flow Logs for the specified Application Load Balancer.  # noqa: E501
+        Retrieves the flow logs for the specified Application Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_get(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -766,17 +766,17 @@
                  returns the request thread.
         :rtype: FlowLogs
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_flowlogs_get_with_http_info(datacenter_id, application_load_balancer_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_flowlogs_get_with_http_info(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """List ALB Flow Logs  # noqa: E501
+        """Get ALB Flow Logs  # noqa: E501
 
-        List the Flow Logs for the specified Application Load Balancer.  # noqa: E501
+        Retrieves the flow logs for the specified Application Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_get_with_http_info(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -901,30 +901,30 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_flowlogs_patch(self, datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log_properties, **kwargs):  # noqa: E501
-        """Partially modify ALB Flow Logs  # noqa: E501
+        """Partially Modify an ALB Flow Log by ID  # noqa: E501
 
-        Update the properties of the specified Application Load Balancer Flow Log.  # noqa: E501
+        Updates the properties of the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_patch(datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
-        :param application_load_balancer_flow_log_properties: The properties of the ALB Flow Log to be updated. (required)
+        :param application_load_balancer_flow_log_properties: The properties of the ALB flow log to be updated. (required)
         :type application_load_balancer_flow_log_properties: FlowLogProperties
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -943,30 +943,30 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_flowlogs_patch_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log_properties, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_flowlogs_patch_with_http_info(self, datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log_properties, **kwargs):  # noqa: E501
-        """Partially modify ALB Flow Logs  # noqa: E501
+        """Partially Modify an ALB Flow Log by ID  # noqa: E501
 
-        Update the properties of the specified Application Load Balancer Flow Log.  # noqa: E501
+        Updates the properties of the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_patch_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
-        :param application_load_balancer_flow_log_properties: The properties of the ALB Flow Log to be updated. (required)
+        :param application_load_balancer_flow_log_properties: The properties of the ALB flow log to be updated. (required)
         :type application_load_balancer_flow_log_properties: FlowLogProperties
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -1096,28 +1096,28 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_flowlogs_post(self, datacenter_id, application_load_balancer_id, application_load_balancer_flow_log, **kwargs):  # noqa: E501
-        """Create ALB Flow Logs  # noqa: E501
+        """Create an ALB Flow Log  # noqa: E501
 
-        Add a new Flow Log for the Application Load Balancer.  # noqa: E501
+        Creates a flow log for the Application Load Balancer specified by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_post(datacenter_id, application_load_balancer_id, application_load_balancer_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param application_load_balancer_flow_log: The Flow Log to create. (required)
+        :param application_load_balancer_flow_log: The flow log to create. (required)
         :type application_load_balancer_flow_log: FlowLog
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -1136,28 +1136,28 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_flowlogs_post_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer_flow_log, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_flowlogs_post_with_http_info(self, datacenter_id, application_load_balancer_id, application_load_balancer_flow_log, **kwargs):  # noqa: E501
-        """Create ALB Flow Logs  # noqa: E501
+        """Create an ALB Flow Log  # noqa: E501
 
-        Add a new Flow Log for the Application Load Balancer.  # noqa: E501
+        Creates a flow log for the Application Load Balancer specified by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_post_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param application_load_balancer_flow_log: The Flow Log to create. (required)
+        :param application_load_balancer_flow_log: The flow log to create. (required)
         :type application_load_balancer_flow_log: FlowLog
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -1284,30 +1284,30 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_flowlogs_put(self, datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log, **kwargs):  # noqa: E501
-        """Modify ALB Flow Logs  # noqa: E501
+        """Modify an ALB Flow Log by ID  # noqa: E501
 
-        Modify the specified Application Load Balancer Flow Log.  # noqa: E501
+        Modifies the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_put(datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
-        :param application_load_balancer_flow_log: The modified ALB Flow Log. (required)
+        :param application_load_balancer_flow_log: The modified ALB flow log. (required)
         :type application_load_balancer_flow_log: FlowLogPut
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -1326,30 +1326,30 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_flowlogs_put_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_flowlogs_put_with_http_info(self, datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log, **kwargs):  # noqa: E501
-        """Modify ALB Flow Logs  # noqa: E501
+        """Modify an ALB Flow Log by ID  # noqa: E501
 
-        Modify the specified Application Load Balancer Flow Log.  # noqa: E501
+        Modifies the Application Load Balancer flow log specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_flowlogs_put_with_http_info(datacenter_id, application_load_balancer_id, flow_log_id, application_load_balancer_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
         :type datacenter_id: str
         :param application_load_balancer_id: The unique ID of the Application Load Balancer. (required)
         :type application_load_balancer_id: str
-        :param flow_log_id: The unique ID of the Flow Log. (required)
+        :param flow_log_id: The unique ID of the flow log. (required)
         :type flow_log_id: str
-        :param application_load_balancer_flow_log: The modified ALB Flow Log. (required)
+        :param application_load_balancer_flow_log: The modified ALB flow log. (required)
         :type application_load_balancer_flow_log: FlowLogPut
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -1483,17 +1483,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_forwardingrules_delete(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, **kwargs):  # noqa: E501
-        """Delete ALB forwarding rules  # noqa: E501
+        """Delete an ALB Forwarding Rule by ID  # noqa: E501
 
-        Delete the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Deletes the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_delete(datacenter_id, application_load_balancer_id, forwarding_rule_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1523,17 +1523,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_forwardingrules_delete_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_forwardingrules_delete_with_http_info(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, **kwargs):  # noqa: E501
-        """Delete ALB forwarding rules  # noqa: E501
+        """Delete an ALB Forwarding Rule by ID  # noqa: E501
 
-        Delete the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Deletes the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_delete_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1667,17 +1667,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_forwardingrules_find_by_forwarding_rule_id(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, **kwargs):  # noqa: E501
-        """Retrieve ALB forwarding rules  # noqa: E501
+        """Get an ALB Forwarding Rule by ID  # noqa: E501
 
-        Retrieve the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Retrieves the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_find_by_forwarding_rule_id(datacenter_id, application_load_balancer_id, forwarding_rule_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1707,17 +1707,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancerForwardingRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_forwardingrules_find_by_forwarding_rule_id_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_forwardingrules_find_by_forwarding_rule_id_with_http_info(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, **kwargs):  # noqa: E501
-        """Retrieve ALB forwarding rules  # noqa: E501
+        """Get an ALB Forwarding Rule by ID  # noqa: E501
 
-        Retrieve the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Retrieves the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_find_by_forwarding_rule_id_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1851,17 +1851,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_forwardingrules_get(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """List ALB forwarding rules  # noqa: E501
+        """Get ALB Forwarding Rules  # noqa: E501
 
-        List the forwarding rules for the specified Application Load Balancer.  # noqa: E501
+        Lists the forwarding rules of the specified Application Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_get(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1889,17 +1889,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancerForwardingRules
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_forwardingrules_get_with_http_info(datacenter_id, application_load_balancer_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_forwardingrules_get_with_http_info(self, datacenter_id, application_load_balancer_id, **kwargs):  # noqa: E501
-        """List ALB forwarding rules  # noqa: E501
+        """Get ALB Forwarding Rules  # noqa: E501
 
-        List the forwarding rules for the specified Application Load Balancer.  # noqa: E501
+        Lists the forwarding rules of the specified Application Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_get_with_http_info(datacenter_id, application_load_balancer_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2024,17 +2024,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_forwardingrules_patch(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule_properties, **kwargs):  # noqa: E501
-        """Partially modify ALB forwarding rules  # noqa: E501
+        """Partially modify an ALB Forwarding Rule by ID  # noqa: E501
 
-        Update the properties of the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Updates the properties of the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_patch(datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2066,17 +2066,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancerForwardingRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_forwardingrules_patch_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule_properties, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_forwardingrules_patch_with_http_info(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule_properties, **kwargs):  # noqa: E501
-        """Partially modify ALB forwarding rules  # noqa: E501
+        """Partially modify an ALB Forwarding Rule by ID  # noqa: E501
 
-        Update the properties of the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Updates the properties of the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_patch_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2219,17 +2219,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_forwardingrules_post(self, datacenter_id, application_load_balancer_id, application_load_balancer_forwarding_rule, **kwargs):  # noqa: E501
-        """Create ALB forwarding rules  # noqa: E501
+        """Create an ALB Forwarding Rule  # noqa: E501
 
-        Create a forwarding rule for the Application Load Balancer.  # noqa: E501
+        Creates a forwarding rule for the specified Application Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_post(datacenter_id, application_load_balancer_id, application_load_balancer_forwarding_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2259,17 +2259,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancerForwardingRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_forwardingrules_post_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer_forwarding_rule, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_forwardingrules_post_with_http_info(self, datacenter_id, application_load_balancer_id, application_load_balancer_forwarding_rule, **kwargs):  # noqa: E501
-        """Create ALB forwarding rules  # noqa: E501
+        """Create an ALB Forwarding Rule  # noqa: E501
 
-        Create a forwarding rule for the Application Load Balancer.  # noqa: E501
+        Creates a forwarding rule for the specified Application Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_post_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer_forwarding_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2407,17 +2407,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_forwardingrules_put(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule, **kwargs):  # noqa: E501
-        """Modify ALB forwarding rules  # noqa: E501
+        """Modify an ALB Forwarding Rule by ID  # noqa: E501
 
-        Modify the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Modifies the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_put(datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2449,17 +2449,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancerForwardingRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_forwardingrules_put_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_forwardingrules_put_with_http_info(self, datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule, **kwargs):  # noqa: E501
-        """Modify ALB forwarding rules  # noqa: E501
+        """Modify an ALB Forwarding Rule by ID  # noqa: E501
 
-        Modify the specified Application Load Balancer forwarding rule.  # noqa: E501
+        Modifies the Application Load Balancer forwarding rule specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_forwardingrules_put_with_http_info(datacenter_id, application_load_balancer_id, forwarding_rule_id, application_load_balancer_forwarding_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2606,17 +2606,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_get(self, datacenter_id, **kwargs):  # noqa: E501
-        """List Application Load Balancers  # noqa: E501
+        """Get Application Load Balancers  # noqa: E501
 
-        List all Application Load Balancers within the data center.  # noqa: E501
+        Lists all Application Load Balancers within a data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_get(datacenter_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2646,17 +2646,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancers
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_get_with_http_info(datacenter_id, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_get_with_http_info(self, datacenter_id, **kwargs):  # noqa: E501
-        """List Application Load Balancers  # noqa: E501
+        """Get Application Load Balancers  # noqa: E501
 
-        List all Application Load Balancers within the data center.  # noqa: E501
+        Lists all Application Load Balancers within a data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_get_with_http_info(datacenter_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2788,17 +2788,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_patch(self, datacenter_id, application_load_balancer_id, application_load_balancer_properties, **kwargs):  # noqa: E501
-        """Partially modify Application Load Balancers  # noqa: E501
+        """Partially Modify an Application Load Balancer by ID  # noqa: E501
 
-        Update the properties of the specified Application Load Balancer within the data center.  # noqa: E501
+        Updates the properties of the specified Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_patch(datacenter_id, application_load_balancer_id, application_load_balancer_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2828,17 +2828,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_patch_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer_properties, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_patch_with_http_info(self, datacenter_id, application_load_balancer_id, application_load_balancer_properties, **kwargs):  # noqa: E501
-        """Partially modify Application Load Balancers  # noqa: E501
+        """Partially Modify an Application Load Balancer by ID  # noqa: E501
 
-        Update the properties of the specified Application Load Balancer within the data center.  # noqa: E501
+        Updates the properties of the specified Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_patch_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2972,17 +2972,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_post(self, datacenter_id, application_load_balancer, **kwargs):  # noqa: E501
-        """Create Application Load Balancers  # noqa: E501
+        """Create an Application Load Balancer  # noqa: E501
 
-        Create an Application Load Balancer within the datacenter.  # noqa: E501
+        Creates an Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_post(datacenter_id, application_load_balancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3010,17 +3010,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_post_with_http_info(datacenter_id, application_load_balancer, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_post_with_http_info(self, datacenter_id, application_load_balancer, **kwargs):  # noqa: E501
-        """Create Application Load Balancers  # noqa: E501
+        """Create an Application Load Balancer  # noqa: E501
 
-        Create an Application Load Balancer within the datacenter.  # noqa: E501
+        Creates an Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_post_with_http_info(datacenter_id, application_load_balancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3149,17 +3149,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_applicationloadbalancers_put(self, datacenter_id, application_load_balancer_id, application_load_balancer, **kwargs):  # noqa: E501
-        """Modify Application Load Balancers  # noqa: E501
+        """Modify an Application Load Balancer by ID  # noqa: E501
 
-        Modify the properties of the specified Application Load Balancer within the data center.  # noqa: E501
+        Modifies the properties of the specified Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_put(datacenter_id, application_load_balancer_id, application_load_balancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3189,17 +3189,17 @@
                  returns the request thread.
         :rtype: ApplicationLoadBalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_applicationloadbalancers_put_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer, **kwargs)  # noqa: E501
 
     def datacenters_applicationloadbalancers_put_with_http_info(self, datacenter_id, application_load_balancer_id, application_load_balancer, **kwargs):  # noqa: E501
-        """Modify Application Load Balancers  # noqa: E501
+        """Modify an Application Load Balancer by ID  # noqa: E501
 
-        Modify the properties of the specified Application Load Balancer within the data center.  # noqa: E501
+        Modifies the properties of the specified Application Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_applicationloadbalancers_put_with_http_info(datacenter_id, application_load_balancer_id, application_load_balancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/backup_units_api.py` & `ionoscloud-6.1.5/ionoscloud/api/backup_units_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/api/contract_resources_api.py` & `ionoscloud-6.1.5/ionoscloud/api/contract_resources_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def contracts_get(self, **kwargs):  # noqa: E501
-        """Retrieve contracts  # noqa: E501
+        """Get Contract Information  # noqa: E501
 
-        Retrieve the properties of the user's contract. In this version, the resource became a collection.  # noqa: E501
+        Retrieves the properties of the user's contract. This operation allows you to obtain the resource limits and the general contract information.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.contracts_get(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -48,17 +48,17 @@
                  returns the request thread.
         :rtype: Contracts
         """
         kwargs['_return_http_data_only'] = True
         return self.contracts_get_with_http_info(**kwargs)  # noqa: E501
 
     def contracts_get_with_http_info(self, **kwargs):  # noqa: E501
-        """Retrieve contracts  # noqa: E501
+        """Get Contract Information  # noqa: E501
 
-        Retrieve the properties of the user's contract. In this version, the resource became a collection.  # noqa: E501
+        Retrieves the properties of the user's contract. This operation allows you to obtain the resource limits and the general contract information.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.contracts_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/data_centers_api.py` & `ionoscloud-6.1.5/ionoscloud/api/data_centers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,17 +509,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_patch(self, datacenter_id, datacenter, **kwargs):  # noqa: E501
-        """Partially modify data centers  # noqa: E501
+        """Partially modify a Data Center by ID  # noqa: E501
 
-        Update the properties of the specified data center, rename it, or change the description.  # noqa: E501
+        Updates the properties of the specified data center, rename it, or change the description.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_patch(datacenter_id, datacenter, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -547,17 +547,17 @@
                  returns the request thread.
         :rtype: Datacenter
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_patch_with_http_info(datacenter_id, datacenter, **kwargs)  # noqa: E501
 
     def datacenters_patch_with_http_info(self, datacenter_id, datacenter, **kwargs):  # noqa: E501
-        """Partially modify data centers  # noqa: E501
+        """Partially modify a Data Center by ID  # noqa: E501
 
-        Update the properties of the specified data center, rename it, or change the description.  # noqa: E501
+        Updates the properties of the specified data center, rename it, or change the description.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_patch_with_http_info(datacenter_id, datacenter, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -686,17 +686,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_post(self, datacenter, **kwargs):  # noqa: E501
-        """Create data centers  # noqa: E501
+        """Create a Data Center  # noqa: E501
 
-        Create new data centers, and data centers that already contain elements, such as servers and storage volumes.  Virtual data centers are the foundation of the platform; they act as logical containers for all other objects you create, such as servers and storage volumes. You can provision as many data centers as needed. Data centers have their own private networks and are logically segmented from each other to create isolation.  # noqa: E501
+        Creates new data centers, and data centers that already contain elements, such as servers and storage volumes.  Virtual data centers are the foundation of the platform; they act as logical containers for all other objects you create, such as servers and storage volumes. You can provision as many data centers as needed. Data centers have their own private networks and are logically segmented from each other to create isolation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_post(datacenter, async_req=True)
         >>> result = thread.get()
 
         :param datacenter: The data center to create. (required)
@@ -722,17 +722,17 @@
                  returns the request thread.
         :rtype: Datacenter
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_post_with_http_info(datacenter, **kwargs)  # noqa: E501
 
     def datacenters_post_with_http_info(self, datacenter, **kwargs):  # noqa: E501
-        """Create data centers  # noqa: E501
+        """Create a Data Center  # noqa: E501
 
-        Create new data centers, and data centers that already contain elements, such as servers and storage volumes.  Virtual data centers are the foundation of the platform; they act as logical containers for all other objects you create, such as servers and storage volumes. You can provision as many data centers as needed. Data centers have their own private networks and are logically segmented from each other to create isolation.  # noqa: E501
+        Creates new data centers, and data centers that already contain elements, such as servers and storage volumes.  Virtual data centers are the foundation of the platform; they act as logical containers for all other objects you create, such as servers and storage volumes. You can provision as many data centers as needed. Data centers have their own private networks and are logically segmented from each other to create isolation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_post_with_http_info(datacenter, async_req=True)
         >>> result = thread.get()
 
         :param datacenter: The data center to create. (required)
@@ -852,17 +852,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_put(self, datacenter_id, datacenter, **kwargs):  # noqa: E501
-        """Modify data centers  # noqa: E501
+        """Modify a Data Center by ID  # noqa: E501
 
-        Modify the properties of the specified data center, rename it, or change the description.  # noqa: E501
+        Modifies the properties of the specified data center, rename it, or change the description.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_put(datacenter_id, datacenter, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -890,17 +890,17 @@
                  returns the request thread.
         :rtype: Datacenter
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_put_with_http_info(datacenter_id, datacenter, **kwargs)  # noqa: E501
 
     def datacenters_put_with_http_info(self, datacenter_id, datacenter, **kwargs):  # noqa: E501
-        """Modify data centers  # noqa: E501
+        """Modify a Data Center by ID  # noqa: E501
 
-        Modify the properties of the specified data center, rename it, or change the description.  # noqa: E501
+        Modifies the properties of the specified data center, rename it, or change the description.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_put_with_http_info(datacenter_id, datacenter, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/firewall_rules_api.py` & `ionoscloud-6.1.5/ionoscloud/api/firewall_rules_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -818,17 +818,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_nics_firewallrules_post(self, datacenter_id, server_id, nic_id, firewallrule, **kwargs):  # noqa: E501
-        """Create firewall rules  # noqa: E501
+        """Create a Firewall Rule  # noqa: E501
 
-        Create a firewall rule for the specified NIC.  # noqa: E501
+        Creates a firewall rule for the specified NIC.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_firewallrules_post(datacenter_id, server_id, nic_id, firewallrule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -860,17 +860,17 @@
                  returns the request thread.
         :rtype: FirewallRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_nics_firewallrules_post_with_http_info(datacenter_id, server_id, nic_id, firewallrule, **kwargs)  # noqa: E501
 
     def datacenters_servers_nics_firewallrules_post_with_http_info(self, datacenter_id, server_id, nic_id, firewallrule, **kwargs):  # noqa: E501
-        """Create firewall rules  # noqa: E501
+        """Create a Firewall Rule  # noqa: E501
 
-        Create a firewall rule for the specified NIC.  # noqa: E501
+        Creates a firewall rule for the specified NIC.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_firewallrules_post_with_http_info(datacenter_id, server_id, nic_id, firewallrule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1017,17 +1017,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_nics_firewallrules_put(self, datacenter_id, server_id, nic_id, firewallrule_id, firewallrule, **kwargs):  # noqa: E501
-        """Modify firewall rules  # noqa: E501
+        """Modify a Firewall Rule  # noqa: E501
 
-        Modify the properties of the specified firewall rule.  # noqa: E501
+        Modifies the properties of the specified firewall rule.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_firewallrules_put(datacenter_id, server_id, nic_id, firewallrule_id, firewallrule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1061,17 +1061,17 @@
                  returns the request thread.
         :rtype: FirewallRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_nics_firewallrules_put_with_http_info(datacenter_id, server_id, nic_id, firewallrule_id, firewallrule, **kwargs)  # noqa: E501
 
     def datacenters_servers_nics_firewallrules_put_with_http_info(self, datacenter_id, server_id, nic_id, firewallrule_id, firewallrule, **kwargs):  # noqa: E501
-        """Modify firewall rules  # noqa: E501
+        """Modify a Firewall Rule  # noqa: E501
 
-        Modify the properties of the specified firewall rule.  # noqa: E501
+        Modifies the properties of the specified firewall rule.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_firewallrules_put_with_http_info(datacenter_id, server_id, nic_id, firewallrule_id, firewallrule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/flow_logs_api.py` & `ionoscloud-6.1.5/ionoscloud/api/flow_logs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,17 +790,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_nics_flowlogs_post(self, datacenter_id, server_id, nic_id, flowlog, **kwargs):  # noqa: E501
-        """Create Flow Logs  # noqa: E501
+        """Create a Flow Log  # noqa: E501
 
-        Add a new Flow Log for the specified NIC.  # noqa: E501
+        Adds a new Flow Log for the specified NIC.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_flowlogs_post(datacenter_id, server_id, nic_id, flowlog, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -830,17 +830,17 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_nics_flowlogs_post_with_http_info(datacenter_id, server_id, nic_id, flowlog, **kwargs)  # noqa: E501
 
     def datacenters_servers_nics_flowlogs_post_with_http_info(self, datacenter_id, server_id, nic_id, flowlog, **kwargs):  # noqa: E501
-        """Create Flow Logs  # noqa: E501
+        """Create a Flow Log  # noqa: E501
 
-        Add a new Flow Log for the specified NIC.  # noqa: E501
+        Adds a new Flow Log for the specified NIC.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_flowlogs_post_with_http_info(datacenter_id, server_id, nic_id, flowlog, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/images_api.py` & `ionoscloud-6.1.5/ionoscloud/api/images_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,17 +666,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def images_put(self, image_id, image, **kwargs):  # noqa: E501
-        """Modify images  # noqa: E501
+        """Modify an Image by ID  # noqa: E501
 
-        Modify the properties of the specified image.  # noqa: E501
+        Modifies the properties of the specified image.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.images_put(image_id, image, async_req=True)
         >>> result = thread.get()
 
         :param image_id: The unique ID of the image. (required)
@@ -704,17 +704,17 @@
                  returns the request thread.
         :rtype: Image
         """
         kwargs['_return_http_data_only'] = True
         return self.images_put_with_http_info(image_id, image, **kwargs)  # noqa: E501
 
     def images_put_with_http_info(self, image_id, image, **kwargs):  # noqa: E501
-        """Modify images  # noqa: E501
+        """Modify an Image by ID  # noqa: E501
 
-        Modify the properties of the specified image.  # noqa: E501
+        Modifies the properties of the specified image.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.images_put_with_http_info(image_id, image, async_req=True)
         >>> result = thread.get()
 
         :param image_id: The unique ID of the image. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/ip_blocks_api.py` & `ionoscloud-6.1.5/ionoscloud/api/ip_blocks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,17 +686,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def ipblocks_post(self, ipblock, **kwargs):  # noqa: E501
-        """Reserve IP blocks  # noqa: E501
+        """Reserve a IP Block  # noqa: E501
 
-        Reserve a new IP block.  # noqa: E501
+        Reserves a new IP block.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.ipblocks_post(ipblock, async_req=True)
         >>> result = thread.get()
 
         :param ipblock: The IP block to be reserved. (required)
@@ -722,17 +722,17 @@
                  returns the request thread.
         :rtype: IpBlock
         """
         kwargs['_return_http_data_only'] = True
         return self.ipblocks_post_with_http_info(ipblock, **kwargs)  # noqa: E501
 
     def ipblocks_post_with_http_info(self, ipblock, **kwargs):  # noqa: E501
-        """Reserve IP blocks  # noqa: E501
+        """Reserve a IP Block  # noqa: E501
 
-        Reserve a new IP block.  # noqa: E501
+        Reserves a new IP block.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.ipblocks_post_with_http_info(ipblock, async_req=True)
         >>> result = thread.get()
 
         :param ipblock: The IP block to be reserved. (required)
@@ -852,17 +852,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def ipblocks_put(self, ipblock_id, ipblock, **kwargs):  # noqa: E501
-        """Modify IP blocks  # noqa: E501
+        """Modify a IP Block by ID  # noqa: E501
 
-        Modify the properties of the specified IP block.  # noqa: E501
+        Modifies the properties of the specified IP block.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.ipblocks_put(ipblock_id, ipblock, async_req=True)
         >>> result = thread.get()
 
         :param ipblock_id: The unique ID of the IP block. (required)
@@ -890,17 +890,17 @@
                  returns the request thread.
         :rtype: IpBlock
         """
         kwargs['_return_http_data_only'] = True
         return self.ipblocks_put_with_http_info(ipblock_id, ipblock, **kwargs)  # noqa: E501
 
     def ipblocks_put_with_http_info(self, ipblock_id, ipblock, **kwargs):  # noqa: E501
-        """Modify IP blocks  # noqa: E501
+        """Modify a IP Block by ID  # noqa: E501
 
-        Modify the properties of the specified IP block.  # noqa: E501
+        Modifies the properties of the specified IP block.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.ipblocks_put_with_http_info(ipblock_id, ipblock, async_req=True)
         >>> result = thread.get()
 
         :param ipblock_id: The unique ID of the IP block. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/kubernetes_api.py` & `ionoscloud-6.1.5/ionoscloud/api/kubernetes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def k8s_delete(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """Delete Kubernetes clusters  # noqa: E501
+        """Delete a Kubernetes Cluster by ID  # noqa: E501
 
-        Delete the specified Kubernetes cluster.  # noqa: E501
+        Deletes the K8s cluster specified  by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_delete(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -50,17 +50,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_delete_with_http_info(k8s_cluster_id, **kwargs)  # noqa: E501
 
     def k8s_delete_with_http_info(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """Delete Kubernetes clusters  # noqa: E501
+        """Delete a Kubernetes Cluster by ID  # noqa: E501
 
-        Delete the specified Kubernetes cluster.  # noqa: E501
+        Deletes the K8s cluster specified  by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_delete_with_http_info(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -176,24 +176,24 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_find_by_cluster_id(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes clusters  # noqa: E501
+        """Get a Kubernetes Cluster by ID  # noqa: E501
 
-        Retrieve the specified Kubernetes cluster.  # noqa: E501
+        Retrieves the K8s cluster specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_find_by_cluster_id(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
-        :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
+        :param k8s_cluster_id: The unique ID of the K8s cluster to be retrieved. (required)
         :type k8s_cluster_id: str
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -212,24 +212,24 @@
                  returns the request thread.
         :rtype: KubernetesCluster
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_find_by_cluster_id_with_http_info(k8s_cluster_id, **kwargs)  # noqa: E501
 
     def k8s_find_by_cluster_id_with_http_info(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes clusters  # noqa: E501
+        """Get a Kubernetes Cluster by ID  # noqa: E501
 
-        Retrieve the specified Kubernetes cluster.  # noqa: E501
+        Retrieves the K8s cluster specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_find_by_cluster_id_with_http_info(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
-        :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
+        :param k8s_cluster_id: The unique ID of the K8s cluster to be retrieved. (required)
         :type k8s_cluster_id: str
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
         :type pretty: bool
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
         :type x_contract_number: int
@@ -338,17 +338,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_get(self, **kwargs):  # noqa: E501
-        """List Kubernetes clusters  # noqa: E501
+        """Get Kubernetes Clusters  # noqa: E501
 
-        List all available Kubernetes clusters.  # noqa: E501
+        Retrieves a list of all K8s clusters provisioned under your account.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_get(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -372,17 +372,17 @@
                  returns the request thread.
         :rtype: KubernetesClusters
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_get_with_http_info(**kwargs)  # noqa: E501
 
     def k8s_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List Kubernetes clusters  # noqa: E501
+        """Get Kubernetes Clusters  # noqa: E501
 
-        List all available Kubernetes clusters.  # noqa: E501
+        Retrieves a list of all K8s clusters provisioned under your account.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -489,17 +489,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_kubeconfig_get(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes configuration files  # noqa: E501
+        """Get Kubernetes Configuration File  # noqa: E501
 
-        Retrieve a configuration file for the specified Kubernetes cluster, in YAML or JSON format as defined in the Accept header; the default Accept header is application/yaml.  # noqa: E501
+        Retrieves the configuration file for the specified K8s cluster. You can define the format (YAML or JSON) of the returned file in the Accept header. By default, 'application/yaml' is specified.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_kubeconfig_get(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -525,17 +525,17 @@
                  returns the request thread.
         :rtype: str
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_kubeconfig_get_with_http_info(k8s_cluster_id, **kwargs)  # noqa: E501
 
     def k8s_kubeconfig_get_with_http_info(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes configuration files  # noqa: E501
+        """Get Kubernetes Configuration File  # noqa: E501
 
-        Retrieve a configuration file for the specified Kubernetes cluster, in YAML or JSON format as defined in the Accept header; the default Accept header is application/yaml.  # noqa: E501
+        Retrieves the configuration file for the specified K8s cluster. You can define the format (YAML or JSON) of the returned file in the Accept header. By default, 'application/yaml' is specified.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_kubeconfig_get_with_http_info(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -651,17 +651,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_delete(self, k8s_cluster_id, nodepool_id, **kwargs):  # noqa: E501
-        """Delete Kubernetes node pools  # noqa: E501
+        """Delete a Kubernetes Node Pool by ID  # noqa: E501
 
-        Delete the specified Kubernetes node pool.  # noqa: E501
+        Deletes the K8s node pool specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_delete(k8s_cluster_id, nodepool_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -689,17 +689,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_delete_with_http_info(k8s_cluster_id, nodepool_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_delete_with_http_info(self, k8s_cluster_id, nodepool_id, **kwargs):  # noqa: E501
-        """Delete Kubernetes node pools  # noqa: E501
+        """Delete a Kubernetes Node Pool by ID  # noqa: E501
 
-        Delete the specified Kubernetes node pool.  # noqa: E501
+        Deletes the K8s node pool specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_delete_with_http_info(k8s_cluster_id, nodepool_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -824,17 +824,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_find_by_id(self, k8s_cluster_id, nodepool_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes node pools  # noqa: E501
+        """Get a Kubernetes Node Pool by ID  # noqa: E501
 
-        Retrieve the specified Kubernetes node pool.  # noqa: E501
+        Retrieves the K8s node pool specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_find_by_id(k8s_cluster_id, nodepool_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -862,17 +862,17 @@
                  returns the request thread.
         :rtype: KubernetesNodePool
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_find_by_id_with_http_info(k8s_cluster_id, nodepool_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_find_by_id_with_http_info(self, k8s_cluster_id, nodepool_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes node pools  # noqa: E501
+        """Get a Kubernetes Node Pool by ID  # noqa: E501
 
-        Retrieve the specified Kubernetes node pool.  # noqa: E501
+        Retrieves the K8s node pool specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_find_by_id_with_http_info(k8s_cluster_id, nodepool_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -997,17 +997,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_get(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """List Kubernetes node pools  # noqa: E501
+        """Get Kubernetes Node Pools  # noqa: E501
 
-        List all Kubernetes node pools, included the specified Kubernetes cluster.  # noqa: E501
+        Retrieves a list of K8s node pools of a cluster specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_get(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1033,17 +1033,17 @@
                  returns the request thread.
         :rtype: KubernetesNodePools
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_get_with_http_info(k8s_cluster_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_get_with_http_info(self, k8s_cluster_id, **kwargs):  # noqa: E501
-        """List Kubernetes node pools  # noqa: E501
+        """Get Kubernetes Node Pools  # noqa: E501
 
-        List all Kubernetes node pools, included the specified Kubernetes cluster.  # noqa: E501
+        Retrieves a list of K8s node pools of a cluster specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_get_with_http_info(k8s_cluster_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1159,17 +1159,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_nodes_delete(self, k8s_cluster_id, nodepool_id, node_id, **kwargs):  # noqa: E501
-        """Delete Kubernetes nodes  # noqa: E501
+        """Delete a Kubernetes Node by ID  # noqa: E501
 
-        Delete the specified Kubernetes node.  # noqa: E501
+        Deletes the K8s node specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_delete(k8s_cluster_id, nodepool_id, node_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1199,17 +1199,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_nodes_delete_with_http_info(k8s_cluster_id, nodepool_id, node_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_nodes_delete_with_http_info(self, k8s_cluster_id, nodepool_id, node_id, **kwargs):  # noqa: E501
-        """Delete Kubernetes nodes  # noqa: E501
+        """Delete a Kubernetes Node by ID  # noqa: E501
 
-        Delete the specified Kubernetes node.  # noqa: E501
+        Deletes the K8s node specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_delete_with_http_info(k8s_cluster_id, nodepool_id, node_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1343,17 +1343,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_nodes_find_by_id(self, k8s_cluster_id, nodepool_id, node_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes nodes  # noqa: E501
+        """Get Kubernetes Node by ID  # noqa: E501
 
-        Retrieve the specified Kubernetes node.  # noqa: E501
+        Retrieves the K8s node specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_find_by_id(k8s_cluster_id, nodepool_id, node_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1383,17 +1383,17 @@
                  returns the request thread.
         :rtype: KubernetesNode
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_nodes_find_by_id_with_http_info(k8s_cluster_id, nodepool_id, node_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_nodes_find_by_id_with_http_info(self, k8s_cluster_id, nodepool_id, node_id, **kwargs):  # noqa: E501
-        """Retrieve Kubernetes nodes  # noqa: E501
+        """Get Kubernetes Node by ID  # noqa: E501
 
-        Retrieve the specified Kubernetes node.  # noqa: E501
+        Retrieves the K8s node specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_find_by_id_with_http_info(k8s_cluster_id, nodepool_id, node_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1527,17 +1527,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_nodes_get(self, k8s_cluster_id, nodepool_id, **kwargs):  # noqa: E501
-        """List Kubernetes nodes  # noqa: E501
+        """Get Kubernetes Nodes  # noqa: E501
 
-        List all the nodes, included in the specified Kubernetes node pool.  # noqa: E501
+        Retrieves the list of all K8s nodes of the specified node pool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_get(k8s_cluster_id, nodepool_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1565,17 +1565,17 @@
                  returns the request thread.
         :rtype: KubernetesNodes
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_nodes_get_with_http_info(k8s_cluster_id, nodepool_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_nodes_get_with_http_info(self, k8s_cluster_id, nodepool_id, **kwargs):  # noqa: E501
-        """List Kubernetes nodes  # noqa: E501
+        """Get Kubernetes Nodes  # noqa: E501
 
-        List all the nodes, included in the specified Kubernetes node pool.  # noqa: E501
+        Retrieves the list of all K8s nodes of the specified node pool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_get_with_http_info(k8s_cluster_id, nodepool_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1700,17 +1700,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_nodes_replace_post(self, k8s_cluster_id, nodepool_id, node_id, **kwargs):  # noqa: E501
-        """Recreate Kubernetes nodes  # noqa: E501
+        """Recreate a Kubernetes Node by ID  # noqa: E501
 
-        Recreate the specified Kubernetes node.  A new node is created and configured by Managed Kubernetes, based on the node pool template. Once the status is  \"Active\", all the pods are migrated from the faulty node, which is then deleted once empty. During this operation, the node pool will have an additional billable  \"Active\" node.  # noqa: E501
+        Recreates the K8s node specified by its ID.  If a node becomes unusable, Managed Kubernetes allows you to recreate it with a configuration based on the node pool template. Once the status is 'Active,' all the pods from the failed node will be migrated to the new node. The node pool has an additional billable 'active' node during this process.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_replace_post(k8s_cluster_id, nodepool_id, node_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1740,17 +1740,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_nodes_replace_post_with_http_info(k8s_cluster_id, nodepool_id, node_id, **kwargs)  # noqa: E501
 
     def k8s_nodepools_nodes_replace_post_with_http_info(self, k8s_cluster_id, nodepool_id, node_id, **kwargs):  # noqa: E501
-        """Recreate Kubernetes nodes  # noqa: E501
+        """Recreate a Kubernetes Node by ID  # noqa: E501
 
-        Recreate the specified Kubernetes node.  A new node is created and configured by Managed Kubernetes, based on the node pool template. Once the status is  \"Active\", all the pods are migrated from the faulty node, which is then deleted once empty. During this operation, the node pool will have an additional billable  \"Active\" node.  # noqa: E501
+        Recreates the K8s node specified by its ID.  If a node becomes unusable, Managed Kubernetes allows you to recreate it with a configuration based on the node pool template. Once the status is 'Active,' all the pods from the failed node will be migrated to the new node. The node pool has an additional billable 'active' node during this process.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_nodes_replace_post_with_http_info(k8s_cluster_id, nodepool_id, node_id, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1884,17 +1884,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_post(self, k8s_cluster_id, kubernetes_node_pool, **kwargs):  # noqa: E501
-        """Create Kubernetes node pools  # noqa: E501
+        """Create a Kubernetes Node Pool  # noqa: E501
 
-        Create a Kubernetes node pool inside the specified Kubernetes cluster.  # noqa: E501
+        Creates a node pool inside the specified K8s cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_post(k8s_cluster_id, kubernetes_node_pool, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -1922,17 +1922,17 @@
                  returns the request thread.
         :rtype: KubernetesNodePool
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_post_with_http_info(k8s_cluster_id, kubernetes_node_pool, **kwargs)  # noqa: E501
 
     def k8s_nodepools_post_with_http_info(self, k8s_cluster_id, kubernetes_node_pool, **kwargs):  # noqa: E501
-        """Create Kubernetes node pools  # noqa: E501
+        """Create a Kubernetes Node Pool  # noqa: E501
 
-        Create a Kubernetes node pool inside the specified Kubernetes cluster.  # noqa: E501
+        Creates a node pool inside the specified K8s cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_post_with_http_info(k8s_cluster_id, kubernetes_node_pool, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -2061,17 +2061,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_nodepools_put(self, k8s_cluster_id, nodepool_id, kubernetes_node_pool, **kwargs):  # noqa: E501
-        """Modify Kubernetes node pools  # noqa: E501
+        """Modify a Kubernetes Node Pool by ID  # noqa: E501
 
-        Modify the specified Kubernetes node pool.  # noqa: E501
+        Modifies the K8s node pool specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_put(k8s_cluster_id, nodepool_id, kubernetes_node_pool, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -2101,17 +2101,17 @@
                  returns the request thread.
         :rtype: KubernetesNodePool
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_nodepools_put_with_http_info(k8s_cluster_id, nodepool_id, kubernetes_node_pool, **kwargs)  # noqa: E501
 
     def k8s_nodepools_put_with_http_info(self, k8s_cluster_id, nodepool_id, kubernetes_node_pool, **kwargs):  # noqa: E501
-        """Modify Kubernetes node pools  # noqa: E501
+        """Modify a Kubernetes Node Pool by ID  # noqa: E501
 
-        Modify the specified Kubernetes node pool.  # noqa: E501
+        Modifies the K8s node pool specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_nodepools_put_with_http_info(k8s_cluster_id, nodepool_id, kubernetes_node_pool, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -2249,17 +2249,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_post(self, kubernetes_cluster, **kwargs):  # noqa: E501
-        """Create Kubernetes clusters  # noqa: E501
+        """Create a Kubernetes Cluster  # noqa: E501
 
-        Create a Kubernetes cluster.  # noqa: E501
+        Creates a K8s cluster provisioned under your account.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_post(kubernetes_cluster, async_req=True)
         >>> result = thread.get()
 
         :param kubernetes_cluster: The Kubernetes cluster to create. (required)
@@ -2285,17 +2285,17 @@
                  returns the request thread.
         :rtype: KubernetesCluster
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_post_with_http_info(kubernetes_cluster, **kwargs)  # noqa: E501
 
     def k8s_post_with_http_info(self, kubernetes_cluster, **kwargs):  # noqa: E501
-        """Create Kubernetes clusters  # noqa: E501
+        """Create a Kubernetes Cluster  # noqa: E501
 
-        Create a Kubernetes cluster.  # noqa: E501
+        Creates a K8s cluster provisioned under your account.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_post_with_http_info(kubernetes_cluster, async_req=True)
         >>> result = thread.get()
 
         :param kubernetes_cluster: The Kubernetes cluster to create. (required)
@@ -2415,17 +2415,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_put(self, k8s_cluster_id, kubernetes_cluster, **kwargs):  # noqa: E501
-        """Modify Kubernetes clusters  # noqa: E501
+        """Modify a Kubernetes Cluster by ID  # noqa: E501
 
-        Modify the specified Kubernetes cluster.  # noqa: E501
+        Modifies the K8s cluster specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_put(k8s_cluster_id, kubernetes_cluster, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -2453,17 +2453,17 @@
                  returns the request thread.
         :rtype: KubernetesCluster
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_put_with_http_info(k8s_cluster_id, kubernetes_cluster, **kwargs)  # noqa: E501
 
     def k8s_put_with_http_info(self, k8s_cluster_id, kubernetes_cluster, **kwargs):  # noqa: E501
-        """Modify Kubernetes clusters  # noqa: E501
+        """Modify a Kubernetes Cluster by ID  # noqa: E501
 
-        Modify the specified Kubernetes cluster.  # noqa: E501
+        Modifies the K8s cluster specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_put_with_http_info(k8s_cluster_id, kubernetes_cluster, async_req=True)
         >>> result = thread.get()
 
         :param k8s_cluster_id: The unique ID of the Kubernetes cluster. (required)
@@ -2592,17 +2592,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_versions_default_get(self, **kwargs):  # noqa: E501
-        """Retrieve current default Kubernetes version  # noqa: E501
+        """Get Default Kubernetes Version  # noqa: E501
 
-        Retrieve current default Kubernetes version for clusters and nodepools.  # noqa: E501
+        Retrieves the current default K8s version to be used by the clusters and node pools.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_versions_default_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
@@ -2620,17 +2620,17 @@
                  returns the request thread.
         :rtype: str
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_versions_default_get_with_http_info(**kwargs)  # noqa: E501
 
     def k8s_versions_default_get_with_http_info(self, **kwargs):  # noqa: E501
-        """Retrieve current default Kubernetes version  # noqa: E501
+        """Get Default Kubernetes Version  # noqa: E501
 
-        Retrieve current default Kubernetes version for clusters and nodepools.  # noqa: E501
+        Retrieves the current default K8s version to be used by the clusters and node pools.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_versions_default_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
@@ -2718,17 +2718,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def k8s_versions_get(self, **kwargs):  # noqa: E501
-        """List Kubernetes versions  # noqa: E501
+        """Get Kubernetes Versions  # noqa: E501
 
-        List available Kubernetes versions.  # noqa: E501
+        Lists available K8s versions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_versions_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
@@ -2746,17 +2746,17 @@
                  returns the request thread.
         :rtype: list[str]
         """
         kwargs['_return_http_data_only'] = True
         return self.k8s_versions_get_with_http_info(**kwargs)  # noqa: E501
 
     def k8s_versions_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List Kubernetes versions  # noqa: E501
+        """Get Kubernetes Versions  # noqa: E501
 
-        List available Kubernetes versions.  # noqa: E501
+        Lists available K8s versions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.k8s_versions_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/labels_api.py` & `ionoscloud-6.1.5/ionoscloud/api/labels_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,17 +522,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_labels_post(self, datacenter_id, label, **kwargs):  # noqa: E501
-        """Create data center labels  # noqa: E501
+        """Create a Data Center Label  # noqa: E501
 
-        Add a new label to the specified data center.  # noqa: E501
+        Adds a new label to the specified data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_labels_post(datacenter_id, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -560,17 +560,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_labels_post_with_http_info(datacenter_id, label, **kwargs)  # noqa: E501
 
     def datacenters_labels_post_with_http_info(self, datacenter_id, label, **kwargs):  # noqa: E501
-        """Create data center labels  # noqa: E501
+        """Create a Data Center Label  # noqa: E501
 
-        Add a new label to the specified data center.  # noqa: E501
+        Adds a new label to the specified data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_labels_post_with_http_info(datacenter_id, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -699,17 +699,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_labels_put(self, datacenter_id, key, label, **kwargs):  # noqa: E501
-        """Modify data center labels  # noqa: E501
+        """Modify a Data Center Label by Key  # noqa: E501
 
-        Modify the specified data center label.  # noqa: E501
+        Modifies the specified data center label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_labels_put(datacenter_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -739,17 +739,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_labels_put_with_http_info(datacenter_id, key, label, **kwargs)  # noqa: E501
 
     def datacenters_labels_put_with_http_info(self, datacenter_id, key, label, **kwargs):  # noqa: E501
-        """Modify data center labels  # noqa: E501
+        """Modify a Data Center Label by Key  # noqa: E501
 
-        Modify the specified data center label.  # noqa: E501
+        Modifies the specified data center label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_labels_put_with_http_info(datacenter_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1428,17 +1428,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_labels_post(self, datacenter_id, server_id, label, **kwargs):  # noqa: E501
-        """Create server labels  # noqa: E501
+        """Create a Server Label  # noqa: E501
 
-        Add a new label to the specified server.  # noqa: E501
+        Adds a new label to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_labels_post(datacenter_id, server_id, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1468,17 +1468,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_labels_post_with_http_info(datacenter_id, server_id, label, **kwargs)  # noqa: E501
 
     def datacenters_servers_labels_post_with_http_info(self, datacenter_id, server_id, label, **kwargs):  # noqa: E501
-        """Create server labels  # noqa: E501
+        """Create a Server Label  # noqa: E501
 
-        Add a new label to the specified server.  # noqa: E501
+        Adds a new label to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_labels_post_with_http_info(datacenter_id, server_id, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1616,17 +1616,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_labels_put(self, datacenter_id, server_id, key, label, **kwargs):  # noqa: E501
-        """Modify server labels  # noqa: E501
+        """Modify a Server Label  # noqa: E501
 
-        Modify the specified server label.  # noqa: E501
+        Modifies the specified server label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_labels_put(datacenter_id, server_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1658,17 +1658,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_labels_put_with_http_info(datacenter_id, server_id, key, label, **kwargs)  # noqa: E501
 
     def datacenters_servers_labels_put_with_http_info(self, datacenter_id, server_id, key, label, **kwargs):  # noqa: E501
-        """Modify server labels  # noqa: E501
+        """Modify a Server Label  # noqa: E501
 
-        Modify the specified server label.  # noqa: E501
+        Modifies the specified server label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_labels_put_with_http_info(datacenter_id, server_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2356,17 +2356,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_volumes_labels_post(self, datacenter_id, volume_id, label, **kwargs):  # noqa: E501
-        """Create volume labels  # noqa: E501
+        """Create a Volume Label  # noqa: E501
 
-        Add a new label to the specified volume.  # noqa: E501
+        Adds a new label to the specified volume.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_labels_post(datacenter_id, volume_id, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2396,17 +2396,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_volumes_labels_post_with_http_info(datacenter_id, volume_id, label, **kwargs)  # noqa: E501
 
     def datacenters_volumes_labels_post_with_http_info(self, datacenter_id, volume_id, label, **kwargs):  # noqa: E501
-        """Create volume labels  # noqa: E501
+        """Create a Volume Label  # noqa: E501
 
-        Add a new label to the specified volume.  # noqa: E501
+        Adds a new label to the specified volume.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_labels_post_with_http_info(datacenter_id, volume_id, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2544,17 +2544,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_volumes_labels_put(self, datacenter_id, volume_id, key, label, **kwargs):  # noqa: E501
-        """Modify volume labels  # noqa: E501
+        """Modify a Volume Label  # noqa: E501
 
-        Modify the specified volume label.  # noqa: E501
+        Modifies the specified volume label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_labels_put(datacenter_id, volume_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2586,17 +2586,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_volumes_labels_put_with_http_info(datacenter_id, volume_id, key, label, **kwargs)  # noqa: E501
 
     def datacenters_volumes_labels_put_with_http_info(self, datacenter_id, volume_id, key, label, **kwargs):  # noqa: E501
-        """Modify volume labels  # noqa: E501
+        """Modify a Volume Label  # noqa: E501
 
-        Modify the specified volume label.  # noqa: E501
+        Modifies the specified volume label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_labels_put_with_http_info(datacenter_id, volume_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3428,17 +3428,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def ipblocks_labels_put(self, ipblock_id, key, label, **kwargs):  # noqa: E501
-        """Modify IP block labels  # noqa: E501
+        """Modify a IP Block Label by ID  # noqa: E501
 
-        Modify the specified IP block label.  # noqa: E501
+        Modifies the specified IP block label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.ipblocks_labels_put(ipblock_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param ipblock_id: The unique ID of the IP block. (required)
@@ -3468,17 +3468,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.ipblocks_labels_put_with_http_info(ipblock_id, key, label, **kwargs)  # noqa: E501
 
     def ipblocks_labels_put_with_http_info(self, ipblock_id, key, label, **kwargs):  # noqa: E501
-        """Modify IP block labels  # noqa: E501
+        """Modify a IP Block Label by ID  # noqa: E501
 
-        Modify the specified IP block label.  # noqa: E501
+        Modifies the specified IP block label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.ipblocks_labels_put_with_http_info(ipblock_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param ipblock_id: The unique ID of the IP block. (required)
@@ -4437,17 +4437,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def snapshots_labels_post(self, snapshot_id, label, **kwargs):  # noqa: E501
-        """Create snapshot labels  # noqa: E501
+        """Create a Snapshot Label  # noqa: E501
 
-        Add a new label to the specified snapshot.  # noqa: E501
+        Adds a new label to the specified snapshot.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.snapshots_labels_post(snapshot_id, label, async_req=True)
         >>> result = thread.get()
 
         :param snapshot_id: The unique ID of the snapshot. (required)
@@ -4475,17 +4475,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.snapshots_labels_post_with_http_info(snapshot_id, label, **kwargs)  # noqa: E501
 
     def snapshots_labels_post_with_http_info(self, snapshot_id, label, **kwargs):  # noqa: E501
-        """Create snapshot labels  # noqa: E501
+        """Create a Snapshot Label  # noqa: E501
 
-        Add a new label to the specified snapshot.  # noqa: E501
+        Adds a new label to the specified snapshot.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.snapshots_labels_post_with_http_info(snapshot_id, label, async_req=True)
         >>> result = thread.get()
 
         :param snapshot_id: The unique ID of the snapshot. (required)
@@ -4614,17 +4614,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def snapshots_labels_put(self, snapshot_id, key, label, **kwargs):  # noqa: E501
-        """Modify snapshot labels  # noqa: E501
+        """Modify a Snapshot Label by ID  # noqa: E501
 
-        Modify the specified snapshot label.  # noqa: E501
+        Modifies the specified snapshot label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.snapshots_labels_put(snapshot_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param snapshot_id: The unique ID of the snapshot. (required)
@@ -4654,17 +4654,17 @@
                  returns the request thread.
         :rtype: LabelResource
         """
         kwargs['_return_http_data_only'] = True
         return self.snapshots_labels_put_with_http_info(snapshot_id, key, label, **kwargs)  # noqa: E501
 
     def snapshots_labels_put_with_http_info(self, snapshot_id, key, label, **kwargs):  # noqa: E501
-        """Modify snapshot labels  # noqa: E501
+        """Modify a Snapshot Label by ID  # noqa: E501
 
-        Modify the specified snapshot label.  # noqa: E501
+        Modifies the specified snapshot label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.snapshots_labels_put_with_http_info(snapshot_id, key, label, async_req=True)
         >>> result = thread.get()
 
         :param snapshot_id: The unique ID of the snapshot. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/lans_api.py` & `ionoscloud-6.1.5/ionoscloud/api/lans_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,176 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def datacenters_lans_enable_ipv6(self, datacenter_id, **kwargs):  # noqa: E501
+        """Enable IPv6 in the current Virtual Datacenter  # noqa: E501
+
+        Enable IPv6 for all NICs in the current Virtual Datacenter.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.datacenters_lans_enable_ipv6(datacenter_id, async_req=True)
+        >>> result = thread.get()
+
+        :param datacenter_id: The unique ID of the data center. (required)
+        :type datacenter_id: str
+        :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
+        :type pretty: bool
+        :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
+        :type depth: int
+        :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
+        :type x_contract_number: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.datacenters_lans_enable_ipv6_with_http_info(datacenter_id, **kwargs)  # noqa: E501
+
+    def datacenters_lans_enable_ipv6_with_http_info(self, datacenter_id, **kwargs):  # noqa: E501
+        """Enable IPv6 in the current Virtual Datacenter  # noqa: E501
+
+        Enable IPv6 for all NICs in the current Virtual Datacenter.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.datacenters_lans_enable_ipv6_with_http_info(datacenter_id, async_req=True)
+        >>> result = thread.get()
+
+        :param datacenter_id: The unique ID of the data center. (required)
+        :type datacenter_id: str
+        :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
+        :type pretty: bool
+        :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
+        :type depth: int
+        :param x_contract_number: Users with multiple contracts must provide the contract number, for which all API requests are to be executed.
+        :type x_contract_number: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'datacenter_id',
+            'pretty',
+            'depth',
+            'x_contract_number'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                'response_type',
+                'query_params'
+            ]
+        )
+
+        for local_var_params_key, local_var_params_val in six.iteritems(local_var_params['kwargs']):
+            if local_var_params_key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method datacenters_lans_enable_ipv6" % local_var_params_key
+                )
+            local_var_params[local_var_params_key] = local_var_params_val
+        del local_var_params['kwargs']
+        # verify the required parameter 'datacenter_id' is set
+        if self.api_client.client_side_validation and ('datacenter_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['datacenter_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `datacenter_id` when calling `datacenters_lans_enable_ipv6`")  # noqa: E501
+
+        if self.api_client.client_side_validation and 'depth' in local_var_params and local_var_params['depth'] > 10:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `depth` when calling `datacenters_lans_enable_ipv6`, must be a value less than or equal to `10`")  # noqa: E501
+        if self.api_client.client_side_validation and 'depth' in local_var_params and local_var_params['depth'] < 0:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `depth` when calling `datacenters_lans_enable_ipv6`, must be a value greater than or equal to `0`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'datacenter_id' in local_var_params:
+            path_params['datacenterId'] = local_var_params['datacenter_id']  # noqa: E501
+
+        query_params = list(local_var_params.get('query_params', {}).items())
+        if 'pretty' in local_var_params and local_var_params['pretty'] is not None:  # noqa: E501
+            query_params.append(('pretty', local_var_params['pretty']))  # noqa: E501
+        if 'depth' in local_var_params and local_var_params['depth'] is not None:  # noqa: E501
+            query_params.append(('depth', local_var_params['depth']))  # noqa: E501
+
+        header_params = {}
+        if 'x_contract_number' in local_var_params:
+            header_params['X-Contract-Number'] = local_var_params['x_contract_number']  # noqa: E501
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['*/*'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['Basic Authentication', 'Token Authentication']  # noqa: E501
+
+        response_type = None
+        if 'response_type' in kwargs:
+            response_type = kwargs['response_type']
+
+        return self.api_client.call_api(
+            '/datacenters/{datacenterId}/lans/enable-ipv6', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=response_type,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def datacenters_lans_find_by_id(self, datacenter_id, lan_id, **kwargs):  # noqa: E501
         """Retrieve LANs  # noqa: E501
 
         Retrieve the properties of the specified LAN within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -1297,15 +1459,15 @@
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_lans_post(self, datacenter_id, lan, **kwargs):  # noqa: E501
         """Create LANs  # noqa: E501
 
-        Create a LAN within the data center.  # noqa: E501
+        Creates a LAN within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_lans_post(datacenter_id, lan, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1335,15 +1497,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_lans_post_with_http_info(datacenter_id, lan, **kwargs)  # noqa: E501
 
     def datacenters_lans_post_with_http_info(self, datacenter_id, lan, **kwargs):  # noqa: E501
         """Create LANs  # noqa: E501
 
-        Create a LAN within the data center.  # noqa: E501
+        Creates a LAN within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_lans_post_with_http_info(datacenter_id, lan, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/load_balancers_api.py` & `ionoscloud-6.1.5/ionoscloud/api/load_balancers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_loadbalancers_balancednics_post(self, datacenter_id, loadbalancer_id, nic, **kwargs):  # noqa: E501
         """Attach balanced NICs  # noqa: E501
 
-        Attach an existing NIC to the specified Load Balancer.  # noqa: E501
+        Attachs an existing NIC to the specified Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_loadbalancers_balancednics_post(datacenter_id, loadbalancer_id, nic, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -597,15 +597,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_loadbalancers_balancednics_post_with_http_info(datacenter_id, loadbalancer_id, nic, **kwargs)  # noqa: E501
 
     def datacenters_loadbalancers_balancednics_post_with_http_info(self, datacenter_id, loadbalancer_id, nic, **kwargs):  # noqa: E501
         """Attach balanced NICs  # noqa: E501
 
-        Attach an existing NIC to the specified Load Balancer.  # noqa: E501
+        Attachs an existing NIC to the specified Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_loadbalancers_balancednics_post_with_http_info(datacenter_id, loadbalancer_id, nic, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1459,17 +1459,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_loadbalancers_post(self, datacenter_id, loadbalancer, **kwargs):  # noqa: E501
-        """Create Load Balancers  # noqa: E501
+        """Create a Load Balancer  # noqa: E501
 
-        Create a Load Balancer within the data center.  # noqa: E501
+        Creates a Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_loadbalancers_post(datacenter_id, loadbalancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1497,17 +1497,17 @@
                  returns the request thread.
         :rtype: Loadbalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_loadbalancers_post_with_http_info(datacenter_id, loadbalancer, **kwargs)  # noqa: E501
 
     def datacenters_loadbalancers_post_with_http_info(self, datacenter_id, loadbalancer, **kwargs):  # noqa: E501
-        """Create Load Balancers  # noqa: E501
+        """Create a Load Balancer  # noqa: E501
 
-        Create a Load Balancer within the data center.  # noqa: E501
+        Creates a Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_loadbalancers_post_with_http_info(datacenter_id, loadbalancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1636,17 +1636,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_loadbalancers_put(self, datacenter_id, loadbalancer_id, loadbalancer, **kwargs):  # noqa: E501
-        """Modify Load Balancers  # noqa: E501
+        """Modify a Load Balancer by ID  # noqa: E501
 
-        Modify the properties of the specified Load Balancer within the data center.  # noqa: E501
+        Modifies the properties of the specified Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_loadbalancers_put(datacenter_id, loadbalancer_id, loadbalancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1676,17 +1676,17 @@
                  returns the request thread.
         :rtype: Loadbalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_loadbalancers_put_with_http_info(datacenter_id, loadbalancer_id, loadbalancer, **kwargs)  # noqa: E501
 
     def datacenters_loadbalancers_put_with_http_info(self, datacenter_id, loadbalancer_id, loadbalancer, **kwargs):  # noqa: E501
-        """Modify Load Balancers  # noqa: E501
+        """Modify a Load Balancer by ID  # noqa: E501
 
-        Modify the properties of the specified Load Balancer within the data center.  # noqa: E501
+        Modifies the properties of the specified Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_loadbalancers_put_with_http_info(datacenter_id, loadbalancer_id, loadbalancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/locations_api.py` & `ionoscloud-6.1.5/ionoscloud/api/locations_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def locations_find_by_region_id(self, region_id, **kwargs):  # noqa: E501
-        """List locations within regions  # noqa: E501
+        """Get Locations within a Region  # noqa: E501
 
-        List locations by the region ID.  # noqa: E501
+        Retrieves the available locations in a region specified by its ID. The 'regionId' consists of the two character identifier of the region (country), e.g., 'de'.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.locations_find_by_region_id(region_id, async_req=True)
         >>> result = thread.get()
 
         :param region_id: The unique ID of the region. (required)
@@ -50,17 +50,17 @@
                  returns the request thread.
         :rtype: Locations
         """
         kwargs['_return_http_data_only'] = True
         return self.locations_find_by_region_id_with_http_info(region_id, **kwargs)  # noqa: E501
 
     def locations_find_by_region_id_with_http_info(self, region_id, **kwargs):  # noqa: E501
-        """List locations within regions  # noqa: E501
+        """Get Locations within a Region  # noqa: E501
 
-        List locations by the region ID.  # noqa: E501
+        Retrieves the available locations in a region specified by its ID. The 'regionId' consists of the two character identifier of the region (country), e.g., 'de'.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.locations_find_by_region_id_with_http_info(region_id, async_req=True)
         >>> result = thread.get()
 
         :param region_id: The unique ID of the region. (required)
@@ -176,17 +176,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def locations_find_by_region_id_and_id(self, region_id, location_id, **kwargs):  # noqa: E501
-        """Retrieve specified locations  # noqa: E501
+        """Get Location by ID  # noqa: E501
 
-        Retrieve the properties of the specified location  # noqa: E501
+        Retrieves the information about the location specified by its ID. The 'locationId' consists of the three-digit identifier of the city according to the IATA code.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.locations_find_by_region_id_and_id(region_id, location_id, async_req=True)
         >>> result = thread.get()
 
         :param region_id: The unique ID of the region. (required)
@@ -214,17 +214,17 @@
                  returns the request thread.
         :rtype: Location
         """
         kwargs['_return_http_data_only'] = True
         return self.locations_find_by_region_id_and_id_with_http_info(region_id, location_id, **kwargs)  # noqa: E501
 
     def locations_find_by_region_id_and_id_with_http_info(self, region_id, location_id, **kwargs):  # noqa: E501
-        """Retrieve specified locations  # noqa: E501
+        """Get Location by ID  # noqa: E501
 
-        Retrieve the properties of the specified location  # noqa: E501
+        Retrieves the information about the location specified by its ID. The 'locationId' consists of the three-digit identifier of the city according to the IATA code.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.locations_find_by_region_id_and_id_with_http_info(region_id, location_id, async_req=True)
         >>> result = thread.get()
 
         :param region_id: The unique ID of the region. (required)
@@ -349,17 +349,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def locations_get(self, **kwargs):  # noqa: E501
-        """List locations  # noqa: E501
+        """Get Locations  # noqa: E501
 
-        List the available locations for provisioning your virtual data centers.  # noqa: E501
+        Retrieves the available physical locations where you can deploy cloud resources in a VDC.    A location is identified by a combination of the following characters:    * a two-character **regionId**, which represents a country (example: 'de')    * a three-character **locationId**, which represents a city. The 'locationId' is typically based on the IATA code of the city's airport (example: 'txl').    >Note that 'locations' are read-only and cannot be changed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.locations_get(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -383,17 +383,17 @@
                  returns the request thread.
         :rtype: Locations
         """
         kwargs['_return_http_data_only'] = True
         return self.locations_get_with_http_info(**kwargs)  # noqa: E501
 
     def locations_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List locations  # noqa: E501
+        """Get Locations  # noqa: E501
 
-        List the available locations for provisioning your virtual data centers.  # noqa: E501
+        Retrieves the available physical locations where you can deploy cloud resources in a VDC.    A location is identified by a combination of the following characters:    * a two-character **regionId**, which represents a country (example: 'de')    * a three-character **locationId**, which represents a city. The 'locationId' is typically based on the IATA code of the city's airport (example: 'txl').    >Note that 'locations' are read-only and cannot be changed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.locations_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/nat_gateways_api.py` & `ionoscloud-6.1.5/ionoscloud/api/nat_gateways_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1088,17 +1088,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_natgateways_flowlogs_post(self, datacenter_id, nat_gateway_id, nat_gateway_flow_log, **kwargs):  # noqa: E501
-        """Create NAT Gateway Flow Logs  # noqa: E501
+        """Create a NAT Gateway Flow Log  # noqa: E501
 
-        Add a new Flow Log for the specified NAT Gateway.  # noqa: E501
+        Adds a new Flow Log to the specified NAT Gateway.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_flowlogs_post(datacenter_id, nat_gateway_id, nat_gateway_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1126,17 +1126,17 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_natgateways_flowlogs_post_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_flow_log, **kwargs)  # noqa: E501
 
     def datacenters_natgateways_flowlogs_post_with_http_info(self, datacenter_id, nat_gateway_id, nat_gateway_flow_log, **kwargs):  # noqa: E501
-        """Create NAT Gateway Flow Logs  # noqa: E501
+        """Create a NAT Gateway Flow Log  # noqa: E501
 
-        Add a new Flow Log for the specified NAT Gateway.  # noqa: E501
+        Adds a new Flow Log to the specified NAT Gateway.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_flowlogs_post_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1807,17 +1807,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_natgateways_post(self, datacenter_id, nat_gateway, **kwargs):  # noqa: E501
-        """Create NAT Gateways  # noqa: E501
+        """Create a NAT Gateway  # noqa: E501
 
-        Create a NAT Gateway within the data center.  This operation is restricted to contract owner, admin, and users with 'createInternetAccess' privileges.  # noqa: E501
+        Creates a NAT Gateway within the data center.  This operation is restricted to contract owner, admin, and users with 'createInternetAccess' privileges.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_post(datacenter_id, nat_gateway, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1845,17 +1845,17 @@
                  returns the request thread.
         :rtype: NatGateway
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_natgateways_post_with_http_info(datacenter_id, nat_gateway, **kwargs)  # noqa: E501
 
     def datacenters_natgateways_post_with_http_info(self, datacenter_id, nat_gateway, **kwargs):  # noqa: E501
-        """Create NAT Gateways  # noqa: E501
+        """Create a NAT Gateway  # noqa: E501
 
-        Create a NAT Gateway within the data center.  This operation is restricted to contract owner, admin, and users with 'createInternetAccess' privileges.  # noqa: E501
+        Creates a NAT Gateway within the data center.  This operation is restricted to contract owner, admin, and users with 'createInternetAccess' privileges.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_post_with_http_info(datacenter_id, nat_gateway, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2713,17 +2713,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_natgateways_rules_patch(self, datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule_properties, **kwargs):  # noqa: E501
-        """Partially modify NAT Gateway rules  # noqa: E501
+        """Partially Modify a NAT Gateway Rule by ID  # noqa: E501
 
-        Update the properties of the specified NAT Gateway rule.  # noqa: E501
+        Updates the properties of the specified NAT Gateway rule.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_rules_patch(datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2755,17 +2755,17 @@
                  returns the request thread.
         :rtype: NatGatewayRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_natgateways_rules_patch_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule_properties, **kwargs)  # noqa: E501
 
     def datacenters_natgateways_rules_patch_with_http_info(self, datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule_properties, **kwargs):  # noqa: E501
-        """Partially modify NAT Gateway rules  # noqa: E501
+        """Partially Modify a NAT Gateway Rule by ID  # noqa: E501
 
-        Update the properties of the specified NAT Gateway rule.  # noqa: E501
+        Updates the properties of the specified NAT Gateway rule.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_rules_patch_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule_properties, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2908,17 +2908,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_natgateways_rules_post(self, datacenter_id, nat_gateway_id, nat_gateway_rule, **kwargs):  # noqa: E501
-        """Create NAT Gateway rules  # noqa: E501
+        """Create a NAT Gateway Rule  # noqa: E501
 
-        Create a rule for the specified NAT Gateway.  # noqa: E501
+        Creates a rule for the specified NAT Gateway.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_rules_post(datacenter_id, nat_gateway_id, nat_gateway_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2948,17 +2948,17 @@
                  returns the request thread.
         :rtype: NatGatewayRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_natgateways_rules_post_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_rule, **kwargs)  # noqa: E501
 
     def datacenters_natgateways_rules_post_with_http_info(self, datacenter_id, nat_gateway_id, nat_gateway_rule, **kwargs):  # noqa: E501
-        """Create NAT Gateway rules  # noqa: E501
+        """Create a NAT Gateway Rule  # noqa: E501
 
-        Create a rule for the specified NAT Gateway.  # noqa: E501
+        Creates a rule for the specified NAT Gateway.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_rules_post_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3096,15 +3096,15 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_natgateways_rules_put(self, datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule, **kwargs):  # noqa: E501
-        """Modify NAT Gateway rules  # noqa: E501
+        """Modify a NAT Gateway Rule by ID  # noqa: E501
 
         Modify the specified NAT Gateway rule.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_rules_put(datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule, async_req=True)
         >>> result = thread.get()
@@ -3138,15 +3138,15 @@
                  returns the request thread.
         :rtype: NatGatewayRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_natgateways_rules_put_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule, **kwargs)  # noqa: E501
 
     def datacenters_natgateways_rules_put_with_http_info(self, datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule, **kwargs):  # noqa: E501
-        """Modify NAT Gateway rules  # noqa: E501
+        """Modify a NAT Gateway Rule by ID  # noqa: E501
 
         Modify the specified NAT Gateway rule.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_natgateways_rules_put_with_http_info(datacenter_id, nat_gateway_id, nat_gateway_rule_id, nat_gateway_rule, async_req=True)
         >>> result = thread.get()
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/network_interfaces_api.py` & `ionoscloud-6.1.5/ionoscloud/api/network_interfaces_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,17 +774,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_nics_post(self, datacenter_id, server_id, nic, **kwargs):  # noqa: E501
-        """Create NICs  # noqa: E501
+        """Create a NIC  # noqa: E501
 
-        Add a NIC to the specified server. The combined total of NICs and attached volumes cannot exceed 24 per server.  # noqa: E501
+        Adds a NIC to the specified server. The combined total of NICs and attached volumes cannot exceed 24 per server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_post(datacenter_id, server_id, nic, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -814,17 +814,17 @@
                  returns the request thread.
         :rtype: Nic
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_nics_post_with_http_info(datacenter_id, server_id, nic, **kwargs)  # noqa: E501
 
     def datacenters_servers_nics_post_with_http_info(self, datacenter_id, server_id, nic, **kwargs):  # noqa: E501
-        """Create NICs  # noqa: E501
+        """Create a NIC  # noqa: E501
 
-        Add a NIC to the specified server. The combined total of NICs and attached volumes cannot exceed 24 per server.  # noqa: E501
+        Adds a NIC to the specified server. The combined total of NICs and attached volumes cannot exceed 24 per server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_nics_post_with_http_info(datacenter_id, server_id, nic, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/network_load_balancers_api.py` & `ionoscloud-6.1.5/ionoscloud/api/network_load_balancers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1096,17 +1096,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_networkloadbalancers_flowlogs_post(self, datacenter_id, network_load_balancer_id, network_load_balancer_flow_log, **kwargs):  # noqa: E501
-        """Create NLB Flow Logs  # noqa: E501
+        """Create a NLB Flow Log  # noqa: E501
 
-        Add a new Flow Log for the Network Load Balancer.  # noqa: E501
+        Adds a new Flow Log for the Network Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_networkloadbalancers_flowlogs_post(datacenter_id, network_load_balancer_id, network_load_balancer_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1136,17 +1136,17 @@
                  returns the request thread.
         :rtype: FlowLog
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_networkloadbalancers_flowlogs_post_with_http_info(datacenter_id, network_load_balancer_id, network_load_balancer_flow_log, **kwargs)  # noqa: E501
 
     def datacenters_networkloadbalancers_flowlogs_post_with_http_info(self, datacenter_id, network_load_balancer_id, network_load_balancer_flow_log, **kwargs):  # noqa: E501
-        """Create NLB Flow Logs  # noqa: E501
+        """Create a NLB Flow Log  # noqa: E501
 
-        Add a new Flow Log for the Network Load Balancer.  # noqa: E501
+        Adds a new Flow Log for the Network Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_networkloadbalancers_flowlogs_post_with_http_info(datacenter_id, network_load_balancer_id, network_load_balancer_flow_log, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2219,17 +2219,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_networkloadbalancers_forwardingrules_post(self, datacenter_id, network_load_balancer_id, network_load_balancer_forwarding_rule, **kwargs):  # noqa: E501
-        """Create NLB forwarding rules  # noqa: E501
+        """Create a NLB Forwarding Rule  # noqa: E501
 
-        Create a forwarding rule for the specified Network Load Balancer.  # noqa: E501
+        Creates a forwarding rule for the specified Network Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_networkloadbalancers_forwardingrules_post(datacenter_id, network_load_balancer_id, network_load_balancer_forwarding_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2259,17 +2259,17 @@
                  returns the request thread.
         :rtype: NetworkLoadBalancerForwardingRule
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_networkloadbalancers_forwardingrules_post_with_http_info(datacenter_id, network_load_balancer_id, network_load_balancer_forwarding_rule, **kwargs)  # noqa: E501
 
     def datacenters_networkloadbalancers_forwardingrules_post_with_http_info(self, datacenter_id, network_load_balancer_id, network_load_balancer_forwarding_rule, **kwargs):  # noqa: E501
-        """Create NLB forwarding rules  # noqa: E501
+        """Create a NLB Forwarding Rule  # noqa: E501
 
-        Create a forwarding rule for the specified Network Load Balancer.  # noqa: E501
+        Creates a forwarding rule for the specified Network Load Balancer.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_networkloadbalancers_forwardingrules_post_with_http_info(datacenter_id, network_load_balancer_id, network_load_balancer_forwarding_rule, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2972,17 +2972,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_networkloadbalancers_post(self, datacenter_id, network_load_balancer, **kwargs):  # noqa: E501
-        """Create Network Load Balancers  # noqa: E501
+        """Create a Network Load Balancer  # noqa: E501
 
-        Create a Network Load Balancer within the data center.  # noqa: E501
+        Creates a Network Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_networkloadbalancers_post(datacenter_id, network_load_balancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3010,17 +3010,17 @@
                  returns the request thread.
         :rtype: NetworkLoadBalancer
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_networkloadbalancers_post_with_http_info(datacenter_id, network_load_balancer, **kwargs)  # noqa: E501
 
     def datacenters_networkloadbalancers_post_with_http_info(self, datacenter_id, network_load_balancer, **kwargs):  # noqa: E501
-        """Create Network Load Balancers  # noqa: E501
+        """Create a Network Load Balancer  # noqa: E501
 
-        Create a Network Load Balancer within the data center.  # noqa: E501
+        Creates a Network Load Balancer within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_networkloadbalancers_post_with_http_info(datacenter_id, network_load_balancer, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/private_cross_connects_api.py` & `ionoscloud-6.1.5/ionoscloud/api/private_cross_connects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,17 +666,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def pccs_post(self, pcc, **kwargs):  # noqa: E501
-        """Create private Cross-Connects  # noqa: E501
+        """Create a Private Cross-Connect  # noqa: E501
 
-        Create a private Cross-Connect.  # noqa: E501
+        Creates a private Cross-Connect.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.pccs_post(pcc, async_req=True)
         >>> result = thread.get()
 
         :param pcc: The private Cross-Connect to create. (required)
@@ -702,17 +702,17 @@
                  returns the request thread.
         :rtype: PrivateCrossConnect
         """
         kwargs['_return_http_data_only'] = True
         return self.pccs_post_with_http_info(pcc, **kwargs)  # noqa: E501
 
     def pccs_post_with_http_info(self, pcc, **kwargs):  # noqa: E501
-        """Create private Cross-Connects  # noqa: E501
+        """Create a Private Cross-Connect  # noqa: E501
 
-        Create a private Cross-Connect.  # noqa: E501
+        Creates a private Cross-Connect.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.pccs_post_with_http_info(pcc, async_req=True)
         >>> result = thread.get()
 
         :param pcc: The private Cross-Connect to create. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/requests_api.py` & `ionoscloud-6.1.5/ionoscloud/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/api/servers_api.py` & `ionoscloud-6.1.5/ionoscloud/api/servers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def datacenters_servers_cdroms_delete(self, datacenter_id, server_id, cdrom_id, **kwargs):  # noqa: E501
-        """Detach CD-ROMs  # noqa: E501
+        """Detach a CD-ROM by ID  # noqa: E501
 
-        Detach the specified CD-ROM from the server.  # noqa: E501
+        Detachs the specified CD-ROM from the server.  Detaching a CD-ROM deletes the CD-ROM. The image will not be deleted.  Note that detaching a CD-ROM leads to a reset of the server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_delete(datacenter_id, server_id, cdrom_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -54,17 +54,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_cdroms_delete_with_http_info(datacenter_id, server_id, cdrom_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_cdroms_delete_with_http_info(self, datacenter_id, server_id, cdrom_id, **kwargs):  # noqa: E501
-        """Detach CD-ROMs  # noqa: E501
+        """Detach a CD-ROM by ID  # noqa: E501
 
-        Detach the specified CD-ROM from the server.  # noqa: E501
+        Detachs the specified CD-ROM from the server.  Detaching a CD-ROM deletes the CD-ROM. The image will not be deleted.  Note that detaching a CD-ROM leads to a reset of the server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_delete_with_http_info(datacenter_id, server_id, cdrom_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -198,17 +198,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_cdroms_find_by_id(self, datacenter_id, server_id, cdrom_id, **kwargs):  # noqa: E501
-        """Retrieve attached CD-ROMs  # noqa: E501
+        """Get Attached CD-ROM by ID  # noqa: E501
 
-        Retrieve the properties of the CD-ROM, attached to the specified server.  # noqa: E501
+        Retrieves the properties of the CD-ROM attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_find_by_id(datacenter_id, server_id, cdrom_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -238,17 +238,17 @@
                  returns the request thread.
         :rtype: Image
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_cdroms_find_by_id_with_http_info(datacenter_id, server_id, cdrom_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_cdroms_find_by_id_with_http_info(self, datacenter_id, server_id, cdrom_id, **kwargs):  # noqa: E501
-        """Retrieve attached CD-ROMs  # noqa: E501
+        """Get Attached CD-ROM by ID  # noqa: E501
 
-        Retrieve the properties of the CD-ROM, attached to the specified server.  # noqa: E501
+        Retrieves the properties of the CD-ROM attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_find_by_id_with_http_info(datacenter_id, server_id, cdrom_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -382,17 +382,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_cdroms_get(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """List attached CD-ROMs   # noqa: E501
+        """Get Attached CD-ROMs   # noqa: E501
 
-        List all CD-ROMs, attached to the specified server.  # noqa: E501
+        Lists all CD-ROMs attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_get(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -424,17 +424,17 @@
                  returns the request thread.
         :rtype: Cdroms
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_cdroms_get_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_cdroms_get_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """List attached CD-ROMs   # noqa: E501
+        """Get Attached CD-ROMs   # noqa: E501
 
-        List all CD-ROMs, attached to the specified server.  # noqa: E501
+        Lists all CD-ROMs attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_get_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -575,17 +575,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_cdroms_post(self, datacenter_id, server_id, cdrom, **kwargs):  # noqa: E501
-        """Attach CD-ROMs  # noqa: E501
+        """Attach a CD-ROM  # noqa: E501
 
-        Attach a CD-ROM to an existing server. Up to two CD-ROMs can be attached to the same server.   # noqa: E501
+        Attachs a CD-ROM to an existing server specified by its ID.   CD-ROMs cannot be created stand-alone like volumes. They are either attached to a server or do not exist. They always have an ISO-Image associated; empty CD-ROMs can not be provisioned. It is possible to attach up to two CD-ROMs to the same server.   Note that attaching a CD-ROM leads to a reset of the server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_post(datacenter_id, server_id, cdrom, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -615,17 +615,17 @@
                  returns the request thread.
         :rtype: Image
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_cdroms_post_with_http_info(datacenter_id, server_id, cdrom, **kwargs)  # noqa: E501
 
     def datacenters_servers_cdroms_post_with_http_info(self, datacenter_id, server_id, cdrom, **kwargs):  # noqa: E501
-        """Attach CD-ROMs  # noqa: E501
+        """Attach a CD-ROM  # noqa: E501
 
-        Attach a CD-ROM to an existing server. Up to two CD-ROMs can be attached to the same server.   # noqa: E501
+        Attachs a CD-ROM to an existing server specified by its ID.   CD-ROMs cannot be created stand-alone like volumes. They are either attached to a server or do not exist. They always have an ISO-Image associated; empty CD-ROMs can not be provisioned. It is possible to attach up to two CD-ROMs to the same server.   Note that attaching a CD-ROM leads to a reset of the server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_cdroms_post_with_http_info(datacenter_id, server_id, cdrom, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -765,15 +765,15 @@
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_delete(self, datacenter_id, server_id, **kwargs):  # noqa: E501
         """Delete servers  # noqa: E501
 
-        Delete the specified server in your data center. The attached storage volumes will not be removed — a separate API call must be made for these actions.  # noqa: E501
+        Delete the specified server in your data center. The attached storage volumes will also be removed if the query parameter is set to true otherwise a separate API call must be made for these actions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_delete(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -805,15 +805,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_delete_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_delete_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
         """Delete servers  # noqa: E501
 
-        Delete the specified server in your data center. The attached storage volumes will not be removed — a separate API call must be made for these actions.  # noqa: E501
+        Delete the specified server in your data center. The attached storage volumes will also be removed if the query parameter is set to true otherwise a separate API call must be made for these actions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_delete_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1493,17 +1493,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_post(self, datacenter_id, server, **kwargs):  # noqa: E501
-        """Create servers  # noqa: E501
+        """Create a Server  # noqa: E501
 
-        Create a server within the specified data center. You can also use this request to configure the boot volumes and connect to existing LANs at the same time.  # noqa: E501
+        Creates a server within the specified data center. You can also use this request to configure the boot volumes and connect to existing LANs at the same time.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_post(datacenter_id, server, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1531,17 +1531,17 @@
                  returns the request thread.
         :rtype: Server
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_post_with_http_info(datacenter_id, server, **kwargs)  # noqa: E501
 
     def datacenters_servers_post_with_http_info(self, datacenter_id, server, **kwargs):  # noqa: E501
-        """Create servers  # noqa: E501
+        """Create a Server  # noqa: E501
 
-        Create a server within the specified data center. You can also use this request to configure the boot volumes and connect to existing LANs at the same time.  # noqa: E501
+        Creates a server within the specified data center. You can also use this request to configure the boot volumes and connect to existing LANs at the same time.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_post_with_http_info(datacenter_id, server, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1670,17 +1670,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_put(self, datacenter_id, server_id, server, **kwargs):  # noqa: E501
-        """Modify servers  # noqa: E501
+        """Modify a Server by ID  # noqa: E501
 
-        Modify the properties of the specified server within the data center.  Starting with v5, the 'allowReboot' attribute is retired; while previously required for changing certain server properties, this behavior is now implicit, and the backend will perform this automatically. For example, in earlier versions, when the CPU family is changed, 'allowReboot' had to be set to 'true'; this is no longer required, the reboot will be performed automatically.  # noqa: E501
+        Modifies the properties of the specified server within the data center.  Starting with v5, the 'allowReboot' attribute is retired; while previously required for changing certain server properties, this behavior is now implicit, and the backend will perform this automatically. For example, in earlier versions, when the CPU family is changed, 'allowReboot' had to be set to 'true'; this is no longer required, the reboot will be performed automatically.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_put(datacenter_id, server_id, server, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1710,17 +1710,17 @@
                  returns the request thread.
         :rtype: Server
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_put_with_http_info(datacenter_id, server_id, server, **kwargs)  # noqa: E501
 
     def datacenters_servers_put_with_http_info(self, datacenter_id, server_id, server, **kwargs):  # noqa: E501
-        """Modify servers  # noqa: E501
+        """Modify a Server by ID  # noqa: E501
 
-        Modify the properties of the specified server within the data center.  Starting with v5, the 'allowReboot' attribute is retired; while previously required for changing certain server properties, this behavior is now implicit, and the backend will perform this automatically. For example, in earlier versions, when the CPU family is changed, 'allowReboot' had to be set to 'true'; this is no longer required, the reboot will be performed automatically.  # noqa: E501
+        Modifies the properties of the specified server within the data center.  Starting with v5, the 'allowReboot' attribute is retired; while previously required for changing certain server properties, this behavior is now implicit, and the backend will perform this automatically. For example, in earlier versions, when the CPU family is changed, 'allowReboot' had to be set to 'true'; this is no longer required, the reboot will be performed automatically.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_put_with_http_info(datacenter_id, server_id, server, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2204,17 +2204,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_resume_post(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Resume Cubes instances  # noqa: E501
+        """Resume a Cube Server by ID  # noqa: E501
 
-        Resume a suspended Cube instance; no billing event will be generated.  This operation is only supported for the Cubes.  # noqa: E501
+        Resumes a suspended Cube Server specified by its ID.  Since the suspended instance was not deleted the allocated resources continue to be billed. You can perform this operation only for Cube Servers.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_resume_post(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2242,17 +2242,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_resume_post_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_resume_post_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Resume Cubes instances  # noqa: E501
+        """Resume a Cube Server by ID  # noqa: E501
 
-        Resume a suspended Cube instance; no billing event will be generated.  This operation is only supported for the Cubes.  # noqa: E501
+        Resumes a suspended Cube Server specified by its ID.  Since the suspended instance was not deleted the allocated resources continue to be billed. You can perform this operation only for Cube Servers.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_resume_post_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2377,17 +2377,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_start_post(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Start servers  # noqa: E501
+        """Start an Enterprise Server by ID  # noqa: E501
 
-        Start the specified server within the data center; if the server's public IP address has been deallocated, a new IP address will be assigned.  # noqa: E501
+        Starts the Enterprise Server specified by its ID.  >Note that you cannot use this method to start a Cube Server.  By starting the Enterprise Server, cores and RAM are provisioned, and the billing continues.  If the server's public IPv4 address has been deallocated, a new IPv4 address will be assigned. IPv6 blocks and addresses will remain unchanged when stopping and starting a server.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_start_post(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2415,17 +2415,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_start_post_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_start_post_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Start servers  # noqa: E501
+        """Start an Enterprise Server by ID  # noqa: E501
 
-        Start the specified server within the data center; if the server's public IP address has been deallocated, a new IP address will be assigned.  # noqa: E501
+        Starts the Enterprise Server specified by its ID.  >Note that you cannot use this method to start a Cube Server.  By starting the Enterprise Server, cores and RAM are provisioned, and the billing continues.  If the server's public IPv4 address has been deallocated, a new IPv4 address will be assigned. IPv6 blocks and addresses will remain unchanged when stopping and starting a server.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_start_post_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2550,17 +2550,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_stop_post(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Stop VMs  # noqa: E501
+        """Stop an Enterprise Server by ID  # noqa: E501
 
-        Stop the specified server within the data center: the VM will be forcefully shut down, the billing will cease, and any allocated public IPs will be deallocated.  This operation is not supported for the Cubes.  # noqa: E501
+        Stops the Enterprise Server specified by its ID.   >Note that you cannot use this method to stop a Cube Server.   By stopping the Enterprise Server, cores and RAM are freed and no longer charged.  Public IPv4 IPs that are not reserved are returned to the IPv4 pool. IPv6 blocks and addresses will remain unchanged when stopping and starting a server.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_stop_post(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2588,17 +2588,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_stop_post_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_stop_post_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Stop VMs  # noqa: E501
+        """Stop an Enterprise Server by ID  # noqa: E501
 
-        Stop the specified server within the data center: the VM will be forcefully shut down, the billing will cease, and any allocated public IPs will be deallocated.  This operation is not supported for the Cubes.  # noqa: E501
+        Stops the Enterprise Server specified by its ID.   >Note that you cannot use this method to stop a Cube Server.   By stopping the Enterprise Server, cores and RAM are freed and no longer charged.  Public IPv4 IPs that are not reserved are returned to the IPv4 pool. IPv6 blocks and addresses will remain unchanged when stopping and starting a server.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_stop_post_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2723,17 +2723,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_suspend_post(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Suspend Cubes instances  # noqa: E501
+        """Suspend a Cube Server by ID  # noqa: E501
 
-        Suspend the specified Cubes instance within the data center. The instance will not be deleted, and allocated resources will continue to be billed.  This operation is only supported for the Cubes.  # noqa: E501
+        Suspends the specified Cubes instance within the data center.   The instance is not deleted and allocated resources continue to be billed. You can perform this operation only for Cube Servers.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_suspend_post(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -2761,17 +2761,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_suspend_post_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_suspend_post_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Suspend Cubes instances  # noqa: E501
+        """Suspend a Cube Server by ID  # noqa: E501
 
-        Suspend the specified Cubes instance within the data center. The instance will not be deleted, and allocated resources will continue to be billed.  This operation is only supported for the Cubes.  # noqa: E501
+        Suspends the specified Cubes instance within the data center.   The instance is not deleted and allocated resources continue to be billed. You can perform this operation only for Cube Servers.  To check the status of the request, you can use the 'Location' HTTP header in the response (see 'Requests' for more information).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_suspend_post_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3069,17 +3069,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_upgrade_post(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Upgrade servers  # noqa: E501
+        """Upgrade a Server by ID  # noqa: E501
 
-        Upgrade the server version, if needed. To determine if an upgrade is available, execute  the following call:  '/datacenters/{datacenterId}/servers?upgradeNeeded=true'  # noqa: E501
+        Upgrades the server version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_upgrade_post(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3107,17 +3107,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_upgrade_post_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_upgrade_post_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """Upgrade servers  # noqa: E501
+        """Upgrade a Server by ID  # noqa: E501
 
-        Upgrade the server version, if needed. To determine if an upgrade is available, execute  the following call:  '/datacenters/{datacenterId}/servers?upgradeNeeded=true'  # noqa: E501
+        Upgrades the server version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_upgrade_post_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3242,17 +3242,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_volumes_delete(self, datacenter_id, server_id, volume_id, **kwargs):  # noqa: E501
-        """Detach volumes  # noqa: E501
+        """Detach a Volume by ID  # noqa: E501
 
-        Detach the specified volume from the server without deleting it from the data center. A separate request must be made to perform the deletion.  # noqa: E501
+        Detachs the specified volume from the server.  Note that only the volume's connection to the specified server is disconnected. If you want to delete the volume, you must submit a separate request to perform the deletion.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_delete(datacenter_id, server_id, volume_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3282,17 +3282,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_volumes_delete_with_http_info(datacenter_id, server_id, volume_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_volumes_delete_with_http_info(self, datacenter_id, server_id, volume_id, **kwargs):  # noqa: E501
-        """Detach volumes  # noqa: E501
+        """Detach a Volume by ID  # noqa: E501
 
-        Detach the specified volume from the server without deleting it from the data center. A separate request must be made to perform the deletion.  # noqa: E501
+        Detachs the specified volume from the server.  Note that only the volume's connection to the specified server is disconnected. If you want to delete the volume, you must submit a separate request to perform the deletion.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_delete_with_http_info(datacenter_id, server_id, volume_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3426,17 +3426,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_volumes_find_by_id(self, datacenter_id, server_id, volume_id, **kwargs):  # noqa: E501
-        """Retrieve attached volumes  # noqa: E501
+        """Get Attached Volume by ID  # noqa: E501
 
-        Retrieve the properties of the volume, attached to the specified server.  # noqa: E501
+        Retrieves the properties of the volume attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_find_by_id(datacenter_id, server_id, volume_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3466,17 +3466,17 @@
                  returns the request thread.
         :rtype: Volume
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_volumes_find_by_id_with_http_info(datacenter_id, server_id, volume_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_volumes_find_by_id_with_http_info(self, datacenter_id, server_id, volume_id, **kwargs):  # noqa: E501
-        """Retrieve attached volumes  # noqa: E501
+        """Get Attached Volume by ID  # noqa: E501
 
-        Retrieve the properties of the volume, attached to the specified server.  # noqa: E501
+        Retrieves the properties of the volume attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_find_by_id_with_http_info(datacenter_id, server_id, volume_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3610,17 +3610,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_volumes_get(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """List attached volumes  # noqa: E501
+        """Get Attached Volumes  # noqa: E501
 
-        List all volumes, attached to the specified server.  # noqa: E501
+        Lists all volumes attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_get(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3652,17 +3652,17 @@
                  returns the request thread.
         :rtype: AttachedVolumes
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_volumes_get_with_http_info(datacenter_id, server_id, **kwargs)  # noqa: E501
 
     def datacenters_servers_volumes_get_with_http_info(self, datacenter_id, server_id, **kwargs):  # noqa: E501
-        """List attached volumes  # noqa: E501
+        """Get Attached Volumes  # noqa: E501
 
-        List all volumes, attached to the specified server.  # noqa: E501
+        Lists all volumes attached to the specified server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_get_with_http_info(datacenter_id, server_id, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3803,17 +3803,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_servers_volumes_post(self, datacenter_id, server_id, volume, **kwargs):  # noqa: E501
-        """Attach volumes  # noqa: E501
+        """Attach a Volume to a Server  # noqa: E501
 
-        Attach an existing storage volume to the specified server.  A volume scan also be created and attached in one step by providing the new volume description as payload.  The combined total of attached volumes and NICs cannot exceed 24 per server.  # noqa: E501
+        Attachs an existing storage volume to the specified server.  You can attach an existing volume in the VDC to a server. To move a volume from one server to another, you must first detach the volume from the first server and attach it to the second server.  It is also possible to create and attach a volume in one step by simply providing a new volume description as a payload. The only difference is the URL; see 'Creating a Volume' for details about volumes.  Note that the combined total of attached volumes and NICs cannot exceed 24 per server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_post(datacenter_id, server_id, volume, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -3843,17 +3843,17 @@
                  returns the request thread.
         :rtype: Volume
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_servers_volumes_post_with_http_info(datacenter_id, server_id, volume, **kwargs)  # noqa: E501
 
     def datacenters_servers_volumes_post_with_http_info(self, datacenter_id, server_id, volume, **kwargs):  # noqa: E501
-        """Attach volumes  # noqa: E501
+        """Attach a Volume to a Server  # noqa: E501
 
-        Attach an existing storage volume to the specified server.  A volume scan also be created and attached in one step by providing the new volume description as payload.  The combined total of attached volumes and NICs cannot exceed 24 per server.  # noqa: E501
+        Attachs an existing storage volume to the specified server.  You can attach an existing volume in the VDC to a server. To move a volume from one server to another, you must first detach the volume from the first server and attach it to the second server.  It is also possible to create and attach a volume in one step by simply providing a new volume description as a payload. The only difference is the URL; see 'Creating a Volume' for details about volumes.  Note that the combined total of attached volumes and NICs cannot exceed 24 per server.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_servers_volumes_post_with_http_info(datacenter_id, server_id, volume, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/snapshots_api.py` & `ionoscloud-6.1.5/ionoscloud/api/snapshots_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,17 +666,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def snapshots_put(self, snapshot_id, snapshot, **kwargs):  # noqa: E501
-        """Modify snapshots  # noqa: E501
+        """Modify a Snapshot by ID  # noqa: E501
 
-        Modify the properties of the specified snapshot.  # noqa: E501
+        Modifies the properties of the specified snapshot.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.snapshots_put(snapshot_id, snapshot, async_req=True)
         >>> result = thread.get()
 
         :param snapshot_id: The unique ID of the snapshot. (required)
@@ -704,17 +704,17 @@
                  returns the request thread.
         :rtype: Snapshot
         """
         kwargs['_return_http_data_only'] = True
         return self.snapshots_put_with_http_info(snapshot_id, snapshot, **kwargs)  # noqa: E501
 
     def snapshots_put_with_http_info(self, snapshot_id, snapshot, **kwargs):  # noqa: E501
-        """Modify snapshots  # noqa: E501
+        """Modify a Snapshot by ID  # noqa: E501
 
-        Modify the properties of the specified snapshot.  # noqa: E501
+        Modifies the properties of the specified snapshot.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.snapshots_put_with_http_info(snapshot_id, snapshot, async_req=True)
         >>> result = thread.get()
 
         :param snapshot_id: The unique ID of the snapshot. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/target_groups_api.py` & `ionoscloud-6.1.5/ionoscloud/api/target_groups_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def target_groups_delete(self, target_group_id, **kwargs):  # noqa: E501
-        """Remove target groups  # noqa: E501
+        """Delete a Target Group by ID  # noqa: E501
 
-        Remove the specified target group.  # noqa: E501
+        Deletes the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.target_groups_delete(target_group_id, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -50,17 +50,17 @@
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.target_groups_delete_with_http_info(target_group_id, **kwargs)  # noqa: E501
 
     def target_groups_delete_with_http_info(self, target_group_id, **kwargs):  # noqa: E501
-        """Remove target groups  # noqa: E501
+        """Delete a Target Group by ID  # noqa: E501
 
-        Remove the specified target group.  # noqa: E501
+        Deletes the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.target_groups_delete_with_http_info(target_group_id, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -176,17 +176,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def targetgroups_find_by_target_group_id(self, target_group_id, **kwargs):  # noqa: E501
-        """Retrieve target groups  # noqa: E501
+        """Get a Target Group by ID  # noqa: E501
 
-        Retrieve the properties of the specified target group.  # noqa: E501
+        Retrieves the properties of the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_find_by_target_group_id(target_group_id, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -212,17 +212,17 @@
                  returns the request thread.
         :rtype: TargetGroup
         """
         kwargs['_return_http_data_only'] = True
         return self.targetgroups_find_by_target_group_id_with_http_info(target_group_id, **kwargs)  # noqa: E501
 
     def targetgroups_find_by_target_group_id_with_http_info(self, target_group_id, **kwargs):  # noqa: E501
-        """Retrieve target groups  # noqa: E501
+        """Get a Target Group by ID  # noqa: E501
 
-        Retrieve the properties of the specified target group.  # noqa: E501
+        Retrieves the properties of the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_find_by_target_group_id_with_http_info(target_group_id, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -338,17 +338,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def targetgroups_get(self, **kwargs):  # noqa: E501
-        """List target groups  # noqa: E501
+        """Get Target Groups  # noqa: E501
 
-        List all target groups.  # noqa: E501
+        Lists target groups.  A target group is a set of one or more registered targets. You must specify an IP address, a port number, and a weight for each target. Any object with an IP address in your VDC can be a target, for example, a VM, another load balancer, etc. You can register a target with multiple target groups.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_get(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -376,17 +376,17 @@
                  returns the request thread.
         :rtype: TargetGroups
         """
         kwargs['_return_http_data_only'] = True
         return self.targetgroups_get_with_http_info(**kwargs)  # noqa: E501
 
     def targetgroups_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List target groups  # noqa: E501
+        """Get Target Groups  # noqa: E501
 
-        List all target groups.  # noqa: E501
+        Lists target groups.  A target group is a set of one or more registered targets. You must specify an IP address, a port number, and a weight for each target. Any object with an IP address in your VDC can be a target, for example, a VM, another load balancer, etc. You can register a target with multiple target groups.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param pretty: Controls whether the response is pretty-printed (with indentations and new lines).
@@ -509,17 +509,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def targetgroups_patch(self, target_group_id, target_group_properties, **kwargs):  # noqa: E501
-        """Partially modify target groups  # noqa: E501
+        """Partially Modify a Target Group by ID  # noqa: E501
 
-        Update the properties of the specified target group.  # noqa: E501
+        Updates the properties of the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_patch(target_group_id, target_group_properties, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -547,17 +547,17 @@
                  returns the request thread.
         :rtype: TargetGroup
         """
         kwargs['_return_http_data_only'] = True
         return self.targetgroups_patch_with_http_info(target_group_id, target_group_properties, **kwargs)  # noqa: E501
 
     def targetgroups_patch_with_http_info(self, target_group_id, target_group_properties, **kwargs):  # noqa: E501
-        """Partially modify target groups  # noqa: E501
+        """Partially Modify a Target Group by ID  # noqa: E501
 
-        Update the properties of the specified target group.  # noqa: E501
+        Updates the properties of the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_patch_with_http_info(target_group_id, target_group_properties, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -682,17 +682,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def targetgroups_post(self, target_group, **kwargs):  # noqa: E501
-        """Create target groups  # noqa: E501
+        """Create a Target Group  # noqa: E501
 
-        Create a target group.  # noqa: E501
+        Creates a target group.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_post(target_group, async_req=True)
         >>> result = thread.get()
 
         :param target_group: The target group to create. (required)
@@ -718,17 +718,17 @@
                  returns the request thread.
         :rtype: TargetGroup
         """
         kwargs['_return_http_data_only'] = True
         return self.targetgroups_post_with_http_info(target_group, **kwargs)  # noqa: E501
 
     def targetgroups_post_with_http_info(self, target_group, **kwargs):  # noqa: E501
-        """Create target groups  # noqa: E501
+        """Create a Target Group  # noqa: E501
 
-        Create a target group.  # noqa: E501
+        Creates a target group.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_post_with_http_info(target_group, async_req=True)
         >>> result = thread.get()
 
         :param target_group: The target group to create. (required)
@@ -848,17 +848,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def targetgroups_put(self, target_group_id, target_group, **kwargs):  # noqa: E501
-        """Modify target groups  # noqa: E501
+        """Modify a Target Group by ID  # noqa: E501
 
-        Modify the properties of the specified target group.  # noqa: E501
+        Modifies the properties of the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_put(target_group_id, target_group, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
@@ -886,17 +886,17 @@
                  returns the request thread.
         :rtype: TargetGroup
         """
         kwargs['_return_http_data_only'] = True
         return self.targetgroups_put_with_http_info(target_group_id, target_group, **kwargs)  # noqa: E501
 
     def targetgroups_put_with_http_info(self, target_group_id, target_group, **kwargs):  # noqa: E501
-        """Modify target groups  # noqa: E501
+        """Modify a Target Group by ID  # noqa: E501
 
-        Modify the properties of the specified target group.  # noqa: E501
+        Modifies the properties of the target group specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.targetgroups_put_with_http_info(target_group_id, target_group, async_req=True)
         >>> result = thread.get()
 
         :param target_group_id: The unique ID of the target group. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/templates_api.py` & `ionoscloud-6.1.5/ionoscloud/api/templates_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def templates_find_by_id(self, template_id, **kwargs):  # noqa: E501
-        """Retrieve Cubes Templates  # noqa: E501
+        """Get Cubes Template by ID  # noqa: E501
 
-        Retrieve the properties of the specified Cubes Template.  This operation is only supported for the Cubes.  # noqa: E501
+        Retrieves the properties of the Cubes template specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.templates_find_by_id(template_id, async_req=True)
         >>> result = thread.get()
 
-        :param template_id: The unique Template ID. (required)
+        :param template_id: The unique template ID. (required)
         :type template_id: str
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -46,24 +46,24 @@
                  returns the request thread.
         :rtype: Template
         """
         kwargs['_return_http_data_only'] = True
         return self.templates_find_by_id_with_http_info(template_id, **kwargs)  # noqa: E501
 
     def templates_find_by_id_with_http_info(self, template_id, **kwargs):  # noqa: E501
-        """Retrieve Cubes Templates  # noqa: E501
+        """Get Cubes Template by ID  # noqa: E501
 
-        Retrieve the properties of the specified Cubes Template.  This operation is only supported for the Cubes.  # noqa: E501
+        Retrieves the properties of the Cubes template specified by its ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.templates_find_by_id_with_http_info(template_id, async_req=True)
         >>> result = thread.get()
 
-        :param template_id: The unique Template ID. (required)
+        :param template_id: The unique template ID. (required)
         :type template_id: str
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
         :type depth: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -162,17 +162,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def templates_get(self, **kwargs):  # noqa: E501
-        """List Cubes Templates  # noqa: E501
+        """Get Cubes Templates  # noqa: E501
 
-        List all of the available Cubes Templates.  This operation is only supported for the Cubes.  # noqa: E501
+        Retrieves all available templates.  Templates provide a pre-defined configuration for Cube servers.    >Templates are read-only and cannot be created, modified, or deleted by users.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.templates_get(async_req=True)
         >>> result = thread.get()
 
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
@@ -192,17 +192,17 @@
                  returns the request thread.
         :rtype: Templates
         """
         kwargs['_return_http_data_only'] = True
         return self.templates_get_with_http_info(**kwargs)  # noqa: E501
 
     def templates_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List Cubes Templates  # noqa: E501
+        """Get Cubes Templates  # noqa: E501
 
-        List all of the available Cubes Templates.  This operation is only supported for the Cubes.  # noqa: E501
+        Retrieves all available templates.  Templates provide a pre-defined configuration for Cube servers.    >Templates are read-only and cannot be created, modified, or deleted by users.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.templates_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param depth: Controls the detail depth of the response objects.  GET /datacenters/[ID]  - depth=0: Only direct properties are included; children (servers and other elements) are not included.  - depth=1: Direct properties and children references are included.  - depth=2: Direct properties and children properties are included.  - depth=3: Direct properties and children properties and children's children are included.  - depth=... and so on
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/user_management_api.py` & `ionoscloud-6.1.5/ionoscloud/api/user_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2209,17 +2209,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def um_groups_users_post(self, group_id, user, **kwargs):  # noqa: E501
-        """Add group members  # noqa: E501
+        """Add a Group Member  # noqa: E501
 
-        Add an existing user to the specified group.   # noqa: E501
+        Adds an existing user to the specified group.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.um_groups_users_post(group_id, user, async_req=True)
         >>> result = thread.get()
 
         :param group_id: The unique ID of the group. (required)
@@ -2247,17 +2247,17 @@
                  returns the request thread.
         :rtype: User
         """
         kwargs['_return_http_data_only'] = True
         return self.um_groups_users_post_with_http_info(group_id, user, **kwargs)  # noqa: E501
 
     def um_groups_users_post_with_http_info(self, group_id, user, **kwargs):  # noqa: E501
-        """Add group members  # noqa: E501
+        """Add a Group Member  # noqa: E501
 
-        Add an existing user to the specified group.   # noqa: E501
+        Adds an existing user to the specified group.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.um_groups_users_post_with_http_info(group_id, user, async_req=True)
         >>> result = thread.get()
 
         :param group_id: The unique ID of the group. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/user_s3_keys_api.py` & `ionoscloud-6.1.5/ionoscloud/api/user_s3_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,17 +684,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def um_users_s3keys_put(self, user_id, key_id, s3_key, **kwargs):  # noqa: E501
-        """Modify S3 keys by key ID  # noqa: E501
+        """Modify a S3 Key by Key ID  # noqa: E501
 
-        Enable or disable the specified user S3 key.  # noqa: E501
+        Enables or disables the specified user S3 key.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.um_users_s3keys_put(user_id, key_id, s3_key, async_req=True)
         >>> result = thread.get()
 
         :param user_id: The unique ID of the user. (required)
@@ -724,17 +724,17 @@
                  returns the request thread.
         :rtype: S3Key
         """
         kwargs['_return_http_data_only'] = True
         return self.um_users_s3keys_put_with_http_info(user_id, key_id, s3_key, **kwargs)  # noqa: E501
 
     def um_users_s3keys_put_with_http_info(self, user_id, key_id, s3_key, **kwargs):  # noqa: E501
-        """Modify S3 keys by key ID  # noqa: E501
+        """Modify a S3 Key by Key ID  # noqa: E501
 
-        Enable or disable the specified user S3 key.  # noqa: E501
+        Enables or disables the specified user S3 key.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.um_users_s3keys_put_with_http_info(user_id, key_id, s3_key, async_req=True)
         >>> result = thread.get()
 
         :param user_id: The unique ID of the user. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api/volumes_api.py` & `ionoscloud-6.1.5/ionoscloud/api/volumes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -935,17 +935,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_volumes_post(self, datacenter_id, volume, **kwargs):  # noqa: E501
-        """Create volumes  # noqa: E501
+        """Create a Volume  # noqa: E501
 
-        Create a storage volume within the specified data center. The volume will not be attached! Attaching volumes is described in the Servers section.  # noqa: E501
+        Creates a storage volume within the specified data center. The volume will not be attached! Attaching volumes is described in the Servers section.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_post(datacenter_id, volume, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -973,17 +973,17 @@
                  returns the request thread.
         :rtype: Volume
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_volumes_post_with_http_info(datacenter_id, volume, **kwargs)  # noqa: E501
 
     def datacenters_volumes_post_with_http_info(self, datacenter_id, volume, **kwargs):  # noqa: E501
-        """Create volumes  # noqa: E501
+        """Create a Volume  # noqa: E501
 
-        Create a storage volume within the specified data center. The volume will not be attached! Attaching volumes is described in the Servers section.  # noqa: E501
+        Creates a storage volume within the specified data center. The volume will not be attached! Attaching volumes is described in the Servers section.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_post_with_http_info(datacenter_id, volume, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1112,17 +1112,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def datacenters_volumes_put(self, datacenter_id, volume_id, volume, **kwargs):  # noqa: E501
-        """Modify volumes  # noqa: E501
+        """Modify a Volume by ID  # noqa: E501
 
-        Modify the properties of the specified volume within the data center.  # noqa: E501
+        Modifies the properties of the specified volume within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_put(datacenter_id, volume_id, volume, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
@@ -1152,17 +1152,17 @@
                  returns the request thread.
         :rtype: Volume
         """
         kwargs['_return_http_data_only'] = True
         return self.datacenters_volumes_put_with_http_info(datacenter_id, volume_id, volume, **kwargs)  # noqa: E501
 
     def datacenters_volumes_put_with_http_info(self, datacenter_id, volume_id, volume, **kwargs):  # noqa: E501
-        """Modify volumes  # noqa: E501
+        """Modify a Volume by ID  # noqa: E501
 
-        Modify the properties of the specified volume within the data center.  # noqa: E501
+        Modifies the properties of the specified volume within the data center.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.datacenters_volumes_put_with_http_info(datacenter_id, volume_id, volume, async_req=True)
         >>> result = thread.get()
 
         :param datacenter_id: The unique ID of the data center. (required)
```

### Comparing `ionoscloud-6.1.4/ionoscloud/api_client.py` & `ionoscloud-6.1.5/ionoscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'ionos-cloud-sdk-python/6.1.4'
+        self.user_agent = 'ionos-cloud-sdk-python/6.1.5'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ionoscloud-6.1.4/ionoscloud/configuration.py` & `ionoscloud-6.1.5/ionoscloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 6.0\n"\
-               "SDK Package Version: 6.1.4".\
+               "SDK Package Version: 6.1.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ionoscloud-6.1.4/ionoscloud/exceptions.py` & `ionoscloud-6.1.5/ionoscloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/__init__.py` & `ionoscloud-6.1.5/ionoscloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,26 +135,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this ApplicationLoadBalancer.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this ApplicationLoadBalancer.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this ApplicationLoadBalancer.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this ApplicationLoadBalancer.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rule.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this ApplicationLoadBalancerForwardingRule.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this ApplicationLoadBalancerForwardingRule.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this ApplicationLoadBalancerForwardingRule.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this ApplicationLoadBalancerForwardingRule.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rule_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,26 +118,26 @@
 
         self._name = name
 
     @property
     def protocol(self):
         """Gets the protocol of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
 
-        Balancing protocol  # noqa: E501
+        The balancing protocol.  # noqa: E501
 
         :return: The protocol of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :rtype: str
         """
         return self._protocol
 
     @protocol.setter
     def protocol(self, protocol):
         """Sets the protocol of this ApplicationLoadBalancerForwardingRuleProperties.
 
-        Balancing protocol  # noqa: E501
+        The balancing protocol.  # noqa: E501
 
         :param protocol: The protocol of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :type protocol: str
         """
         if self.local_vars_configuration.client_side_validation and protocol is None:  # noqa: E501
             raise ValueError("Invalid value for `protocol`, must not be `None`")  # noqa: E501
         allowed_values = ["HTTP"]  # noqa: E501
@@ -149,51 +149,51 @@
 
         self._protocol = protocol
 
     @property
     def listener_ip(self):
         """Gets the listener_ip of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
 
-        Listening (inbound) IP  # noqa: E501
+        The listening (inbound) IP.  # noqa: E501
 
         :return: The listener_ip of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :rtype: str
         """
         return self._listener_ip
 
     @listener_ip.setter
     def listener_ip(self, listener_ip):
         """Sets the listener_ip of this ApplicationLoadBalancerForwardingRuleProperties.
 
-        Listening (inbound) IP  # noqa: E501
+        The listening (inbound) IP.  # noqa: E501
 
         :param listener_ip: The listener_ip of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :type listener_ip: str
         """
         if self.local_vars_configuration.client_side_validation and listener_ip is None:  # noqa: E501
             raise ValueError("Invalid value for `listener_ip`, must not be `None`")  # noqa: E501
 
         self._listener_ip = listener_ip
 
     @property
     def listener_port(self):
         """Gets the listener_port of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
 
-        Listening (inbound) port number; valid range is 1 to 65535.  # noqa: E501
+        The listening (inbound) port number; the valid range is 1 to 65535.  # noqa: E501
 
         :return: The listener_port of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :rtype: int
         """
         return self._listener_port
 
     @listener_port.setter
     def listener_port(self, listener_port):
         """Sets the listener_port of this ApplicationLoadBalancerForwardingRuleProperties.
 
-        Listening (inbound) port number; valid range is 1 to 65535.  # noqa: E501
+        The listening (inbound) port number; the valid range is 1 to 65535.  # noqa: E501
 
         :param listener_port: The listener_port of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :type listener_port: int
         """
         if self.local_vars_configuration.client_side_validation and listener_port is None:  # noqa: E501
             raise ValueError("Invalid value for `listener_port`, must not be `None`")  # noqa: E501
 
@@ -245,26 +245,26 @@
 
         self._server_certificates = server_certificates
 
     @property
     def http_rules(self):
         """Gets the http_rules of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
 
-        An array of items in the collection. The original order of rules is perserved during processing, except for Forward-type rules are processed after the rules with other action defined. The relative order of Forward-type rules is also preserved during the processing.  # noqa: E501
+        An array of items in the collection. The original order of rules is preserved during processing, except that rules of the 'FORWARD' type are processed after the rules with other defined actions. The relative order of the 'FORWARD' type rules is also preserved during the processing.  # noqa: E501
 
         :return: The http_rules of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :rtype: list[ApplicationLoadBalancerHttpRule]
         """
         return self._http_rules
 
     @http_rules.setter
     def http_rules(self, http_rules):
         """Sets the http_rules of this ApplicationLoadBalancerForwardingRuleProperties.
 
-        An array of items in the collection. The original order of rules is perserved during processing, except for Forward-type rules are processed after the rules with other action defined. The relative order of Forward-type rules is also preserved during the processing.  # noqa: E501
+        An array of items in the collection. The original order of rules is preserved during processing, except that rules of the 'FORWARD' type are processed after the rules with other defined actions. The relative order of the 'FORWARD' type rules is also preserved during the processing.  # noqa: E501
 
         :param http_rules: The http_rules of this ApplicationLoadBalancerForwardingRuleProperties.  # noqa: E501
         :type http_rules: list[ApplicationLoadBalancerHttpRule]
         """
 
         self._http_rules = http_rules
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rule_put.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rule_put.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,26 +121,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this ApplicationLoadBalancerForwardingRulePut.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this ApplicationLoadBalancerForwardingRulePut.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this ApplicationLoadBalancerForwardingRulePut.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this ApplicationLoadBalancerForwardingRulePut.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_forwarding_rules.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_forwarding_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,26 +143,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this ApplicationLoadBalancerForwardingRules.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this ApplicationLoadBalancerForwardingRules.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this ApplicationLoadBalancerForwardingRules.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this ApplicationLoadBalancerForwardingRules.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_http_rule.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_http_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,26 +134,26 @@
 
         self._name = name
 
     @property
     def type(self):
         """Gets the type of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        Type of the HTTP rule.  # noqa: E501
+        The HTTP rule type.  # noqa: E501
 
         :return: The type of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this ApplicationLoadBalancerHttpRule.
 
-        Type of the HTTP rule.  # noqa: E501
+        The HTTP rule type.  # noqa: E501
 
         :param type: The type of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
         allowed_values = ["FORWARD", "STATIC", "REDIRECT"]  # noqa: E501
@@ -165,170 +165,164 @@
 
         self._type = type
 
     @property
     def target_group(self):
         """Gets the target_group of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        The ID of the target group; mandatory and only valid for FORWARD actions.  # noqa: E501
+        The ID of the target group; this parameter is mandatory and is valid only for 'FORWARD' actions.  # noqa: E501
 
         :return: The target_group of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: str
         """
         return self._target_group
 
     @target_group.setter
     def target_group(self, target_group):
         """Sets the target_group of this ApplicationLoadBalancerHttpRule.
 
-        The ID of the target group; mandatory and only valid for FORWARD actions.  # noqa: E501
+        The ID of the target group; this parameter is mandatory and is valid only for 'FORWARD' actions.  # noqa: E501
 
         :param target_group: The target_group of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type target_group: str
         """
 
         self._target_group = target_group
 
     @property
     def drop_query(self):
         """Gets the drop_query of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        Default is false; valid only for REDIRECT actions.  # noqa: E501
+        Indicates whether the query part of the URI should be dropped and is valid only for 'REDIRECT' actions. Default value is 'FALSE', the redirect URI does not contain any query parameters.  # noqa: E501
 
         :return: The drop_query of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: bool
         """
         return self._drop_query
 
     @drop_query.setter
     def drop_query(self, drop_query):
         """Sets the drop_query of this ApplicationLoadBalancerHttpRule.
 
-        Default is false; valid only for REDIRECT actions.  # noqa: E501
+        Indicates whether the query part of the URI should be dropped and is valid only for 'REDIRECT' actions. Default value is 'FALSE', the redirect URI does not contain any query parameters.  # noqa: E501
 
         :param drop_query: The drop_query of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type drop_query: bool
         """
 
         self._drop_query = drop_query
 
     @property
     def location(self):
         """Gets the location of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        The location for redirecting; mandatory and valid only for REDIRECT actions.  # noqa: E501
+        The location for the redirection; this parameter is mandatory and valid only for 'REDIRECT' actions.  # noqa: E501
 
         :return: The location of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: str
         """
         return self._location
 
     @location.setter
     def location(self, location):
         """Sets the location of this ApplicationLoadBalancerHttpRule.
 
-        The location for redirecting; mandatory and valid only for REDIRECT actions.  # noqa: E501
+        The location for the redirection; this parameter is mandatory and valid only for 'REDIRECT' actions.  # noqa: E501
 
         :param location: The location of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type location: str
         """
 
         self._location = location
 
     @property
     def status_code(self):
         """Gets the status_code of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        Valid only for REDIRECT and STATIC actions. For REDIRECT actions, default is 301 and possible values are 301, 302, 303, 307, and 308. For STATIC actions, default is 503 and valid range is 200 to 599.  # noqa: E501
+        The status code is for 'REDIRECT' and 'STATIC' actions only.   If the HTTP rule is 'REDIRECT' the valid values are: 301, 302, 303, 307, 308; default value is '301'.  If the HTTP rule is 'STATIC' the valid values are from the range 200-599; default value is '503'.  # noqa: E501
 
         :return: The status_code of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: int
         """
         return self._status_code
 
     @status_code.setter
     def status_code(self, status_code):
         """Sets the status_code of this ApplicationLoadBalancerHttpRule.
 
-        Valid only for REDIRECT and STATIC actions. For REDIRECT actions, default is 301 and possible values are 301, 302, 303, 307, and 308. For STATIC actions, default is 503 and valid range is 200 to 599.  # noqa: E501
+        The status code is for 'REDIRECT' and 'STATIC' actions only.   If the HTTP rule is 'REDIRECT' the valid values are: 301, 302, 303, 307, 308; default value is '301'.  If the HTTP rule is 'STATIC' the valid values are from the range 200-599; default value is '503'.  # noqa: E501
 
         :param status_code: The status_code of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type status_code: int
         """
-        allowed_values = [301, 302, 303, 307, 308, 200, 503, 599]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and status_code not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `status_code` ({0}), must be one of {1}"  # noqa: E501
-                .format(status_code, allowed_values)
-            )
 
         self._status_code = status_code
 
     @property
     def response_message(self):
         """Gets the response_message of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        The response message of the request; mandatory for STATIC actions.  # noqa: E501
+        The response message of the request; this parameter is mandatory for 'STATIC' actions.  # noqa: E501
 
         :return: The response_message of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: str
         """
         return self._response_message
 
     @response_message.setter
     def response_message(self, response_message):
         """Sets the response_message of this ApplicationLoadBalancerHttpRule.
 
-        The response message of the request; mandatory for STATIC actions.  # noqa: E501
+        The response message of the request; this parameter is mandatory for 'STATIC' actions.  # noqa: E501
 
         :param response_message: The response_message of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type response_message: str
         """
 
         self._response_message = response_message
 
     @property
     def content_type(self):
         """Gets the content_type of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        Valid only for STATIC actions.  # noqa: E501
+        Specifies the content type and is valid only for 'STATIC' actions.  # noqa: E501
 
         :return: The content_type of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: str
         """
         return self._content_type
 
     @content_type.setter
     def content_type(self, content_type):
         """Sets the content_type of this ApplicationLoadBalancerHttpRule.
 
-        Valid only for STATIC actions.  # noqa: E501
+        Specifies the content type and is valid only for 'STATIC' actions.  # noqa: E501
 
         :param content_type: The content_type of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type content_type: str
         """
 
         self._content_type = content_type
 
     @property
     def conditions(self):
         """Gets the conditions of this ApplicationLoadBalancerHttpRule.  # noqa: E501
 
-        An array of items in the collection.The action is only performed if each and every condition is met; if no conditions are set, the rule will always be performed.  # noqa: E501
+        An array of items in the collection. The action will be executed only if each condition is met; the rule will always be applied if no conditions are set.  # noqa: E501
 
         :return: The conditions of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :rtype: list[ApplicationLoadBalancerHttpRuleCondition]
         """
         return self._conditions
 
     @conditions.setter
     def conditions(self, conditions):
         """Sets the conditions of this ApplicationLoadBalancerHttpRule.
 
-        An array of items in the collection.The action is only performed if each and every condition is met; if no conditions are set, the rule will always be performed.  # noqa: E501
+        An array of items in the collection. The action will be executed only if each condition is met; the rule will always be applied if no conditions are set.  # noqa: E501
 
         :param conditions: The conditions of this ApplicationLoadBalancerHttpRule.  # noqa: E501
         :type conditions: list[ApplicationLoadBalancerHttpRuleCondition]
         """
 
         self._conditions = conditions
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_http_rule_condition.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_http_rule_condition.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,26 +81,26 @@
             self.value = value
 
 
     @property
     def type(self):
         """Gets the type of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
 
-        Type of the HTTP rule condition.  # noqa: E501
+        The HTTP rule condition type.  # noqa: E501
 
         :return: The type of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this ApplicationLoadBalancerHttpRuleCondition.
 
-        Type of the HTTP rule condition.  # noqa: E501
+        The HTTP rule condition type.  # noqa: E501
 
         :param type: The type of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
         allowed_values = ["HEADER", "PATH", "QUERY", "METHOD", "HOST", "COOKIE", "SOURCE_IP"]  # noqa: E501
@@ -112,26 +112,26 @@
 
         self._type = type
 
     @property
     def condition(self):
         """Gets the condition of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
 
-        Matching rule for the HTTP rule condition attribute; mandatory for HEADER, PATH, QUERY, METHOD, HOST, and COOKIE types; must be null when type is SOURCE_IP.  # noqa: E501
+        The matching rule for the HTTP rule condition attribute; this parameter is mandatory for 'HEADER', 'PATH', 'QUERY', 'METHOD', 'HOST', and 'COOKIE' types. It must be 'null' if the type is 'SOURCE_IP'.  # noqa: E501
 
         :return: The condition of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :rtype: str
         """
         return self._condition
 
     @condition.setter
     def condition(self, condition):
         """Sets the condition of this ApplicationLoadBalancerHttpRuleCondition.
 
-        Matching rule for the HTTP rule condition attribute; mandatory for HEADER, PATH, QUERY, METHOD, HOST, and COOKIE types; must be null when type is SOURCE_IP.  # noqa: E501
+        The matching rule for the HTTP rule condition attribute; this parameter is mandatory for 'HEADER', 'PATH', 'QUERY', 'METHOD', 'HOST', and 'COOKIE' types. It must be 'null' if the type is 'SOURCE_IP'.  # noqa: E501
 
         :param condition: The condition of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :type condition: str
         """
         if self.local_vars_configuration.client_side_validation and condition is None:  # noqa: E501
             raise ValueError("Invalid value for `condition`, must not be `None`")  # noqa: E501
         allowed_values = ["EXISTS", "CONTAINS", "EQUALS", "MATCHES", "STARTS_WITH", "ENDS_WITH"]  # noqa: E501
@@ -143,72 +143,72 @@
 
         self._condition = condition
 
     @property
     def negate(self):
         """Gets the negate of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
 
-        Specifies whether the condition is negated or not; the default is False.  # noqa: E501
+        Specifies whether the condition should be negated; the default value is 'FALSE'.  # noqa: E501
 
         :return: The negate of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :rtype: bool
         """
         return self._negate
 
     @negate.setter
     def negate(self, negate):
         """Sets the negate of this ApplicationLoadBalancerHttpRuleCondition.
 
-        Specifies whether the condition is negated or not; the default is False.  # noqa: E501
+        Specifies whether the condition should be negated; the default value is 'FALSE'.  # noqa: E501
 
         :param negate: The negate of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :type negate: bool
         """
 
         self._negate = negate
 
     @property
     def key(self):
         """Gets the key of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
 
-        Must be null when type is PATH, METHOD, HOST, or SOURCE_IP. Key can only be set when type is COOKIES, HEADER, or QUERY.  # noqa: E501
+        The key can only be set when the HTTP rule condition type is 'COOKIES', 'HEADER', or 'QUERY'. For the type 'PATH', 'METHOD', 'HOST', or 'SOURCE_IP' the value must be 'null'.  # noqa: E501
 
         :return: The key of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :rtype: str
         """
         return self._key
 
     @key.setter
     def key(self, key):
         """Sets the key of this ApplicationLoadBalancerHttpRuleCondition.
 
-        Must be null when type is PATH, METHOD, HOST, or SOURCE_IP. Key can only be set when type is COOKIES, HEADER, or QUERY.  # noqa: E501
+        The key can only be set when the HTTP rule condition type is 'COOKIES', 'HEADER', or 'QUERY'. For the type 'PATH', 'METHOD', 'HOST', or 'SOURCE_IP' the value must be 'null'.  # noqa: E501
 
         :param key: The key of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :type key: str
         """
 
         self._key = key
 
     @property
     def value(self):
         """Gets the value of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
 
-        Mandatory for conditions CONTAINS, EQUALS, MATCHES, STARTS_WITH, ENDS_WITH; must be null when condition is EXISTS; should be a valid CIDR if provided and if type is SOURCE_IP.  # noqa: E501
+        This parameter is mandatory for the conditions 'CONTAINS', 'EQUALS', 'MATCHES', 'STARTS_WITH', 'ENDS_WITH', or if the type is 'SOURCE_IP'. Specify a valid CIDR. If the condition is 'EXISTS', the value must be 'null'.  # noqa: E501
 
         :return: The value of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :rtype: str
         """
         return self._value
 
     @value.setter
     def value(self, value):
         """Sets the value of this ApplicationLoadBalancerHttpRuleCondition.
 
-        Mandatory for conditions CONTAINS, EQUALS, MATCHES, STARTS_WITH, ENDS_WITH; must be null when condition is EXISTS; should be a valid CIDR if provided and if type is SOURCE_IP.  # noqa: E501
+        This parameter is mandatory for the conditions 'CONTAINS', 'EQUALS', 'MATCHES', 'STARTS_WITH', 'ENDS_WITH', or if the type is 'SOURCE_IP'. Specify a valid CIDR. If the condition is 'EXISTS', the value must be 'null'.  # noqa: E501
 
         :param value: The value of this ApplicationLoadBalancerHttpRuleCondition.  # noqa: E501
         :type value: str
         """
 
         self._value = value
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,99 +80,99 @@
             self.lb_private_ips = lb_private_ips
 
 
     @property
     def name(self):
         """Gets the name of this ApplicationLoadBalancerProperties.  # noqa: E501
 
-        The name of the Application Load Balancer.  # noqa: E501
+        The Application Load Balancer name.  # noqa: E501
 
         :return: The name of this ApplicationLoadBalancerProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ApplicationLoadBalancerProperties.
 
-        The name of the Application Load Balancer.  # noqa: E501
+        The Application Load Balancer name.  # noqa: E501
 
         :param name: The name of this ApplicationLoadBalancerProperties.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def listener_lan(self):
         """Gets the listener_lan of this ApplicationLoadBalancerProperties.  # noqa: E501
 
-        ID of the listening (inbound) LAN.  # noqa: E501
+        The ID of the listening (inbound) LAN.  # noqa: E501
 
         :return: The listener_lan of this ApplicationLoadBalancerProperties.  # noqa: E501
         :rtype: int
         """
         return self._listener_lan
 
     @listener_lan.setter
     def listener_lan(self, listener_lan):
         """Sets the listener_lan of this ApplicationLoadBalancerProperties.
 
-        ID of the listening (inbound) LAN.  # noqa: E501
+        The ID of the listening (inbound) LAN.  # noqa: E501
 
         :param listener_lan: The listener_lan of this ApplicationLoadBalancerProperties.  # noqa: E501
         :type listener_lan: int
         """
         if self.local_vars_configuration.client_side_validation and listener_lan is None:  # noqa: E501
             raise ValueError("Invalid value for `listener_lan`, must not be `None`")  # noqa: E501
 
         self._listener_lan = listener_lan
 
     @property
     def ips(self):
         """Gets the ips of this ApplicationLoadBalancerProperties.  # noqa: E501
 
-        Collection of the Application Load Balancer IP addresses. (Inbound and outbound) IPs of the listenerLan are customer-reserved public IPs for the public Load Balancers, and private IPs for the private Load Balancers.  # noqa: E501
+        Collection of the Application Load Balancer IP addresses. (Inbound and outbound) IPs of the 'listenerLan' are customer-reserved public IPs for the public load balancers, and private IPs for the private load balancers.  # noqa: E501
 
         :return: The ips of this ApplicationLoadBalancerProperties.  # noqa: E501
         :rtype: list[str]
         """
         return self._ips
 
     @ips.setter
     def ips(self, ips):
         """Sets the ips of this ApplicationLoadBalancerProperties.
 
-        Collection of the Application Load Balancer IP addresses. (Inbound and outbound) IPs of the listenerLan are customer-reserved public IPs for the public Load Balancers, and private IPs for the private Load Balancers.  # noqa: E501
+        Collection of the Application Load Balancer IP addresses. (Inbound and outbound) IPs of the 'listenerLan' are customer-reserved public IPs for the public load balancers, and private IPs for the private load balancers.  # noqa: E501
 
         :param ips: The ips of this ApplicationLoadBalancerProperties.  # noqa: E501
         :type ips: list[str]
         """
 
         self._ips = ips
 
     @property
     def target_lan(self):
         """Gets the target_lan of this ApplicationLoadBalancerProperties.  # noqa: E501
 
-        ID of the balanced private target LAN (outbound).  # noqa: E501
+        The ID of the balanced private target LAN (outbound).  # noqa: E501
 
         :return: The target_lan of this ApplicationLoadBalancerProperties.  # noqa: E501
         :rtype: int
         """
         return self._target_lan
 
     @target_lan.setter
     def target_lan(self, target_lan):
         """Sets the target_lan of this ApplicationLoadBalancerProperties.
 
-        ID of the balanced private target LAN (outbound).  # noqa: E501
+        The ID of the balanced private target LAN (outbound).  # noqa: E501
 
         :param target_lan: The target_lan of this ApplicationLoadBalancerProperties.  # noqa: E501
         :type target_lan: int
         """
         if self.local_vars_configuration.client_side_validation and target_lan is None:  # noqa: E501
             raise ValueError("Invalid value for `target_lan`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancer_put.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancer_put.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,26 +121,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this ApplicationLoadBalancerPut.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this ApplicationLoadBalancerPut.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this ApplicationLoadBalancerPut.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this ApplicationLoadBalancerPut.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/application_load_balancers.py` & `ionoscloud-6.1.5/ionoscloud/models/application_load_balancers.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,26 +143,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this ApplicationLoadBalancers.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this ApplicationLoadBalancers.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this ApplicationLoadBalancers.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this ApplicationLoadBalancers.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/attached_volumes.py` & `ionoscloud-6.1.5/ionoscloud/models/attached_volumes.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,26 +143,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this AttachedVolumes.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this AttachedVolumes.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this AttachedVolumes.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this AttachedVolumes.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/backup_unit.py` & `ionoscloud-6.1.5/ionoscloud/models/backup_unit.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/backup_unit_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/backup_unit_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/backup_unit_sso.py` & `ionoscloud-6.1.5/ionoscloud/models/backup_unit_sso.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/backup_units.py` & `ionoscloud-6.1.5/ionoscloud/models/backup_units.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/balanced_nics.py` & `ionoscloud-6.1.5/ionoscloud/models/balanced_nics.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/cdroms.py` & `ionoscloud-6.1.5/ionoscloud/models/cdroms.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/connectable_datacenter.py` & `ionoscloud-6.1.5/ionoscloud/models/connectable_datacenter.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/contract.py` & `ionoscloud-6.1.5/ionoscloud/models/contract.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/contract_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/contract_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,49 +106,49 @@
 
         self._contract_number = contract_number
 
     @property
     def owner(self):
         """Gets the owner of this ContractProperties.  # noqa: E501
 
-        The owner of the contract.  # noqa: E501
+        The contract owner's user name.  # noqa: E501
 
         :return: The owner of this ContractProperties.  # noqa: E501
         :rtype: str
         """
         return self._owner
 
     @owner.setter
     def owner(self, owner):
         """Sets the owner of this ContractProperties.
 
-        The owner of the contract.  # noqa: E501
+        The contract owner's user name.  # noqa: E501
 
         :param owner: The owner of this ContractProperties.  # noqa: E501
         :type owner: str
         """
 
         self._owner = owner
 
     @property
     def status(self):
         """Gets the status of this ContractProperties.  # noqa: E501
 
-        The status of the contract.  # noqa: E501
+        The contract status.  # noqa: E501
 
         :return: The status of this ContractProperties.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this ContractProperties.
 
-        The status of the contract.  # noqa: E501
+        The contract status.  # noqa: E501
 
         :param status: The status of this ContractProperties.  # noqa: E501
         :type status: str
         """
 
         self._status = status
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/contracts.py` & `ionoscloud-6.1.5/ionoscloud/models/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,26 +122,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this Contracts.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this Contracts.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this Contracts.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this Contracts.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/cpu_architecture_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/cpu_architecture_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/data_center_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/data_center_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/datacenter.py` & `ionoscloud-6.1.5/ionoscloud/models/datacenter.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/datacenter_element_metadata.py` & `ionoscloud-6.1.5/ionoscloud/models/datacenter_element_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,31 +265,31 @@
 
         self._last_modified_by_user_id = last_modified_by_user_id
 
     @property
     def state(self):
         """Gets the state of this DatacenterElementMetadata.  # noqa: E501
 
-        State of the resource. *AVAILABLE* There are no pending modification requests for this item; *BUSY* There is at least one modification request pending and all following requests will be queued; *INACTIVE* Resource has been de-provisioned; *DEPLOYING* Resource state DEPLOYING - relevant for Kubernetes cluster/nodepool; *ACTIVE* Resource state ACTIVE - relevant for Kubernetes cluster/nodepool; *FAILED* Resource state FAILED - relevant for Kubernetes cluster/nodepool; *SUSPENDED* Resource state SUSPENDED - relevant for Kubernetes cluster/nodepool; *FAILED_SUSPENDED* Resource state FAILED_SUSPENDED - relevant for Kubernetes cluster; *UPDATING* Resource state UPDATING - relevant for Kubernetes cluster/nodepool; *FAILED_UPDATING* Resource state FAILED_UPDATING - relevant for Kubernetes cluster/nodepool; *DESTROYING* Resource state DESTROYING - relevant for Kubernetes cluster; *FAILED_DESTROYING* Resource state FAILED_DESTROYING - relevant for Kubernetes cluster/nodepool; *TERMINATED* Resource state TERMINATED - relevant for Kubernetes cluster/nodepool.  # noqa: E501
+        State of the resource. *AVAILABLE* There are no pending modification requests for this item; *BUSY* There is at least one modification request pending and all following requests will be queued; *INACTIVE* Resource has been de-provisioned; *DEPLOYING* Resource state DEPLOYING - relevant for Kubernetes cluster/nodepool; *ACTIVE* Resource state ACTIVE - relevant for Kubernetes cluster/nodepool; *FAILED* Resource state FAILED - relevant for Kubernetes cluster/nodepool; *SUSPENDED* Resource state SUSPENDED - relevant for Kubernetes cluster/nodepool; *FAILED_SUSPENDED* Resource state FAILED_SUSPENDED - relevant for Kubernetes cluster; *UPDATING* Resource state UPDATING - relevant for Kubernetes cluster/nodepool; *FAILED_UPDATING* Resource state FAILED_UPDATING - relevant for Kubernetes cluster/nodepool; *DESTROYING* Resource state DESTROYING - relevant for Kubernetes cluster; *FAILED_DESTROYING* Resource state FAILED_DESTROYING - relevant for Kubernetes cluster/nodepool; *TERMINATED* Resource state TERMINATED - relevant for Kubernetes cluster/nodepool; *HIBERNATING* Resource state HIBERNATING - relevant for Kubernetes cluster/nodepool; *FAILED_HIBERNATING* Resource state FAILED_HIBERNATING - relevant for Kubernetes cluster/nodepool; *MAINTENANCE* Resource state MAINTENANCE - relevant for Kubernetes cluster/nodepool; *FAILED_HIBERNATING* Resource state FAILED_HIBERNATING - relevant for Kubernetes cluster/nodepool.  # noqa: E501
 
         :return: The state of this DatacenterElementMetadata.  # noqa: E501
         :rtype: str
         """
         return self._state
 
     @state.setter
     def state(self, state):
         """Sets the state of this DatacenterElementMetadata.
 
-        State of the resource. *AVAILABLE* There are no pending modification requests for this item; *BUSY* There is at least one modification request pending and all following requests will be queued; *INACTIVE* Resource has been de-provisioned; *DEPLOYING* Resource state DEPLOYING - relevant for Kubernetes cluster/nodepool; *ACTIVE* Resource state ACTIVE - relevant for Kubernetes cluster/nodepool; *FAILED* Resource state FAILED - relevant for Kubernetes cluster/nodepool; *SUSPENDED* Resource state SUSPENDED - relevant for Kubernetes cluster/nodepool; *FAILED_SUSPENDED* Resource state FAILED_SUSPENDED - relevant for Kubernetes cluster; *UPDATING* Resource state UPDATING - relevant for Kubernetes cluster/nodepool; *FAILED_UPDATING* Resource state FAILED_UPDATING - relevant for Kubernetes cluster/nodepool; *DESTROYING* Resource state DESTROYING - relevant for Kubernetes cluster; *FAILED_DESTROYING* Resource state FAILED_DESTROYING - relevant for Kubernetes cluster/nodepool; *TERMINATED* Resource state TERMINATED - relevant for Kubernetes cluster/nodepool.  # noqa: E501
+        State of the resource. *AVAILABLE* There are no pending modification requests for this item; *BUSY* There is at least one modification request pending and all following requests will be queued; *INACTIVE* Resource has been de-provisioned; *DEPLOYING* Resource state DEPLOYING - relevant for Kubernetes cluster/nodepool; *ACTIVE* Resource state ACTIVE - relevant for Kubernetes cluster/nodepool; *FAILED* Resource state FAILED - relevant for Kubernetes cluster/nodepool; *SUSPENDED* Resource state SUSPENDED - relevant for Kubernetes cluster/nodepool; *FAILED_SUSPENDED* Resource state FAILED_SUSPENDED - relevant for Kubernetes cluster; *UPDATING* Resource state UPDATING - relevant for Kubernetes cluster/nodepool; *FAILED_UPDATING* Resource state FAILED_UPDATING - relevant for Kubernetes cluster/nodepool; *DESTROYING* Resource state DESTROYING - relevant for Kubernetes cluster; *FAILED_DESTROYING* Resource state FAILED_DESTROYING - relevant for Kubernetes cluster/nodepool; *TERMINATED* Resource state TERMINATED - relevant for Kubernetes cluster/nodepool; *HIBERNATING* Resource state HIBERNATING - relevant for Kubernetes cluster/nodepool; *FAILED_HIBERNATING* Resource state FAILED_HIBERNATING - relevant for Kubernetes cluster/nodepool; *MAINTENANCE* Resource state MAINTENANCE - relevant for Kubernetes cluster/nodepool; *FAILED_HIBERNATING* Resource state FAILED_HIBERNATING - relevant for Kubernetes cluster/nodepool.  # noqa: E501
 
         :param state: The state of this DatacenterElementMetadata.  # noqa: E501
         :type state: str
         """
-        allowed_values = ["AVAILABLE", "INACTIVE", "BUSY", "DEPLOYING", "ACTIVE", "FAILED", "SUSPENDED", "FAILED_SUSPENDED", "UPDATING", "FAILED_UPDATING", "DESTROYING", "FAILED_DESTROYING", "TERMINATED"]  # noqa: E501
+        allowed_values = ["AVAILABLE", "INACTIVE", "BUSY", "DEPLOYING", "ACTIVE", "FAILED", "SUSPENDED", "FAILED_SUSPENDED", "UPDATING", "FAILED_UPDATING", "DESTROYING", "FAILED_DESTROYING", "TERMINATED", "HIBERNATING", "FAILED_HIBERNATING", "MAINTENANCE", "FAILED_MAINTENANCE", "UNKNOWN"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and state not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `state` ({0}), must be one of {1}"  # noqa: E501
                 .format(state, allowed_values)
             )
 
         self._state = state
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/datacenter_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/datacenter_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/datacenters.py` & `ionoscloud-6.1.5/ionoscloud/models/datacenters.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/error.py` & `ionoscloud-6.1.5/ionoscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/error_message.py` & `ionoscloud-6.1.5/ionoscloud/models/error_message.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/firewall_rule.py` & `ionoscloud-6.1.5/ionoscloud/models/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/firewall_rules.py` & `ionoscloud-6.1.5/ionoscloud/models/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/firewallrule_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/firewallrule_properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
         'name': 'str',
 
         'protocol': 'str',
 
         'source_mac': 'str',
 
+        'ip_version': 'str',
+
         'source_ip': 'str',
 
         'target_ip': 'str',
 
         'icmp_code': 'int',
 
         'icmp_type': 'int',
@@ -59,14 +61,16 @@
 
         'name': 'name',
 
         'protocol': 'protocol',
 
         'source_mac': 'sourceMac',
 
+        'ip_version': 'ipVersion',
+
         'source_ip': 'sourceIp',
 
         'target_ip': 'targetIp',
 
         'icmp_code': 'icmpCode',
 
         'icmp_type': 'icmpType',
@@ -74,36 +78,39 @@
         'port_range_start': 'portRangeStart',
 
         'port_range_end': 'portRangeEnd',
 
         'type': 'type',
     }
 
-    def __init__(self, name=None, protocol=None, source_mac=None, source_ip=None, target_ip=None, icmp_code=None, icmp_type=None, port_range_start=None, port_range_end=None, type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, protocol=None, source_mac=None, ip_version=None, source_ip=None, target_ip=None, icmp_code=None, icmp_type=None, port_range_start=None, port_range_end=None, type=None, local_vars_configuration=None):  # noqa: E501
         """FirewallruleProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._protocol = None
         self._source_mac = None
+        self._ip_version = None
         self._source_ip = None
         self._target_ip = None
         self._icmp_code = None
         self._icmp_type = None
         self._port_range_start = None
         self._port_range_end = None
         self._type = None
         self.discriminator = None
 
         if name is not None:
             self.name = name
         self.protocol = protocol
         self.source_mac = source_mac
+        if ip_version is not None:
+            self.ip_version = ip_version
         self.source_ip = source_ip
         self.target_ip = target_ip
         self.icmp_code = icmp_code
         self.icmp_type = icmp_type
         if port_range_start is not None:
             self.port_range_start = port_range_start
         if port_range_end is not None:
@@ -153,15 +160,15 @@
         The protocol for the rule. Property cannot be modified after it is created (disallowed in update requests).  # noqa: E501
 
         :param protocol: The protocol of this FirewallruleProperties.  # noqa: E501
         :type protocol: str
         """
         if self.local_vars_configuration.client_side_validation and protocol is None:  # noqa: E501
             raise ValueError("Invalid value for `protocol`, must not be `None`")  # noqa: E501
-        allowed_values = ["TCP", "UDP", "ICMP", "ANY"]  # noqa: E501
+        allowed_values = ["TCP", "UDP", "ICMP", "ICMPv6", "ANY"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and protocol not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `protocol` ({0}), must be one of {1}"  # noqa: E501
                 .format(protocol, allowed_values)
             )
 
         self._protocol = protocol
@@ -182,88 +189,108 @@
         """Sets the source_mac of this FirewallruleProperties.
 
         Only traffic originating from the respective MAC address is allowed. Valid format: aa:bb:cc:dd:ee:ff. Value null allows traffic from any MAC address.  # noqa: E501
 
         :param source_mac: The source_mac of this FirewallruleProperties.  # noqa: E501
         :type source_mac: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                source_mac is not None and not re.search(r'^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$', source_mac)):  # noqa: E501
-            raise ValueError(r"Invalid value for `source_mac`, must be a follow pattern or equal to `/^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$/`")  # noqa: E501
 
         self._source_mac = source_mac
 
     @property
+    def ip_version(self):
+        """Gets the ip_version of this FirewallruleProperties.  # noqa: E501
+
+        The IP version for this rule. If sourceIp or targetIp are specified, you can omit this value - the IP version will then be deduced from the IP address(es) used; if you specify it anyway, it must match the specified IP address(es). If neither sourceIp nor targetIp are specified, this rule allows traffic only for the specified IP version. If neither sourceIp, targetIp nor ipVersion are specified, this rule will only allow IPv4 traffic.  # noqa: E501
+
+        :return: The ip_version of this FirewallruleProperties.  # noqa: E501
+        :rtype: str
+        """
+        return self._ip_version
+
+    @ip_version.setter
+    def ip_version(self, ip_version):
+        """Sets the ip_version of this FirewallruleProperties.
+
+        The IP version for this rule. If sourceIp or targetIp are specified, you can omit this value - the IP version will then be deduced from the IP address(es) used; if you specify it anyway, it must match the specified IP address(es). If neither sourceIp nor targetIp are specified, this rule allows traffic only for the specified IP version. If neither sourceIp, targetIp nor ipVersion are specified, this rule will only allow IPv4 traffic.  # noqa: E501
+
+        :param ip_version: The ip_version of this FirewallruleProperties.  # noqa: E501
+        :type ip_version: str
+        """
+        allowed_values = ["IPv4", "IPv6"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and ip_version not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `ip_version` ({0}), must be one of {1}"  # noqa: E501
+                .format(ip_version, allowed_values)
+            )
+
+        self._ip_version = ip_version
+
+    @property
     def source_ip(self):
         """Gets the source_ip of this FirewallruleProperties.  # noqa: E501
 
-        Only traffic originating from the respective IPv4 address is allowed. Value null allows traffic from any IP address.  # noqa: E501
+        Only traffic originating from the respective IP address (or CIDR block) is allowed. Value null allows traffic from any IP address (according to the selected ipVersion).  # noqa: E501
 
         :return: The source_ip of this FirewallruleProperties.  # noqa: E501
         :rtype: str
         """
         return self._source_ip
 
     @source_ip.setter
     def source_ip(self, source_ip):
         """Sets the source_ip of this FirewallruleProperties.
 
-        Only traffic originating from the respective IPv4 address is allowed. Value null allows traffic from any IP address.  # noqa: E501
+        Only traffic originating from the respective IP address (or CIDR block) is allowed. Value null allows traffic from any IP address (according to the selected ipVersion).  # noqa: E501
 
         :param source_ip: The source_ip of this FirewallruleProperties.  # noqa: E501
         :type source_ip: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                source_ip is not None and not re.search(r'^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$', source_ip)):  # noqa: E501
-            raise ValueError(r"Invalid value for `source_ip`, must be a follow pattern or equal to `/^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/`")  # noqa: E501
 
         self._source_ip = source_ip
 
     @property
     def target_ip(self):
         """Gets the target_ip of this FirewallruleProperties.  # noqa: E501
 
-        If the target NIC has multiple IP addresses, only the traffic directed to the respective IP address of the NIC is allowed. Value null Value null allows traffic to any target IP address.  # noqa: E501
+        If the target NIC has multiple IP addresses, only the traffic directed to the respective IP address (or CIDR block) of the NIC is allowed. Value null allows traffic to any target IP address (according to the selected ipVersion).  # noqa: E501
 
         :return: The target_ip of this FirewallruleProperties.  # noqa: E501
         :rtype: str
         """
         return self._target_ip
 
     @target_ip.setter
     def target_ip(self, target_ip):
         """Sets the target_ip of this FirewallruleProperties.
 
-        If the target NIC has multiple IP addresses, only the traffic directed to the respective IP address of the NIC is allowed. Value null Value null allows traffic to any target IP address.  # noqa: E501
+        If the target NIC has multiple IP addresses, only the traffic directed to the respective IP address (or CIDR block) of the NIC is allowed. Value null allows traffic to any target IP address (according to the selected ipVersion).  # noqa: E501
 
         :param target_ip: The target_ip of this FirewallruleProperties.  # noqa: E501
         :type target_ip: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                target_ip is not None and not re.search(r'^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$', target_ip)):  # noqa: E501
-            raise ValueError(r"Invalid value for `target_ip`, must be a follow pattern or equal to `/^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/`")  # noqa: E501
 
         self._target_ip = target_ip
 
     @property
     def icmp_code(self):
         """Gets the icmp_code of this FirewallruleProperties.  # noqa: E501
 
-        Defines the allowed code (from 0 to 254) if protocol ICMP is chosen. Value null allows all codes.  # noqa: E501
+        Defines the allowed code (from 0 to 254) if protocol ICMP or ICMPv6 is chosen. Value null allows all codes.  # noqa: E501
 
         :return: The icmp_code of this FirewallruleProperties.  # noqa: E501
         :rtype: int
         """
         return self._icmp_code
 
     @icmp_code.setter
     def icmp_code(self, icmp_code):
         """Sets the icmp_code of this FirewallruleProperties.
 
-        Defines the allowed code (from 0 to 254) if protocol ICMP is chosen. Value null allows all codes.  # noqa: E501
+        Defines the allowed code (from 0 to 254) if protocol ICMP or ICMPv6 is chosen. Value null allows all codes.  # noqa: E501
 
         :param icmp_code: The icmp_code of this FirewallruleProperties.  # noqa: E501
         :type icmp_code: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 icmp_code is not None and icmp_code > 254):  # noqa: E501
             raise ValueError("Invalid value for `icmp_code`, must be a value less than or equal to `254`")  # noqa: E501
@@ -273,26 +300,26 @@
 
         self._icmp_code = icmp_code
 
     @property
     def icmp_type(self):
         """Gets the icmp_type of this FirewallruleProperties.  # noqa: E501
 
-        Defines the allowed type (from 0 to 254) if the protocol ICMP is chosen. Value null allows all types.  # noqa: E501
+        Defines the allowed type (from 0 to 254) if the protocol ICMP or ICMPv6 is chosen. Value null allows all types.  # noqa: E501
 
         :return: The icmp_type of this FirewallruleProperties.  # noqa: E501
         :rtype: int
         """
         return self._icmp_type
 
     @icmp_type.setter
     def icmp_type(self, icmp_type):
         """Sets the icmp_type of this FirewallruleProperties.
 
-        Defines the allowed type (from 0 to 254) if the protocol ICMP is chosen. Value null allows all types.  # noqa: E501
+        Defines the allowed type (from 0 to 254) if the protocol ICMP or ICMPv6 is chosen. Value null allows all types.  # noqa: E501
 
         :param icmp_type: The icmp_type of this FirewallruleProperties.  # noqa: E501
         :type icmp_type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 icmp_type is not None and icmp_type > 254):  # noqa: E501
             raise ValueError("Invalid value for `icmp_type`, must be a value less than or equal to `254`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/flow_log.py` & `ionoscloud-6.1.5/ionoscloud/models/flow_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this FlowLog.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this FlowLog.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this FlowLog.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this FlowLog.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/flow_log_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/flow_log_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,26 +72,26 @@
         self.bucket = bucket
 
 
     @property
     def name(self):
         """Gets the name of this FlowLogProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The resource name.  # noqa: E501
 
         :return: The name of this FlowLogProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this FlowLogProperties.
 
-        The name of the  resource.  # noqa: E501
+        The resource name.  # noqa: E501
 
         :param name: The name of this FlowLogProperties.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
@@ -159,26 +159,26 @@
 
         self._direction = direction
 
     @property
     def bucket(self):
         """Gets the bucket of this FlowLogProperties.  # noqa: E501
 
-        S3 bucket name of an existing IONOS Cloud S3 bucket.  # noqa: E501
+        The S3 bucket name of an existing IONOS Cloud S3 bucket.  # noqa: E501
 
         :return: The bucket of this FlowLogProperties.  # noqa: E501
         :rtype: str
         """
         return self._bucket
 
     @bucket.setter
     def bucket(self, bucket):
         """Sets the bucket of this FlowLogProperties.
 
-        S3 bucket name of an existing IONOS Cloud S3 bucket.  # noqa: E501
+        The S3 bucket name of an existing IONOS Cloud S3 bucket.  # noqa: E501
 
         :param bucket: The bucket of this FlowLogProperties.  # noqa: E501
         :type bucket: str
         """
         if self.local_vars_configuration.client_side_validation and bucket is None:  # noqa: E501
             raise ValueError("Invalid value for `bucket`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/flow_log_put.py` & `ionoscloud-6.1.5/ionoscloud/models/flow_log_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/flow_logs.py` & `ionoscloud-6.1.5/ionoscloud/models/flow_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,26 +143,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this FlowLogs.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this FlowLogs.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this FlowLogs.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this FlowLogs.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group.py` & `ionoscloud-6.1.5/ionoscloud/models/group.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/group_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_members.py` & `ionoscloud-6.1.5/ionoscloud/models/group_members.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/group_properties.py`

 * *Files 26% similar despite different names*

```diff
@@ -57,14 +57,20 @@
         'create_flow_log': 'bool',
 
         'access_and_manage_monitoring': 'bool',
 
         'access_and_manage_certificates': 'bool',
 
         'manage_dbaas': 'bool',
+
+        'access_and_manage_dns': 'bool',
+
+        'manage_registry': 'bool',
+
+        'manage_dataplatform': 'bool',
     }
 
     attribute_map = {
 
         'name': 'name',
 
         'create_data_center': 'createDataCenter',
@@ -88,17 +94,23 @@
         'create_flow_log': 'createFlowLog',
 
         'access_and_manage_monitoring': 'accessAndManageMonitoring',
 
         'access_and_manage_certificates': 'accessAndManageCertificates',
 
         'manage_dbaas': 'manageDBaaS',
+
+        'access_and_manage_dns': 'accessAndManageDns',
+
+        'manage_registry': 'manageRegistry',
+
+        'manage_dataplatform': 'manageDataplatform',
     }
 
-    def __init__(self, name=None, create_data_center=None, create_snapshot=None, reserve_ip=None, access_activity_log=None, create_pcc=None, s3_privilege=None, create_backup_unit=None, create_internet_access=None, create_k8s_cluster=None, create_flow_log=None, access_and_manage_monitoring=None, access_and_manage_certificates=None, manage_dbaas=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, create_data_center=None, create_snapshot=None, reserve_ip=None, access_activity_log=None, create_pcc=None, s3_privilege=None, create_backup_unit=None, create_internet_access=None, create_k8s_cluster=None, create_flow_log=None, access_and_manage_monitoring=None, access_and_manage_certificates=None, manage_dbaas=None, access_and_manage_dns=None, manage_registry=None, manage_dataplatform=None, local_vars_configuration=None):  # noqa: E501
         """GroupProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._create_data_center = None
@@ -110,14 +122,17 @@
         self._create_backup_unit = None
         self._create_internet_access = None
         self._create_k8s_cluster = None
         self._create_flow_log = None
         self._access_and_manage_monitoring = None
         self._access_and_manage_certificates = None
         self._manage_dbaas = None
+        self._access_and_manage_dns = None
+        self._manage_registry = None
+        self._manage_dataplatform = None
         self.discriminator = None
 
         if name is not None:
             self.name = name
         if create_data_center is not None:
             self.create_data_center = create_data_center
         if create_snapshot is not None:
@@ -140,32 +155,38 @@
             self.create_flow_log = create_flow_log
         if access_and_manage_monitoring is not None:
             self.access_and_manage_monitoring = access_and_manage_monitoring
         if access_and_manage_certificates is not None:
             self.access_and_manage_certificates = access_and_manage_certificates
         if manage_dbaas is not None:
             self.manage_dbaas = manage_dbaas
+        if access_and_manage_dns is not None:
+            self.access_and_manage_dns = access_and_manage_dns
+        if manage_registry is not None:
+            self.manage_registry = manage_registry
+        if manage_dataplatform is not None:
+            self.manage_dataplatform = manage_dataplatform
 
 
     @property
     def name(self):
         """Gets the name of this GroupProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The name of the resource.  # noqa: E501
 
         :return: The name of this GroupProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this GroupProperties.
 
-        The name of the  resource.  # noqa: E501
+        The name of the resource.  # noqa: E501
 
         :param name: The name of this GroupProperties.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
@@ -463,14 +484,83 @@
         Privilege for a group to manage DBaaS related functionality.  # noqa: E501
 
         :param manage_dbaas: The manage_dbaas of this GroupProperties.  # noqa: E501
         :type manage_dbaas: bool
         """
 
         self._manage_dbaas = manage_dbaas
+
+    @property
+    def access_and_manage_dns(self):
+        """Gets the access_and_manage_dns of this GroupProperties.  # noqa: E501
+
+        Privilege for a group to access and manage dns records.  # noqa: E501
+
+        :return: The access_and_manage_dns of this GroupProperties.  # noqa: E501
+        :rtype: bool
+        """
+        return self._access_and_manage_dns
+
+    @access_and_manage_dns.setter
+    def access_and_manage_dns(self, access_and_manage_dns):
+        """Sets the access_and_manage_dns of this GroupProperties.
+
+        Privilege for a group to access and manage dns records.  # noqa: E501
+
+        :param access_and_manage_dns: The access_and_manage_dns of this GroupProperties.  # noqa: E501
+        :type access_and_manage_dns: bool
+        """
+
+        self._access_and_manage_dns = access_and_manage_dns
+
+    @property
+    def manage_registry(self):
+        """Gets the manage_registry of this GroupProperties.  # noqa: E501
+
+        Privilege for group accessing container registry related functionality.  # noqa: E501
+
+        :return: The manage_registry of this GroupProperties.  # noqa: E501
+        :rtype: bool
+        """
+        return self._manage_registry
+
+    @manage_registry.setter
+    def manage_registry(self, manage_registry):
+        """Sets the manage_registry of this GroupProperties.
+
+        Privilege for group accessing container registry related functionality.  # noqa: E501
+
+        :param manage_registry: The manage_registry of this GroupProperties.  # noqa: E501
+        :type manage_registry: bool
+        """
+
+        self._manage_registry = manage_registry
+
+    @property
+    def manage_dataplatform(self):
+        """Gets the manage_dataplatform of this GroupProperties.  # noqa: E501
+
+        Privilege for a group to access and manage Data Platform.  # noqa: E501
+
+        :return: The manage_dataplatform of this GroupProperties.  # noqa: E501
+        :rtype: bool
+        """
+        return self._manage_dataplatform
+
+    @manage_dataplatform.setter
+    def manage_dataplatform(self, manage_dataplatform):
+        """Sets the manage_dataplatform of this GroupProperties.
+
+        Privilege for a group to access and manage Data Platform.  # noqa: E501
+
+        :param manage_dataplatform: The manage_dataplatform of this GroupProperties.  # noqa: E501
+        :type manage_dataplatform: bool
+        """
+
+        self._manage_dataplatform = manage_dataplatform
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_share.py` & `ionoscloud-6.1.5/ionoscloud/models/group_share.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_share_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/group_share_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_shares.py` & `ionoscloud-6.1.5/ionoscloud/models/group_shares.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/group_users.py` & `ionoscloud-6.1.5/ionoscloud/models/group_users.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/groups.py` & `ionoscloud-6.1.5/ionoscloud/models/groups.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/image.py` & `ionoscloud-6.1.5/ionoscloud/models/image.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/image_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/image_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,26 +180,26 @@
             self.cloud_init = cloud_init
 
 
     @property
     def name(self):
         """Gets the name of this ImageProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The resource name.  # noqa: E501
 
         :return: The name of this ImageProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this ImageProperties.
 
-        The name of the  resource.  # noqa: E501
+        The resource name.  # noqa: E501
 
         :param name: The name of this ImageProperties.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
@@ -226,49 +226,49 @@
 
         self._description = description
 
     @property
     def location(self):
         """Gets the location of this ImageProperties.  # noqa: E501
 
-        Location of that image/snapshot.   # noqa: E501
+        The location of this image/snapshot.  # noqa: E501
 
         :return: The location of this ImageProperties.  # noqa: E501
         :rtype: str
         """
         return self._location
 
     @location.setter
     def location(self, location):
         """Sets the location of this ImageProperties.
 
-        Location of that image/snapshot.   # noqa: E501
+        The location of this image/snapshot.  # noqa: E501
 
         :param location: The location of this ImageProperties.  # noqa: E501
         :type location: str
         """
 
         self._location = location
 
     @property
     def size(self):
         """Gets the size of this ImageProperties.  # noqa: E501
 
-        The size of the image in GB.  # noqa: E501
+        The image size in GB.  # noqa: E501
 
         :return: The size of this ImageProperties.  # noqa: E501
         :rtype: float
         """
         return self._size
 
     @size.setter
     def size(self, size):
         """Sets the size of this ImageProperties.
 
-        The size of the image in GB.  # noqa: E501
+        The image size in GB.  # noqa: E501
 
         :param size: The size of this ImageProperties.  # noqa: E501
         :type size: float
         """
 
         self._size = size
 
@@ -502,26 +502,26 @@
 
         self._disc_scsi_hot_unplug = disc_scsi_hot_unplug
 
     @property
     def licence_type(self):
         """Gets the licence_type of this ImageProperties.  # noqa: E501
 
-        OS type for this image.  # noqa: E501
+        The OS type of this image.  # noqa: E501
 
         :return: The licence_type of this ImageProperties.  # noqa: E501
         :rtype: str
         """
         return self._licence_type
 
     @licence_type.setter
     def licence_type(self, licence_type):
         """Sets the licence_type of this ImageProperties.
 
-        OS type for this image.  # noqa: E501
+        The OS type of this image.  # noqa: E501
 
         :param licence_type: The licence_type of this ImageProperties.  # noqa: E501
         :type licence_type: str
         """
         if self.local_vars_configuration.client_side_validation and licence_type is None:  # noqa: E501
             raise ValueError("Invalid value for `licence_type`, must not be `None`")  # noqa: E501
         allowed_values = ["UNKNOWN", "WINDOWS", "WINDOWS2016", "WINDOWS2022", "LINUX", "OTHER"]  # noqa: E501
@@ -585,26 +585,26 @@
 
         self._public = public
 
     @property
     def image_aliases(self):
         """Gets the image_aliases of this ImageProperties.  # noqa: E501
 
-        List of image aliases mapped for this Image  # noqa: E501
+        List of image aliases mapped for this image  # noqa: E501
 
         :return: The image_aliases of this ImageProperties.  # noqa: E501
         :rtype: list[str]
         """
         return self._image_aliases
 
     @image_aliases.setter
     def image_aliases(self, image_aliases):
         """Sets the image_aliases of this ImageProperties.
 
-        List of image aliases mapped for this Image  # noqa: E501
+        List of image aliases mapped for this image  # noqa: E501
 
         :param image_aliases: The image_aliases of this ImageProperties.  # noqa: E501
         :type image_aliases: list[str]
         """
 
         self._image_aliases = image_aliases
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/images.py` & `ionoscloud-6.1.5/ionoscloud/models/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,26 +122,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this Images.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this Images.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this Images.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this Images.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/info.py` & `ionoscloud-6.1.5/ionoscloud/models/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,72 +69,72 @@
             self.version = version
 
 
     @property
     def href(self):
         """Gets the href of this Info.  # noqa: E501
 
-        API entry point  # noqa: E501
+        The API entry point.  # noqa: E501
 
         :return: The href of this Info.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this Info.
 
-        API entry point  # noqa: E501
+        The API entry point.  # noqa: E501
 
         :param href: The href of this Info.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def name(self):
         """Gets the name of this Info.  # noqa: E501
 
-        Name of the API  # noqa: E501
+        The API name.  # noqa: E501
 
         :return: The name of this Info.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this Info.
 
-        Name of the API  # noqa: E501
+        The API name.  # noqa: E501
 
         :param name: The name of this Info.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
     @property
     def version(self):
         """Gets the version of this Info.  # noqa: E501
 
-        Version of the API  # noqa: E501
+        The API version.  # noqa: E501
 
         :return: The version of this Info.  # noqa: E501
         :rtype: str
         """
         return self._version
 
     @version.setter
     def version(self, version):
         """Sets the version of this Info.
 
-        Version of the API  # noqa: E501
+        The API version.  # noqa: E501
 
         :param version: The version of this Info.  # noqa: E501
         :type version: str
         """
 
         self._version = version
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/ip_block.py` & `ionoscloud-6.1.5/ionoscloud/models/ip_block.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/ip_block_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/ip_block_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/ip_blocks.py` & `ionoscloud-6.1.5/ionoscloud/models/ip_blocks.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/ip_consumer.py` & `ionoscloud-6.1.5/ionoscloud/models/ip_consumer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/ip_failover.py` & `ionoscloud-6.1.5/ionoscloud/models/ip_failover.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_auto_scaling.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_auto_scaling.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,51 +60,51 @@
         self.max_node_count = max_node_count
 
 
     @property
     def min_node_count(self):
         """Gets the min_node_count of this KubernetesAutoScaling.  # noqa: E501
 
-        The minimum number of worker nodes that the managed node group can scale in. Should be set together with 'maxNodeCount'. Value for this attribute must be greater than equal to 1 and less than equal to maxNodeCount.  # noqa: E501
+        The minimum number of working nodes that the managed node pool can scale must be >= 1 and >= nodeCount. Required if autoScaling is specified.  # noqa: E501
 
         :return: The min_node_count of this KubernetesAutoScaling.  # noqa: E501
         :rtype: int
         """
         return self._min_node_count
 
     @min_node_count.setter
     def min_node_count(self, min_node_count):
         """Sets the min_node_count of this KubernetesAutoScaling.
 
-        The minimum number of worker nodes that the managed node group can scale in. Should be set together with 'maxNodeCount'. Value for this attribute must be greater than equal to 1 and less than equal to maxNodeCount.  # noqa: E501
+        The minimum number of working nodes that the managed node pool can scale must be >= 1 and >= nodeCount. Required if autoScaling is specified.  # noqa: E501
 
         :param min_node_count: The min_node_count of this KubernetesAutoScaling.  # noqa: E501
         :type min_node_count: int
         """
         if self.local_vars_configuration.client_side_validation and min_node_count is None:  # noqa: E501
             raise ValueError("Invalid value for `min_node_count`, must not be `None`")  # noqa: E501
 
         self._min_node_count = min_node_count
 
     @property
     def max_node_count(self):
         """Gets the max_node_count of this KubernetesAutoScaling.  # noqa: E501
 
-        The maximum number of worker nodes that the managed node pool can scale-out. Should be set together with 'minNodeCount'. Value for this attribute must be greater than equal to 1 and minNodeCount.  # noqa: E501
+        The maximum number of worker nodes that the managed node pool can scale in. Must be >= minNodeCount and must be >= nodeCount. Required if autoScaling is specified.  # noqa: E501
 
         :return: The max_node_count of this KubernetesAutoScaling.  # noqa: E501
         :rtype: int
         """
         return self._max_node_count
 
     @max_node_count.setter
     def max_node_count(self, max_node_count):
         """Sets the max_node_count of this KubernetesAutoScaling.
 
-        The maximum number of worker nodes that the managed node pool can scale-out. Should be set together with 'minNodeCount'. Value for this attribute must be greater than equal to 1 and minNodeCount.  # noqa: E501
+        The maximum number of worker nodes that the managed node pool can scale in. Must be >= minNodeCount and must be >= nodeCount. Required if autoScaling is specified.  # noqa: E501
 
         :param max_node_count: The max_node_count of this KubernetesAutoScaling.  # noqa: E501
         :type max_node_count: int
         """
         if self.local_vars_configuration.client_side_validation and max_node_count is None:  # noqa: E501
             raise ValueError("Invalid value for `max_node_count`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,49 +89,49 @@
             self.entities = entities
 
 
     @property
     def id(self):
         """Gets the id of this KubernetesCluster.  # noqa: E501
 
-        The resource's unique identifier.  # noqa: E501
+        The resource unique identifier.  # noqa: E501
 
         :return: The id of this KubernetesCluster.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this KubernetesCluster.
 
-        The resource's unique identifier.  # noqa: E501
+        The resource unique identifier.  # noqa: E501
 
         :param id: The id of this KubernetesCluster.  # noqa: E501
         :type id: str
         """
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesCluster.  # noqa: E501
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :return: The type of this KubernetesCluster.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesCluster.
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :param type: The type of this KubernetesCluster.  # noqa: E501
         :type type: str
         """
         allowed_values = ["k8s"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -141,26 +141,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesCluster.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesCluster.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesCluster.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesCluster.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_for_post.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_for_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,49 +89,49 @@
             self.entities = entities
 
 
     @property
     def id(self):
         """Gets the id of this KubernetesClusterForPost.  # noqa: E501
 
-        The resource's unique identifier.  # noqa: E501
+        The resource unique identifier.  # noqa: E501
 
         :return: The id of this KubernetesClusterForPost.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this KubernetesClusterForPost.
 
-        The resource's unique identifier.  # noqa: E501
+        The resource unique identifier.  # noqa: E501
 
         :param id: The id of this KubernetesClusterForPost.  # noqa: E501
         :type id: str
         """
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesClusterForPost.  # noqa: E501
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :return: The type of this KubernetesClusterForPost.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesClusterForPost.
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :param type: The type of this KubernetesClusterForPost.  # noqa: E501
         :type type: str
         """
         allowed_values = ["k8s"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -141,26 +141,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesClusterForPost.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesClusterForPost.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesClusterForPost.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesClusterForPost.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_for_put.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_for_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_properties_for_post.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_properties_for_put.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class KubernetesClusterPropertiesForPost(object):
+class KubernetesClusterPropertiesForPut(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -55,15 +55,15 @@
 
         'api_subnet_allow_list': 'apiSubnetAllowList',
 
         's3_buckets': 's3Buckets',
     }
 
     def __init__(self, name=None, k8s_version=None, maintenance_window=None, api_subnet_allow_list=None, s3_buckets=None, local_vars_configuration=None):  # noqa: E501
-        """KubernetesClusterPropertiesForPost - a model defined in OpenAPI"""  # noqa: E501
+        """KubernetesClusterPropertiesForPut - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._k8s_version = None
         self._maintenance_window = None
@@ -80,122 +80,122 @@
             self.api_subnet_allow_list = api_subnet_allow_list
         if s3_buckets is not None:
             self.s3_buckets = s3_buckets
 
 
     @property
     def name(self):
-        """Gets the name of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        """Gets the name of this KubernetesClusterPropertiesForPut.  # noqa: E501
 
         A Kubernetes cluster name. Valid Kubernetes cluster name must be 63 characters or less and must be empty or begin and end with an alphanumeric character ([a-z0-9A-Z]) with dashes (-), underscores (_), dots (.), and alphanumerics between.  # noqa: E501
 
-        :return: The name of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :return: The name of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this KubernetesClusterPropertiesForPost.
+        """Sets the name of this KubernetesClusterPropertiesForPut.
 
         A Kubernetes cluster name. Valid Kubernetes cluster name must be 63 characters or less and must be empty or begin and end with an alphanumeric character ([a-z0-9A-Z]) with dashes (-), underscores (_), dots (.), and alphanumerics between.  # noqa: E501
 
-        :param name: The name of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :param name: The name of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def k8s_version(self):
-        """Gets the k8s_version of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        """Gets the k8s_version of this KubernetesClusterPropertiesForPut.  # noqa: E501
 
-        The Kubernetes version the cluster is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version that the cluster is running. This limits which Kubernetes versions can run in a cluster's node pools. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
-        :return: The k8s_version of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :return: The k8s_version of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :rtype: str
         """
         return self._k8s_version
 
     @k8s_version.setter
     def k8s_version(self, k8s_version):
-        """Sets the k8s_version of this KubernetesClusterPropertiesForPost.
+        """Sets the k8s_version of this KubernetesClusterPropertiesForPut.
 
-        The Kubernetes version the cluster is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version that the cluster is running. This limits which Kubernetes versions can run in a cluster's node pools. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
-        :param k8s_version: The k8s_version of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :param k8s_version: The k8s_version of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :type k8s_version: str
         """
 
         self._k8s_version = k8s_version
 
     @property
     def maintenance_window(self):
-        """Gets the maintenance_window of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        """Gets the maintenance_window of this KubernetesClusterPropertiesForPut.  # noqa: E501
 
 
-        :return: The maintenance_window of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :return: The maintenance_window of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :rtype: KubernetesMaintenanceWindow
         """
         return self._maintenance_window
 
     @maintenance_window.setter
     def maintenance_window(self, maintenance_window):
-        """Sets the maintenance_window of this KubernetesClusterPropertiesForPost.
+        """Sets the maintenance_window of this KubernetesClusterPropertiesForPut.
 
 
-        :param maintenance_window: The maintenance_window of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :param maintenance_window: The maintenance_window of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :type maintenance_window: KubernetesMaintenanceWindow
         """
 
         self._maintenance_window = maintenance_window
 
     @property
     def api_subnet_allow_list(self):
-        """Gets the api_subnet_allow_list of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        """Gets the api_subnet_allow_list of this KubernetesClusterPropertiesForPut.  # noqa: E501
 
-        Access to the K8s API server is restricted to these CIDRs. Traffic, internal to the cluster, is not affected by this restriction. If no allowlist is specified, access is not restricted. If an IP without subnet mask is provided, the default value is used: 32 for IPv4 and 128 for IPv6.  # noqa: E501
+        Access to the K8s API server is restricted to these CIDRs. Intra-cluster traffic is not affected by this restriction. If no AllowList is specified, access is not limited. If an IP is specified without a subnet mask, the default value is 32 for IPv4 and 128 for IPv6.  # noqa: E501
 
-        :return: The api_subnet_allow_list of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :return: The api_subnet_allow_list of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :rtype: list[str]
         """
         return self._api_subnet_allow_list
 
     @api_subnet_allow_list.setter
     def api_subnet_allow_list(self, api_subnet_allow_list):
-        """Sets the api_subnet_allow_list of this KubernetesClusterPropertiesForPost.
+        """Sets the api_subnet_allow_list of this KubernetesClusterPropertiesForPut.
 
-        Access to the K8s API server is restricted to these CIDRs. Traffic, internal to the cluster, is not affected by this restriction. If no allowlist is specified, access is not restricted. If an IP without subnet mask is provided, the default value is used: 32 for IPv4 and 128 for IPv6.  # noqa: E501
+        Access to the K8s API server is restricted to these CIDRs. Intra-cluster traffic is not affected by this restriction. If no AllowList is specified, access is not limited. If an IP is specified without a subnet mask, the default value is 32 for IPv4 and 128 for IPv6.  # noqa: E501
 
-        :param api_subnet_allow_list: The api_subnet_allow_list of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :param api_subnet_allow_list: The api_subnet_allow_list of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :type api_subnet_allow_list: list[str]
         """
 
         self._api_subnet_allow_list = api_subnet_allow_list
 
     @property
     def s3_buckets(self):
-        """Gets the s3_buckets of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        """Gets the s3_buckets of this KubernetesClusterPropertiesForPut.  # noqa: E501
 
-        List of S3 bucket configured for K8s usage. For now it contains only an S3 bucket used to store K8s API audit logs  # noqa: E501
+        List of S3 buckets configured for K8s usage. At the moment, it contains only one S3 bucket that is used to store K8s API audit logs.  # noqa: E501
 
-        :return: The s3_buckets of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :return: The s3_buckets of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :rtype: list[S3Bucket]
         """
         return self._s3_buckets
 
     @s3_buckets.setter
     def s3_buckets(self, s3_buckets):
-        """Sets the s3_buckets of this KubernetesClusterPropertiesForPost.
+        """Sets the s3_buckets of this KubernetesClusterPropertiesForPut.
 
-        List of S3 bucket configured for K8s usage. For now it contains only an S3 bucket used to store K8s API audit logs  # noqa: E501
+        List of S3 buckets configured for K8s usage. At the moment, it contains only one S3 bucket that is used to store K8s API audit logs.  # noqa: E501
 
-        :param s3_buckets: The s3_buckets of this KubernetesClusterPropertiesForPost.  # noqa: E501
+        :param s3_buckets: The s3_buckets of this KubernetesClusterPropertiesForPut.  # noqa: E501
         :type s3_buckets: list[S3Bucket]
         """
 
         self._s3_buckets = s3_buckets
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -226,18 +226,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, KubernetesClusterPropertiesForPost):
+        if not isinstance(other, KubernetesClusterPropertiesForPut):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, KubernetesClusterPropertiesForPost):
+        if not isinstance(other, KubernetesClusterPropertiesForPut):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_cluster_properties_for_put.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_cluster_properties_for_post.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud.configuration import Configuration
 
 
-class KubernetesClusterPropertiesForPut(object):
+class KubernetesClusterPropertiesForPost(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -55,15 +55,15 @@
 
         'api_subnet_allow_list': 'apiSubnetAllowList',
 
         's3_buckets': 's3Buckets',
     }
 
     def __init__(self, name=None, k8s_version=None, maintenance_window=None, api_subnet_allow_list=None, s3_buckets=None, local_vars_configuration=None):  # noqa: E501
-        """KubernetesClusterPropertiesForPut - a model defined in OpenAPI"""  # noqa: E501
+        """KubernetesClusterPropertiesForPost - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._k8s_version = None
         self._maintenance_window = None
@@ -80,122 +80,122 @@
             self.api_subnet_allow_list = api_subnet_allow_list
         if s3_buckets is not None:
             self.s3_buckets = s3_buckets
 
 
     @property
     def name(self):
-        """Gets the name of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        """Gets the name of this KubernetesClusterPropertiesForPost.  # noqa: E501
 
         A Kubernetes cluster name. Valid Kubernetes cluster name must be 63 characters or less and must be empty or begin and end with an alphanumeric character ([a-z0-9A-Z]) with dashes (-), underscores (_), dots (.), and alphanumerics between.  # noqa: E501
 
-        :return: The name of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :return: The name of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this KubernetesClusterPropertiesForPut.
+        """Sets the name of this KubernetesClusterPropertiesForPost.
 
         A Kubernetes cluster name. Valid Kubernetes cluster name must be 63 characters or less and must be empty or begin and end with an alphanumeric character ([a-z0-9A-Z]) with dashes (-), underscores (_), dots (.), and alphanumerics between.  # noqa: E501
 
-        :param name: The name of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :param name: The name of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def k8s_version(self):
-        """Gets the k8s_version of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        """Gets the k8s_version of this KubernetesClusterPropertiesForPost.  # noqa: E501
 
-        The Kubernetes version the cluster is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version that the cluster is running. This limits which Kubernetes versions can run in a cluster's node pools. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
-        :return: The k8s_version of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :return: The k8s_version of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :rtype: str
         """
         return self._k8s_version
 
     @k8s_version.setter
     def k8s_version(self, k8s_version):
-        """Sets the k8s_version of this KubernetesClusterPropertiesForPut.
+        """Sets the k8s_version of this KubernetesClusterPropertiesForPost.
 
-        The Kubernetes version the cluster is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version that the cluster is running. This limits which Kubernetes versions can run in a cluster's node pools. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
-        :param k8s_version: The k8s_version of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :param k8s_version: The k8s_version of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :type k8s_version: str
         """
 
         self._k8s_version = k8s_version
 
     @property
     def maintenance_window(self):
-        """Gets the maintenance_window of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        """Gets the maintenance_window of this KubernetesClusterPropertiesForPost.  # noqa: E501
 
 
-        :return: The maintenance_window of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :return: The maintenance_window of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :rtype: KubernetesMaintenanceWindow
         """
         return self._maintenance_window
 
     @maintenance_window.setter
     def maintenance_window(self, maintenance_window):
-        """Sets the maintenance_window of this KubernetesClusterPropertiesForPut.
+        """Sets the maintenance_window of this KubernetesClusterPropertiesForPost.
 
 
-        :param maintenance_window: The maintenance_window of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :param maintenance_window: The maintenance_window of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :type maintenance_window: KubernetesMaintenanceWindow
         """
 
         self._maintenance_window = maintenance_window
 
     @property
     def api_subnet_allow_list(self):
-        """Gets the api_subnet_allow_list of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        """Gets the api_subnet_allow_list of this KubernetesClusterPropertiesForPost.  # noqa: E501
 
-        Access to the K8s API server is restricted to these CIDRs. Traffic, internal to the cluster, is not affected by this restriction. If no allowlist is specified, access is not restricted. If an IP without subnet mask is provided, the default value is used: 32 for IPv4 and 128 for IPv6.  # noqa: E501
+        Access to the K8s API server is restricted to these CIDRs. Intra-cluster traffic is not affected by this restriction. If no AllowList is specified, access is not limited. If an IP is specified without a subnet mask, the default value is 32 for IPv4 and 128 for IPv6.  # noqa: E501
 
-        :return: The api_subnet_allow_list of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :return: The api_subnet_allow_list of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :rtype: list[str]
         """
         return self._api_subnet_allow_list
 
     @api_subnet_allow_list.setter
     def api_subnet_allow_list(self, api_subnet_allow_list):
-        """Sets the api_subnet_allow_list of this KubernetesClusterPropertiesForPut.
+        """Sets the api_subnet_allow_list of this KubernetesClusterPropertiesForPost.
 
-        Access to the K8s API server is restricted to these CIDRs. Traffic, internal to the cluster, is not affected by this restriction. If no allowlist is specified, access is not restricted. If an IP without subnet mask is provided, the default value is used: 32 for IPv4 and 128 for IPv6.  # noqa: E501
+        Access to the K8s API server is restricted to these CIDRs. Intra-cluster traffic is not affected by this restriction. If no AllowList is specified, access is not limited. If an IP is specified without a subnet mask, the default value is 32 for IPv4 and 128 for IPv6.  # noqa: E501
 
-        :param api_subnet_allow_list: The api_subnet_allow_list of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :param api_subnet_allow_list: The api_subnet_allow_list of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :type api_subnet_allow_list: list[str]
         """
 
         self._api_subnet_allow_list = api_subnet_allow_list
 
     @property
     def s3_buckets(self):
-        """Gets the s3_buckets of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        """Gets the s3_buckets of this KubernetesClusterPropertiesForPost.  # noqa: E501
 
-        List of S3 bucket configured for K8s usage. For now it contains only an S3 bucket used to store K8s API audit logs  # noqa: E501
+        List of S3 buckets configured for K8s usage. At the moment, it contains only one S3 bucket that is used to store K8s API audit logs.  # noqa: E501
 
-        :return: The s3_buckets of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :return: The s3_buckets of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :rtype: list[S3Bucket]
         """
         return self._s3_buckets
 
     @s3_buckets.setter
     def s3_buckets(self, s3_buckets):
-        """Sets the s3_buckets of this KubernetesClusterPropertiesForPut.
+        """Sets the s3_buckets of this KubernetesClusterPropertiesForPost.
 
-        List of S3 bucket configured for K8s usage. For now it contains only an S3 bucket used to store K8s API audit logs  # noqa: E501
+        List of S3 buckets configured for K8s usage. At the moment, it contains only one S3 bucket that is used to store K8s API audit logs.  # noqa: E501
 
-        :param s3_buckets: The s3_buckets of this KubernetesClusterPropertiesForPut.  # noqa: E501
+        :param s3_buckets: The s3_buckets of this KubernetesClusterPropertiesForPost.  # noqa: E501
         :type s3_buckets: list[S3Bucket]
         """
 
         self._s3_buckets = s3_buckets
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -226,18 +226,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, KubernetesClusterPropertiesForPut):
+        if not isinstance(other, KubernetesClusterPropertiesForPost):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, KubernetesClusterPropertiesForPut):
+        if not isinstance(other, KubernetesClusterPropertiesForPost):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_clusters.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_clusters.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,49 +76,49 @@
             self.items = items
 
 
     @property
     def id(self):
         """Gets the id of this KubernetesClusters.  # noqa: E501
 
-        A unique representation of the Kubernetes cluster as a resource collection.  # noqa: E501
+        The unique representation of the K8s cluster as a resource collection.  # noqa: E501
 
         :return: The id of this KubernetesClusters.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this KubernetesClusters.
 
-        A unique representation of the Kubernetes cluster as a resource collection.  # noqa: E501
+        The unique representation of the K8s cluster as a resource collection.  # noqa: E501
 
         :param id: The id of this KubernetesClusters.  # noqa: E501
         :type id: str
         """
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesClusters.  # noqa: E501
 
-        The type of resource within a collection.  # noqa: E501
+        The resource type within a collection.  # noqa: E501
 
         :return: The type of this KubernetesClusters.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesClusters.
 
-        The type of resource within a collection.  # noqa: E501
+        The resource type within a collection.  # noqa: E501
 
         :param type: The type of this KubernetesClusters.  # noqa: E501
         :type type: str
         """
         allowed_values = ["collection"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -128,49 +128,49 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesClusters.  # noqa: E501
 
-        URL to the collection representation (absolute path).  # noqa: E501
+        The URL to the collection representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesClusters.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesClusters.
 
-        URL to the collection representation (absolute path).  # noqa: E501
+        The URL to the collection representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesClusters.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def items(self):
         """Gets the items of this KubernetesClusters.  # noqa: E501
 
-        Array of items in the collection.  # noqa: E501
+        Array of K8s clusters in the collection.  # noqa: E501
 
         :return: The items of this KubernetesClusters.  # noqa: E501
         :rtype: list[KubernetesCluster]
         """
         return self._items
 
     @items.setter
     def items(self, items):
         """Sets the items of this KubernetesClusters.
 
-        Array of items in the collection.  # noqa: E501
+        Array of K8s clusters in the collection.  # noqa: E501
 
         :param items: The items of this KubernetesClusters.  # noqa: E501
         :type items: list[KubernetesCluster]
         """
 
         self._items = items
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_maintenance_window.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_maintenance_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,26 @@
         self.time = time
 
 
     @property
     def day_of_the_week(self):
         """Gets the day_of_the_week of this KubernetesMaintenanceWindow.  # noqa: E501
 
-        The day of the week for a maintenance window.  # noqa: E501
+        The weekday for a maintenance window.  # noqa: E501
 
         :return: The day_of_the_week of this KubernetesMaintenanceWindow.  # noqa: E501
         :rtype: str
         """
         return self._day_of_the_week
 
     @day_of_the_week.setter
     def day_of_the_week(self, day_of_the_week):
         """Sets the day_of_the_week of this KubernetesMaintenanceWindow.
 
-        The day of the week for a maintenance window.  # noqa: E501
+        The weekday for a maintenance window.  # noqa: E501
 
         :param day_of_the_week: The day_of_the_week of this KubernetesMaintenanceWindow.  # noqa: E501
         :type day_of_the_week: str
         """
         if self.local_vars_configuration.client_side_validation and day_of_the_week is None:  # noqa: E501
             raise ValueError("Invalid value for `day_of_the_week`, must not be `None`")  # noqa: E501
         allowed_values = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]  # noqa: E501
@@ -91,26 +91,26 @@
 
         self._day_of_the_week = day_of_the_week
 
     @property
     def time(self):
         """Gets the time of this KubernetesMaintenanceWindow.  # noqa: E501
 
-        The time to use for a maintenance window. Accepted formats are: HH:mm:ss; HH:mm:ss\"Z\"; HH:mm:ssZ. This time may varies by 15 minutes.  # noqa: E501
+        The time to use for a maintenance window. Accepted formats are: HH:mm:ss; HH:mm:ss\"Z\"; HH:mm:ssZ. This time may vary by 15 minutes.  # noqa: E501
 
         :return: The time of this KubernetesMaintenanceWindow.  # noqa: E501
         :rtype: str
         """
         return self._time
 
     @time.setter
     def time(self, time):
         """Sets the time of this KubernetesMaintenanceWindow.
 
-        The time to use for a maintenance window. Accepted formats are: HH:mm:ss; HH:mm:ss\"Z\"; HH:mm:ssZ. This time may varies by 15 minutes.  # noqa: E501
+        The time to use for a maintenance window. Accepted formats are: HH:mm:ss; HH:mm:ss\"Z\"; HH:mm:ssZ. This time may vary by 15 minutes.  # noqa: E501
 
         :param time: The time of this KubernetesMaintenanceWindow.  # noqa: E501
         :type time: str
         """
         if self.local_vars_configuration.client_side_validation and time is None:  # noqa: E501
             raise ValueError("Invalid value for `time`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,26 +105,26 @@
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesNode.  # noqa: E501
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :return: The type of this KubernetesNode.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesNode.
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :param type: The type of this KubernetesNode.  # noqa: E501
         :type type: str
         """
         allowed_values = ["node"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -134,26 +134,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesNode.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesNode.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesNode.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesNode.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_metadata.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,95 +83,95 @@
             self.last_software_updated_date = last_software_updated_date
 
 
     @property
     def etag(self):
         """Gets the etag of this KubernetesNodeMetadata.  # noqa: E501
 
-        Resource's Entity Tag as defined in http://www.w3.org/Protocols/rfc2616/rfc2616-sec3.html#sec3.11  Entity Tag is also added as an 'ETag response header to requests which don't use 'depth' parameter.   # noqa: E501
+        The resource entity tag as defined in http://www.w3.org/Protocols/rfc2616/rfc2616-sec3.html#sec3.11  Entity tags are also added as 'ETag' response headers to requests that do not use the 'depth' parameter.  # noqa: E501
 
         :return: The etag of this KubernetesNodeMetadata.  # noqa: E501
         :rtype: str
         """
         return self._etag
 
     @etag.setter
     def etag(self, etag):
         """Sets the etag of this KubernetesNodeMetadata.
 
-        Resource's Entity Tag as defined in http://www.w3.org/Protocols/rfc2616/rfc2616-sec3.html#sec3.11  Entity Tag is also added as an 'ETag response header to requests which don't use 'depth' parameter.   # noqa: E501
+        The resource entity tag as defined in http://www.w3.org/Protocols/rfc2616/rfc2616-sec3.html#sec3.11  Entity tags are also added as 'ETag' response headers to requests that do not use the 'depth' parameter.  # noqa: E501
 
         :param etag: The etag of this KubernetesNodeMetadata.  # noqa: E501
         :type etag: str
         """
 
         self._etag = etag
 
     @property
     def created_date(self):
         """Gets the created_date of this KubernetesNodeMetadata.  # noqa: E501
 
-        The last time the resource was created.  # noqa: E501
+        The date the resource was created.  # noqa: E501
 
         :return: The created_date of this KubernetesNodeMetadata.  # noqa: E501
         :rtype: datetime
         """
         return self._created_date
 
     @created_date.setter
     def created_date(self, created_date):
         """Sets the created_date of this KubernetesNodeMetadata.
 
-        The last time the resource was created.  # noqa: E501
+        The date the resource was created.  # noqa: E501
 
         :param created_date: The created_date of this KubernetesNodeMetadata.  # noqa: E501
         :type created_date: datetime
         """
 
         self._created_date = created_date
 
     @property
     def last_modified_date(self):
         """Gets the last_modified_date of this KubernetesNodeMetadata.  # noqa: E501
 
-        The last time the resource was modified.  # noqa: E501
+        The date the resource was last modified.  # noqa: E501
 
         :return: The last_modified_date of this KubernetesNodeMetadata.  # noqa: E501
         :rtype: datetime
         """
         return self._last_modified_date
 
     @last_modified_date.setter
     def last_modified_date(self, last_modified_date):
         """Sets the last_modified_date of this KubernetesNodeMetadata.
 
-        The last time the resource was modified.  # noqa: E501
+        The date the resource was last modified.  # noqa: E501
 
         :param last_modified_date: The last_modified_date of this KubernetesNodeMetadata.  # noqa: E501
         :type last_modified_date: datetime
         """
 
         self._last_modified_date = last_modified_date
 
     @property
     def state(self):
         """Gets the state of this KubernetesNodeMetadata.  # noqa: E501
 
-        State of the resource.  # noqa: E501
+        The resource state.  # noqa: E501
 
         :return: The state of this KubernetesNodeMetadata.  # noqa: E501
         :rtype: str
         """
         return self._state
 
     @state.setter
     def state(self, state):
         """Sets the state of this KubernetesNodeMetadata.
 
-        State of the resource.  # noqa: E501
+        The resource state.  # noqa: E501
 
         :param state: The state of this KubernetesNodeMetadata.  # noqa: E501
         :type state: str
         """
         allowed_values = ["PROVISIONING", "PROVISIONED", "READY", "TERMINATING", "REBUILDING", "BUSY"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and state not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -181,26 +181,26 @@
 
         self._state = state
 
     @property
     def last_software_updated_date(self):
         """Gets the last_software_updated_date of this KubernetesNodeMetadata.  # noqa: E501
 
-        The last time the software was updated on the node.  # noqa: E501
+        The date when the software on the node was last updated.  # noqa: E501
 
         :return: The last_software_updated_date of this KubernetesNodeMetadata.  # noqa: E501
         :rtype: datetime
         """
         return self._last_software_updated_date
 
     @last_software_updated_date.setter
     def last_software_updated_date(self, last_software_updated_date):
         """Sets the last_software_updated_date of this KubernetesNodeMetadata.
 
-        The last time the software was updated on the node.  # noqa: E501
+        The date when the software on the node was last updated.  # noqa: E501
 
         :param last_software_updated_date: The last_software_updated_date of this KubernetesNodeMetadata.  # noqa: E501
         :type last_software_updated_date: datetime
         """
 
         self._last_software_updated_date = last_software_updated_date
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,26 +105,26 @@
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesNodePool.  # noqa: E501
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :return: The type of this KubernetesNodePool.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesNodePool.
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :param type: The type of this KubernetesNodePool.  # noqa: E501
         :type type: str
         """
         allowed_values = ["nodepool"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -134,26 +134,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesNodePool.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesNodePool.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesNodePool.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesNodePool.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_for_post.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_for_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,26 +105,26 @@
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesNodePoolForPost.  # noqa: E501
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :return: The type of this KubernetesNodePoolForPost.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesNodePoolForPost.
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :param type: The type of this KubernetesNodePoolForPost.  # noqa: E501
         :type type: str
         """
         allowed_values = ["nodepool"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -134,26 +134,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesNodePoolForPost.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesNodePoolForPost.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesNodePoolForPost.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesNodePoolForPost.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_for_put.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_for_put.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,26 +105,26 @@
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesNodePoolForPut.  # noqa: E501
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :return: The type of this KubernetesNodePoolForPut.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesNodePoolForPut.
 
-        The type of object.  # noqa: E501
+        The object type.  # noqa: E501
 
         :param type: The type of this KubernetesNodePoolForPut.  # noqa: E501
         :type type: str
         """
         allowed_values = ["nodepool"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -134,26 +134,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesNodePoolForPut.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesNodePoolForPut.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesNodePoolForPut.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesNodePoolForPut.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_lan.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_lan.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,112 +30,142 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
+        'datacenter_id': 'str',
+
         'id': 'int',
 
         'dhcp': 'bool',
 
         'routes': 'list[KubernetesNodePoolLanRoutes]',
     }
 
     attribute_map = {
 
+        'datacenter_id': 'datacenterId',
+
         'id': 'id',
 
         'dhcp': 'dhcp',
 
         'routes': 'routes',
     }
 
-    def __init__(self, id=None, dhcp=None, routes=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, datacenter_id=None, id=None, dhcp=None, routes=None, local_vars_configuration=None):  # noqa: E501
         """KubernetesNodePoolLan - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._datacenter_id = None
         self._id = None
         self._dhcp = None
         self._routes = None
         self.discriminator = None
 
+        if datacenter_id is not None:
+            self.datacenter_id = datacenter_id
         self.id = id
         if dhcp is not None:
             self.dhcp = dhcp
         if routes is not None:
             self.routes = routes
 
 
     @property
+    def datacenter_id(self):
+        """Gets the datacenter_id of this KubernetesNodePoolLan.  # noqa: E501
+
+        The datacenter ID, requires system privileges, for internal usage only  # noqa: E501
+
+        :return: The datacenter_id of this KubernetesNodePoolLan.  # noqa: E501
+        :rtype: str
+        """
+        return self._datacenter_id
+
+    @datacenter_id.setter
+    def datacenter_id(self, datacenter_id):
+        """Sets the datacenter_id of this KubernetesNodePoolLan.
+
+        The datacenter ID, requires system privileges, for internal usage only  # noqa: E501
+
+        :param datacenter_id: The datacenter_id of this KubernetesNodePoolLan.  # noqa: E501
+        :type datacenter_id: str
+        """
+
+        self._datacenter_id = datacenter_id
+
+    @property
     def id(self):
         """Gets the id of this KubernetesNodePoolLan.  # noqa: E501
 
-        The LAN ID of an existing LAN at the related datacenter  # noqa: E501
+        The LAN ID of an existing LAN at the related data center  # noqa: E501
 
         :return: The id of this KubernetesNodePoolLan.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this KubernetesNodePoolLan.
 
-        The LAN ID of an existing LAN at the related datacenter  # noqa: E501
+        The LAN ID of an existing LAN at the related data center  # noqa: E501
 
         :param id: The id of this KubernetesNodePoolLan.  # noqa: E501
         :type id: int
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def dhcp(self):
         """Gets the dhcp of this KubernetesNodePoolLan.  # noqa: E501
 
-        Indicates if the Kubernetes node pool LAN will reserve an IP using DHCP.  # noqa: E501
+        Specifies whether the Kubernetes node pool LAN reserves an IP with DHCP.  # noqa: E501
 
         :return: The dhcp of this KubernetesNodePoolLan.  # noqa: E501
         :rtype: bool
         """
         return self._dhcp
 
     @dhcp.setter
     def dhcp(self, dhcp):
         """Sets the dhcp of this KubernetesNodePoolLan.
 
-        Indicates if the Kubernetes node pool LAN will reserve an IP using DHCP.  # noqa: E501
+        Specifies whether the Kubernetes node pool LAN reserves an IP with DHCP.  # noqa: E501
 
         :param dhcp: The dhcp of this KubernetesNodePoolLan.  # noqa: E501
         :type dhcp: bool
         """
 
         self._dhcp = dhcp
 
     @property
     def routes(self):
         """Gets the routes of this KubernetesNodePoolLan.  # noqa: E501
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of additional LANs attached to worker nodes.  # noqa: E501
 
         :return: The routes of this KubernetesNodePoolLan.  # noqa: E501
         :rtype: list[KubernetesNodePoolLanRoutes]
         """
         return self._routes
 
     @routes.setter
     def routes(self, routes):
         """Sets the routes of this KubernetesNodePoolLan.
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of additional LANs attached to worker nodes.  # noqa: E501
 
         :param routes: The routes of this KubernetesNodePoolLan.  # noqa: E501
         :type routes: list[KubernetesNodePoolLanRoutes]
         """
 
         self._routes = routes
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_lan_routes.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_lan_routes.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,126 +183,126 @@
 
         self._name = name
 
     @property
     def datacenter_id(self):
         """Gets the datacenter_id of this KubernetesNodePoolProperties.  # noqa: E501
 
-        A valid ID of the data center, to which user has access.  # noqa: E501
+        The unique identifier of the VDC where the worker nodes of the node pool are provisioned.Note that the data center is located in the exact place where the parent cluster of the node pool is located.  # noqa: E501
 
         :return: The datacenter_id of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: str
         """
         return self._datacenter_id
 
     @datacenter_id.setter
     def datacenter_id(self, datacenter_id):
         """Sets the datacenter_id of this KubernetesNodePoolProperties.
 
-        A valid ID of the data center, to which user has access.  # noqa: E501
+        The unique identifier of the VDC where the worker nodes of the node pool are provisioned.Note that the data center is located in the exact place where the parent cluster of the node pool is located.  # noqa: E501
 
         :param datacenter_id: The datacenter_id of this KubernetesNodePoolProperties.  # noqa: E501
         :type datacenter_id: str
         """
         if self.local_vars_configuration.client_side_validation and datacenter_id is None:  # noqa: E501
             raise ValueError("Invalid value for `datacenter_id`, must not be `None`")  # noqa: E501
 
         self._datacenter_id = datacenter_id
 
     @property
     def node_count(self):
         """Gets the node_count of this KubernetesNodePoolProperties.  # noqa: E501
 
-        The number of nodes that make up the node pool.  # noqa: E501
+        The number of worker nodes of the node pool.  # noqa: E501
 
         :return: The node_count of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: int
         """
         return self._node_count
 
     @node_count.setter
     def node_count(self, node_count):
         """Sets the node_count of this KubernetesNodePoolProperties.
 
-        The number of nodes that make up the node pool.  # noqa: E501
+        The number of worker nodes of the node pool.  # noqa: E501
 
         :param node_count: The node_count of this KubernetesNodePoolProperties.  # noqa: E501
         :type node_count: int
         """
         if self.local_vars_configuration.client_side_validation and node_count is None:  # noqa: E501
             raise ValueError("Invalid value for `node_count`, must not be `None`")  # noqa: E501
 
         self._node_count = node_count
 
     @property
     def cpu_family(self):
         """Gets the cpu_family of this KubernetesNodePoolProperties.  # noqa: E501
 
-        A valid CPU family name.  # noqa: E501
+        The CPU type for the nodes.  # noqa: E501
 
         :return: The cpu_family of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: str
         """
         return self._cpu_family
 
     @cpu_family.setter
     def cpu_family(self, cpu_family):
         """Sets the cpu_family of this KubernetesNodePoolProperties.
 
-        A valid CPU family name.  # noqa: E501
+        The CPU type for the nodes.  # noqa: E501
 
         :param cpu_family: The cpu_family of this KubernetesNodePoolProperties.  # noqa: E501
         :type cpu_family: str
         """
         if self.local_vars_configuration.client_side_validation and cpu_family is None:  # noqa: E501
             raise ValueError("Invalid value for `cpu_family`, must not be `None`")  # noqa: E501
 
         self._cpu_family = cpu_family
 
     @property
     def cores_count(self):
         """Gets the cores_count of this KubernetesNodePoolProperties.  # noqa: E501
 
-        The number of cores for the node.  # noqa: E501
+        The total number of cores for the nodes.  # noqa: E501
 
         :return: The cores_count of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: int
         """
         return self._cores_count
 
     @cores_count.setter
     def cores_count(self, cores_count):
         """Sets the cores_count of this KubernetesNodePoolProperties.
 
-        The number of cores for the node.  # noqa: E501
+        The total number of cores for the nodes.  # noqa: E501
 
         :param cores_count: The cores_count of this KubernetesNodePoolProperties.  # noqa: E501
         :type cores_count: int
         """
         if self.local_vars_configuration.client_side_validation and cores_count is None:  # noqa: E501
             raise ValueError("Invalid value for `cores_count`, must not be `None`")  # noqa: E501
 
         self._cores_count = cores_count
 
     @property
     def ram_size(self):
         """Gets the ram_size of this KubernetesNodePoolProperties.  # noqa: E501
 
-        The RAM size for the node. Must be set in multiples of 1024 MB, with minimum size is of 2048 MB.  # noqa: E501
+        The RAM size for the nodes. Must be specified in multiples of 1024 MB, with a minimum size of 2048 MB.  # noqa: E501
 
         :return: The ram_size of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: int
         """
         return self._ram_size
 
     @ram_size.setter
     def ram_size(self, ram_size):
         """Sets the ram_size of this KubernetesNodePoolProperties.
 
-        The RAM size for the node. Must be set in multiples of 1024 MB, with minimum size is of 2048 MB.  # noqa: E501
+        The RAM size for the nodes. Must be specified in multiples of 1024 MB, with a minimum size of 2048 MB.  # noqa: E501
 
         :param ram_size: The ram_size of this KubernetesNodePoolProperties.  # noqa: E501
         :type ram_size: int
         """
         if self.local_vars_configuration.client_side_validation and ram_size is None:  # noqa: E501
             raise ValueError("Invalid value for `ram_size`, must not be `None`")  # noqa: E501
 
@@ -339,26 +339,26 @@
 
         self._availability_zone = availability_zone
 
     @property
     def storage_type(self):
         """Gets the storage_type of this KubernetesNodePoolProperties.  # noqa: E501
 
-        The type of hardware for the volume.  # noqa: E501
+        The storage type for the nodes.  # noqa: E501
 
         :return: The storage_type of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: str
         """
         return self._storage_type
 
     @storage_type.setter
     def storage_type(self, storage_type):
         """Sets the storage_type of this KubernetesNodePoolProperties.
 
-        The type of hardware for the volume.  # noqa: E501
+        The storage type for the nodes.  # noqa: E501
 
         :param storage_type: The storage_type of this KubernetesNodePoolProperties.  # noqa: E501
         :type storage_type: str
         """
         if self.local_vars_configuration.client_side_validation and storage_type is None:  # noqa: E501
             raise ValueError("Invalid value for `storage_type`, must not be `None`")  # noqa: E501
         allowed_values = ["HDD", "SSD"]  # noqa: E501
@@ -370,51 +370,51 @@
 
         self._storage_type = storage_type
 
     @property
     def storage_size(self):
         """Gets the storage_size of this KubernetesNodePoolProperties.  # noqa: E501
 
-        The size of the volume in GB. The size should be greater than 10GB.  # noqa: E501
+        The allocated volume size in GB. The allocated volume size in GB. To achieve good performance, we recommend a size greater than 100GB for SSD.  # noqa: E501
 
         :return: The storage_size of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: int
         """
         return self._storage_size
 
     @storage_size.setter
     def storage_size(self, storage_size):
         """Sets the storage_size of this KubernetesNodePoolProperties.
 
-        The size of the volume in GB. The size should be greater than 10GB.  # noqa: E501
+        The allocated volume size in GB. The allocated volume size in GB. To achieve good performance, we recommend a size greater than 100GB for SSD.  # noqa: E501
 
         :param storage_size: The storage_size of this KubernetesNodePoolProperties.  # noqa: E501
         :type storage_size: int
         """
         if self.local_vars_configuration.client_side_validation and storage_size is None:  # noqa: E501
             raise ValueError("Invalid value for `storage_size`, must not be `None`")  # noqa: E501
 
         self._storage_size = storage_size
 
     @property
     def k8s_version(self):
         """Gets the k8s_version of this KubernetesNodePoolProperties.  # noqa: E501
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :return: The k8s_version of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: str
         """
         return self._k8s_version
 
     @k8s_version.setter
     def k8s_version(self, k8s_version):
         """Sets the k8s_version of this KubernetesNodePoolProperties.
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :param k8s_version: The k8s_version of this KubernetesNodePoolProperties.  # noqa: E501
         :type k8s_version: str
         """
 
         self._k8s_version = k8s_version
 
@@ -460,118 +460,118 @@
 
         self._auto_scaling = auto_scaling
 
     @property
     def lans(self):
         """Gets the lans of this KubernetesNodePoolProperties.  # noqa: E501
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of existing private LANs to attach to worker nodes.  # noqa: E501
 
         :return: The lans of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: list[KubernetesNodePoolLan]
         """
         return self._lans
 
     @lans.setter
     def lans(self, lans):
         """Sets the lans of this KubernetesNodePoolProperties.
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of existing private LANs to attach to worker nodes.  # noqa: E501
 
         :param lans: The lans of this KubernetesNodePoolProperties.  # noqa: E501
         :type lans: list[KubernetesNodePoolLan]
         """
 
         self._lans = lans
 
     @property
     def labels(self):
         """Gets the labels of this KubernetesNodePoolProperties.  # noqa: E501
 
-        map of labels attached to node pool.  # noqa: E501
+        The labels attached to the node pool.  # noqa: E501
 
         :return: The labels of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._labels
 
     @labels.setter
     def labels(self, labels):
         """Sets the labels of this KubernetesNodePoolProperties.
 
-        map of labels attached to node pool.  # noqa: E501
+        The labels attached to the node pool.  # noqa: E501
 
         :param labels: The labels of this KubernetesNodePoolProperties.  # noqa: E501
         :type labels: dict(str, str)
         """
 
         self._labels = labels
 
     @property
     def annotations(self):
         """Gets the annotations of this KubernetesNodePoolProperties.  # noqa: E501
 
-        map of annotations attached to node pool.  # noqa: E501
+        The annotations attached to the node pool.  # noqa: E501
 
         :return: The annotations of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._annotations
 
     @annotations.setter
     def annotations(self, annotations):
         """Sets the annotations of this KubernetesNodePoolProperties.
 
-        map of annotations attached to node pool.  # noqa: E501
+        The annotations attached to the node pool.  # noqa: E501
 
         :param annotations: The annotations of this KubernetesNodePoolProperties.  # noqa: E501
         :type annotations: dict(str, str)
         """
 
         self._annotations = annotations
 
     @property
     def public_ips(self):
         """Gets the public_ips of this KubernetesNodePoolProperties.  # noqa: E501
 
-        Optional array of reserved public IP addresses to be used by the nodes. IPs must be from same location as the data center used for the node pool. The array must contain one more IP than maximum number possible number of nodes (nodeCount+1 for fixed number of nodes or maxNodeCount+1 when auto scaling is used). The extra IP is used when the nodes are rebuilt.  # noqa: E501
+        Optional array of reserved public IP addresses to be used by the nodes. The IPs must be from the exact location of the node pool's data center. If autoscaling is used, the array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for a fixed number of nodes or maxNodeCount+1). The extra IP is used when the nodes are rebuilt.  # noqa: E501
 
         :return: The public_ips of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: list[str]
         """
         return self._public_ips
 
     @public_ips.setter
     def public_ips(self, public_ips):
         """Sets the public_ips of this KubernetesNodePoolProperties.
 
-        Optional array of reserved public IP addresses to be used by the nodes. IPs must be from same location as the data center used for the node pool. The array must contain one more IP than maximum number possible number of nodes (nodeCount+1 for fixed number of nodes or maxNodeCount+1 when auto scaling is used). The extra IP is used when the nodes are rebuilt.  # noqa: E501
+        Optional array of reserved public IP addresses to be used by the nodes. The IPs must be from the exact location of the node pool's data center. If autoscaling is used, the array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for a fixed number of nodes or maxNodeCount+1). The extra IP is used when the nodes are rebuilt.  # noqa: E501
 
         :param public_ips: The public_ips of this KubernetesNodePoolProperties.  # noqa: E501
         :type public_ips: list[str]
         """
 
         self._public_ips = public_ips
 
     @property
     def available_upgrade_versions(self):
         """Gets the available_upgrade_versions of this KubernetesNodePoolProperties.  # noqa: E501
 
-        List of available versions for upgrading the node pool.  # noqa: E501
+        The list of available versions for upgrading the node pool.  # noqa: E501
 
         :return: The available_upgrade_versions of this KubernetesNodePoolProperties.  # noqa: E501
         :rtype: list[str]
         """
         return self._available_upgrade_versions
 
     @available_upgrade_versions.setter
     def available_upgrade_versions(self, available_upgrade_versions):
         """Sets the available_upgrade_versions of this KubernetesNodePoolProperties.
 
-        List of available versions for upgrading the node pool.  # noqa: E501
+        The list of available versions for upgrading the node pool.  # noqa: E501
 
         :param available_upgrade_versions: The available_upgrade_versions of this KubernetesNodePoolProperties.  # noqa: E501
         :type available_upgrade_versions: list[str]
         """
 
         self._available_upgrade_versions = available_upgrade_versions
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_properties_for_post.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_properties_for_post.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,126 +176,126 @@
 
         self._name = name
 
     @property
     def datacenter_id(self):
         """Gets the datacenter_id of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        A valid ID of the data center, to which the user has access.  # noqa: E501
+        The unique identifier of the VDC where the worker nodes of the node pool are provisioned.Note that the data center is located in the exact place where the parent cluster of the node pool is located.  # noqa: E501
 
         :return: The datacenter_id of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: str
         """
         return self._datacenter_id
 
     @datacenter_id.setter
     def datacenter_id(self, datacenter_id):
         """Sets the datacenter_id of this KubernetesNodePoolPropertiesForPost.
 
-        A valid ID of the data center, to which the user has access.  # noqa: E501
+        The unique identifier of the VDC where the worker nodes of the node pool are provisioned.Note that the data center is located in the exact place where the parent cluster of the node pool is located.  # noqa: E501
 
         :param datacenter_id: The datacenter_id of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type datacenter_id: str
         """
         if self.local_vars_configuration.client_side_validation and datacenter_id is None:  # noqa: E501
             raise ValueError("Invalid value for `datacenter_id`, must not be `None`")  # noqa: E501
 
         self._datacenter_id = datacenter_id
 
     @property
     def node_count(self):
         """Gets the node_count of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        The number of nodes that make up the node pool.  # noqa: E501
+        The number of worker nodes of the node pool.  # noqa: E501
 
         :return: The node_count of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: int
         """
         return self._node_count
 
     @node_count.setter
     def node_count(self, node_count):
         """Sets the node_count of this KubernetesNodePoolPropertiesForPost.
 
-        The number of nodes that make up the node pool.  # noqa: E501
+        The number of worker nodes of the node pool.  # noqa: E501
 
         :param node_count: The node_count of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type node_count: int
         """
         if self.local_vars_configuration.client_side_validation and node_count is None:  # noqa: E501
             raise ValueError("Invalid value for `node_count`, must not be `None`")  # noqa: E501
 
         self._node_count = node_count
 
     @property
     def cpu_family(self):
         """Gets the cpu_family of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        A valid CPU family name.  # noqa: E501
+        The CPU type for the nodes.  # noqa: E501
 
         :return: The cpu_family of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: str
         """
         return self._cpu_family
 
     @cpu_family.setter
     def cpu_family(self, cpu_family):
         """Sets the cpu_family of this KubernetesNodePoolPropertiesForPost.
 
-        A valid CPU family name.  # noqa: E501
+        The CPU type for the nodes.  # noqa: E501
 
         :param cpu_family: The cpu_family of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type cpu_family: str
         """
         if self.local_vars_configuration.client_side_validation and cpu_family is None:  # noqa: E501
             raise ValueError("Invalid value for `cpu_family`, must not be `None`")  # noqa: E501
 
         self._cpu_family = cpu_family
 
     @property
     def cores_count(self):
         """Gets the cores_count of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        The number of cores for the node.  # noqa: E501
+        The total number of cores for the nodes.  # noqa: E501
 
         :return: The cores_count of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: int
         """
         return self._cores_count
 
     @cores_count.setter
     def cores_count(self, cores_count):
         """Sets the cores_count of this KubernetesNodePoolPropertiesForPost.
 
-        The number of cores for the node.  # noqa: E501
+        The total number of cores for the nodes.  # noqa: E501
 
         :param cores_count: The cores_count of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type cores_count: int
         """
         if self.local_vars_configuration.client_side_validation and cores_count is None:  # noqa: E501
             raise ValueError("Invalid value for `cores_count`, must not be `None`")  # noqa: E501
 
         self._cores_count = cores_count
 
     @property
     def ram_size(self):
         """Gets the ram_size of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        The RAM size for the node. Must be set in multiples of 1024 MB, with minimum size is of 2048 MB.  # noqa: E501
+        The RAM size for the nodes. Must be specified in multiples of 1024 MB, with a minimum size of 2048 MB.  # noqa: E501
 
         :return: The ram_size of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: int
         """
         return self._ram_size
 
     @ram_size.setter
     def ram_size(self, ram_size):
         """Sets the ram_size of this KubernetesNodePoolPropertiesForPost.
 
-        The RAM size for the node. Must be set in multiples of 1024 MB, with minimum size is of 2048 MB.  # noqa: E501
+        The RAM size for the nodes. Must be specified in multiples of 1024 MB, with a minimum size of 2048 MB.  # noqa: E501
 
         :param ram_size: The ram_size of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type ram_size: int
         """
         if self.local_vars_configuration.client_side_validation and ram_size is None:  # noqa: E501
             raise ValueError("Invalid value for `ram_size`, must not be `None`")  # noqa: E501
 
@@ -332,26 +332,26 @@
 
         self._availability_zone = availability_zone
 
     @property
     def storage_type(self):
         """Gets the storage_type of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        The type of hardware for the volume.  # noqa: E501
+        The storage type for the nodes.  # noqa: E501
 
         :return: The storage_type of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: str
         """
         return self._storage_type
 
     @storage_type.setter
     def storage_type(self, storage_type):
         """Sets the storage_type of this KubernetesNodePoolPropertiesForPost.
 
-        The type of hardware for the volume.  # noqa: E501
+        The storage type for the nodes.  # noqa: E501
 
         :param storage_type: The storage_type of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type storage_type: str
         """
         if self.local_vars_configuration.client_side_validation and storage_type is None:  # noqa: E501
             raise ValueError("Invalid value for `storage_type`, must not be `None`")  # noqa: E501
         allowed_values = ["HDD", "SSD"]  # noqa: E501
@@ -363,51 +363,51 @@
 
         self._storage_type = storage_type
 
     @property
     def storage_size(self):
         """Gets the storage_size of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        The size of the volume in GB. The size should be greater than 10GB.  # noqa: E501
+        The allocated volume size in GB. The allocated volume size in GB. To achieve good performance, we recommend a size greater than 100GB for SSD.  # noqa: E501
 
         :return: The storage_size of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: int
         """
         return self._storage_size
 
     @storage_size.setter
     def storage_size(self, storage_size):
         """Sets the storage_size of this KubernetesNodePoolPropertiesForPost.
 
-        The size of the volume in GB. The size should be greater than 10GB.  # noqa: E501
+        The allocated volume size in GB. The allocated volume size in GB. To achieve good performance, we recommend a size greater than 100GB for SSD.  # noqa: E501
 
         :param storage_size: The storage_size of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type storage_size: int
         """
         if self.local_vars_configuration.client_side_validation and storage_size is None:  # noqa: E501
             raise ValueError("Invalid value for `storage_size`, must not be `None`")  # noqa: E501
 
         self._storage_size = storage_size
 
     @property
     def k8s_version(self):
         """Gets the k8s_version of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :return: The k8s_version of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: str
         """
         return self._k8s_version
 
     @k8s_version.setter
     def k8s_version(self, k8s_version):
         """Sets the k8s_version of this KubernetesNodePoolPropertiesForPost.
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :param k8s_version: The k8s_version of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type k8s_version: str
         """
 
         self._k8s_version = k8s_version
 
@@ -453,95 +453,95 @@
 
         self._auto_scaling = auto_scaling
 
     @property
     def lans(self):
         """Gets the lans of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of existing private LANs to attach to worker nodes.  # noqa: E501
 
         :return: The lans of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: list[KubernetesNodePoolLan]
         """
         return self._lans
 
     @lans.setter
     def lans(self, lans):
         """Sets the lans of this KubernetesNodePoolPropertiesForPost.
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of existing private LANs to attach to worker nodes.  # noqa: E501
 
         :param lans: The lans of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type lans: list[KubernetesNodePoolLan]
         """
 
         self._lans = lans
 
     @property
     def labels(self):
         """Gets the labels of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        map of labels attached to node pool.  # noqa: E501
+        The labels attached to the node pool.  # noqa: E501
 
         :return: The labels of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._labels
 
     @labels.setter
     def labels(self, labels):
         """Sets the labels of this KubernetesNodePoolPropertiesForPost.
 
-        map of labels attached to node pool.  # noqa: E501
+        The labels attached to the node pool.  # noqa: E501
 
         :param labels: The labels of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type labels: dict(str, str)
         """
 
         self._labels = labels
 
     @property
     def annotations(self):
         """Gets the annotations of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        map of annotations attached to node pool.  # noqa: E501
+        The annotations attached to the node pool.  # noqa: E501
 
         :return: The annotations of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._annotations
 
     @annotations.setter
     def annotations(self, annotations):
         """Sets the annotations of this KubernetesNodePoolPropertiesForPost.
 
-        map of annotations attached to node pool.  # noqa: E501
+        The annotations attached to the node pool.  # noqa: E501
 
         :param annotations: The annotations of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type annotations: dict(str, str)
         """
 
         self._annotations = annotations
 
     @property
     def public_ips(self):
         """Gets the public_ips of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
 
-        Optional array of reserved public IP addresses to be used by the nodes. IPs must be from same location as the data center used for the node pool. The array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for fixed number of nodes or maxNodeCount+1 when auto scaling is used). The extra IP is used when the nodes are rebuilt.  # noqa: E501
+        Optional array of reserved public IP addresses to be used by the nodes. The IPs must be from the exact location of the node pool's data center. If autoscaling is used, the array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for a fixed number of nodes or maxNodeCount+1). The extra IP is used when the nodes are rebuilt.  # noqa: E501
 
         :return: The public_ips of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :rtype: list[str]
         """
         return self._public_ips
 
     @public_ips.setter
     def public_ips(self, public_ips):
         """Sets the public_ips of this KubernetesNodePoolPropertiesForPost.
 
-        Optional array of reserved public IP addresses to be used by the nodes. IPs must be from same location as the data center used for the node pool. The array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for fixed number of nodes or maxNodeCount+1 when auto scaling is used). The extra IP is used when the nodes are rebuilt.  # noqa: E501
+        Optional array of reserved public IP addresses to be used by the nodes. The IPs must be from the exact location of the node pool's data center. If autoscaling is used, the array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for a fixed number of nodes or maxNodeCount+1). The extra IP is used when the nodes are rebuilt.  # noqa: E501
 
         :param public_ips: The public_ips of this KubernetesNodePoolPropertiesForPost.  # noqa: E501
         :type public_ips: list[str]
         """
 
         self._public_ips = public_ips
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pool_properties_for_put.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pool_properties_for_put.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,51 +133,51 @@
 
         self._name = name
 
     @property
     def node_count(self):
         """Gets the node_count of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
 
-        The number of nodes that make up the node pool.  # noqa: E501
+        The number of worker nodes of the node pool.  # noqa: E501
 
         :return: The node_count of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :rtype: int
         """
         return self._node_count
 
     @node_count.setter
     def node_count(self, node_count):
         """Sets the node_count of this KubernetesNodePoolPropertiesForPut.
 
-        The number of nodes that make up the node pool.  # noqa: E501
+        The number of worker nodes of the node pool.  # noqa: E501
 
         :param node_count: The node_count of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :type node_count: int
         """
         if self.local_vars_configuration.client_side_validation and node_count is None:  # noqa: E501
             raise ValueError("Invalid value for `node_count`, must not be `None`")  # noqa: E501
 
         self._node_count = node_count
 
     @property
     def k8s_version(self):
         """Gets the k8s_version of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :return: The k8s_version of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :rtype: str
         """
         return self._k8s_version
 
     @k8s_version.setter
     def k8s_version(self, k8s_version):
         """Sets the k8s_version of this KubernetesNodePoolPropertiesForPut.
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :param k8s_version: The k8s_version of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :type k8s_version: str
         """
 
         self._k8s_version = k8s_version
 
@@ -223,95 +223,95 @@
 
         self._auto_scaling = auto_scaling
 
     @property
     def lans(self):
         """Gets the lans of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of existing private LANs to attach to worker nodes.  # noqa: E501
 
         :return: The lans of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :rtype: list[KubernetesNodePoolLan]
         """
         return self._lans
 
     @lans.setter
     def lans(self, lans):
         """Sets the lans of this KubernetesNodePoolPropertiesForPut.
 
-        array of additional LANs attached to worker nodes  # noqa: E501
+        The array of existing private LANs to attach to worker nodes.  # noqa: E501
 
         :param lans: The lans of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :type lans: list[KubernetesNodePoolLan]
         """
 
         self._lans = lans
 
     @property
     def labels(self):
         """Gets the labels of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
 
-        map of labels attached to node pool.  # noqa: E501
+        The labels attached to the node pool.  # noqa: E501
 
         :return: The labels of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._labels
 
     @labels.setter
     def labels(self, labels):
         """Sets the labels of this KubernetesNodePoolPropertiesForPut.
 
-        map of labels attached to node pool.  # noqa: E501
+        The labels attached to the node pool.  # noqa: E501
 
         :param labels: The labels of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :type labels: dict(str, str)
         """
 
         self._labels = labels
 
     @property
     def annotations(self):
         """Gets the annotations of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
 
-        map of annotations attached to node pool.  # noqa: E501
+        The annotations attached to the node pool.  # noqa: E501
 
         :return: The annotations of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._annotations
 
     @annotations.setter
     def annotations(self, annotations):
         """Sets the annotations of this KubernetesNodePoolPropertiesForPut.
 
-        map of annotations attached to node pool.  # noqa: E501
+        The annotations attached to the node pool.  # noqa: E501
 
         :param annotations: The annotations of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :type annotations: dict(str, str)
         """
 
         self._annotations = annotations
 
     @property
     def public_ips(self):
         """Gets the public_ips of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
 
-        Optional array of reserved public IP addresses to be used by the nodes. IPs must be from same location as the data center used for the node pool. The array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for fixed number of nodes or maxNodeCount+1 when auto scaling is used). The extra IP is used when the nodes are rebuilt.  # noqa: E501
+        Optional array of reserved public IP addresses to be used by the nodes. The IPs must be from the exact location of the node pool's data center. If autoscaling is used, the array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for a fixed number of nodes or maxNodeCount+1). The extra IP is used when the nodes are rebuilt.  # noqa: E501
 
         :return: The public_ips of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :rtype: list[str]
         """
         return self._public_ips
 
     @public_ips.setter
     def public_ips(self, public_ips):
         """Sets the public_ips of this KubernetesNodePoolPropertiesForPut.
 
-        Optional array of reserved public IP addresses to be used by the nodes. IPs must be from same location as the data center used for the node pool. The array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for fixed number of nodes or maxNodeCount+1 when auto scaling is used). The extra IP is used when the nodes are rebuilt.  # noqa: E501
+        Optional array of reserved public IP addresses to be used by the nodes. The IPs must be from the exact location of the node pool's data center. If autoscaling is used, the array must contain one more IP than the maximum possible number of nodes (nodeCount+1 for a fixed number of nodes or maxNodeCount+1). The extra IP is used when the nodes are rebuilt.  # noqa: E501
 
         :param public_ips: The public_ips of this KubernetesNodePoolPropertiesForPut.  # noqa: E501
         :type public_ips: list[str]
         """
 
         self._public_ips = public_ips
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_pools.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_pools.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,26 +99,26 @@
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesNodePools.  # noqa: E501
 
-        The type of resource within a collection.  # noqa: E501
+        The resource type within a collection.  # noqa: E501
 
         :return: The type of this KubernetesNodePools.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesNodePools.
 
-        The type of resource within a collection.  # noqa: E501
+        The resource type within a collection.  # noqa: E501
 
         :param type: The type of this KubernetesNodePools.  # noqa: E501
         :type type: str
         """
         allowed_values = ["collection"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesNodePools.  # noqa: E501
 
-        URL to the collection representation (absolute path).  # noqa: E501
+        The URL to the collection representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesNodePools.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesNodePools.
 
-        URL to the collection representation (absolute path).  # noqa: E501
+        The URL to the collection representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesNodePools.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_node_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_node_properties.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,97 +74,97 @@
         self.k8s_version = k8s_version
 
 
     @property
     def name(self):
         """Gets the name of this KubernetesNodeProperties.  # noqa: E501
 
-        A Kubernetes node name.  # noqa: E501
+        The Kubernetes node name.  # noqa: E501
 
         :return: The name of this KubernetesNodeProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this KubernetesNodeProperties.
 
-        A Kubernetes node name.  # noqa: E501
+        The Kubernetes node name.  # noqa: E501
 
         :param name: The name of this KubernetesNodeProperties.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def public_ip(self):
         """Gets the public_ip of this KubernetesNodeProperties.  # noqa: E501
 
-        A valid public IP.  # noqa: E501
+        The public IP associated with the node.  # noqa: E501
 
         :return: The public_ip of this KubernetesNodeProperties.  # noqa: E501
         :rtype: str
         """
         return self._public_ip
 
     @public_ip.setter
     def public_ip(self, public_ip):
         """Sets the public_ip of this KubernetesNodeProperties.
 
-        A valid public IP.  # noqa: E501
+        The public IP associated with the node.  # noqa: E501
 
         :param public_ip: The public_ip of this KubernetesNodeProperties.  # noqa: E501
         :type public_ip: str
         """
 
         self._public_ip = public_ip
 
     @property
     def private_ip(self):
         """Gets the private_ip of this KubernetesNodeProperties.  # noqa: E501
 
-        A valid private IP.  # noqa: E501
+        The private IP associated with the node.  # noqa: E501
 
         :return: The private_ip of this KubernetesNodeProperties.  # noqa: E501
         :rtype: str
         """
         return self._private_ip
 
     @private_ip.setter
     def private_ip(self, private_ip):
         """Sets the private_ip of this KubernetesNodeProperties.
 
-        A valid private IP.  # noqa: E501
+        The private IP associated with the node.  # noqa: E501
 
         :param private_ip: The private_ip of this KubernetesNodeProperties.  # noqa: E501
         :type private_ip: str
         """
 
         self._private_ip = private_ip
 
     @property
     def k8s_version(self):
         """Gets the k8s_version of this KubernetesNodeProperties.  # noqa: E501
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :return: The k8s_version of this KubernetesNodeProperties.  # noqa: E501
         :rtype: str
         """
         return self._k8s_version
 
     @k8s_version.setter
     def k8s_version(self, k8s_version):
         """Sets the k8s_version of this KubernetesNodeProperties.
 
-        The Kubernetes version the nodepool is running. This imposes restrictions on what Kubernetes versions can be run in a cluster's nodepools. Additionally, not all Kubernetes versions are viable upgrade targets for all prior versions.  # noqa: E501
+        The Kubernetes version running in the node pool. Note that this imposes restrictions on which Kubernetes versions can run in the node pools of a cluster. Also, not all Kubernetes versions are suitable upgrade targets for all earlier versions.  # noqa: E501
 
         :param k8s_version: The k8s_version of this KubernetesNodeProperties.  # noqa: E501
         :type k8s_version: str
         """
         if self.local_vars_configuration.client_side_validation and k8s_version is None:  # noqa: E501
             raise ValueError("Invalid value for `k8s_version`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/kubernetes_nodes.py` & `ionoscloud-6.1.5/ionoscloud/models/kubernetes_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,26 +99,26 @@
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this KubernetesNodes.  # noqa: E501
 
-        The type of resource within a collection.  # noqa: E501
+        The resource type within a collection.  # noqa: E501
 
         :return: The type of this KubernetesNodes.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this KubernetesNodes.
 
-        The type of resource within a collection.  # noqa: E501
+        The resource type within a collection.  # noqa: E501
 
         :param type: The type of this KubernetesNodes.  # noqa: E501
         :type type: str
         """
         allowed_values = ["collection"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this KubernetesNodes.  # noqa: E501
 
-        URL to the collection representation (absolute path).  # noqa: E501
+        The URL to the collection representation (absolute path).  # noqa: E501
 
         :return: The href of this KubernetesNodes.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this KubernetesNodes.
 
-        URL to the collection representation (absolute path).  # noqa: E501
+        The URL to the collection representation (absolute path).  # noqa: E501
 
         :param href: The href of this KubernetesNodes.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/label.py` & `ionoscloud-6.1.5/ionoscloud/models/label.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/label_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/label_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/label_resource.py` & `ionoscloud-6.1.5/ionoscloud/models/label_resource.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/label_resource_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/label_resource_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/label_resources.py` & `ionoscloud-6.1.5/ionoscloud/models/label_resources.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/labels.py` & `ionoscloud-6.1.5/ionoscloud/models/labels.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lan.py` & `ionoscloud-6.1.5/ionoscloud/models/lan.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lan_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/lan_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lan_nics.py` & `ionoscloud-6.1.5/ionoscloud/models/lan_nics.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lan_post.py` & `ionoscloud-6.1.5/ionoscloud/models/lan_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lan_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/lan_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lan_properties_post.py` & `ionoscloud-6.1.5/ionoscloud/models/lan_properties_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/lans.py` & `ionoscloud-6.1.5/ionoscloud/models/lans.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/loadbalancer.py` & `ionoscloud-6.1.5/ionoscloud/models/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/loadbalancer_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/loadbalancer_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/loadbalancer_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/loadbalancer_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -107,17 +107,14 @@
         """Sets the ip of this LoadbalancerProperties.
 
         IPv4 address of the loadbalancer. All attached NICs will inherit this IP. Leaving value null will assign IP automatically.  # noqa: E501
 
         :param ip: The ip of this LoadbalancerProperties.  # noqa: E501
         :type ip: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                ip is not None and not re.search(r'^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$', ip)):  # noqa: E501
-            raise ValueError(r"Invalid value for `ip`, must be a follow pattern or equal to `/^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/`")  # noqa: E501
 
         self._ip = ip
 
     @property
     def dhcp(self):
         """Gets the dhcp of this LoadbalancerProperties.  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/loadbalancers.py` & `ionoscloud-6.1.5/ionoscloud/models/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/location.py` & `ionoscloud-6.1.5/ionoscloud/models/location.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/location_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/location_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,95 +76,95 @@
             self.cpu_architecture = cpu_architecture
 
 
     @property
     def name(self):
         """Gets the name of this LocationProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The location name.  # noqa: E501
 
         :return: The name of this LocationProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this LocationProperties.
 
-        The name of the  resource.  # noqa: E501
+        The location name.  # noqa: E501
 
         :param name: The name of this LocationProperties.  # noqa: E501
         :type name: str
         """
 
         self._name = name
 
     @property
     def features(self):
         """Gets the features of this LocationProperties.  # noqa: E501
 
-        List of features supported by the location  # noqa: E501
+        A list of available features in the location.  # noqa: E501
 
         :return: The features of this LocationProperties.  # noqa: E501
         :rtype: list[str]
         """
         return self._features
 
     @features.setter
     def features(self, features):
         """Sets the features of this LocationProperties.
 
-        List of features supported by the location  # noqa: E501
+        A list of available features in the location.  # noqa: E501
 
         :param features: The features of this LocationProperties.  # noqa: E501
         :type features: list[str]
         """
 
         self._features = features
 
     @property
     def image_aliases(self):
         """Gets the image_aliases of this LocationProperties.  # noqa: E501
 
-        List of image aliases available for the location  # noqa: E501
+        A list of image aliases available in the location.  # noqa: E501
 
         :return: The image_aliases of this LocationProperties.  # noqa: E501
         :rtype: list[str]
         """
         return self._image_aliases
 
     @image_aliases.setter
     def image_aliases(self, image_aliases):
         """Sets the image_aliases of this LocationProperties.
 
-        List of image aliases available for the location  # noqa: E501
+        A list of image aliases available in the location.  # noqa: E501
 
         :param image_aliases: The image_aliases of this LocationProperties.  # noqa: E501
         :type image_aliases: list[str]
         """
 
         self._image_aliases = image_aliases
 
     @property
     def cpu_architecture(self):
         """Gets the cpu_architecture of this LocationProperties.  # noqa: E501
 
-        Array of features and CPU families available in a location  # noqa: E501
+        A list of available CPU types and related resources available in the location.  # noqa: E501
 
         :return: The cpu_architecture of this LocationProperties.  # noqa: E501
         :rtype: list[CpuArchitectureProperties]
         """
         return self._cpu_architecture
 
     @cpu_architecture.setter
     def cpu_architecture(self, cpu_architecture):
         """Sets the cpu_architecture of this LocationProperties.
 
-        Array of features and CPU families available in a location  # noqa: E501
+        A list of available CPU types and related resources available in the location.  # noqa: E501
 
         :param cpu_architecture: The cpu_architecture of this LocationProperties.  # noqa: E501
         :type cpu_architecture: list[CpuArchitectureProperties]
         """
 
         self._cpu_architecture = cpu_architecture
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/locations.py` & `ionoscloud-6.1.5/ionoscloud/models/locations.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_lan_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_lan_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_put.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_protocol.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_protocol.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_put.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rule_type.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rule_type.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateway_rules.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateway_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nat_gateways.py` & `ionoscloud-6.1.5/ionoscloud/models/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_health_check.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,26 +178,26 @@
 
         self._protocol = protocol
 
     @property
     def listener_ip(self):
         """Gets the listener_ip of this NetworkLoadBalancerForwardingRuleProperties.  # noqa: E501
 
-        Listening (inbound) IP  # noqa: E501
+        Listening (inbound) IP.  # noqa: E501
 
         :return: The listener_ip of this NetworkLoadBalancerForwardingRuleProperties.  # noqa: E501
         :rtype: str
         """
         return self._listener_ip
 
     @listener_ip.setter
     def listener_ip(self, listener_ip):
         """Sets the listener_ip of this NetworkLoadBalancerForwardingRuleProperties.
 
-        Listening (inbound) IP  # noqa: E501
+        Listening (inbound) IP.  # noqa: E501
 
         :param listener_ip: The listener_ip of this NetworkLoadBalancerForwardingRuleProperties.  # noqa: E501
         :type listener_ip: str
         """
         if self.local_vars_configuration.client_side_validation and listener_ip is None:  # noqa: E501
             raise ValueError("Invalid value for `listener_ip`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_put.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_target.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_target.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rule_target_health_check.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_forwarding_rules.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancer_put.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancer_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/network_load_balancers.py` & `ionoscloud-6.1.5/ionoscloud/models/network_load_balancers.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nic.py` & `ionoscloud-6.1.5/ionoscloud/models/nic.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nic_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/nic_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nic_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/nic_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         'firewall_type': 'firewallType',
 
         'device_number': 'deviceNumber',
 
         'pci_slot': 'pciSlot',
     }
 
-    def __init__(self, name=None, mac=None, ips=None, dhcp=None, lan=None, firewall_active=None, firewall_type=None, device_number=None, pci_slot=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, mac=None, ips=None, dhcp=True, lan=None, firewall_active=None, firewall_type=None, device_number=None, pci_slot=None, local_vars_configuration=None):  # noqa: E501
         """NicProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._mac = None
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nic_put.py` & `ionoscloud-6.1.5/ionoscloud/models/nic_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/nics.py` & `ionoscloud-6.1.5/ionoscloud/models/nics.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/no_state_meta_data.py` & `ionoscloud-6.1.5/ionoscloud/models/no_state_meta_data.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/pagination_links.py` & `ionoscloud-6.1.5/ionoscloud/models/pagination_links.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/peer.py` & `ionoscloud-6.1.5/ionoscloud/models/peer.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/private_cross_connect.py` & `ionoscloud-6.1.5/ionoscloud/models/private_cross_connect.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/private_cross_connect_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/private_cross_connect_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/private_cross_connects.py` & `ionoscloud-6.1.5/ionoscloud/models/private_cross_connects.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/remote_console_url.py` & `ionoscloud-6.1.5/ionoscloud/models/remote_console_url.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/request.py` & `ionoscloud-6.1.5/ionoscloud/models/request.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/request_metadata.py` & `ionoscloud-6.1.5/ionoscloud/models/request_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/request_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/request_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/request_status.py` & `ionoscloud-6.1.5/ionoscloud/models/request_status.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/request_status_metadata.py` & `ionoscloud-6.1.5/ionoscloud/models/request_status_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/request_target.py` & `ionoscloud-6.1.5/ionoscloud/models/request_target.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/requests.py` & `ionoscloud-6.1.5/ionoscloud/models/requests.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resource.py` & `ionoscloud-6.1.5/ionoscloud/models/resource.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resource_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/resource_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resource_groups.py` & `ionoscloud-6.1.5/ionoscloud/models/resource_groups.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resource_limits.py` & `ionoscloud-6.1.5/ionoscloud/models/resource_limits.py`

 * *Files 11% similar despite different names*

```diff
@@ -180,551 +180,551 @@
         self.nat_gateway_provisioned = nat_gateway_provisioned
 
 
     @property
     def cores_per_server(self):
         """Gets the cores_per_server of this ResourceLimits.  # noqa: E501
 
-        The maximum number of cores per server.  # noqa: E501
+        The maximum number of CPU cores per server.  # noqa: E501
 
         :return: The cores_per_server of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._cores_per_server
 
     @cores_per_server.setter
     def cores_per_server(self, cores_per_server):
         """Sets the cores_per_server of this ResourceLimits.
 
-        The maximum number of cores per server.  # noqa: E501
+        The maximum number of CPU cores per server.  # noqa: E501
 
         :param cores_per_server: The cores_per_server of this ResourceLimits.  # noqa: E501
         :type cores_per_server: int
         """
         if self.local_vars_configuration.client_side_validation and cores_per_server is None:  # noqa: E501
             raise ValueError("Invalid value for `cores_per_server`, must not be `None`")  # noqa: E501
 
         self._cores_per_server = cores_per_server
 
     @property
     def cores_per_contract(self):
         """Gets the cores_per_contract of this ResourceLimits.  # noqa: E501
 
-        The maximum number of cores per contract.  # noqa: E501
+        The maximum number of CPU cores per contract.  # noqa: E501
 
         :return: The cores_per_contract of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._cores_per_contract
 
     @cores_per_contract.setter
     def cores_per_contract(self, cores_per_contract):
         """Sets the cores_per_contract of this ResourceLimits.
 
-        The maximum number of cores per contract.  # noqa: E501
+        The maximum number of CPU cores per contract.  # noqa: E501
 
         :param cores_per_contract: The cores_per_contract of this ResourceLimits.  # noqa: E501
         :type cores_per_contract: int
         """
         if self.local_vars_configuration.client_side_validation and cores_per_contract is None:  # noqa: E501
             raise ValueError("Invalid value for `cores_per_contract`, must not be `None`")  # noqa: E501
 
         self._cores_per_contract = cores_per_contract
 
     @property
     def cores_provisioned(self):
         """Gets the cores_provisioned of this ResourceLimits.  # noqa: E501
 
-        The number of cores provisioned.  # noqa: E501
+        The number of CPU cores provisioned.  # noqa: E501
 
         :return: The cores_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._cores_provisioned
 
     @cores_provisioned.setter
     def cores_provisioned(self, cores_provisioned):
         """Sets the cores_provisioned of this ResourceLimits.
 
-        The number of cores provisioned.  # noqa: E501
+        The number of CPU cores provisioned.  # noqa: E501
 
         :param cores_provisioned: The cores_provisioned of this ResourceLimits.  # noqa: E501
         :type cores_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and cores_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `cores_provisioned`, must not be `None`")  # noqa: E501
 
         self._cores_provisioned = cores_provisioned
 
     @property
     def ram_per_server(self):
         """Gets the ram_per_server of this ResourceLimits.  # noqa: E501
 
-        The maximum RAM per server.  # noqa: E501
+        The maximum amount of RAM (in MB) that can be provisioned for a particular server under this contract.  # noqa: E501
 
         :return: The ram_per_server of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._ram_per_server
 
     @ram_per_server.setter
     def ram_per_server(self, ram_per_server):
         """Sets the ram_per_server of this ResourceLimits.
 
-        The maximum RAM per server.  # noqa: E501
+        The maximum amount of RAM (in MB) that can be provisioned for a particular server under this contract.  # noqa: E501
 
         :param ram_per_server: The ram_per_server of this ResourceLimits.  # noqa: E501
         :type ram_per_server: int
         """
         if self.local_vars_configuration.client_side_validation and ram_per_server is None:  # noqa: E501
             raise ValueError("Invalid value for `ram_per_server`, must not be `None`")  # noqa: E501
 
         self._ram_per_server = ram_per_server
 
     @property
     def ram_per_contract(self):
         """Gets the ram_per_contract of this ResourceLimits.  # noqa: E501
 
-        The maximum RAM per contract.  # noqa: E501
+        The maximum amount of RAM (in MB) that can be provisioned under this contract.  # noqa: E501
 
         :return: The ram_per_contract of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._ram_per_contract
 
     @ram_per_contract.setter
     def ram_per_contract(self, ram_per_contract):
         """Sets the ram_per_contract of this ResourceLimits.
 
-        The maximum RAM per contract.  # noqa: E501
+        The maximum amount of RAM (in MB) that can be provisioned under this contract.  # noqa: E501
 
         :param ram_per_contract: The ram_per_contract of this ResourceLimits.  # noqa: E501
         :type ram_per_contract: int
         """
         if self.local_vars_configuration.client_side_validation and ram_per_contract is None:  # noqa: E501
             raise ValueError("Invalid value for `ram_per_contract`, must not be `None`")  # noqa: E501
 
         self._ram_per_contract = ram_per_contract
 
     @property
     def ram_provisioned(self):
         """Gets the ram_provisioned of this ResourceLimits.  # noqa: E501
 
-        RAM provisioned.  # noqa: E501
+        The amount of RAM (in MB) provisioned under this contract.  # noqa: E501
 
         :return: The ram_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._ram_provisioned
 
     @ram_provisioned.setter
     def ram_provisioned(self, ram_provisioned):
         """Sets the ram_provisioned of this ResourceLimits.
 
-        RAM provisioned.  # noqa: E501
+        The amount of RAM (in MB) provisioned under this contract.  # noqa: E501
 
         :param ram_provisioned: The ram_provisioned of this ResourceLimits.  # noqa: E501
         :type ram_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and ram_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `ram_provisioned`, must not be `None`")  # noqa: E501
 
         self._ram_provisioned = ram_provisioned
 
     @property
     def hdd_limit_per_volume(self):
         """Gets the hdd_limit_per_volume of this ResourceLimits.  # noqa: E501
 
-        HDD limit per volume.  # noqa: E501
+        The maximum size (in MB) of an idividual hard disk volume.  # noqa: E501
 
         :return: The hdd_limit_per_volume of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._hdd_limit_per_volume
 
     @hdd_limit_per_volume.setter
     def hdd_limit_per_volume(self, hdd_limit_per_volume):
         """Sets the hdd_limit_per_volume of this ResourceLimits.
 
-        HDD limit per volume.  # noqa: E501
+        The maximum size (in MB) of an idividual hard disk volume.  # noqa: E501
 
         :param hdd_limit_per_volume: The hdd_limit_per_volume of this ResourceLimits.  # noqa: E501
         :type hdd_limit_per_volume: int
         """
         if self.local_vars_configuration.client_side_validation and hdd_limit_per_volume is None:  # noqa: E501
             raise ValueError("Invalid value for `hdd_limit_per_volume`, must not be `None`")  # noqa: E501
 
         self._hdd_limit_per_volume = hdd_limit_per_volume
 
     @property
     def hdd_limit_per_contract(self):
         """Gets the hdd_limit_per_contract of this ResourceLimits.  # noqa: E501
 
-        HDD limit per contract.  # noqa: E501
+        The maximum amount of disk space (in MB) that can be provided under this contract.  # noqa: E501
 
         :return: The hdd_limit_per_contract of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._hdd_limit_per_contract
 
     @hdd_limit_per_contract.setter
     def hdd_limit_per_contract(self, hdd_limit_per_contract):
         """Sets the hdd_limit_per_contract of this ResourceLimits.
 
-        HDD limit per contract.  # noqa: E501
+        The maximum amount of disk space (in MB) that can be provided under this contract.  # noqa: E501
 
         :param hdd_limit_per_contract: The hdd_limit_per_contract of this ResourceLimits.  # noqa: E501
         :type hdd_limit_per_contract: int
         """
         if self.local_vars_configuration.client_side_validation and hdd_limit_per_contract is None:  # noqa: E501
             raise ValueError("Invalid value for `hdd_limit_per_contract`, must not be `None`")  # noqa: E501
 
         self._hdd_limit_per_contract = hdd_limit_per_contract
 
     @property
     def hdd_volume_provisioned(self):
         """Gets the hdd_volume_provisioned of this ResourceLimits.  # noqa: E501
 
-        HDD volume provisioned.  # noqa: E501
+        The amount of hard disk space (in MB) that is currently provisioned.  # noqa: E501
 
         :return: The hdd_volume_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._hdd_volume_provisioned
 
     @hdd_volume_provisioned.setter
     def hdd_volume_provisioned(self, hdd_volume_provisioned):
         """Sets the hdd_volume_provisioned of this ResourceLimits.
 
-        HDD volume provisioned.  # noqa: E501
+        The amount of hard disk space (in MB) that is currently provisioned.  # noqa: E501
 
         :param hdd_volume_provisioned: The hdd_volume_provisioned of this ResourceLimits.  # noqa: E501
         :type hdd_volume_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and hdd_volume_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `hdd_volume_provisioned`, must not be `None`")  # noqa: E501
 
         self._hdd_volume_provisioned = hdd_volume_provisioned
 
     @property
     def ssd_limit_per_volume(self):
         """Gets the ssd_limit_per_volume of this ResourceLimits.  # noqa: E501
 
-        SSD limit per volume.  # noqa: E501
+        The maximum size (in MB) of an individual solid state disk volume.  # noqa: E501
 
         :return: The ssd_limit_per_volume of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._ssd_limit_per_volume
 
     @ssd_limit_per_volume.setter
     def ssd_limit_per_volume(self, ssd_limit_per_volume):
         """Sets the ssd_limit_per_volume of this ResourceLimits.
 
-        SSD limit per volume.  # noqa: E501
+        The maximum size (in MB) of an individual solid state disk volume.  # noqa: E501
 
         :param ssd_limit_per_volume: The ssd_limit_per_volume of this ResourceLimits.  # noqa: E501
         :type ssd_limit_per_volume: int
         """
         if self.local_vars_configuration.client_side_validation and ssd_limit_per_volume is None:  # noqa: E501
             raise ValueError("Invalid value for `ssd_limit_per_volume`, must not be `None`")  # noqa: E501
 
         self._ssd_limit_per_volume = ssd_limit_per_volume
 
     @property
     def ssd_limit_per_contract(self):
         """Gets the ssd_limit_per_contract of this ResourceLimits.  # noqa: E501
 
-        SSD limit per contract.  # noqa: E501
+        The maximum amount of solid state disk space (in MB) that can be provisioned under this contract.  # noqa: E501
 
         :return: The ssd_limit_per_contract of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._ssd_limit_per_contract
 
     @ssd_limit_per_contract.setter
     def ssd_limit_per_contract(self, ssd_limit_per_contract):
         """Sets the ssd_limit_per_contract of this ResourceLimits.
 
-        SSD limit per contract.  # noqa: E501
+        The maximum amount of solid state disk space (in MB) that can be provisioned under this contract.  # noqa: E501
 
         :param ssd_limit_per_contract: The ssd_limit_per_contract of this ResourceLimits.  # noqa: E501
         :type ssd_limit_per_contract: int
         """
         if self.local_vars_configuration.client_side_validation and ssd_limit_per_contract is None:  # noqa: E501
             raise ValueError("Invalid value for `ssd_limit_per_contract`, must not be `None`")  # noqa: E501
 
         self._ssd_limit_per_contract = ssd_limit_per_contract
 
     @property
     def ssd_volume_provisioned(self):
         """Gets the ssd_volume_provisioned of this ResourceLimits.  # noqa: E501
 
-        SSD volume provisioned.  # noqa: E501
+        The amount of solid state disk space (in MB) that is currently provisioned.  # noqa: E501
 
         :return: The ssd_volume_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._ssd_volume_provisioned
 
     @ssd_volume_provisioned.setter
     def ssd_volume_provisioned(self, ssd_volume_provisioned):
         """Sets the ssd_volume_provisioned of this ResourceLimits.
 
-        SSD volume provisioned.  # noqa: E501
+        The amount of solid state disk space (in MB) that is currently provisioned.  # noqa: E501
 
         :param ssd_volume_provisioned: The ssd_volume_provisioned of this ResourceLimits.  # noqa: E501
         :type ssd_volume_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and ssd_volume_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `ssd_volume_provisioned`, must not be `None`")  # noqa: E501
 
         self._ssd_volume_provisioned = ssd_volume_provisioned
 
     @property
     def das_volume_provisioned(self):
         """Gets the das_volume_provisioned of this ResourceLimits.  # noqa: E501
 
-        DAS (Direct Attached Storage) volume provisioned.  # noqa: E501
+        The amount of DAS disk space (in MB) in a Cube server that is currently provisioned.  # noqa: E501
 
         :return: The das_volume_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._das_volume_provisioned
 
     @das_volume_provisioned.setter
     def das_volume_provisioned(self, das_volume_provisioned):
         """Sets the das_volume_provisioned of this ResourceLimits.
 
-        DAS (Direct Attached Storage) volume provisioned.  # noqa: E501
+        The amount of DAS disk space (in MB) in a Cube server that is currently provisioned.  # noqa: E501
 
         :param das_volume_provisioned: The das_volume_provisioned of this ResourceLimits.  # noqa: E501
         :type das_volume_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and das_volume_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `das_volume_provisioned`, must not be `None`")  # noqa: E501
 
         self._das_volume_provisioned = das_volume_provisioned
 
     @property
     def reservable_ips(self):
         """Gets the reservable_ips of this ResourceLimits.  # noqa: E501
 
-        Total reservable IP limit for the customer.  # noqa: E501
+        The maximum number of static public IP addresses that can be reserved by this customer across contracts.  # noqa: E501
 
         :return: The reservable_ips of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._reservable_ips
 
     @reservable_ips.setter
     def reservable_ips(self, reservable_ips):
         """Sets the reservable_ips of this ResourceLimits.
 
-        Total reservable IP limit for the customer.  # noqa: E501
+        The maximum number of static public IP addresses that can be reserved by this customer across contracts.  # noqa: E501
 
         :param reservable_ips: The reservable_ips of this ResourceLimits.  # noqa: E501
         :type reservable_ips: int
         """
         if self.local_vars_configuration.client_side_validation and reservable_ips is None:  # noqa: E501
             raise ValueError("Invalid value for `reservable_ips`, must not be `None`")  # noqa: E501
 
         self._reservable_ips = reservable_ips
 
     @property
     def reserved_ips_on_contract(self):
         """Gets the reserved_ips_on_contract of this ResourceLimits.  # noqa: E501
 
-        Reserved ips for the contract.  # noqa: E501
+        The maximum number of static public IP addresses that can be reserved for this contract.  # noqa: E501
 
         :return: The reserved_ips_on_contract of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._reserved_ips_on_contract
 
     @reserved_ips_on_contract.setter
     def reserved_ips_on_contract(self, reserved_ips_on_contract):
         """Sets the reserved_ips_on_contract of this ResourceLimits.
 
-        Reserved ips for the contract.  # noqa: E501
+        The maximum number of static public IP addresses that can be reserved for this contract.  # noqa: E501
 
         :param reserved_ips_on_contract: The reserved_ips_on_contract of this ResourceLimits.  # noqa: E501
         :type reserved_ips_on_contract: int
         """
         if self.local_vars_configuration.client_side_validation and reserved_ips_on_contract is None:  # noqa: E501
             raise ValueError("Invalid value for `reserved_ips_on_contract`, must not be `None`")  # noqa: E501
 
         self._reserved_ips_on_contract = reserved_ips_on_contract
 
     @property
     def reserved_ips_in_use(self):
         """Gets the reserved_ips_in_use of this ResourceLimits.  # noqa: E501
 
-        Reserved ips in use.  # noqa: E501
+        The number of static public IP addresses in use.  # noqa: E501
 
         :return: The reserved_ips_in_use of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._reserved_ips_in_use
 
     @reserved_ips_in_use.setter
     def reserved_ips_in_use(self, reserved_ips_in_use):
         """Sets the reserved_ips_in_use of this ResourceLimits.
 
-        Reserved ips in use.  # noqa: E501
+        The number of static public IP addresses in use.  # noqa: E501
 
         :param reserved_ips_in_use: The reserved_ips_in_use of this ResourceLimits.  # noqa: E501
         :type reserved_ips_in_use: int
         """
         if self.local_vars_configuration.client_side_validation and reserved_ips_in_use is None:  # noqa: E501
             raise ValueError("Invalid value for `reserved_ips_in_use`, must not be `None`")  # noqa: E501
 
         self._reserved_ips_in_use = reserved_ips_in_use
 
     @property
     def k8s_cluster_limit_total(self):
         """Gets the k8s_cluster_limit_total of this ResourceLimits.  # noqa: E501
 
-        K8s clusters total limit.  # noqa: E501
+        The maximum number of Kubernetes clusters that can be created under this contract.  # noqa: E501
 
         :return: The k8s_cluster_limit_total of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._k8s_cluster_limit_total
 
     @k8s_cluster_limit_total.setter
     def k8s_cluster_limit_total(self, k8s_cluster_limit_total):
         """Sets the k8s_cluster_limit_total of this ResourceLimits.
 
-        K8s clusters total limit.  # noqa: E501
+        The maximum number of Kubernetes clusters that can be created under this contract.  # noqa: E501
 
         :param k8s_cluster_limit_total: The k8s_cluster_limit_total of this ResourceLimits.  # noqa: E501
         :type k8s_cluster_limit_total: int
         """
         if self.local_vars_configuration.client_side_validation and k8s_cluster_limit_total is None:  # noqa: E501
             raise ValueError("Invalid value for `k8s_cluster_limit_total`, must not be `None`")  # noqa: E501
 
         self._k8s_cluster_limit_total = k8s_cluster_limit_total
 
     @property
     def k8s_clusters_provisioned(self):
         """Gets the k8s_clusters_provisioned of this ResourceLimits.  # noqa: E501
 
-        K8s clusters provisioned.  # noqa: E501
+        The amount of Kubernetes clusters that is currently provisioned.  # noqa: E501
 
         :return: The k8s_clusters_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._k8s_clusters_provisioned
 
     @k8s_clusters_provisioned.setter
     def k8s_clusters_provisioned(self, k8s_clusters_provisioned):
         """Sets the k8s_clusters_provisioned of this ResourceLimits.
 
-        K8s clusters provisioned.  # noqa: E501
+        The amount of Kubernetes clusters that is currently provisioned.  # noqa: E501
 
         :param k8s_clusters_provisioned: The k8s_clusters_provisioned of this ResourceLimits.  # noqa: E501
         :type k8s_clusters_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and k8s_clusters_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `k8s_clusters_provisioned`, must not be `None`")  # noqa: E501
 
         self._k8s_clusters_provisioned = k8s_clusters_provisioned
 
     @property
     def nlb_limit_total(self):
         """Gets the nlb_limit_total of this ResourceLimits.  # noqa: E501
 
-        NLB total limit.  # noqa: E501
+        The NLB total limit.  # noqa: E501
 
         :return: The nlb_limit_total of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._nlb_limit_total
 
     @nlb_limit_total.setter
     def nlb_limit_total(self, nlb_limit_total):
         """Sets the nlb_limit_total of this ResourceLimits.
 
-        NLB total limit.  # noqa: E501
+        The NLB total limit.  # noqa: E501
 
         :param nlb_limit_total: The nlb_limit_total of this ResourceLimits.  # noqa: E501
         :type nlb_limit_total: int
         """
         if self.local_vars_configuration.client_side_validation and nlb_limit_total is None:  # noqa: E501
             raise ValueError("Invalid value for `nlb_limit_total`, must not be `None`")  # noqa: E501
 
         self._nlb_limit_total = nlb_limit_total
 
     @property
     def nlb_provisioned(self):
         """Gets the nlb_provisioned of this ResourceLimits.  # noqa: E501
 
-        NLBs provisioned.  # noqa: E501
+        The NLBs provisioned.  # noqa: E501
 
         :return: The nlb_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._nlb_provisioned
 
     @nlb_provisioned.setter
     def nlb_provisioned(self, nlb_provisioned):
         """Sets the nlb_provisioned of this ResourceLimits.
 
-        NLBs provisioned.  # noqa: E501
+        The NLBs provisioned.  # noqa: E501
 
         :param nlb_provisioned: The nlb_provisioned of this ResourceLimits.  # noqa: E501
         :type nlb_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and nlb_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `nlb_provisioned`, must not be `None`")  # noqa: E501
 
         self._nlb_provisioned = nlb_provisioned
 
     @property
     def nat_gateway_limit_total(self):
         """Gets the nat_gateway_limit_total of this ResourceLimits.  # noqa: E501
 
-        NAT Gateway total limit.  # noqa: E501
+        The NAT Gateway total limit.  # noqa: E501
 
         :return: The nat_gateway_limit_total of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._nat_gateway_limit_total
 
     @nat_gateway_limit_total.setter
     def nat_gateway_limit_total(self, nat_gateway_limit_total):
         """Sets the nat_gateway_limit_total of this ResourceLimits.
 
-        NAT Gateway total limit.  # noqa: E501
+        The NAT Gateway total limit.  # noqa: E501
 
         :param nat_gateway_limit_total: The nat_gateway_limit_total of this ResourceLimits.  # noqa: E501
         :type nat_gateway_limit_total: int
         """
         if self.local_vars_configuration.client_side_validation and nat_gateway_limit_total is None:  # noqa: E501
             raise ValueError("Invalid value for `nat_gateway_limit_total`, must not be `None`")  # noqa: E501
 
         self._nat_gateway_limit_total = nat_gateway_limit_total
 
     @property
     def nat_gateway_provisioned(self):
         """Gets the nat_gateway_provisioned of this ResourceLimits.  # noqa: E501
 
-        NAT Gateways provisioned.  # noqa: E501
+        The NAT Gateways provisioned.  # noqa: E501
 
         :return: The nat_gateway_provisioned of this ResourceLimits.  # noqa: E501
         :rtype: int
         """
         return self._nat_gateway_provisioned
 
     @nat_gateway_provisioned.setter
     def nat_gateway_provisioned(self, nat_gateway_provisioned):
         """Sets the nat_gateway_provisioned of this ResourceLimits.
 
-        NAT Gateways provisioned.  # noqa: E501
+        The NAT Gateways provisioned.  # noqa: E501
 
         :param nat_gateway_provisioned: The nat_gateway_provisioned of this ResourceLimits.  # noqa: E501
         :type nat_gateway_provisioned: int
         """
         if self.local_vars_configuration.client_side_validation and nat_gateway_provisioned is None:  # noqa: E501
             raise ValueError("Invalid value for `nat_gateway_provisioned`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resource_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/resource_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resource_reference.py` & `ionoscloud-6.1.5/ionoscloud/models/resource_reference.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resources.py` & `ionoscloud-6.1.5/ionoscloud/models/resources.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/resources_users.py` & `ionoscloud-6.1.5/ionoscloud/models/resources_users.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/s3_bucket.py` & `ionoscloud-6.1.5/ionoscloud/models/s3_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,26 @@
         self.name = name
 
 
     @property
     def name(self):
         """Gets the name of this S3Bucket.  # noqa: E501
 
-        Name of the S3 bucket  # noqa: E501
+        The name of the S3 bucket.  # noqa: E501
 
         :return: The name of this S3Bucket.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this S3Bucket.
 
-        Name of the S3 bucket  # noqa: E501
+        The name of the S3 bucket.  # noqa: E501
 
         :param name: The name of this S3Bucket.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/s3_key.py` & `ionoscloud-6.1.5/ionoscloud/models/s3_key.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/s3_key_metadata.py` & `ionoscloud-6.1.5/ionoscloud/models/s3_key_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/s3_key_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/s3_key_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/s3_keys.py` & `ionoscloud-6.1.5/ionoscloud/models/s3_keys.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/s3_object_storage_sso.py` & `ionoscloud-6.1.5/ionoscloud/models/s3_object_storage_sso.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/server.py` & `ionoscloud-6.1.5/ionoscloud/models/server.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/server_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/server_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/server_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/server_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,18 @@
         self._type = None
         self.discriminator = None
 
         if template_uuid is not None:
             self.template_uuid = template_uuid
         if name is not None:
             self.name = name
-        self.cores = cores
-        self.ram = ram
+        if cores is not None:
+            self.cores = cores
+        if ram is not None:
+            self.ram = ram
         if availability_zone is not None:
             self.availability_zone = availability_zone
         if vm_state is not None:
             self.vm_state = vm_state
         if boot_cdrom is not None:
             self.boot_cdrom = boot_cdrom
         if boot_volume is not None:
@@ -162,57 +164,53 @@
 
         self._name = name
 
     @property
     def cores(self):
         """Gets the cores of this ServerProperties.  # noqa: E501
 
-        The total number of cores for the server.  # noqa: E501
+        The total number of cores for the enterprise server.  # noqa: E501
 
         :return: The cores of this ServerProperties.  # noqa: E501
         :rtype: int
         """
         return self._cores
 
     @cores.setter
     def cores(self, cores):
         """Sets the cores of this ServerProperties.
 
-        The total number of cores for the server.  # noqa: E501
+        The total number of cores for the enterprise server.  # noqa: E501
 
         :param cores: The cores of this ServerProperties.  # noqa: E501
         :type cores: int
         """
-        if self.local_vars_configuration.client_side_validation and cores is None:  # noqa: E501
-            raise ValueError("Invalid value for `cores`, must not be `None`")  # noqa: E501
 
         self._cores = cores
 
     @property
     def ram(self):
         """Gets the ram of this ServerProperties.  # noqa: E501
 
-        The memory size for the server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
+        The memory size for the enterprise server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
 
         :return: The ram of this ServerProperties.  # noqa: E501
         :rtype: int
         """
         return self._ram
 
     @ram.setter
     def ram(self, ram):
         """Sets the ram of this ServerProperties.
 
-        The memory size for the server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
+        The memory size for the enterprise server in MB, such as 2048. Size must be specified in multiples of 256 MB with a minimum of 256 MB; however, if you set ramHotPlug to TRUE then you must use a minimum of 1024 MB. If you set the RAM size more than 240GB, then ramHotPlug will be set to FALSE and can not be set to TRUE unless RAM size not set to less than 240GB.  # noqa: E501
 
         :param ram: The ram of this ServerProperties.  # noqa: E501
         :type ram: int
         """
-        if self.local_vars_configuration.client_side_validation and ram is None:  # noqa: E501
-            raise ValueError("Invalid value for `ram`, must not be `None`")  # noqa: E501
 
         self._ram = ram
 
     @property
     def availability_zone(self):
         """Gets the availability_zone of this ServerProperties.  # noqa: E501
 
@@ -312,53 +310,59 @@
 
         self._boot_volume = boot_volume
 
     @property
     def cpu_family(self):
         """Gets the cpu_family of this ServerProperties.  # noqa: E501
 
-        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource.  # noqa: E501
+        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource; must not be provided for CUBE servers.  # noqa: E501
 
         :return: The cpu_family of this ServerProperties.  # noqa: E501
         :rtype: str
         """
         return self._cpu_family
 
     @cpu_family.setter
     def cpu_family(self, cpu_family):
         """Sets the cpu_family of this ServerProperties.
 
-        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource.  # noqa: E501
+        CPU architecture on which server gets provisioned; not all CPU architectures are available in all datacenter regions; available CPU architectures can be retrieved from the datacenter resource; must not be provided for CUBE servers.  # noqa: E501
 
         :param cpu_family: The cpu_family of this ServerProperties.  # noqa: E501
         :type cpu_family: str
         """
 
         self._cpu_family = cpu_family
 
     @property
     def type(self):
         """Gets the type of this ServerProperties.  # noqa: E501
 
-        server usages: ENTERPRISE or CUBE  # noqa: E501
+        Server type.  # noqa: E501
 
         :return: The type of this ServerProperties.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this ServerProperties.
 
-        server usages: ENTERPRISE or CUBE  # noqa: E501
+        Server type.  # noqa: E501
 
         :param type: The type of this ServerProperties.  # noqa: E501
         :type type: str
         """
+        allowed_values = ["ENTERPRISE", "CUBE", "VCPU_INSTANCE"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/servers.py` & `ionoscloud-6.1.5/ionoscloud/models/servers.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/snapshot.py` & `ionoscloud-6.1.5/ionoscloud/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/snapshot_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/snapshot_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/snapshots.py` & `ionoscloud-6.1.5/ionoscloud/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_group.py` & `ionoscloud-6.1.5/ionoscloud/models/target_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this TargetGroup.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this TargetGroup.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this TargetGroup.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this TargetGroup.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_group_health_check.py` & `ionoscloud-6.1.5/ionoscloud/models/target_group_health_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,72 +69,72 @@
             self.retries = retries
 
 
     @property
     def check_timeout(self):
         """Gets the check_timeout of this TargetGroupHealthCheck.  # noqa: E501
 
-        The maximum time in milliseconds to wait for a target to respond to a check. For target VMs with 'Check Interval' set, the lesser of the two  values is used once the TCP connection is established.  # noqa: E501
+        The maximum time in milliseconds is to wait for a target to respond to a check. For target VMs with a 'Check Interval' set, the smaller of the two values is used once the TCP connection is established.  # noqa: E501
 
         :return: The check_timeout of this TargetGroupHealthCheck.  # noqa: E501
         :rtype: int
         """
         return self._check_timeout
 
     @check_timeout.setter
     def check_timeout(self, check_timeout):
         """Sets the check_timeout of this TargetGroupHealthCheck.
 
-        The maximum time in milliseconds to wait for a target to respond to a check. For target VMs with 'Check Interval' set, the lesser of the two  values is used once the TCP connection is established.  # noqa: E501
+        The maximum time in milliseconds is to wait for a target to respond to a check. For target VMs with a 'Check Interval' set, the smaller of the two values is used once the TCP connection is established.  # noqa: E501
 
         :param check_timeout: The check_timeout of this TargetGroupHealthCheck.  # noqa: E501
         :type check_timeout: int
         """
 
         self._check_timeout = check_timeout
 
     @property
     def check_interval(self):
         """Gets the check_interval of this TargetGroupHealthCheck.  # noqa: E501
 
-        The interval in milliseconds between consecutive health checks; default is 2000.  # noqa: E501
+        The interval in milliseconds between consecutive health checks; the default value is '2000'.  # noqa: E501
 
         :return: The check_interval of this TargetGroupHealthCheck.  # noqa: E501
         :rtype: int
         """
         return self._check_interval
 
     @check_interval.setter
     def check_interval(self, check_interval):
         """Sets the check_interval of this TargetGroupHealthCheck.
 
-        The interval in milliseconds between consecutive health checks; default is 2000.  # noqa: E501
+        The interval in milliseconds between consecutive health checks; the default value is '2000'.  # noqa: E501
 
         :param check_interval: The check_interval of this TargetGroupHealthCheck.  # noqa: E501
         :type check_interval: int
         """
 
         self._check_interval = check_interval
 
     @property
     def retries(self):
         """Gets the retries of this TargetGroupHealthCheck.  # noqa: E501
 
-        The maximum number of attempts to reconnect to a target after a connection failure. Valid range is 0 to 65535, and default is three reconnection attempts.  # noqa: E501
+        The maximum number of attempts to reconnect to a target after a connection failure. The valid range is '0 to 65535'; the default value is '3'.  # noqa: E501
 
         :return: The retries of this TargetGroupHealthCheck.  # noqa: E501
         :rtype: int
         """
         return self._retries
 
     @retries.setter
     def retries(self, retries):
         """Sets the retries of this TargetGroupHealthCheck.
 
-        The maximum number of attempts to reconnect to a target after a connection failure. Valid range is 0 to 65535, and default is three reconnection attempts.  # noqa: E501
+        The maximum number of attempts to reconnect to a target after a connection failure. The valid range is '0 to 65535'; the default value is '3'.  # noqa: E501
 
         :param retries: The retries of this TargetGroupHealthCheck.  # noqa: E501
         :type retries: int
         """
 
         self._retries = retries
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_group_http_health_check.py` & `ionoscloud-6.1.5/ionoscloud/models/target_group_http_health_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -88,49 +88,49 @@
             self.negate = negate
 
 
     @property
     def path(self):
         """Gets the path of this TargetGroupHttpHealthCheck.  # noqa: E501
 
-        The path (destination URL) for the HTTP health check request; the default is /.  # noqa: E501
+        The destination URL for HTTP the health check; the default is '/'.  # noqa: E501
 
         :return: The path of this TargetGroupHttpHealthCheck.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
         """Sets the path of this TargetGroupHttpHealthCheck.
 
-        The path (destination URL) for the HTTP health check request; the default is /.  # noqa: E501
+        The destination URL for HTTP the health check; the default is '/'.  # noqa: E501
 
         :param path: The path of this TargetGroupHttpHealthCheck.  # noqa: E501
         :type path: str
         """
 
         self._path = path
 
     @property
     def method(self):
         """Gets the method of this TargetGroupHttpHealthCheck.  # noqa: E501
 
-        The method for the HTTP health check.  # noqa: E501
+        The method used for the health check request.  # noqa: E501
 
         :return: The method of this TargetGroupHttpHealthCheck.  # noqa: E501
         :rtype: str
         """
         return self._method
 
     @method.setter
     def method(self, method):
         """Sets the method of this TargetGroupHttpHealthCheck.
 
-        The method for the HTTP health check.  # noqa: E501
+        The method used for the health check request.  # noqa: E501
 
         :param method: The method of this TargetGroupHttpHealthCheck.  # noqa: E501
         :type method: str
         """
         allowed_values = ["HEAD", "PUT", "POST", "GET", "TRACE", "PATCH", "OPTIONS"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and method not in allowed_values:  # noqa: E501
             raise ValueError(
@@ -140,26 +140,26 @@
 
         self._method = method
 
     @property
     def match_type(self):
         """Gets the match_type of this TargetGroupHttpHealthCheck.  # noqa: E501
 
-          # noqa: E501
+        Specify the target's response type to match ALB's request.  # noqa: E501
 
         :return: The match_type of this TargetGroupHttpHealthCheck.  # noqa: E501
         :rtype: str
         """
         return self._match_type
 
     @match_type.setter
     def match_type(self, match_type):
         """Sets the match_type of this TargetGroupHttpHealthCheck.
 
-          # noqa: E501
+        Specify the target's response type to match ALB's request.  # noqa: E501
 
         :param match_type: The match_type of this TargetGroupHttpHealthCheck.  # noqa: E501
         :type match_type: str
         """
         if self.local_vars_configuration.client_side_validation and match_type is None:  # noqa: E501
             raise ValueError("Invalid value for `match_type`, must not be `None`")  # noqa: E501
         allowed_values = ["STATUS_CODE", "RESPONSE_BODY"]  # noqa: E501
@@ -171,74 +171,74 @@
 
         self._match_type = match_type
 
     @property
     def response(self):
         """Gets the response of this TargetGroupHttpHealthCheck.  # noqa: E501
 
-        The response returned by the request, depending on the match type.  # noqa: E501
+        The response returned by the request. It can be a status code or a response body depending on the definition of 'matchType'.  # noqa: E501
 
         :return: The response of this TargetGroupHttpHealthCheck.  # noqa: E501
         :rtype: str
         """
         return self._response
 
     @response.setter
     def response(self, response):
         """Sets the response of this TargetGroupHttpHealthCheck.
 
-        The response returned by the request, depending on the match type.  # noqa: E501
+        The response returned by the request. It can be a status code or a response body depending on the definition of 'matchType'.  # noqa: E501
 
         :param response: The response of this TargetGroupHttpHealthCheck.  # noqa: E501
         :type response: str
         """
         if self.local_vars_configuration.client_side_validation and response is None:  # noqa: E501
             raise ValueError("Invalid value for `response`, must not be `None`")  # noqa: E501
 
         self._response = response
 
     @property
     def regex(self):
         """Gets the regex of this TargetGroupHttpHealthCheck.  # noqa: E501
 
-          # noqa: E501
+        Specifies whether to use a regular expression to parse the response body; the default value is 'FALSE'.  By using regular expressions, you can flexibly customize the expected response from a healthy server.  # noqa: E501
 
         :return: The regex of this TargetGroupHttpHealthCheck.  # noqa: E501
         :rtype: bool
         """
         return self._regex
 
     @regex.setter
     def regex(self, regex):
         """Sets the regex of this TargetGroupHttpHealthCheck.
 
-          # noqa: E501
+        Specifies whether to use a regular expression to parse the response body; the default value is 'FALSE'.  By using regular expressions, you can flexibly customize the expected response from a healthy server.  # noqa: E501
 
         :param regex: The regex of this TargetGroupHttpHealthCheck.  # noqa: E501
         :type regex: bool
         """
 
         self._regex = regex
 
     @property
     def negate(self):
         """Gets the negate of this TargetGroupHttpHealthCheck.  # noqa: E501
 
-          # noqa: E501
+        Specifies whether to negate an individual entry; the default value is 'FALSE'.  # noqa: E501
 
         :return: The negate of this TargetGroupHttpHealthCheck.  # noqa: E501
         :rtype: bool
         """
         return self._negate
 
     @negate.setter
     def negate(self, negate):
         """Sets the negate of this TargetGroupHttpHealthCheck.
 
-          # noqa: E501
+        Specifies whether to negate an individual entry; the default value is 'FALSE'.  # noqa: E501
 
         :param negate: The negate of this TargetGroupHttpHealthCheck.  # noqa: E501
         :type negate: bool
         """
 
         self._negate = negate
     def to_dict(self):
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_group_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/target_group_properties.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,51 +87,51 @@
             self.http_health_check = http_health_check
 
 
     @property
     def name(self):
         """Gets the name of this TargetGroupProperties.  # noqa: E501
 
-        The name of the target group.  # noqa: E501
+        The target group name.  # noqa: E501
 
         :return: The name of this TargetGroupProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this TargetGroupProperties.
 
-        The name of the target group.  # noqa: E501
+        The target group name.  # noqa: E501
 
         :param name: The name of this TargetGroupProperties.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def algorithm(self):
         """Gets the algorithm of this TargetGroupProperties.  # noqa: E501
 
-        Balancing algorithm  # noqa: E501
+        The balancing algorithm. A balancing algorithm consists of predefined rules with the logic that a load balancer uses to distribute network traffic between servers.  - **Round Robin**: Targets are served alternately according to their weighting.  - **Least Connection**: The target with the least active connection is served.  - **Random**: The targets are served based on a consistent pseudorandom algorithm.  - **Source IP**: It is ensured that the same client IP address reaches the same target.  # noqa: E501
 
         :return: The algorithm of this TargetGroupProperties.  # noqa: E501
         :rtype: str
         """
         return self._algorithm
 
     @algorithm.setter
     def algorithm(self, algorithm):
         """Sets the algorithm of this TargetGroupProperties.
 
-        Balancing algorithm  # noqa: E501
+        The balancing algorithm. A balancing algorithm consists of predefined rules with the logic that a load balancer uses to distribute network traffic between servers.  - **Round Robin**: Targets are served alternately according to their weighting.  - **Least Connection**: The target with the least active connection is served.  - **Random**: The targets are served based on a consistent pseudorandom algorithm.  - **Source IP**: It is ensured that the same client IP address reaches the same target.  # noqa: E501
 
         :param algorithm: The algorithm of this TargetGroupProperties.  # noqa: E501
         :type algorithm: str
         """
         if self.local_vars_configuration.client_side_validation and algorithm is None:  # noqa: E501
             raise ValueError("Invalid value for `algorithm`, must not be `None`")  # noqa: E501
         allowed_values = ["ROUND_ROBIN", "LEAST_CONNECTION", "RANDOM", "SOURCE_IP"]  # noqa: E501
@@ -143,26 +143,26 @@
 
         self._algorithm = algorithm
 
     @property
     def protocol(self):
         """Gets the protocol of this TargetGroupProperties.  # noqa: E501
 
-        Balancing protocol  # noqa: E501
+        The forwarding protocol. Only the value 'HTTP' is allowed.  # noqa: E501
 
         :return: The protocol of this TargetGroupProperties.  # noqa: E501
         :rtype: str
         """
         return self._protocol
 
     @protocol.setter
     def protocol(self, protocol):
         """Sets the protocol of this TargetGroupProperties.
 
-        Balancing protocol  # noqa: E501
+        The forwarding protocol. Only the value 'HTTP' is allowed.  # noqa: E501
 
         :param protocol: The protocol of this TargetGroupProperties.  # noqa: E501
         :type protocol: str
         """
         if self.local_vars_configuration.client_side_validation and protocol is None:  # noqa: E501
             raise ValueError("Invalid value for `protocol`, must not be `None`")  # noqa: E501
         allowed_values = ["HTTP"]  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_group_put.py` & `ionoscloud-6.1.5/ionoscloud/models/target_group_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,26 +121,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this TargetGroupPut.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this TargetGroupPut.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this TargetGroupPut.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this TargetGroupPut.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_group_target.py` & `ionoscloud-6.1.5/ionoscloud/models/target_group_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,76 +80,76 @@
             self.maintenance_enabled = maintenance_enabled
 
 
     @property
     def ip(self):
         """Gets the ip of this TargetGroupTarget.  # noqa: E501
 
-        The IP of the balanced target VM.  # noqa: E501
+        The IP address of the balanced target.  # noqa: E501
 
         :return: The ip of this TargetGroupTarget.  # noqa: E501
         :rtype: str
         """
         return self._ip
 
     @ip.setter
     def ip(self, ip):
         """Sets the ip of this TargetGroupTarget.
 
-        The IP of the balanced target VM.  # noqa: E501
+        The IP address of the balanced target.  # noqa: E501
 
         :param ip: The ip of this TargetGroupTarget.  # noqa: E501
         :type ip: str
         """
         if self.local_vars_configuration.client_side_validation and ip is None:  # noqa: E501
             raise ValueError("Invalid value for `ip`, must not be `None`")  # noqa: E501
 
         self._ip = ip
 
     @property
     def port(self):
         """Gets the port of this TargetGroupTarget.  # noqa: E501
 
-        The port of the balanced target service; valid range is 1 to 65535.  # noqa: E501
+        The port of the balanced target service; the valid range is 1 to 65535.  # noqa: E501
 
         :return: The port of this TargetGroupTarget.  # noqa: E501
         :rtype: int
         """
         return self._port
 
     @port.setter
     def port(self, port):
         """Sets the port of this TargetGroupTarget.
 
-        The port of the balanced target service; valid range is 1 to 65535.  # noqa: E501
+        The port of the balanced target service; the valid range is 1 to 65535.  # noqa: E501
 
         :param port: The port of this TargetGroupTarget.  # noqa: E501
         :type port: int
         """
         if self.local_vars_configuration.client_side_validation and port is None:  # noqa: E501
             raise ValueError("Invalid value for `port`, must not be `None`")  # noqa: E501
 
         self._port = port
 
     @property
     def weight(self):
         """Gets the weight of this TargetGroupTarget.  # noqa: E501
 
-        Traffic is distributed in proportion to target weight, relative to the combined weight of all targets. A target with higher weight receives a greater share of traffic. Valid range is 0 to 256 and default is 1; targets with weight of 0 do not participate in load balancing but still accept persistent connections. It is best use values in the middle of the range to leave room for later adjustments.  # noqa: E501
+        The traffic is distributed proportionally to target weight, which is the ratio of the total weight of all targets. A target with higher weight receives a larger share of traffic. The valid range is from 0 to 256; the default value is '1'. Targets with a weight of '0' do not participate in load balancing but still accept persistent connections. We recommend using values in the middle range to leave room for later adjustments.  # noqa: E501
 
         :return: The weight of this TargetGroupTarget.  # noqa: E501
         :rtype: int
         """
         return self._weight
 
     @weight.setter
     def weight(self, weight):
         """Sets the weight of this TargetGroupTarget.
 
-        Traffic is distributed in proportion to target weight, relative to the combined weight of all targets. A target with higher weight receives a greater share of traffic. Valid range is 0 to 256 and default is 1; targets with weight of 0 do not participate in load balancing but still accept persistent connections. It is best use values in the middle of the range to leave room for later adjustments.  # noqa: E501
+        The traffic is distributed proportionally to target weight, which is the ratio of the total weight of all targets. A target with higher weight receives a larger share of traffic. The valid range is from 0 to 256; the default value is '1'. Targets with a weight of '0' do not participate in load balancing but still accept persistent connections. We recommend using values in the middle range to leave room for later adjustments.  # noqa: E501
 
         :param weight: The weight of this TargetGroupTarget.  # noqa: E501
         :type weight: int
         """
         if self.local_vars_configuration.client_side_validation and weight is None:  # noqa: E501
             raise ValueError("Invalid value for `weight`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_groups.py` & `ionoscloud-6.1.5/ionoscloud/models/target_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,26 +143,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this TargetGroups.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this TargetGroups.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this TargetGroups.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this TargetGroups.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/target_port_range.py` & `ionoscloud-6.1.5/ionoscloud/models/target_port_range.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/template.py` & `ionoscloud-6.1.5/ionoscloud/models/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this Template.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this Template.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this Template.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this Template.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/template_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/template_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,26 +72,26 @@
         self.storage_size = storage_size
 
 
     @property
     def name(self):
         """Gets the name of this TemplateProperties.  # noqa: E501
 
-        The name of the  resource.  # noqa: E501
+        The resource name.  # noqa: E501
 
         :return: The name of this TemplateProperties.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this TemplateProperties.
 
-        The name of the  resource.  # noqa: E501
+        The resource name.  # noqa: E501
 
         :param name: The name of this TemplateProperties.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/templates.py` & `ionoscloud-6.1.5/ionoscloud/models/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,26 +122,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this Templates.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this Templates.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this Templates.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this Templates.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/token.py` & `ionoscloud-6.1.5/ionoscloud/models/token.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/type.py` & `ionoscloud-6.1.5/ionoscloud/models/type.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user.py` & `ionoscloud-6.1.5/ionoscloud/models/user.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user_metadata.py` & `ionoscloud-6.1.5/ionoscloud/models/user_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user_post.py` & `ionoscloud-6.1.5/ionoscloud/models/user_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/user_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user_properties_post.py` & `ionoscloud-6.1.5/ionoscloud/models/user_properties_post.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user_properties_put.py` & `ionoscloud-6.1.5/ionoscloud/models/user_properties_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/user_put.py` & `ionoscloud-6.1.5/ionoscloud/models/user_put.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/users.py` & `ionoscloud-6.1.5/ionoscloud/models/users.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/users_entities.py` & `ionoscloud-6.1.5/ionoscloud/models/users_entities.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/models/volume.py` & `ionoscloud-6.1.5/ionoscloud/models/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,26 +128,26 @@
 
         self._type = type
 
     @property
     def href(self):
         """Gets the href of this Volume.  # noqa: E501
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :return: The href of this Volume.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
         """Sets the href of this Volume.
 
-        URL to the object representation (absolute path).  # noqa: E501
+        The URL to the object representation (absolute path).  # noqa: E501
 
         :param href: The href of this Volume.  # noqa: E501
         :type href: str
         """
 
         self._href = href
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/volume_properties.py` & `ionoscloud-6.1.5/ionoscloud/models/volume_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,16 +193,15 @@
             self.pci_slot = pci_slot
         if backupunit_id is not None:
             self.backupunit_id = backupunit_id
         if user_data is not None:
             self.user_data = user_data
         if boot_server is not None:
             self.boot_server = boot_server
-        if boot_order is not None:
-            self.boot_order = boot_order
+        self.boot_order = boot_order
 
 
     @property
     def name(self):
         """Gets the name of this VolumeProperties.  # noqa: E501
 
         The name of the  resource.  # noqa: E501
@@ -724,15 +723,15 @@
         """Sets the boot_order of this VolumeProperties.
 
         Determines whether the volume will be used as a boot volume. Set to `NONE`, the volume will not be used as boot volume. Set to `PRIMARY`, the volume will be used as boot volume and all other volumes must be set to `NONE`. Set to `AUTO` or `null` requires all volumes to be set to `AUTO` or `null`; this will use the legacy behavior, which is to use the volume as a boot volume only if there are no other volumes or cdrom devices.  # noqa: E501
 
         :param boot_order: The boot_order of this VolumeProperties.  # noqa: E501
         :type boot_order: str
         """
-        allowed_values = ["AUTO", "NONE", "PRIMARY"]  # noqa: E501
+        allowed_values = [None,"AUTO", "NONE", "PRIMARY"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and boot_order not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `boot_order` ({0}), must be one of {1}"  # noqa: E501
                 .format(boot_order, allowed_values)
             )
 
         self._boot_order = boot_order
```

### Comparing `ionoscloud-6.1.4/ionoscloud/models/volumes.py` & `ionoscloud-6.1.5/ionoscloud/models/volumes.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud/rest.py` & `ionoscloud-6.1.5/ionoscloud/rest.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-6.1.4/ionoscloud.egg-info/SOURCES.txt` & `ionoscloud-6.1.5/ionoscloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 ionoscloud/__init__.py
 ionoscloud/api_client.py
 ionoscloud/configuration.py
 ionoscloud/exceptions.py
```

### Comparing `ionoscloud-6.1.4/setup.py` & `ionoscloud-6.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup  # noqa: H301
 import os
 import codecs
 
 NAME = "ionoscloud"
-VERSION = "6.1.4"
+VERSION = "6.1.5"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

