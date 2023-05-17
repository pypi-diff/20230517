# Comparing `tmp/kubemarine-0.16.0.tar.gz` & `tmp/kubemarine-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.16.0.tar", last modified: Wed Apr 26 09:35:28 2023, max compression
+gzip compressed data, was "kubemarine-0.17.0.tar", last modified: Mon May 15 10:01:30 2023, max compression
```

## Comparing `kubemarine-0.16.0.tar` & `kubemarine-0.17.0.tar`

### file list

```diff
@@ -1,235 +1,237 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.509318 kubemarine-0.16.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-26 09:35:14.000000 kubemarine-0.16.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-26 09:35:14.000000 kubemarine-0.16.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12361 2023-04-26 09:35:28.509318 kubemarine-0.16.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-26 09:35:14.000000 kubemarine-0.16.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.485318 kubemarine-0.16.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-04-26 09:35:14.000000 kubemarine-0.16.0/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-04-26 09:35:14.000000 kubemarine-0.16.0/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.489318 kubemarine-0.16.0/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8380 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    44652 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15402 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    23933 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    15921 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    17948 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    39980 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    12720 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8220 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15178 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    20046 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     6769 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     2627 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6492 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3784 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    19878 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10879 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11275 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    63972 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    19658 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1112 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/patches/p1_helm_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    38251 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    14938 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    18029 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222019 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4910 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20629 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2620 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50542 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    74051 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5053 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26777 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1760 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1658 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    15470 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2371 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6679 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    13644 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    13192 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     3162 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     4638 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     3345 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     5199 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     2489 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    27019 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     9376 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.485318 kubemarine-0.16.0/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/etalons/patches/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      615 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2217 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3096 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9465 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4856 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      936 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4092 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5128 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1619 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2826 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1206 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    32103 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.509318 kubemarine-0.16.0/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    10441 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    13898 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     4843 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.489318 kubemarine-0.16.0/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12361 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8783 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2553 2023-04-26 09:35:14.000000 kubemarine-0.16.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 09:35:28.509318 kubemarine-0.16.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1576 2023-04-26 09:35:14.000000 kubemarine-0.16.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.492222 kubemarine-0.17.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-15 10:01:16.000000 kubemarine-0.17.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-15 10:01:16.000000 kubemarine-0.17.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-05-15 10:01:30.492222 kubemarine-0.17.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-05-15 10:01:16.000000 kubemarine-0.17.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.460221 kubemarine-0.17.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-05-15 10:01:16.000000 kubemarine-0.17.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-15 10:01:16.000000 kubemarine-0.17.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.464221 kubemarine-0.17.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8195 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    44406 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15462 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    23611 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    15921 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    18873 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    39980 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    12720 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8286 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    20944 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6492 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3784 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    19878 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10879 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11275 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    63792 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    19658 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/patches/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.468222 kubemarine-0.17.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    38251 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14938 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    18795 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.472221 kubemarine-0.17.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4919 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    20638 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2629 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50500 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    74067 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     5081 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26620 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1769 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1667 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    15479 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2380 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6074 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    13653 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    13619 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    27351 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.456221 kubemarine-0.17.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/etalons/patches/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.476222 kubemarine-0.17.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.480222 kubemarine-0.17.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.480222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.480222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      615 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.484222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.484222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      585 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.484222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4092 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    31848 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.488222 kubemarine-0.17.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.492222 kubemarine-0.17.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    10441 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    13898 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-05-15 10:01:16.000000 kubemarine-0.17.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:01:30.464221 kubemarine-0.17.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8938 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-15 10:01:30.000000 kubemarine-0.17.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-05-15 10:01:16.000000 kubemarine-0.17.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 10:01:30.492222 kubemarine-0.17.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-15 10:01:16.000000 kubemarine-0.17.0/setup.py
```

### Comparing `kubemarine-0.16.0/LICENSE` & `kubemarine-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/PKG-INFO` & `kubemarine-0.17.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.16.0
+Version: 0.17.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
+Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
 Keywords: kubernetes,devops,administration,helm
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -79,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -98,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -127,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.16.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.17.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -172,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.16.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.17.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.16.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.17.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.16.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.17.0/LICENSE)
```

### Comparing `kubemarine-0.16.0/README.md` & `kubemarine-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/bin/kubemarine` & `kubemarine-0.17.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/bin/kubemarine.cmd` & `kubemarine-0.17.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/__init__.py` & `kubemarine-0.17.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/__main__.py` & `kubemarine-0.17.0/kubemarine/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,19 +155,15 @@
         print('''The following procedures available:
 %s
 
 Usage: kubemarine <procedure> <arguments>
 ''' % '\n'.join(descriptions_print_list))
         sys.exit(1)
 
-    result = import_procedure(arguments[0]).main(arguments[1:])
-    if result is not None:
-        from kubemarine.testsuite import TestSuite
-        if isinstance(result, TestSuite) and result.is_any_test_failed():
-            sys.exit(1)
+    import_procedure(arguments[0]).main(arguments[1:])
 
 
 def import_procedure(name):
     module_name = 'kubemarine.procedures.%s' % name
     return __import__(module_name, fromlist=['object'])
```

### Comparing `kubemarine-0.16.0/kubemarine/admission.py` & `kubemarine-0.17.0/kubemarine/admission.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,22 +586,22 @@
         for item in procedure_config["defaults"]:
             if item.endswith("version"):
                 verify_version(item, procedure_config["defaults"][item], minor_version)
             inventory["rbac"]["pss"]["defaults"][item] = procedure_config["defaults"][item]
     if "exemptions" in procedure_config:
         default_merger.merge(inventory["rbac"]["pss"]["exemptions"], procedure_config["exemptions"])
     if "namespaces" in procedure_config:
-        for namespace in procedure_config["namespaces"]:
+        for namespace_item in procedure_config["namespaces"]:
             # check if the namespace has its own profiles
-            if isinstance(namespace, dict):
-                profiles = list(namespace.values())[0]
-                for item in profiles:
-                    if item.endswith("version"):
-                        verify_version(item, profiles[item], minor_version)
-                raise Exception("Custom labels for each namespace are currently not supported")
+            if isinstance(namespace_item, dict):
+                namespace = list(namespace_item.keys())[0]
+                for item in list(namespace_item[namespace]):
+                    if namespace_item[namespace][item]:
+                        if item.endswith("version"):
+                            verify_version(item, namespace_item[namespace][item], minor_version)
     if "namespaces_defaults" in procedure_config:
         for item in procedure_config["namespaces_defaults"]:
             if item.endswith("version"):
                 verify_version(item, procedure_config["namespaces_defaults"][item], minor_version)
 
     return inventory
 
@@ -826,101 +826,93 @@
     group.sudo("rm -f %s" % remote_path)
 
     return result
 
 
 def label_namespace_pss(cluster, manage_type):
     first_control_plane = cluster.nodes["control-plane"].get_first_member()
-    # get default PSS profile
-    profile = cluster.inventory["rbac"]["pss"]["defaults"]["enforce"]
+    # set/delete labels on predifined plugins namsespaces
     for plugin in cluster.inventory["plugins"]:
         is_install = cluster.inventory["plugins"][plugin].get("install")
-        # set/delete label 'pod-security.kubernetes.io/enforce: privileged' for local provisioner and ingress namespaces
         if manage_type in ["apply", "install"]:
-            if is_install and plugin in privileged_plugins.keys() and profile != "privileged":
-                cluster.log.debug("Set PSS labels on namespace %s" % privileged_plugins[plugin])
+            if is_install and plugin in privileged_plugins.keys():
+                # set label 'pod-security.kubernetes.io/enforce: privileged' for local provisioner and ingress namespaces
+                cluster.log.debug(f"Set PSS labels on namespace {privileged_plugins[plugin]}")
                 for mode in valid_modes:
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s=%s --overwrite" 
-                                      % (privileged_plugins[plugin], mode, "privileged"))
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s-version=%s --overwrite" 
-                                      % (privileged_plugins[plugin], mode, "latest"))
-            # set/delete label 'pod-security.kubernetes.io/enforce: baseline' for kubernetes dashboard
-            elif is_install and plugin in baseline_plugins.keys() and profile == "restricted":
-                cluster.log.debug("Set PSS labels on namespace %s" % baseline_plugins[plugin])
+                    first_control_plane.sudo(f"kubectl label ns {privileged_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}=privileged --overwrite")
+                    first_control_plane.sudo(f"kubectl label ns {privileged_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}-version=latest --overwrite")
+            elif is_install and plugin in baseline_plugins.keys():
+                # set label 'pod-security.kubernetes.io/enforce: baseline' for kubernetes dashboard
+                cluster.log.debug(f"Set PSS labels on namespace {baseline_plugins[plugin]}")
                 for mode in valid_modes:
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s=%s --overwrite" 
-                                      % (baseline_plugins[plugin], mode, "baseline"))
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s-version=%s --overwrite" 
-                                      % (baseline_plugins[plugin], mode, "latest"))
+                    first_control_plane.sudo(f"kubectl label ns {baseline_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}=baseline --overwrite")
+                    first_control_plane.sudo(f"kubectl label ns {baseline_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}-version=latest --overwrite")
         elif manage_type == "delete":
             if is_install and plugin in privileged_plugins.keys():
-                cluster.log.debug("Delete PSS labels from namespace %s" % privileged_plugins[plugin])
+                # delete label 'pod-security.kubernetes.io/enforce: privileged' for local provisioner and ingress namespaces
+                cluster.log.debug(f"Delete PSS labels from namespace {privileged_plugins[plugin]}")
                 for mode in valid_modes:
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s- || true" 
-                                      % (privileged_plugins[plugin], mode))
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s-version- || true" 
-                                      % (privileged_plugins[plugin], mode))
+                    first_control_plane.sudo(f"kubectl label ns {privileged_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}- || true")
+                    first_control_plane.sudo(f"kubectl label ns {privileged_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}-version- || true")
             elif is_install and plugin in baseline_plugins.keys():
-                cluster.log.debug("Delete PSS labels from namespace %s" % baseline_plugins[plugin])
+                # delete 'pod-security.kubernetes.io/enforce: baseline' for kubernetes dashboard
+                cluster.log.debug(f"Delete PSS labels from namespace {baseline_plugins[plugin]}")
                 for mode in valid_modes:
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s- || true" 
-                                      % (baseline_plugins[plugin], mode))
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s-version- || true" 
-                                      % (baseline_plugins[plugin], mode))
+                    first_control_plane.sudo(f"kubectl label ns {baseline_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}- || true")
+                    first_control_plane.sudo(f"kubectl label ns {baseline_plugins[plugin]} "
+                                             f"pod-security.kubernetes.io/{mode}-version- || true")
 
     procedure_config = cluster.procedure_inventory["pss"]
     namespaces = procedure_config.get("namespaces")
     # get the list of namespaces that should be labeled then set/delete labels
     if namespaces:
         default_modes = {}
         # check if procedure config has default values for labels
         namespaces_defaults = procedure_config.get("namespaces_defaults")
         if namespaces_defaults:
             for default_mode in namespaces_defaults:
                  default_modes[default_mode] = namespaces_defaults[default_mode]
         for namespace in namespaces:
+            # define name of namespace
+            if isinstance(namespace, dict):
+                ns_name = list(namespace.keys())[0]
+            else:
+                ns_name = namespace
             if manage_type in ["apply", "install"]:
-                # define name of namespace
-                if type(namespace) is dict:
-                    for item in namespace:
-                        if not namespace[item]:
-                            ns_name = item
-                else:
-                    ns_name = namespace
                 if default_modes:
                     # set labels that are set in default section
-                    cluster.log.debug("Set PSS labels on %s namespace from defaults" % ns_name)
+                    cluster.log.debug(f"Set PSS labels on {ns_name} namespace from defaults")
                     for mode in default_modes:
-                        first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s=%s --overwrite" 
-                                          % (ns_name, mode, default_modes[mode]))
-                if type(namespace) is dict:
+                        first_control_plane.sudo(f"kubectl label ns {ns_name} "
+                                f"pod-security.kubernetes.io/{mode}={default_modes[mode]} --overwrite")
+                if isinstance(namespace, dict):
                     # set labels that are set in namespaces section
-                    cluster.log.debug("Set PSS labels on %s namespace" % ns_name)
-                    for mode in namespace: 
-                        if namespace[mode]:
-                            first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s=%s --overwrite" 
-                                              % (ns_name, mode, namespace[mode]))
+                    cluster.log.debug(f"Set PSS labels on {ns_name} namespace")
+                    for item in list(namespace[ns_name]):
+                        first_control_plane.sudo(f"kubectl label ns {ns_name} " 
+                                    f"pod-security.kubernetes.io/{item}={namespace[ns_name][item]} --overwrite")
             elif manage_type == "delete":
-                # define name of namespace
-                if type(namespace) is dict:
-                    for item in namespace:
-                        if not namespace[item]:
-                            ns_name = item
-                else:
-                    ns_name = namespace
                 # delete labels that are set in default section
-                cluster.log.debug("Delete PSS labels on %s namespace from defaults" % ns_name)
-                for mode in default_modes:
-                    first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s-" % (ns_name, mode))
+                if default_modes:
+                    cluster.log.debug(f"Delete PSS labels on {ns_name} namespace from defaults")
+                    for mode in default_modes:
+                        first_control_plane.sudo(f"kubectl label ns {ns_name} pod-security.kubernetes.io/{mode}-")
                 # delete labels that are set in namespaces section
-                cluster.log.debug("Delete PSS labels on %s namespace" % ns_name)
-                if type(namespace) is dict:
-                    for mode in namespace:
-                        if namespace[mode]:
-                            first_control_plane.sudo("kubectl label ns %s pod-security.kubernetes.io/%s-" % (ns_name, mode))
+                cluster.log.debug(f"Delete PSS labels on {ns_name} namespace")
+                if isinstance(namespace, dict):
+                    for item in list(namespace[ns_name]):
+                        first_control_plane.sudo(f"kubectl label ns {ns_name} "
+                                    f"pod-security.kubernetes.io/{item}-")
 
 
 def check_inventory(cluster):
     # check if 'admission' option in cluster.yaml and procedure.yaml are inconsistent 
     if cluster.context.get('initial_procedure') == 'manage_pss' and cluster.inventory["rbac"]["admission"] != "pss" or \
         cluster.context.get('initial_procedure') == 'manage_psp' and cluster.inventory["rbac"]["admission"] != "psp":
         raise Exception("Procedure config and cluster config are inconsistent. Please check 'admission' option")
```

### Comparing `kubemarine-0.16.0/kubemarine/apparmor.py` & `kubemarine-0.17.0/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/apt.py` & `kubemarine-0.17.0/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/audit.py` & `kubemarine-0.17.0/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/controlplane.py` & `kubemarine-0.17.0/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/__init__.py` & `kubemarine-0.17.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/action.py` & `kubemarine-0.17.0/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/annotations.py` & `kubemarine-0.17.0/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/cluster.py` & `kubemarine-0.17.0/kubemarine/core/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         from kubemarine.core import flow
         return flow.is_task_completed(self, task_path)
 
     def get_facts_enrichment_fns(self):
         return [
             "kubemarine.core.schema.verify_inventory",
             "kubemarine.core.defaults.merge_defaults",
+            "kubemarine.kubernetes.verify_initial_version",
             "kubemarine.kubernetes.add_node_enrichment",
             "kubemarine.kubernetes.remove_node_enrichment",
             "kubemarine.controlplane.controlplane_node_enrichment",
             "kubemarine.core.defaults.append_controlplain",
             "kubemarine.core.defaults.compile_inventory",
             "kubemarine.core.defaults.calculate_node_names",
             "kubemarine.core.defaults.verify_node_names",
```

### Comparing `kubemarine-0.16.0/kubemarine/core/connections.py` & `kubemarine-0.17.0/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/defaults.py` & `kubemarine-0.17.0/kubemarine/core/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from kubemarine.core.yaml_merger import default_merger
 
 # All enrichment procedures should not connect to any node.
 # The information about nodes should be collected within KubernetesCluster#detect_nodes_context().
 DEFAULT_ENRICHMENT_FNS = [
     "kubemarine.core.schema.verify_inventory",
     "kubemarine.core.defaults.merge_defaults",
+    "kubemarine.kubernetes.verify_initial_version",
     "kubemarine.admission.enrich_default_admission",
     "kubemarine.kubernetes.add_node_enrichment",
     "kubemarine.kubernetes.remove_node_enrichment",
     "kubemarine.controlplane.controlplane_node_enrichment",
     "kubemarine.core.defaults.append_controlplain",
     "kubemarine.kubernetes.enrich_upgrade_inventory",
     "kubemarine.plugins.enrich_upgrade_inventory",
@@ -61,15 +62,14 @@
     "kubemarine.system.verify_inventory",
     "kubemarine.system.enrich_etc_hosts",
     "kubemarine.packages.enrich_inventory_include_all",
     "kubemarine.audit.verify_inventory",
     "kubemarine.plugins.enrich_inventory",
     "kubemarine.plugins.verify_inventory",
     "kubemarine.plugins.builtin.verify_inventory",
-    "kubemarine.coredns.enrich_add_hosts_config",
     "kubemarine.k8s_certs.renew_verify",
     "kubemarine.cri.enrich_inventory",
     "kubemarine.system.enrich_kernel_modules"
 ]
 
 supported_defaults = {
     'rbac': {
@@ -194,19 +194,15 @@
             }
 
         path = 'plugins."io.containerd.grpc.v1.cri"'
         if not containerd_config.get(path):
             containerd_config[path] = {}
         if not containerd_config[path].get('sandbox_image'):
             kubernetes_version = inventory['services']['kubeadm']['kubernetesVersion']
-            pause_mapping = cluster.globals['compatibility_map']['software']['pause']
-            if kubernetes_version not in pause_mapping:
-                raise Exception(f"Failed to detect pause version for Kubernetes {kubernetes_version}. "
-                                f"Please explicitly specify services.cri.containerdConfig.{path}.sandbox_image section.")
-            pause_version = pause_mapping[kubernetes_version]['version']
+            pause_version = cluster.globals['compatibility_map']['software']['pause'][kubernetes_version]['version']
             containerd_config[path]['sandbox_image'] = \
                 f"{inventory['services']['kubeadm']['imageRepository']}/pause:{pause_version}"
 
     from kubemarine import thirdparties
 
     if thirdparties_address:
         for destination, config in inventory['services']['thirdparties'].items():
```

### Comparing `kubemarine-0.16.0/kubemarine/core/environment.py` & `kubemarine-0.17.0/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/errors.py` & `kubemarine-0.17.0/kubemarine/core/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     },
     "KME0005": {
         "name": "{hostnames} are not sudoers"
     },
     "KME0007": {
         "name": "Docker CRI can not be used with endpoints registry definition."
     },
+    "KME0008": {
+        "name": "Specified Kubernetes version '{version}' - cannot be used! Allowed versions are: {allowed_versions}."
+    }
 }
 
 
 # TODO: support for more complex KME00XX objects with custom constructors
 class KME(RuntimeError):
     def __init__(self, code, **kwargs):
         self.code = code
```

### Comparing `kubemarine-0.16.0/kubemarine/core/executor.py` & `kubemarine-0.17.0/kubemarine/core/executor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/flow.py` & `kubemarine-0.17.0/kubemarine/core/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,78 +13,117 @@
 # limitations under the License.
 
 import argparse
 import os
 import shlex
 import sys
 import time
+from abc import abstractmethod, ABC
 from copy import deepcopy
 from typing import Type, Optional, List, Union
 
-from kubemarine.core import utils, cluster as c, action, resources as res, errors, summary
+from kubemarine.core import utils, cluster as c, action, resources as res, errors, summary, log
 
 DEFAULT_CLUSTER_OBJ: Optional[Type[c.KubernetesCluster]] = None
 TASK_DESCRIPTION_TEMPLATE = """
 tasks list:
     %s
 """
 
 END_OF_TASKS = object()
 
 
-def run_actions(context: Union[dict, res.DynamicResources], actions: List[action.Action],
-                print_summary: bool = True) -> Optional[c.KubernetesCluster]:
+class FlowResult:
+    def __init__(self, context: dict, logger: log.EnhancedLogger):
+        self.context = context
+        self.logger = logger
+
+
+class Flow(ABC):
+    def run_flow(self, context: Union[dict, res.DynamicResources], print_summary: bool = True) -> FlowResult:
+        time_start = time.time()
+
+        resources: res.DynamicResources = context
+        if isinstance(context, dict):
+            resources = res.DynamicResources(context)
+
+        context = resources.context
+        args: dict = context['execution_arguments']
+
+        try:
+            if not args.get('disable_dump', True):
+                utils.prepare_dump_directory(args.get('dump_location'),
+                                             reset_directory=not args.get('disable_dump_cleanup', False))
+            logger = resources.logger()
+            self._run(resources)
+        except Exception as exc:
+            logger = resources.logger_if_initialized()
+            if isinstance(exc, errors.FailException):
+                utils.do_fail(exc.message, exc.reason, exc.hint, log=logger)
+            else:
+                utils.do_fail(f"'{context['initial_procedure'] or 'undefined'}' procedure failed.", exc,
+                              log=logger)
+
+        time_end = time.time()
+
+        if print_summary:
+            summary.schedule_report(resources.working_context, summary.SummaryItem.EXECUTION_TIME,
+                                    utils.get_elapsed_string(time_start, time_end))
+            summary.print_summary(resources.working_context, logger)
+            logger.info("SUCCESSFULLY FINISHED")
+
+        return FlowResult(resources.working_context, logger)
+
+    @abstractmethod
+    def _run(self, resources: res.DynamicResources):
+        pass
+
+
+class ActionsFlow(Flow):
+    def __init__(self, actions: List[action.Action]):
+        self._actions = actions
+
+    def _run(self, resources: res.DynamicResources):
+        run_actions(resources, self._actions)
+
+
+def run_actions(resources: res.DynamicResources, actions: List[action.Action]) -> None:
     """
     Runs actions one by one, recreates inventory when necessary,
     managing such resources as cluster object and raw inventory.
 
     For each initialized cluster object, preserves inventory if any action is succeeded.
     """
-    time_start = time.time()
-
-    resources: res.DynamicResources = context
-    if isinstance(context, dict):
-        resources = res.DynamicResources(context)
 
     context = resources.context
-
-    args: dict = context['execution_arguments']
-    if not args.get('disable_dump', True):
-        utils.prepare_dump_directory(args.get('dump_location'),
-                                     reset_directory=not args.get('disable_dump_cleanup', False))
-
-    log = resources.logger()
+    logger = resources.logger()
 
     successfully_performed = []
     last_cluster = None
     for act in actions:
-        act.prepare_context(resources.context)
+        act.prepare_context(context)
 
         if not successfully_performed:
             # first action in group
             if resources.inventory_filepath:
                 with utils.open_external(resources.inventory_filepath, "r") as stream:
                     utils.dump_file(context, stream, "cluster_initial.yaml")
 
             if resources.procedure_inventory_filepath:
                 with utils.open_external(resources.procedure_inventory_filepath, "r") as stream:
                     utils.dump_file(context, stream, "procedure.yaml")
         try:
-            log.info(f"Running action '{act.identifier}'")
+            logger.info(f"Running action '{act.identifier}'")
             act.run(resources)
             successfully_performed.append(act.identifier)
-        except Exception as exc:
+        except Exception:
             if successfully_performed:
                 _post_process_actions_group(last_cluster, context, successfully_performed, failed=True)
 
-            if isinstance(exc, errors.FailException):
-                utils.do_fail(exc.message, exc.reason, exc.hint, log=log)
-            else:
-                utils.do_fail(f"'{context['initial_procedure'] or 'undefined'}' procedure failed.", exc,
-                              log=log)
+            raise
 
         last_cluster = resources.cluster_if_initialized()
 
         if act.recreate_inventory:
             if resources.inventory_filepath:
                 with utils.open_external(resources.inventory_filepath, "r") as stream:
                     # write original file data to backup file with timestamp
@@ -96,26 +135,16 @@
             _post_process_actions_group(last_cluster, context, successfully_performed)
             successfully_performed = []
             last_cluster = None
 
     if successfully_performed:
         _post_process_actions_group(last_cluster, context, successfully_performed)
 
-    time_end = time.time()
-
-    if print_summary:
-        summary.schedule_report(resources.working_context, summary.SummaryItem.EXECUTION_TIME,
-                                utils.get_elapsed_string(time_start, time_end))
-        summary.print_summary(resources.working_context, log)
-        log.info("SUCCESSFULLY FINISHED")
-
-    return last_cluster
-
 
-def _post_process_actions_group(last_cluster: c.KubernetesCluster, context: dict,
+def _post_process_actions_group(last_cluster: Optional[c.KubernetesCluster], context: dict,
                                 successfully_performed: list, failed=False):
     if last_cluster is None:
         return
     try:
         last_cluster.dump_finalized_inventory()
     finally:
         if context['preserve_inventory']:
@@ -155,15 +184,15 @@
 
     if args.get('without_act', False):
         resources.context['preserve_inventory'] = False
         cluster.log.debug('\nFurther acting manually disabled')
         return
 
     init_tasks_flow(cluster)
-    run_flow(tasks, final_list, cluster, cumulative_points, [])
+    run_tasks_recursive(tasks, final_list, cluster, cumulative_points, [])
     proceed_cumulative_point(cluster, cumulative_points, END_OF_TASKS,
                              force=args.get('force_cumulative_points', False))
 
 
 def create_empty_context(args: dict = None, procedure: str = None):
     if args is None:
         args = {}
@@ -242,16 +271,16 @@
                     final_list += _final_list
         else:
             print("\t%s" % __task_name)
 
     return filtered, final_list
 
 
-def run_flow(tasks: dict, final_task_names: List[str], cluster: c.KubernetesCluster,
-             cumulative_points: dict, _task_path: List[str]):
+def run_tasks_recursive(tasks: dict, final_task_names: List[str], cluster: c.KubernetesCluster,
+                        cumulative_points: dict, _task_path: List[str]):
     for task_name, task in tasks.items():
         __task_path = _task_path + [task_name]
         __task_name = ".".join(__task_path)
         run = __task_name in final_task_names
 
         args = cluster.context['execution_arguments']
         # --force-cumulative-points forcibly run the point only if the related task is going to be executed
@@ -267,15 +296,15 @@
                 add_task_to_proceeded_list(cluster, __task_name)
             except Exception as exc:
                 raise errors.FailException(
                     "TASK FAILED %s" % __task_name, exc,
                     hint=cluster.globals['error_handling']['failure_message'] % (sys.argv[0], __task_name)
                 )
         else:
-            run_flow(task, final_task_names, cluster, cumulative_points, __task_path)
+            run_tasks_recursive(task, final_task_names, cluster, cumulative_points, __task_path)
 
 
 def new_common_parser(cli_help):
 
     parser = argparse.ArgumentParser(description=cli_help,
                                      formatter_class=argparse.RawTextHelpFormatter)
```

### Comparing `kubemarine-0.16.0/kubemarine/core/group.py` & `kubemarine-0.17.0/kubemarine/core/group.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/log.py` & `kubemarine-0.17.0/kubemarine/core/log.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/patch.py` & `kubemarine-0.17.0/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/resources.py` & `kubemarine-0.17.0/kubemarine/core/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
         self._cluster: Optional[c.KubernetesCluster] = None
 
         args: dict = context['execution_arguments']
         self.inventory_filepath = args['config']
         self.procedure_inventory_filepath = args.get('procedure_config')
 
+    def logger_if_initialized(self):
+        return self._logger
+
     def logger(self):
         if self._logger is None:
             self._logger = self._create_logger()
 
         return self._logger
 
     def raw_inventory(self) -> dict:
```

### Comparing `kubemarine-0.16.0/kubemarine/core/schema.py` & `kubemarine-0.17.0/kubemarine/core/schema.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/static.py` & `kubemarine-0.17.0/kubemarine/core/static.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,31 @@
     GLOBALS.clear()
     GLOBALS.update(_load_globals())
 
     global DEFAULTS
     DEFAULTS.clear()
     DEFAULTS.update(_load_defaults())
 
-    global SUPPORTED_VERSIONS
-    SUPPORTED_VERSIONS.clear()
-    SUPPORTED_VERSIONS.update(_load_supported_versions())
+    global KUBERNETES_VERSIONS
+    KUBERNETES_VERSIONS.clear()
+    KUBERNETES_VERSIONS.update(load_kubernetes_versions())
 
 
 def load_compatibility_map(filename: str) -> dict:
     return utils.load_yaml(utils.get_internal_resource_path(
         f"resources/configurations/compatibility/internal/{filename}"))
 
 
+def load_kubernetes_versions() -> dict:
+    kubernetes_versions = utils.load_yaml(
+        utils.get_internal_resource_path('resources/configurations/compatibility/kubernetes_versions.yaml'))
+
+    return kubernetes_versions
+
+
 def _load_globals() -> dict:
     globals = utils.load_yaml(
         utils.get_internal_resource_path('resources/configurations/globals.yaml'))
 
     for config_filename in ('kubernetes_images.yaml', 'packages.yaml', 'plugins.yaml', 'thirdparties.yaml'):
         internal_compatibility = load_compatibility_map(config_filename)
 
@@ -52,19 +59,12 @@
 
 
 def _load_defaults() -> dict:
     return utils.load_yaml(
         utils.get_internal_resource_path('resources/configurations/defaults.yaml'))
 
 
-def _load_supported_versions() -> dict:
-    kubernetes_versions = utils.load_yaml(
-        utils.get_internal_resource_path('resources/configurations/compatibility/kubernetes_versions.yaml'))
-
-    return kubernetes_versions['kubernetes_versions']
-
-
 GLOBALS = {}
 DEFAULTS = {}
-SUPPORTED_VERSIONS = {}
+KUBERNETES_VERSIONS = {}
 
 reload()
```

### Comparing `kubemarine-0.16.0/kubemarine/core/summary.py` & `kubemarine-0.17.0/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/core/utils.py` & `kubemarine-0.17.0/kubemarine/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -414,29 +414,49 @@
     return read_internal(get_version_filepath()).strip()
 
 
 def minor_version(version: str) -> str:
     """
     Converts vN.N.N to vN.N
     """
-    return ".".join(version.split(".")[0:2])
+    return 'v' + '.'.join(map(str, _test_version(version, 3)[0:2]))
 
 
-def version_key(version: str) -> tuple:
+def version_key(version: str) -> Tuple[int, int, int]:
     """
-    Converts vN.N.N to (N, N, N) or vN.N to (N, N) that can be used in comparisons.
+    Converts vN.N.N to (N, N, N) that can be used in comparisons.
     """
-    return tuple(map(int, version[1:].split('.')))
+    return tuple(_test_version(version, 3))
 
 
-def minor_version_key(version: str) -> tuple:
+def minor_version_key(version: str) -> Tuple[int, int]:
     """
-    Converts vN.N.N to (N, N) that can be used in comparisons.
+    Converts vN.N to (N, N) that can be used in comparisons.
     """
-    return version_key(minor_version(version))
+    return tuple(_test_version(version, 2))
+
+
+def _test_version(version: str, numbers_amount: int) -> list:
+    # catch version without "v" at the first symbol
+    if version.startswith('v'):
+        version_list: list = version[1:].split('.')
+        # catch invalid version 'v1.16'
+        if len(version_list) == numbers_amount:
+            # parse str to int and catch invalid symbols in version number
+            try:
+                for i, value in enumerate(version_list):
+                    # whitespace required because python's int() ignores them
+                    version_list[i] = int(value.replace(' ', '.'))
+            except ValueError:
+                pass
+            else:
+                return version_list
+
+    expected_pattern = 'v' + '.'.join('N+' for _ in range(numbers_amount))
+    raise ValueError(f'Incorrect version \"{version}\" format, expected version pattern is \"{expected_pattern}\"')
 
 
 class ClusterStorage:
     """
     File preservation:
     1- Create folder where dumps are stored
     2- Rotating dumps in the storage folder
```

### Comparing `kubemarine-0.16.0/kubemarine/core/yaml_merger.py` & `kubemarine-0.17.0/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/coredns.py` & `kubemarine-0.17.0/kubemarine/coredns.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,14 @@
 import yaml
 
 from kubemarine import system
 from kubemarine.core import utils
 
 import io
 
-
-def enrich_add_hosts_config(inventory, cluster):
-    if not inventory['services']['coredns']['configmap'].get('Hosts'):
-        inventory['services']['coredns']['configmap']['Hosts'] = system.generate_etc_hosts_config(inventory, cluster)
-    return inventory
-
-
 def proceed_section_keyvalue(data, tabsize):
     tab = " "*tabsize
     config = ''
 
     for key, value in data.items():
         if isinstance(value, bool):
             if value:
@@ -116,15 +109,21 @@
             config += '\n' + tab + type + ' {' + proceed_section_keyvalue(data[section['name']]['data'], tabsize + 2)\
                       + '\n' + tab + '}'
 
     return config
 
 
 def generate_configmap(inventory):
+    # coredns.configmap.Hosts must exist even if it's empty
+    if not inventory['services']['coredns']['configmap'].get('Hosts'):
+        # Hosts must exist even if it's empty
+        inventory['services']['coredns']['configmap']['Hosts'] = ""
+
     config = '''apiVersion: v1
+
 kind: ConfigMap
 metadata:
   name: coredns
   namespace: kube-system
 data:'''
 
     for config_type, data in inventory['services']['coredns']['configmap'].items():
@@ -132,14 +131,19 @@
         if config_type == 'Corefile':
             for port, settings in data.items():
                 config += '\n    %s {' % port
                 config += proceed_section_keyvalue(settings, 6)
                 config += '\n    }'
         else:
             config += '\n    ' + data.replace('\n', '\n    ')
+        # add etc_hosts_autogenerated to the configmap
+        if config_type == 'Hosts' and inventory['services']['coredns']['add_etc_hosts_generated']:
+            config += '\n    '
+            config += system.generate_etc_hosts_config(inventory,etc_hosts_part='etc_hosts_generated').replace('\n', '\n    ')
+
     return config + '\n'
 
 
 def apply_configmap(cluster, config):
     utils.dump_file(cluster, config, 'coredns-configmap.yaml')
 
     group = cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_final_nodes()
```

### Comparing `kubemarine-0.16.0/kubemarine/cri/__init__.py` & `kubemarine-0.17.0/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/cri/containerd.py` & `kubemarine-0.17.0/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/cri/docker.py` & `kubemarine-0.17.0/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/demo.py` & `kubemarine-0.17.0/kubemarine/demo.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/etcd.py` & `kubemarine-0.17.0/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/haproxy.py` & `kubemarine-0.17.0/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/jinja.py` & `kubemarine-0.17.0/kubemarine/jinja.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/k8s_certs.py` & `kubemarine-0.17.0/kubemarine/k8s_certs.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,27 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from kubemarine import kubernetes
 
-version_kubectl_alpha_removed = "v1.21.0"
-
 
 def k8s_certs_overview(control_planes):
-    if kubernetes.version_higher_or_equal(control_planes.cluster.inventory['services']['kubeadm']['kubernetesVersion'],
-                                          version_kubectl_alpha_removed):
-        for control_plane in control_planes.get_ordered_members_list(provide_node_configs=True):
-            control_planes.cluster.log.debug(f"Checking certs expiration for control_plane {control_plane['name']}")
-            control_plane['connection'].sudo("kubeadm certs check-expiration", hide=False)
-    else:
-        for control_plane in control_planes.get_ordered_members_list(provide_node_configs=True):
-            control_planes.cluster.log.debug(f"Checking certs expiration for control_plane {control_plane['name']}")
-            control_plane['connection'].sudo("kubeadm alpha certs check-expiration", hide=False)
+    for control_plane in control_planes.get_ordered_members_list(provide_node_configs=True):
+        control_planes.cluster.log.debug(f"Checking certs expiration for control_plane {control_plane['name']}")
+        control_plane['connection'].sudo("kubeadm certs check-expiration", hide=False)
 
 
 def renew_verify(inventory, cluster):
     if cluster.context.get('initial_procedure') != 'cert_renew' or "kubernetes" not in cluster.procedure_inventory:
         return inventory
 
     cert_list = cluster.procedure_inventory["kubernetes"].get("cert-list")
@@ -41,21 +33,16 @@
 
 def renew_apply(control_planes):
     log = control_planes.cluster.log
 
     procedure = control_planes.cluster.procedure_inventory["kubernetes"]
     cert_list = procedure["cert-list"]
 
-    if kubernetes.version_higher_or_equal(control_planes.cluster.inventory['services']['kubeadm']['kubernetesVersion'],
-                                          version_kubectl_alpha_removed):
-        for cert in cert_list:
-            control_planes.sudo(f"kubeadm certs renew {cert}")
-    else:
-        for cert in cert_list:
-            control_planes.sudo(f"kubeadm alpha certs renew {cert}")
+    for cert in cert_list:
+        control_planes.sudo(f"kubeadm certs renew {cert}")
 
     if "all" in cert_list or "admin.conf" in cert_list:
         # need to update cluster-admin config
         kubernetes.copy_admin_config(log, control_planes)
 
     control_planes.call(force_renew_kubelet_serving_certs)
```

### Comparing `kubemarine-0.16.0/kubemarine/keepalived.py` & `kubemarine-0.17.0/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes/__init__.py` & `kubemarine-0.17.0/kubemarine/kubernetes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,30 +13,28 @@
 # limitations under the License.
 
 import io
 import math
 import os
 import time
 from copy import deepcopy
-from typing import List, Dict, Union
+from typing import List, Dict, Tuple
 
 import ruamel.yaml
 import yaml
 from jinja2 import Template
 import ipaddress
 
 from kubemarine import system, plugins, admission, etcd, packages
-from kubemarine.core import utils, static, summary
+from kubemarine.core import utils, static, summary, log, errors
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.errors import KME
 
-version_coredns_path_breakage = "v1.21.2"
-
 ERROR_DOWNGRADE='Kubernetes old version \"%s\" is greater than new one \"%s\"'
 ERROR_SAME='Kubernetes old version \"%s\" is the same as new one \"%s\"'
 ERROR_MAJOR_RANGE_EXCEEDED='Major version \"%s\" rises to new \"%s\" more than one'
 ERROR_MINOR_RANGE_EXCEEDED='Minor version \"%s\" rises to new \"%s\" more than one'
 
 
 def add_node_enrichment(inventory, cluster):
@@ -74,44 +72,25 @@
         if not inventory.get('services'):
             inventory['services'] = {}
         if not inventory['services'].get('kubeadm'):
             inventory['services']['kubeadm'] = {}
         cluster.context['initial_kubernetes_version'] = inventory['services']['kubeadm']['kubernetesVersion']
         inventory['services']['kubeadm']['kubernetesVersion'] = cluster.context['upgrade_version']
 
-        test_version_upgrade_possible(cluster.context['initial_kubernetes_version'], cluster.context['upgrade_version'])
         cluster.log.info(
             '------------------------------------------\nUPGRADING KUBERNETES %s ⭢ %s\n------------------------------------------' % (
             cluster.context['initial_kubernetes_version'], cluster.context['upgrade_version']))
     return inventory
 
 
-def version_higher_or_equal(version, compared_version):
-    '''
-    The method checks target Kubernetes version, is it more/equal than compared_version.
-    '''
-    compared_version_list = compared_version.replace('v', '').split('.')
-    version_list = version.replace('v', '').split('.')
-    if int(version_list[0]) > int(compared_version_list[0]):
-        return True
-    if int(version_list[0]) == int(compared_version_list[0]):
-        if int(version_list[1]) > int(compared_version_list[1]):
-            return True
-        if int(version_list[1]) == int(compared_version_list[1]):
-            if int(version_list[2]) >= int(compared_version_list[2]):
-                return True
-    return False
-
-
 def enrich_inventory(inventory, cluster):
-    if version_higher_or_equal(inventory['services']['kubeadm']['kubernetesVersion'], version_coredns_path_breakage):
-        repository = inventory['services']['kubeadm'].get('imageRepository', "")
-        if repository:
-            inventory['services']['kubeadm']['dns'] = {}
-            inventory['services']['kubeadm']['dns']['imageRepository'] = ("%s/coredns" % repository)
+    repository = inventory['services']['kubeadm'].get('imageRepository', "")
+    if repository:
+        inventory['services']['kubeadm']['dns'] = {}
+        inventory['services']['kubeadm']['dns']['imageRepository'] = ("%s/coredns" % repository)
     # if user redefined apiServer as, string, for example?
     if not isinstance(inventory["services"]["kubeadm"].get('apiServer'), dict):
         inventory["services"]["kubeadm"]['apiServer'] = {}
 
     # if user redefined apiServer.certSANs as, string, or removed it, for example?
     if not isinstance(inventory["services"]["kubeadm"]['apiServer'].get('certSANs'), list):
         inventory["services"]["kubeadm"]['apiServer']['certSANs'] = []
@@ -470,14 +449,16 @@
     log.debug(f"Downloading kubeconfig from node {first_control_plane['name']!r}...")
 
     kubeconfig = list(first_control_plane['connection'].sudo('cat /root/.kube/config').values())[0].stdout
 
     # Replace cluster FQDN with ip
     public_cluster_ip = cluster.inventory.get('public_cluster_ip')
     if public_cluster_ip:
+        if type(ipaddress.ip_address(public_cluster_ip)) is ipaddress.IPv6Address:
+            public_cluster_ip = f"[{public_cluster_ip}]"
         cluster_name = cluster.inventory['cluster_name']
         kubeconfig = kubeconfig.replace(cluster_name, public_cluster_ip)
 
     kubeconfig_filename = os.path.abspath("kubeconfig")
     with utils.open_external(kubeconfig_filename, 'w') as f:
         f.write(kubeconfig)
 
@@ -765,15 +746,16 @@
 
 
 def get_kubeadm_config(inventory):
     kubeadm_kubelet = yaml.dump(inventory["services"]["kubeadm_kubelet"], default_flow_style=False)
     kubeadm = yaml.dump(inventory["services"]["kubeadm"], default_flow_style=False)
     return f'{kubeadm_kubelet}---\n{kubeadm}'
 
-def upgrade_first_control_plane(version, upgrade_group, cluster, drain_timeout=None, grace_period=None):
+def upgrade_first_control_plane(version, upgrade_group, cluster, kubeadm_file,
+                                minor_version, drain_timeout=None, grace_period=None):
     first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
 
     if not upgrade_group.has_node(first_control_plane['name']):
         cluster.log.debug("First control-plane \"%s\" upgrade is not required" % first_control_plane['name'])
         return
 
     cluster.log.debug("Upgrading first control-plane \"%s\"" % first_control_plane)
@@ -794,27 +776,34 @@
     disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
     drain_cmd = prepare_drain_command(first_control_plane, version, cluster.globals, disable_eviction, cluster.nodes,
                                       drain_timeout, grace_period)
     first_control_plane['connection'].sudo(drain_cmd, is_async=False, hide=False)
 
     upgrade_cri_if_required(first_control_plane['connection'])
 
+    # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
+
+    if minor_version == 27:
+        fix_flag_kubelet(first_control_plane, kubeadm_file)
+
     first_control_plane['connection'].sudo(f"sudo kubeadm upgrade apply {version} {flags} && "
                                     f"sudo kubectl uncordon {first_control_plane['name']} && "
                                     f"sudo systemctl restart kubelet", is_async=False, hide=False)
 
     copy_admin_config(cluster.log, first_control_plane['connection'])
 
     expect_kubernetes_version(cluster, version, apply_filter=first_control_plane['name'])
     wait_for_any_pods(cluster, first_control_plane['connection'], apply_filter=first_control_plane['name'])
     exclude_node_from_upgrade_list(first_control_plane['connection'], first_control_plane['name'])
 
 
-def upgrade_other_control_planes(version, upgrade_group, cluster, drain_timeout=None, grace_period=None):
+def upgrade_other_control_planes(version, upgrade_group, cluster, kubeadm_file,
+                                 minor_version, drain_timeout=None, grace_period=None):
     first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+
     for node in cluster.nodes['control-plane'].get_ordered_members_list(provide_node_configs=True):
         if node['name'] != first_control_plane['name']:
 
             if not upgrade_group.has_node(node['name']):
                 cluster.log.debug("Control-plane \"%s\" upgrade is not required" % node['name'])
                 continue
 
@@ -826,14 +815,18 @@
             disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
             drain_cmd = prepare_drain_command(node, version, cluster.globals, disable_eviction, cluster.nodes,
                                               drain_timeout, grace_period)
             node['connection'].sudo(drain_cmd, is_async=False, hide=False)
 
             upgrade_cri_if_required(node['connection'])
 
+            # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
+            if minor_version == 27:
+                fix_flag_kubelet(node, kubeadm_file)
+
             # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
             # and only "else" branch remains
             if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
                 node['connection'].sudo(f"sudo kubeadm upgrade node --certificate-renewal=true && "
                                     f"sudo sed -i 's/--bind-address=.*$/--bind-address={node['internal_address']}/' "
                                     f"/etc/kubernetes/manifests/kube-apiserver.yaml && "
                                     f"sudo kubectl uncordon {node['name']} && "
@@ -877,27 +870,27 @@
     new_image_repo_port = cluster.context.get('patch_image_repo_port', '')
     old_image_repo_port = cluster.context.get('old_image_repo_port', '')
     if new_image_repo_port and old_image_repo_port:
         cluster_config["imageRepository"] = cluster_config["imageRepository"].replace('/k8s.gcr.io', '')
         cluster_config["imageRepository"] = cluster_config["imageRepository"].replace(old_image_repo_port,
                                                                                       new_image_repo_port)
 
-    if version_higher_or_equal(current_kubernetes_version, version_coredns_path_breakage):
-        cluster_config['dns']['imageRepository'] = "%s/coredns" % cluster_config["imageRepository"]
+    cluster_config['dns']['imageRepository'] = "%s/coredns" % cluster_config["imageRepository"]
 
     kubelet_config = first_control_plane["connection"].sudo("cat /var/lib/kubelet/config.yaml").get_simple_out()
     ryaml.dump(cluster_config, updated_config)
     result_config = kubelet_config + "---\n" + updated_config.getvalue()
     first_control_plane["connection"].put(io.StringIO(result_config), "/tmp/kubeadm_config.yaml", sudo=True)
 
     return True
 
 
-def upgrade_workers(version, upgrade_group, cluster, drain_timeout=None, grace_period=None):
+def upgrade_workers(version, upgrade_group, cluster, kubeadm_file, minor_version, drain_timeout=None, grace_period=None):
     first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+
     for node in cluster.nodes.get('worker').exclude_group(cluster.nodes['control-plane']).get_ordered_members_list(
             provide_node_configs=True):
 
         if not upgrade_group.has_node(node['name']):
             cluster.log.debug("Worker \"%s\" upgrade is not required" % node['name'])
             continue
 
@@ -909,14 +902,18 @@
         disable_eviction = cluster.procedure_inventory.get("disable-eviction", True)
         drain_cmd = prepare_drain_command(node, version, cluster.globals, disable_eviction, cluster.nodes,
                                           drain_timeout, grace_period)
         first_control_plane['connection'].sudo(drain_cmd, is_async=False, hide=False)
 
         upgrade_cri_if_required(node['connection'])
 
+        # The procedure for removing the deprecated kubelet flag for versions older than 1.27.0
+        if minor_version == 27:
+            fix_flag_kubelet(node, kubeadm_file)
+
         # TODO: when k8s v1.21 is excluded from Kubemarine, this condition should be removed
         # and only "else" branch remains
         if "v1.21" in cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]:
             node['connection'].sudo("kubeadm upgrade node --certificate-renewal=true && "
                                 "sudo systemctl restart kubelet")
         else:
            node['connection'].sudo("kubeadm upgrade node --certificate-renewal=true --patches=/etc/kubernetes/patches && "
@@ -934,15 +931,15 @@
     drain_globals = globals['nodes']['drain']
     if drain_timeout is None:
         drain_timeout = recalculate_proper_timeout(nodes, drain_globals['timeout'])
     if grace_period is None:
         grace_period = drain_globals['grace_period']
     drain_cmd = f"kubectl drain {node['name']} --force --ignore-daemonsets --delete-emptydir-data " \
                 f"--timeout={drain_timeout}s --grace-period={grace_period}"
-    if version and version >= "v1.18" and disable_eviction:
+    if version and disable_eviction:
         drain_cmd += " --disable-eviction=true"
     return drain_cmd
 
 
 def upgrade_cri_if_required(group):
     # currently it is invoked only for single node
     cluster = group.cluster
@@ -974,27 +971,42 @@
                                                  f"{node['name']}"
                                                  " -o custom-columns='VERSION:.status.nodeInfo.kubeletVersion' "
                                                  "| grep -vw ^VERSION ")
         curr_version = list(result.values())[0].stdout
         test_version_upgrade_possible(curr_version, upgrade_version, skip_equal=True)
 
 
-def verify_target_version(target_version):
-    test_version(target_version)
+def get_initial_kubernetes_version(inventory: dict) -> str:
+    kubernetes_version = inventory.get("services", {}).get("kubeadm", {}).get("kubernetesVersion")
+    if kubernetes_version is None:
+        kubernetes_version = static.DEFAULTS['services']['kubeadm']['kubernetesVersion']
+
+    return kubernetes_version
+
+
+def verify_initial_version(inventory: dict, _) -> dict:
+    version = get_initial_kubernetes_version(inventory)
+    verify_allowed_version(version)
+    return inventory
+
+
+def verify_allowed_version(version: str) -> None:
+    allowed_versions = static.KUBERNETES_VERSIONS['compatibility_map'].keys()
+    if version not in allowed_versions:
+        raise errors.KME('KME0008',
+                         version=version,
+                         allowed_versions=', '.join(map(repr, allowed_versions)))
+
 
-    pos = target_version.rfind(".")
-    target_version = target_version[:pos]
-    supported_versions = static.SUPPORTED_VERSIONS
-    if target_version not in supported_versions:
-        raise Exception("ERROR! Specified target Kubernetes version '%s' - cannot be installed!" % target_version)
-    if not supported_versions.get(target_version, {}).get("supported", False):
-        message = "\033[91mWarning! Specified target Kubernetes version '%s' - is not supported!\033[0m" % target_version
-        print(message)
-        return message
-    return ""
+def verify_supported_version(target_version: str, logger: log.EnhancedLogger) -> None:
+    verify_allowed_version(target_version)
+    minor_version = utils.minor_version(target_version)
+    supported_versions = static.KUBERNETES_VERSIONS['kubernetes_versions']
+    if not supported_versions.get(minor_version, {}).get("supported", False):
+        logger.warning(f"Specified target Kubernetes version {target_version!r} - is not supported!")
 
 
 def expect_kubernetes_version(cluster, version, timeout=None, retries=None, node=None, apply_filter=None):
     if timeout is None:
         timeout = cluster.globals['nodes']['expect']['kubernetes_version']['timeout']
     if retries is None:
         retries = cluster.globals['nodes']['expect']['kubernetes_version']['retries']
@@ -1029,54 +1041,30 @@
             retries -= 1
             cluster.log.debug("Some nodes have invalid Kubernetes version... (%ss left)" % (retries * timeout), result)
             time.sleep(timeout)
 
     raise Exception('In the expected time, the nodes did not receive correct Kubernetes version')
 
 
-def test_version(version: Union[list, str]):
-    version_list: list = version
-    # catch version without "v" at the first symbol
-    if isinstance(version, str):
-        if not version.startswith('v'):
-            raise Exception('Version \"%s\" do not have \"v\" as first symbol, '
-                            'expected version pattern is \"v1.NN.NN\"' % version)
-        version_list = version.replace('v', '').split('.')
-    # catch invalid version 'v1.16'
-    if len(version_list) != 3:
-        raise Exception('Version \"%s\" has invalid amount of numbers, '
-                        'expected version pattern is \"v1.NN.NN\"' % version)
-
-    # parse str to int and catch invalid symbols in version number
-    for i, value in enumerate(version_list):
-        try:
-            # whitespace required because python's int() ignores them
-            version_list[i] = int(value.replace(' ', '.'))
-        except ValueError:
-            raise Exception('Version \"%s\" contains invalid symbols, '
-                            'expected version pattern is \"v1.NN.NN\"' % version) from None
-    return version_list
-
-
-def test_version_upgrade_possible(old, new, skip_equal=False):
+def test_version_upgrade_possible(old: str, new: str, skip_equal=False):
     versions_unchanged = {
         'old': old.strip(),
         'new': new.strip()
     }
-    versions: Dict[str, List[int]] = {}
+    versions: Dict[str, Tuple[int, int, int]] = {}
 
     for v_type, version in versions_unchanged.items():
-        versions[v_type] = test_version(version)
+        versions[v_type] = utils.version_key(version)
 
     # test new is greater than old
-    if tuple(versions['old']) > tuple(versions['new']):
+    if versions['old'] > versions['new']:
         raise Exception(ERROR_DOWNGRADE % (versions_unchanged['old'], versions_unchanged['new']))
 
     # test new is the same as old
-    if tuple(versions['old']) == tuple(versions['new']) and not skip_equal:
+    if versions['old'] == versions['new'] and not skip_equal:
         raise Exception(ERROR_SAME % (versions_unchanged['old'], versions_unchanged['new']))
 
     # test major step is not greater than 1
     if versions['new'][0] - versions['old'][0] > 1:
         raise Exception(ERROR_MAJOR_RANGE_EXCEEDED % (versions_unchanged['old'], versions_unchanged['new']))
 
     # test minor step is not greater than 1
@@ -1096,15 +1084,19 @@
     if cluster.inventory['services']['cri']['containerRuntime'] == "containerd":
         if 'nodeRegistration' not in kubeadm_config:
             kubeadm_config['nodeRegistration'] = {}
         if 'kubeletExtraArgs' not in kubeadm_config['nodeRegistration']:
             kubeadm_config['nodeRegistration']['kubeletExtraArgs'] = {}
 
         kubeadm_config['nodeRegistration']['criSocket'] = '/var/run/containerd/containerd.sock'
-        kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime'] = 'remote'
+
+        minor_version = int(cluster.inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
+        if minor_version < 27:
+            kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime'] = 'remote'
+
         kubeadm_config['nodeRegistration']['kubeletExtraArgs']['container-runtime-endpoint'] = \
             'unix:///run/containerd/containerd.sock'
 
 
 def exclude_node_from_upgrade_list(first_control_plane, node_name):
     if isinstance(first_control_plane, dict):
         first_control_plane = first_control_plane['connection']
@@ -1356,8 +1348,14 @@
             node['connection'].put(io.StringIO(control_plane_patch + "\n"), '/etc/kubernetes/patches/' +
                                  control_plane_patch_files[control_plane_item], sudo=True)
             node['connection'].sudo('chmod 644 /etc/kubernetes/patches/' +
                                  control_plane_patch_files[control_plane_item])
 
     return
 
+def fix_flag_kubelet(node, kubeadm_file):
 
+    #Deprecated flag removal function for kubelet
+    kubeadm_flags = node['connection'].sudo(f"cat {kubeadm_file}", is_async=False).get_simple_out()
+    if kubeadm_flags.find('--container-runtime=remote') != -1:
+        kubeadm_flags = kubeadm_flags.replace('--container-runtime=remote', '')
+        node['connection'].put(io.StringIO(kubeadm_flags), kubeadm_file, backup=True, sudo=True)
```

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.17.0/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes/deployment.py` & `kubemarine-0.17.0/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes/object.py` & `kubemarine-0.17.0/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.17.0/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.17.0/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/kubernetes_accounts.py` & `kubemarine-0.17.0/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/packages.py` & `kubemarine-0.17.0/kubemarine/packages.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/patches/__init__.py` & `kubemarine-0.17.0/kubemarine/patches/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,11 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
-from kubemarine.patches.p1_helm_values import HelmValues
 
 patches: List[Patch] = [
-    HelmValues(),
 ]
 """List of patches which can be executed strictly in the declared order"""
```

### Comparing `kubemarine-0.16.0/kubemarine/plugins/__init__.py` & `kubemarine-0.17.0/kubemarine/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/builtin.py` & `kubemarine-0.17.0/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/calico.py` & `kubemarine-0.17.0/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.17.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.17.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/manifest.py` & `kubemarine-0.17.0/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.17.0/kubemarine/plugins/nginx_ingress.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,28 @@
 
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
+def check_job_for_nginx(cluster: KubernetesCluster):
+    first_control_plane = cluster.nodes['control-plane'].get_first_member(provide_node_configs=True)
+    version = cluster.inventory['plugins']['nginx-ingress-controller']['version'].replace('v', '.').split('.')
+
+    major_version = int(version[1])
+    minor_version = int(version[2])
+
+    check_jobs = first_control_plane['connection'].sudo(f"kubectl get jobs -n ingress-nginx")
+    if list(check_jobs.values())[0].stderr == "" and major_version >= 1 and minor_version >= 4:
+        cluster.log.debug('Delete old jobs for nginx')
+        first_control_plane['connection'].sudo(f"sudo kubectl delete job --all -n ingress-nginx", is_async=False)
+    else:
+        cluster.log.debug('There are no jobs to delete')
+
 def enrich_inventory(inventory, _):
     if not inventory["plugins"]["nginx-ingress-controller"]["install"]:
         return inventory
 
     if inventory["plugins"]["nginx-ingress-controller"].get('custom_headers'):
         if not inventory["plugins"]["nginx-ingress-controller"].get('config_map'):
             inventory["plugins"]["nginx-ingress-controller"]['config_map'] = {}
```

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.17.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/procedures/__init__.py` & `kubemarine-0.17.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/procedures/add_node.py` & `kubemarine-0.17.0/kubemarine/procedures/add_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,12 +124,12 @@
     How to use:
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure='add_node')
 
-    flow.run_actions(context, [AddNodeAction()])
+    flow.ActionsFlow([AddNodeAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/backup.py` & `kubemarine-0.17.0/kubemarine/procedures/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,12 +464,12 @@
         'etcd': {},
         'nodes': {},
         'kubernetes': {
             'resources': {}
         }
     }
 
-    flow.run_actions(context, [BackupAction()])
+    flow.ActionsFlow([BackupAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/cert_renew.py` & `kubemarine-0.17.0/kubemarine/procedures/cert_renew.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,12 @@
     How to use:
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure='cert_renew')
 
-    flow.run_actions(context, [CertRenewAction()])
+    flow.ActionsFlow([CertRenewAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/check_iaas.py` & `kubemarine-0.17.0/kubemarine/procedures/check_iaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -873,19 +873,19 @@
 
             if failed_nodes:
                 raise TestFailure(f"Failed to connect to {len(failed_nodes)} nodes.",
                                   hint=f"Not all needed tcp ports are opened on nodes: {failed_nodes}. "
                                        f"Ports that should be opened: {tcp_ports}")
 
 
-def make_reports(cluster):
-    if not cluster.context['execution_arguments'].get('disable_csv_report', False):
-        cluster.context['testsuite'].save_csv(cluster.context['execution_arguments']['csv_report'], cluster.context['execution_arguments']['csv_report_delimiter'])
-    if not cluster.context['execution_arguments'].get('disable_html_report', False):
-        cluster.context['testsuite'].save_html(cluster.context['execution_arguments']['html_report'], cluster.context['initial_procedure'].upper())
+def make_reports(context: dict):
+    if not context['execution_arguments'].get('disable_csv_report', False):
+        context['testsuite'].save_csv(context['execution_arguments']['csv_report'], context['execution_arguments']['csv_report_delimiter'])
+    if not context['execution_arguments'].get('disable_html_report', False):
+        context['testsuite'].save_html(context['execution_arguments']['html_report'], context['initial_procedure'].upper())
 
 
 tasks = OrderedDict({
     'ssh': {
         # todo this is useless, because flow.load_inventory already fails in case of no connectivity
         'connectivity': connection_ssh_connectivity,
         'latency': {
@@ -974,21 +974,24 @@
                         action='store_true',
                         help='forcibly disable HTML report file creation')
 
     context = flow.create_context(parser, cli_arguments, procedure='check_iaas')
     context['testsuite'] = TestSuite()
     context['preserve_inventory'] = False
 
-    cluster = flow.run_actions(context, [IaasAction()], print_summary=False)
+    flow_ = flow.ActionsFlow([IaasAction()])
+    result = flow_.run_flow(context, print_summary=False)
+
+    context = result.context
+    testsuite: TestSuite = context['testsuite']
 
     # Final summary should be printed only to stdout with custom formatting
     # If test results are required for parsing, they can be found in the test results files
-    print(cluster.context['testsuite'].get_final_summary())
-    cluster.context['testsuite'].print_final_status(cluster.log)
-    make_reports(cluster)
-    return cluster.context['testsuite']
+    print(testsuite.get_final_summary())
+    testsuite.print_final_status(result.logger)
+    make_reports(context)
+    if testsuite.is_any_test_failed():
+        sys.exit(1)
 
 
 if __name__ == '__main__':
-    testsuite = main()
-    if testsuite.is_any_test_failed():
-        sys.exit(1)
+    main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/check_paas.py` & `kubemarine-0.17.0/kubemarine/procedures/check_paas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1416,21 +1416,24 @@
                         action='store_true',
                         help='forcibly disable HTML report file creation')
 
     context = flow.create_context(parser, cli_arguments, procedure='check_paas')
     context['testsuite'] = TestSuite()
     context['preserve_inventory'] = False
 
-    cluster = flow.run_actions(context, [PaasAction()], print_summary=False)
+    flow_ = flow.ActionsFlow([PaasAction()])
+    result = flow_.run_flow(context, print_summary=False)
+
+    context = result.context
+    testsuite: TestSuite = context['testsuite']
 
     # Final summary should be printed only to stdout with custom formatting
     # If tests results required for parsing, they can be found in test results files
-    print(cluster.context['testsuite'].get_final_summary(show_minimal=False, show_recommended=False))
-    cluster.context['testsuite'].print_final_status(cluster.log)
-    check_iaas.make_reports(cluster)
-    return cluster.context['testsuite']
+    print(testsuite.get_final_summary(show_minimal=False, show_recommended=False))
+    testsuite.print_final_status(result.logger)
+    check_iaas.make_reports(context)
+    if testsuite.is_any_test_failed():
+        sys.exit(1)
 
 
 if __name__ == '__main__':
-    testsuite = main()
-    if testsuite.is_any_test_failed():
-        sys.exit(1)
+    main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/do.py` & `kubemarine-0.17.0/kubemarine/procedures/do.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,13 +120,14 @@
                     else:
                         executor_lists[executors_type].append(executors_str.strip())
             return cluster.create_group_from_groups_nodes_names(executor_lists['group'], executor_lists['node'])
         else:
             return cluster.nodes['control-plane'].get_any_member()
 
     no_stream = arguments.get('no_stream')
-    res = resources.DynamicResources(context, silent=False)
-    flow.run_actions(res, [CLIAction(node_group_provider, remote_args, no_stream)], print_summary=False)
+    action = CLIAction(node_group_provider, remote_args, no_stream)
+    res = resources.DynamicResources(context, silent=True)
+    flow.ActionsFlow([action]).run_flow(res, print_summary=False)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/install.py` & `kubemarine-0.17.0/kubemarine/procedures/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from kubemarine.core.errors import KME
 from kubemarine import system, sysctl, haproxy, keepalived, kubernetes, plugins, \
     kubernetes_accounts, selinux, thirdparties, admission, audit, coredns, cri, packages, apparmor
 from kubemarine.core import flow, utils, summary
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroup
 from kubemarine.core.resources import DynamicResources
-from kubemarine import kubernetes
+
 
 def _applicable_for_new_nodes_with_roles(*roles):
     """
     Decorator to annotate installation methods.
     If there are no new nodes with the specified roles to be added / installed to the cluster,
     the decorator skips execution of the method.
     Otherwise, it runs the annotated method with the calculated group of nodes with the specified roles.
@@ -264,15 +264,16 @@
         return
 
     system.update_resolv_conf(group, config=cluster.inventory["services"].get("resolv.conf"))
     cluster.log.debug(group.sudo("ls -la /etc/resolv.conf; sudo lsattr /etc/resolv.conf"))
 
 
 def system_prepare_dns_etc_hosts(cluster):
-    config = system.generate_etc_hosts_config(cluster.inventory, cluster)
+    config = system.generate_etc_hosts_config(cluster.inventory, cluster, 'etc_hosts')
+    config += system.generate_etc_hosts_config(cluster.inventory, cluster, 'etc_hosts_generated')
 
     utils.dump_file(cluster, config, 'etc_hosts')
     cluster.log.debug("\nUploading...")
 
     group = cluster.nodes['all'].get_final_nodes()
 
     system.update_etc_hosts(group, config=config)
@@ -649,23 +650,19 @@
     ]
 }
 
 
 class InstallAction(Action):
     def __init__(self):
         super().__init__('install')
-        self.verification_version_result = ""
+        self.target_version = None
 
     def run(self, res: DynamicResources):
-        cluster_yml = res.raw_inventory()
-        if (cluster_yml.get("services", {})
-                and cluster_yml["services"].get("kubeadm", {})
-                and cluster_yml["services"]["kubeadm"].get("kubernetesVersion")):
-            target_version = cluster_yml["services"]["kubeadm"].get("kubernetesVersion")
-            self.verification_version_result = kubernetes.verify_target_version(target_version)
+        self.target_version = kubernetes.get_initial_kubernetes_version(res.raw_inventory())
+        kubernetes.verify_supported_version(self.target_version, res.logger())
 
         flow.run_tasks(res, tasks, cumulative_points=cumulative_points)
 
 
 def main(cli_arguments=None):
     cli_help = '''
     Script for installing Kubernetes cluster.
@@ -674,15 +671,15 @@
 
     '''
 
     parser = flow.new_tasks_flow_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure='install')
 
     install = InstallAction()
-    flow.run_actions(context, [install])
+    flow_ = flow.ActionsFlow([install])
+    result = flow_.run_flow(context)
 
-    if install.verification_version_result:
-        print(install.verification_version_result)
+    kubernetes.verify_supported_version(install.target_version, result.logger)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/manage_psp.py` & `kubemarine-0.17.0/kubemarine/procedures/manage_psp.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,12 +48,12 @@
     How to use:
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure='manage_psp')
 
-    flow.run_actions(context, [PSPAction()])
+    flow.ActionsFlow([PSPAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/manage_pss.py` & `kubemarine-0.17.0/kubemarine/procedures/manage_pss.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,12 +46,12 @@
     How to use:
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure='manage_pss')
 
-    flow.run_actions(context, [PSSAction()])
+    flow.ActionsFlow([PSSAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.17.0/kubemarine/procedures/migrate_cri.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,12 +323,12 @@
         How to use:
 
         '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure="migrate_cri")
 
-    flow.run_actions(context, [MigrateCRIAction()])
+    flow.ActionsFlow([MigrateCRIAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.17.0/kubemarine/procedures/migrate_kubemarine.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,12 +90,12 @@
                 actions.append(patch.action)
         else:
             actions.append(patch.action)
 
     if not actions:
         print("No patches to apply")
         exit(0)
-    flow.run_actions(context, actions)
+    flow.ActionsFlow(actions).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/reboot.py` & `kubemarine-0.17.0/kubemarine/procedures/reboot.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,12 +65,12 @@
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, optional_config=True, tasks=tasks)
 
     context = flow.create_context(parser, cli_arguments, procedure='reboot')
 
-    flow.run_actions(context, [RebootAction()])
+    flow.ActionsFlow([RebootAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/remove_node.py` & `kubemarine-0.17.0/kubemarine/procedures/remove_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,23 +108,14 @@
             hostnames = [node['name'], node['internal_address']]
             if node.get('address') is not None:
                 hostnames.append(node['address'])
             for name in hostnames:
                 if name in inventory_to_finalize['services']['kubeadm']['apiServer']['certSANs']:
                     inventory_to_finalize['services']['kubeadm']['apiServer']['certSANs'].remove(name)
 
-    if inventory_to_finalize['services'].get('etc_hosts'):
-        for node in nodes_for_removal.get_ordered_members_list(provide_node_configs=True):
-            if inventory_to_finalize['services']['etc_hosts'].get(node['internal_address']):
-                del inventory_to_finalize['services']['etc_hosts'][node['internal_address']]
-            if node.get('address') is not None and inventory_to_finalize['services']['etc_hosts'].get(node['address']):
-                del inventory_to_finalize['services']['etc_hosts'][node['address']]
-
-        coredns.enrich_add_hosts_config(inventory_to_finalize, cluster)
-
     return inventory_to_finalize
 
 
 tasks = OrderedDict({
     "loadbalancer": {
         "remove": {
             "haproxy": loadbalancer_remove_haproxy,
@@ -168,12 +159,12 @@
     How to use:
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
     context = flow.create_context(parser, cli_arguments, procedure='remove_node')
 
-    flow.run_actions(context, [RemoveNodeAction()])
+    flow.ActionsFlow([RemoveNodeAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/restore.py` & `kubemarine-0.17.0/kubemarine/procedures/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,12 +286,12 @@
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
 
     context = flow.create_context(parser, cli_arguments, procedure='restore')
     args = context['execution_arguments']
 
     replace_config_from_backup_if_needed(args['procedure_config'], args['config'])
 
-    flow.run_actions(context, [RestoreAction()])
+    flow.ActionsFlow([RestoreAction()]).run_flow(context)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/procedures/upgrade.py` & `kubemarine-0.17.0/kubemarine/procedures/upgrade.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,34 +12,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from collections import OrderedDict
 from copy import deepcopy
+from distutils.util import strtobool
 from io import StringIO
+from itertools import chain
+from typing import List
 
 import toml
 
-from distutils.util import strtobool
-
+from kubemarine import kubernetes, plugins
+from kubemarine.core import flow
+from kubemarine.core import utils
 from kubemarine.core.action import Action
 from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.resources import DynamicResources
 from kubemarine.core.yaml_merger import default_merger
-from kubemarine.core import flow
 from kubemarine.procedures import install
-from kubemarine import kubernetes, plugins
-from itertools import chain
-from kubemarine.core import utils
-from kubemarine.core.executor import RemoteExecutor
-
-
-
-
 
 
 def system_prepare_thirdparties(cluster):
     if not cluster.inventory['services'].get('thirdparties', {}):
         cluster.log.debug("Skipped - no thirdparties defined in config file")
         return
 
@@ -51,30 +47,33 @@
     fix_cri_socket(cluster)
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
     upgrade_group.call(kubernetes.images_grouped_prepull)
 
 
 def kubernetes_upgrade(cluster):
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
+    minor_version = int(version.split('.')[1])
     upgrade_group = kubernetes.get_group_for_upgrade(cluster)
+    kubeadm_flags_file = "/var/lib/kubelet/kubeadm-flags.env"
+
 
     drain_timeout = cluster.procedure_inventory.get('drain_timeout')
     grace_period = cluster.procedure_inventory.get('grace_period')
 
-    kubernetes.upgrade_first_control_plane(version, upgrade_group, cluster,
-                                    drain_timeout=drain_timeout, grace_period=grace_period)
+    kubernetes.upgrade_first_control_plane(version, upgrade_group, cluster, kubeadm_flags_file, minor_version,
+                                           drain_timeout=drain_timeout, grace_period=grace_period)
 
     # After first control-plane upgrade is finished we may loose our CoreDNS changes.
     # Thus, we need to re-apply our CoreDNS changes immediately after first control-plane upgrade.
     install.deploy_coredns(cluster)
 
-    kubernetes.upgrade_other_control_planes(version, upgrade_group, cluster,
-                                     drain_timeout=drain_timeout, grace_period=grace_period)
+    kubernetes.upgrade_other_control_planes(version, upgrade_group, cluster, kubeadm_flags_file, minor_version,
+                                            drain_timeout=drain_timeout, grace_period=grace_period)
     if cluster.nodes.get('worker', []):
-        kubernetes.upgrade_workers(version, upgrade_group, cluster,
+        kubernetes.upgrade_workers(version, upgrade_group, cluster, kubeadm_flags_file, minor_version,
                                    drain_timeout=drain_timeout, grace_period=grace_period)
 
     cluster.nodes['control-plane'].get_first_member().sudo('rm -f /etc/kubernetes/nodes-k8s-versions.txt')
     cluster.context['cached_nodes_versions_cleaned'] = True
 
 
 def kubernetes_cleanup_nodes_versions(cluster):
@@ -109,26 +108,23 @@
 
 
 def upgrade_containerd(cluster: KubernetesCluster):
     """
         This function fixes the incorrect version of pause during the cluster update procedure
     """
 
-
     cri = cluster.inventory["services"]["cri"]['containerRuntime']
     if cri == 'containerd':
         path = 'plugins."io.containerd.grpc.v1.cri"'
         target_kubernetes_version = cluster.context["upgrade_version"]
-        pause_mapping = cluster.globals['compatibility_map']['software']['pause']
-        if target_kubernetes_version not in pause_mapping:
-            raise Exception(f"Upgrade to {target_kubernetes_version} is not supported")
-        pause_version = pause_mapping[target_kubernetes_version]['version']
+        pause_version = cluster.globals['compatibility_map']['software']['pause'][target_kubernetes_version]['version']
         if not cluster.inventory["services"]["cri"]['containerdConfig'].get(path, False):
             return
-        last_pause_version = cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"].split(":")[2]
+        last_pause_version = cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"].split(":")[
+            2]
         if True:
             sandbox = cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"]
             param_begin_pos = sandbox.rfind(":")
             sandbox = sandbox[:param_begin_pos] + ":" + str(pause_version)
             cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"] = sandbox
             config_string = ""
             containerd_config = cluster.inventory["services"]["cri"]['containerdConfig']
@@ -142,15 +138,16 @@
                     config_string += f"{toml.dumps({key: value})}"
             for key, value in containerd_config.items():
                 # next we process all "complex" `key: dict_value` pairs, representing named sections
                 if isinstance(value, dict):
                     config_string += f"\n[{key}]\n{toml.dumps(value)}"
             utils.dump_file(cluster, config_string, 'containerd-config.toml')
             with RemoteExecutor(cluster) as exe:
-                for node in cluster.nodes['control-plane'].include_group(cluster.nodes.get('worker')).get_ordered_members_list(
+                for node in cluster.nodes['control-plane'].include_group(
+                        cluster.nodes.get('worker')).get_ordered_members_list(
                         provide_node_configs=True):
                     os_specific_associations = cluster.get_associations_for_node(node['connect_to'], 'containerd')
                     node['connection'].put(StringIO(config_string), os_specific_associations['config_location'],
                                            backup=True,
                                            sudo=True, mkdir=True)
                     node['connection'].sudo(f"sudo systemctl restart {os_specific_associations['service_name']} && "
                                             f"systemctl status {os_specific_associations['service_name']}")
@@ -207,14 +204,38 @@
         # Despite we enrich OS specific section inside system.enrich_upgrade_inventory,
         # we still merge global associations section because it has priority during enrichment.
         default_merger.merge(inventory["services"]["packages"], packages_section)
 
     return inventory
 
 
+class UpgradeFlow(flow.Flow):
+    def __init__(self):
+        self.target_version = None
+
+    def _run(self, resources: DynamicResources):
+        logger = resources.logger()
+
+        previous_version = kubernetes.get_initial_kubernetes_version(resources.raw_inventory())
+        upgrade_plan = resources.procedure_inventory().get('upgrade_plan')
+        upgrade_plan = verify_upgrade_plan(previous_version, upgrade_plan)
+        logger.debug(f"Loaded upgrade plan: current ({previous_version}) ⭢ {' ⭢ '.join(upgrade_plan)}")
+
+        self.target_version = upgrade_plan[-1]
+        kubernetes.verify_supported_version(self.target_version, logger)
+
+        args = resources.context['execution_arguments']
+        if (args['tasks'] or args['exclude']) and len(upgrade_plan) > 1:
+            raise Exception("Usage of '--tasks' and '--exclude' is not allowed when upgrading to more than one version")
+
+        # todo inventory is preserved few times, probably need to preserve it once instead.
+        actions = [UpgradeAction(version) for version in upgrade_plan]
+        flow.run_actions(resources, actions)
+
+
 class UpgradeAction(Action):
     def __init__(self, upgrade_version: str):
         super().__init__('upgrade to ' + upgrade_version, recreate_inventory=True)
         self.upgrade_version = upgrade_version
 
     def run(self, res: DynamicResources):
         flow.run_tasks(res, tasks)
@@ -232,65 +253,50 @@
     How to use:
 
     '''
 
     parser = flow.new_procedure_parser(cli_help, tasks=tasks)
 
     context = flow.create_context(parser, cli_arguments, procedure='upgrade')
-    args = context['execution_arguments']
-    resources = DynamicResources(context)
+    flow_ = UpgradeFlow()
+    result = flow_.run_flow(context)
 
-    upgrade_plan = verify_upgrade_plan(resources.procedure_inventory().get('upgrade_plan'))
-    verification_version_result = kubernetes.verify_target_version(upgrade_plan[-1])
+    kubernetes.verify_supported_version(flow_.target_version, result.logger)
 
-    if (args['tasks'] or args['exclude']) and len(upgrade_plan) > 1:
-        raise Exception("Usage of '--tasks' and '--exclude' is not allowed when upgrading to more than one version")
 
-    # todo inventory is preserved few times, probably need to preserve it once instead.
-    actions = [UpgradeAction(version) for version in upgrade_plan]
-    flow.run_actions(resources, actions)
+def verify_upgrade_plan(previous_version: str, upgrade_plan: List[str]):
+    kubernetes.verify_allowed_version(previous_version)
+    for version in upgrade_plan:
+        kubernetes.verify_allowed_version(version)
 
-    if verification_version_result:
-        print(verification_version_result)
+    upgrade_plan.sort(key=utils.version_key)
 
-
-def verify_upgrade_plan(upgrade_plan):
-    if not upgrade_plan:
-        raise Exception('Upgrade plan is not specified or empty')
-
-    upgrade_plan.sort()
-
-    previous_version = None
-    for i in range(0, len(upgrade_plan)):
-        version = upgrade_plan[i]
-        if version == 'v1.24.0':
-            raise Exception('Attempt to upgrade to an unstable version of kubernetes')
-        if previous_version is not None:
-            kubernetes.test_version_upgrade_possible(previous_version, version)
+    for version in upgrade_plan:
+        kubernetes.test_version_upgrade_possible(previous_version, version)
         previous_version = version
 
-    print('Loaded upgrade plan: current ⭢', ' ⭢ '.join(upgrade_plan))
-
     return upgrade_plan
 
 
 def fix_cri_socket(cluster):
     """
     This method fixs the issue with 'kubeadm.alpha.kubernetes.io/cri-socket' node annotation
     and delete the docker socket if it exists
     """
 
     if cluster.inventory["services"]["cri"]["containerRuntime"] == "containerd":
         control_plane = cluster.nodes["control-plane"].get_first_member(provide_node_configs=True)
         control_plane["connection"].sudo(f"sudo kubectl annotate nodes --all \
                                      --overwrite kubeadm.alpha.kubernetes.io/cri-socket=/run/containerd/containerd.sock"
-                                     , is_async=False, hide=True)
+                                         , is_async=False, hide=True)
         upgrade_group = kubernetes.get_group_for_upgrade(cluster)
         upgrade_group.sudo("rm -rf /var/run/docker.sock")
 
+
 def kubernetes_apply_taints(cluster):
     # Apply taints after upgrade
     group = cluster.nodes['control-plane']
     kubernetes.apply_taints(group)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     version: v1.24.11
   v1.25.2:
     version: v1.25.2
   v1.25.7:
     version: v1.25.7
   v1.26.3:
     version: v1.26.3
+  v1.26.4:
+    version: v1.26.4
+  v1.27.1:
+    version: v1.27.1
 kube-controller-manager:
   v1.21.2:
     version: v1.21.2
   v1.21.5:
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
@@ -50,14 +54,18 @@
     version: v1.24.11
   v1.25.2:
     version: v1.25.2
   v1.25.7:
     version: v1.25.7
   v1.26.3:
     version: v1.26.3
+  v1.26.4:
+    version: v1.26.4
+  v1.27.1:
+    version: v1.27.1
 kube-scheduler:
   v1.21.2:
     version: v1.21.2
   v1.21.5:
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
@@ -77,14 +85,18 @@
     version: v1.24.11
   v1.25.2:
     version: v1.25.2
   v1.25.7:
     version: v1.25.7
   v1.26.3:
     version: v1.26.3
+  v1.26.4:
+    version: v1.26.4
+  v1.27.1:
+    version: v1.27.1
 kube-proxy:
   v1.21.2:
     version: v1.21.2
   v1.21.5:
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
@@ -104,14 +116,18 @@
     version: v1.24.11
   v1.25.2:
     version: v1.25.2
   v1.25.7:
     version: v1.25.7
   v1.26.3:
     version: v1.26.3
+  v1.26.4:
+    version: v1.26.4
+  v1.27.1:
+    version: v1.27.1
 pause:
   v1.21.2:
     version: 3.4.1
   v1.21.5:
     version: 3.4.1
   v1.21.12:
     version: 3.4.1
@@ -131,14 +147,18 @@
     version: '3.7'
   v1.25.2:
     version: '3.8'
   v1.25.7:
     version: '3.8'
   v1.26.3:
     version: '3.9'
+  v1.26.4:
+    version: '3.9'
+  v1.27.1:
+    version: '3.9'
 etcd:
   v1.21.2:
     version: 3.4.13-0
   v1.21.5:
     version: 3.4.13-0
   v1.21.12:
     version: 3.4.13-0
@@ -158,14 +178,18 @@
     version: 3.5.6-0
   v1.25.2:
     version: 3.5.4-0
   v1.25.7:
     version: 3.5.6-0
   v1.26.3:
     version: 3.5.6-0
+  v1.26.4:
+    version: 3.5.6-0
+  v1.27.1:
+    version: 3.5.7-0
 coredns/coredns:
   v1.21.2:
     version: v1.8.0
   v1.21.5:
     version: v1.8.0
   v1.21.12:
     version: v1.8.0
@@ -185,7 +209,11 @@
     version: v1.8.6
   v1.25.2:
     version: v1.9.3
   v1.25.7:
     version: v1.9.3
   v1.26.3:
     version: v1.9.3
+  v1.26.4:
+    version: v1.9.3
+  v1.27.1:
+    version: v1.10.1
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This configuration is partially generated and maintained by "scripts/thirdparties/sync.py"
-# If new Kubernetes version is added, the compatibility mapping is inserted with fake "0.0.0" versions.
-# The developer should manually choose the required package versions.
+#
+# If new Kubernetes version is added, the compatibility mapping is taken from the previous Kubernetes versions.
+# The developer should manually change the required package versions if necessary.
 docker:
   v1.21.2:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
   v1.21.5:
     version_rhel: 19.03*
@@ -50,14 +51,22 @@
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
   v1.26.3:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
+  v1.26.4:
+    version_rhel: 19.03*
+    version_rhel8: 19.03*
+    version_debian: 5:20.10.*
+  v1.27.1:
+    version_rhel: 19.03*
+    version_rhel8: 19.03*
+    version_debian: 5:20.10.*
 containerd:
   v1.21.2:
     version_rhel8: 1.4*
     version_debian: 1.5.*
   v1.21.5:
     version_rhel8: 1.4*
     version_debian: 1.5.*
@@ -90,14 +99,20 @@
     version_debian: 1.6.*
   v1.25.7:
     version_rhel8: 1.4*
     version_debian: 1.6.*
   v1.26.3:
     version_rhel8: 1.4*
     version_debian: 1.6.*
+  v1.26.4:
+    version_rhel8: 1.4*
+    version_debian: 1.6.*
+  v1.27.1:
+    version_rhel8: 1.4*
+    version_debian: 1.6.*
 containerdio:
   v1.21.2:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.5.*
   v1.21.5:
     version_rhel: 1.6*
@@ -143,14 +158,22 @@
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.6.*
   v1.26.3:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.6.*
+  v1.26.4:
+    version_rhel: 1.6*
+    version_rhel8: 1.6*
+    version_debian: 1.6.*
+  v1.27.1:
+    version_rhel: 1.6*
+    version_rhel8: 1.6*
+    version_debian: 1.6.*
 podman:
   v1.21.2:
     version_rhel: 1.6.4*
     version_rhel8: "*"
     version_debian: "*"
   v1.21.5:
     version_rhel: 1.6.4*
@@ -196,14 +219,22 @@
     version_rhel: 1.6.4*
     version_rhel8: "*"
     version_debian: "*"
   v1.26.3:
     version_rhel: 1.6.4*
     version_rhel8: "*"
     version_debian: "*"
+  v1.26.4:
+    version_rhel: 1.6.4*
+    version_rhel8: "*"
+    version_debian: "*"
+  v1.27.1:
+    version_rhel: 1.6.4*
+    version_rhel8: "*"
+    version_debian: "*"
 haproxy:
   version_rhel: 1.8*
   version_rhel8: 1.8*
   version_debian: 2.*
 keepalived:
   version_rhel: 1.3*
   version_rhel8: 2.1*
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     version: v3.24.2
   v1.25.2:
     version: v3.24.2
   v1.25.7:
     version: v3.24.2
   v1.26.3:
     version: v3.24.2
+  v1.26.4:
+    version: v3.25.1
+  v1.27.1:
+    version: v3.25.1
 nginx-ingress-controller:
   v1.21.2:
     version: v1.2.0
     webhook-version: v1.1.1
   v1.21.5:
     version: v1.2.0
     webhook-version: v1.1.1
@@ -67,14 +71,20 @@
     webhook-version: v20220916-gd32f8c343
   v1.25.7:
     version: v1.4.0
     webhook-version: v20220916-gd32f8c343
   v1.26.3:
     version: v1.4.0
     webhook-version: v20220916-gd32f8c343
+  v1.26.4:
+    version: v1.7.0
+    webhook-version: v20230312-helm-chart-4.5.2-28-g66a760794
+  v1.27.1:
+    version: v1.7.0
+    webhook-version: v20230312-helm-chart-4.5.2-28-g66a760794
 kubernetes-dashboard:
   v1.21.2:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
   v1.21.5:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
@@ -107,14 +117,20 @@
     metrics-scraper-version: v1.0.8
   v1.25.7:
     version: v2.7.0
     metrics-scraper-version: v1.0.8
   v1.26.3:
     version: v2.7.0
     metrics-scraper-version: v1.0.8
+  v1.26.4:
+    version: v2.7.0
+    metrics-scraper-version: v1.0.8
+  v1.27.1:
+    version: v2.7.0
+    metrics-scraper-version: v1.0.8
 local-path-provisioner:
   v1.21.2:
     version: v0.0.22
     busybox-version: 1.34.1
   v1.21.5:
     version: v0.0.22
     busybox-version: 1.34.1
@@ -147,7 +163,13 @@
     busybox-version: 1.34.1
   v1.25.7:
     version: v0.0.23
     busybox-version: 1.34.1
   v1.26.3:
     version: v0.0.23
     busybox-version: 1.34.1
+  v1.26.4:
+    version: v0.0.24
+    busybox-version: 1.34.1
+  v1.27.1:
+    version: v0.0.24
+    busybox-version: 1.34.1
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     sha1: 7d44b41e36ff71f5f00671d518f2e59b4540653a
   v1.25.2:
     sha1: 72b87eedc9701c1143126f4aa7375b91fc9d46fc
   v1.25.7:
     sha1: 4efb3da49a50d137b728f0529bedee458e8c5f86
   v1.26.3:
     sha1: 86e202f98d22c8fddcadda6656f6698d21eae6ca
+  v1.26.4:
+    sha1: 7b2f579d06d00d545b2dc279df837d3c9d3e7ae6
+  v1.27.1:
+    sha1: d178257fa65dfa4694dea3262c618c6622804eb7
 kubelet:
   v1.21.2:
     sha1: 024e458aa0f74cba6b773401b779590437812fc6
   v1.21.5:
     sha1: 61da22475b977cb678cca8cf7249bf727d72ee89
   v1.21.12:
     sha1: 45a50b60122f35505ecd08479be1ae232b0ac524
@@ -51,14 +55,18 @@
     sha1: 3f332cbeed2f09b5275d56872bb8adcf54c9c98d
   v1.25.2:
     sha1: afdc009cd59759626ecce007667f42bf42e7c1be
   v1.25.7:
     sha1: ace8ce244896aca5d38c8184c44226660a09269a
   v1.26.3:
     sha1: 5fe320fedaabb91d3770da19135412b7454bb28b
+  v1.26.4:
+    sha1: 07fc5049dd34744d1c45258ed23291c3e58d4abf
+  v1.27.1:
+    sha1: 43cb7231a889c01cfd88bd3f27441134e3d1cbff
 kubectl:
   v1.21.2:
     sha1: 2c7a7de9fff41ac49f7c2546a9b1aff2c1d9c468
   v1.21.5:
     sha1: c4648e31ca16fb00e3826f8ab7c653da81eff367
   v1.21.12:
     sha1: 54a381297eb3a94ab968bb8bfff5f91e3d08805a
@@ -78,14 +86,18 @@
     sha1: 3f5d977d9ec38937ecf1dc9ccc3d0f0e48b88655
   v1.25.2:
     sha1: b12c0e102df89cd0579c8a3c769988aaf5dbe4ba
   v1.25.7:
     sha1: a5b32c173670ee6fa7710d7158ea4a0d198c8af5
   v1.26.3:
     sha1: 56916d87c3caef05489db932fd9e48d32ebdf634
+  v1.26.4:
+    sha1: b4880f3423aaf68992cdac384289739ff810a07a
+  v1.27.1:
+    sha1: 0c3f1e262a6c37719ba4d66885df6715f58b60e5
 calicoctl:
 # calicoctl version is duplicated from kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
 # It also corresponds to the plugin version in kubemarine/resources/configurations/compatibility/internal/plugins.yaml
   v1.21.2:
     version: v3.22.2
     sha1: b1e2c550480afe4250a34b0e4529eb38ae06973f
   v1.21.5:
@@ -120,14 +132,20 @@
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
   v1.25.7:
     version: v3.24.2
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
   v1.26.3:
     version: v3.24.2
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
+  v1.26.4:
+    version: v3.25.1
+    sha1: bc3f20a899aca3f62451bb7d9b015b9805305216
+  v1.27.1:
+    version: v3.25.1
+    sha1: bc3f20a899aca3f62451bb7d9b015b9805305216
 crictl:
 # crictl version is duplicated from kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
 # for backward compatibility with clusters in a private environment.
   v1.21.2:
     version: v1.23.0
     sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
   v1.21.5:
@@ -162,7 +180,13 @@
     sha1: b3a24e549ca3b4dfd105b7f4639014c0c508bea3
   v1.25.7:
     version: v1.25.0
     sha1: b3a24e549ca3b4dfd105b7f4639014c0c508bea3
   v1.26.3:
     version: v1.25.0
     sha1: b3a24e549ca3b4dfd105b7f4639014c0c508bea3
+  v1.26.4:
+    version: v1.27.0
+    sha1: 69b4973cd4542224c1790d1847e0e9a504f1a345
+  v1.27.1:
+    version: v1.27.0
+    sha1: 69b4973cd4542224c1790d1847e0e9a504f1a345
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     supported: true
   v1.24:
     supported: true
   v1.25:
     supported: true
   v1.26:
     supported: true
+  v1.27:
+    supported: true
 compatibility_map:
 # This section should be changed manually.
   v1.21.2:
     calico: v3.22.2
     nginx-ingress-controller: v1.2.0
     kubernetes-dashboard: v2.5.1
     local-path-provisioner: v0.0.22
@@ -88,9 +90,28 @@
     crictl: v1.25.0
   v1.26.3:
     calico: v3.24.2
     nginx-ingress-controller: v1.4.0
     kubernetes-dashboard: v2.7.0
     local-path-provisioner: v0.0.23
     crictl: v1.25.0
+  v1.26.4:
+    calico: v3.25.1
+    nginx-ingress-controller: v1.7.0
+    kubernetes-dashboard: v2.7.0
+    local-path-provisioner: v0.0.24
+    crictl: v1.27.0
+  v1.27.1:
+    calico: v3.25.1
+    nginx-ingress-controller: v1.7.0
+    kubernetes-dashboard: v2.7.0
+    local-path-provisioner: v0.0.24
+    crictl: v1.27.0
+
 
 # After any change, please run scripts/thirdparties/sync.py
+
+# The following optional keys are supported in addition to the 5 required software keys:
+#<Kubernetes version>:
+#  webhook: <version>
+#  metrics-scraper: <version>
+#  busybox: <version>
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
     127.0.0.1:
       - localhost
       - localhost.localdomain
     '::1':
       - '{% if not nodes[0]["internal_address"]|isipv4 %}localhost{% endif %}'
       - '{% if not nodes[0]["internal_address"]|isipv4 %}localhost.localdomain{% endif %}'
 
+  etc_hosts_generated: {}
+
   audit:
     cluster_policy:
       apiVersion: audit.k8s.io/v1
       kind: Policy
       # Don't generate audit events for all requests in RequestReceived stage.
       omitStages:
         - "RequestReceived"
@@ -257,14 +259,15 @@
       - '{% if services["cri"]["containerRuntime"] == "docker" %}-w /etc/default/docker -k docker{% endif %}'
       - '{% if services["cri"]["containerRuntime"] == "docker" %}-w /etc/docker/daemon.json -k docker{% endif %}'
       - '{% if services["cri"]["containerRuntime"] == "docker" %}-w /usr/sbin/runc -k docker{% endif %}'
       - '{% if services["cri"]["containerRuntime"] == "docker" %}-w /usr/bin/dockerd -k docker{% endif %}'
       - '-w /usr/bin/containerd -k docker'
 
   coredns:
+    add_etc_hosts_generated: true
     deployment:
       spec:
         template:
           spec:
             volumes:
             - configMap:
                 defaultMode: 420
@@ -334,14 +337,17 @@
               class: IN
               type: AAAA
               data:
                 authority: '{% raw %}{{ .Name }}{% endraw %} 3600 IN SOA coredns.kube-system.svc.cluster.local. hostmaster.coredns.kube-system.svc.cluster.local. (3600 3600 3600 3600 3600)'
           forward:
             - .
             - /etc/resolv.conf
+      Hosts: |
+        127.0.0.1 localhost localhost.localdomain
+        {% if not nodes[0]["internal_address"]|isipv4 %}::1 localhost localhost.localdomain{% endif %}
 
   loadbalancer:
     haproxy:
       defaults:
         timeout_connect: '10s'
         timeout_client: '1m'
         timeout_server: '1m'
@@ -555,14 +561,17 @@
     install: true
     installation:
       registry: k8s.gcr.io
       priority: 1
       procedures:
         - python:
             module: plugins/nginx_ingress.py
+            method: check_job_for_nginx
+        - python:
+            module: plugins/nginx_ingress.py
             method: manage_custom_certificate
         - python:
             module: plugins/builtin.py
             method: apply_yaml
             arguments:
               plugin_name: nginx-ingress-controller
         - expect:
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.17.0/kubemarine/resources/configurations/globals.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,19 @@
           - '7.8'
           - '7.9'
       - os_family: 'rhel8'
         versions:
           - '8.4'
           - '8.6'
           - '8.7'
+    rocky:
+      - os_family: 'rhel8'
+        versions:
+          - '8.6'
+          - '8.7'
     ubuntu:
       - os_family: 'debian'
         versions:
           - '20.04'
           - '22.04'
         unstable_kernel:
           - '5.4.0-132-generic'
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/psp/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.17.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/psp/default.yaml` & `kubemarine-0.17.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.17.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.17.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/reports/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/reports/check_report.css` & `kubemarine-0.17.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/backup.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9076388888888888%*

 * *Differences: {"'description'": "'You can install or upgrade HELM chart on the Kubernetes cluster'",*

 * * "'properties'": "{'chart_path': {'description': 'The path on local host to the Helm chart. The "*

 * *                 "URL link to chart archive is also supported.'}, 'values': {'description': "*

 * *                 '"YAML formatted values for the chart that override values from the values.yaml '*

 * *                 'file from the provided chart. The values from this parameter also override the '*

 * *                 'values from the \ […]*

```diff
@@ -1,32 +1,32 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
-    "description": "You can install or upgrade HELM chart on Kubernetes cluster",
+    "description": "You can install or upgrade HELM chart on the Kubernetes cluster",
     "properties": {
         "chart_path": {
-            "description": "A path on local host to the Helm chart. The URL link to chart archive is also supported.",
+            "description": "The path on local host to the Helm chart. The URL link to chart archive is also supported.",
             "minLength": 1,
             "type": "string"
         },
         "namespace": {
             "default": "default",
-            "description": "A cloud namespace where chart should be installed",
+            "description": "The cloud namespace where the chart should be installed",
             "type": "string"
         },
         "release": {
-            "description": "Target Helm release. It is equal to chart name by default.",
+            "description": "The target Helm release. It is equal to the chart name by default.",
             "type": "string"
         },
         "values": {
-            "description": "YAML formatted values for the chart that override values from values.yaml file from the provided chart. The values from this parameter also override the values from the 'values_file' parameter.",
+            "description": "YAML formatted values for the chart that override values from the values.yaml file from the provided chart. The values from this parameter also override the values from the 'values_file' parameter.",
             "type": "object"
         },
         "values_file": {
-            "description": "A path on local host to the file with YAML formatted values for the chart that override values from values.yaml file from the provided chart.",
+            "description": "The path on local host to the file with YAML formatted values for the chart that override values from the values.yaml file from the provided chart.",
             "type": "string"
         }
     },
     "required": [
         "chart_path"
     ],
     "type": "object"
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'properties'": "{'add_etc_hosts_generated': OrderedDict([('type', 'boolean'), ('default', True), "*

 * *                 "('description', 'Enables to add autogenerated records about cluster nodes to "*

 * *                 "Hosts part of coredns configmap')])}"}*

```diff
@@ -299,14 +299,19 @@
                 ]
             },
             "type": "object"
         }
     },
     "description": "Configure the Coredns service and its DNS rules in the Kubernetes cluster",
     "properties": {
+        "add_etc_hosts_generated": {
+            "default": true,
+            "description": "Enables to add autogenerated records about cluster nodes to Hosts part of coredns configmap",
+            "type": "boolean"
+        },
         "configmap": {
             "additionalProperties": {
                 "type": "string"
             },
             "description": "Configmap parameters that are applied to the Coredns service",
             "properties": {
                 "Corefile": {
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156863%*

 * *Differences: {"'properties'": "{'etc_hosts_generated': OrderedDict([('description', 'Describes auto-generated "*

 * *                 'records about nodes for /etc/hosts and coredns configmap. The key is an '*

 * *                 "IP-address, the value is either a DNS name or an array of names.'), ('$ref', "*

 * *                 "'services/etc_hosts.json')])}"}*

```diff
@@ -11,14 +11,18 @@
         },
         "cri": {
             "$ref": "services/cri.json"
         },
         "etc_hosts": {
             "$ref": "services/etc_hosts.json"
         },
+        "etc_hosts_generated": {
+            "$ref": "services/etc_hosts.json",
+            "description": "Describes auto-generated records about nodes for /etc/hosts and coredns configmap. The key is an IP-address, the value is either a DNS name or an array of names."
+        },
         "kernel_security": {
             "$ref": "services/kernel_security.json"
         },
         "kubeadm": {
             "$ref": "services/kubeadm.json"
         },
         "kubeadm_flags": {
```

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/restore.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.17.0/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.17.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.17.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.17.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.17.0/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/selinux.py` & `kubemarine-0.17.0/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/sysctl.py` & `kubemarine-0.17.0/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/system.py` & `kubemarine-0.17.0/kubemarine/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,38 +44,45 @@
              cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('FallbackNTP')):
         raise Exception('chrony and timesyncd configured both at the same time')
 
     return inventory
 
 
 def enrich_etc_hosts(inventory, cluster):
+# enrich only etc_hosts_generated object, etc_hosts remains as it is
+
+    # if by chance cluster.yaml contains non empty etc_hosts_generated we have to reset it
+    inventory['services']['etc_hosts_generated'] = {}
+
     control_plain = inventory['control_plain']['internal']
 
-    control_plain_names = inventory['services']['etc_hosts'].get(control_plain, [])
+    control_plain_names = []
     control_plain_names.append(cluster.inventory['cluster_name'])
     control_plain_names.append('control-plain')
     control_plain_names = list(OrderedSet(control_plain_names))
-    inventory['services']['etc_hosts'][control_plain] = control_plain_names
+    inventory['services']['etc_hosts_generated'][control_plain] = control_plain_names
 
     for node in cluster.inventory['nodes']:
         if 'remove_node' in node['roles']:
             continue
 
-        internal_node_ip_names = inventory['services']['etc_hosts'].get(node['internal_address'], [])
+        internal_node_ip_names = inventory['services']['etc_hosts_generated'].get(node['internal_address'], [])  
+
         internal_node_ip_names.append("%s.%s" % (node['name'], cluster.inventory['cluster_name']))
         internal_node_ip_names.append(node['name'])
         internal_node_ip_names = list(OrderedSet(internal_node_ip_names))
-        inventory['services']['etc_hosts'][node['internal_address']] = internal_node_ip_names
+        inventory['services']['etc_hosts_generated'][node['internal_address']] = internal_node_ip_names
 
         if node.get('address'):
-            external_node_ip_names = inventory['services']['etc_hosts'].get(node['address'], [])
+            external_node_ip_names = inventory['services']['etc_hosts_generated'].get(node['address'], []) 
+
             external_node_ip_names.append("%s-external.%s" % (node['name'], cluster.inventory['cluster_name']))
             external_node_ip_names.append(node['name'] + "-external")
             external_node_ip_names = list(OrderedSet(external_node_ip_names))
-            inventory['services']['etc_hosts'][node['address']] = external_node_ip_names
+            inventory['services']['etc_hosts_generated'][node['address']] = external_node_ip_names
 
     return inventory
 
 
 def enrich_upgrade_inventory(inventory: dict, cluster: KubernetesCluster):
     if cluster.context.get("initial_procedure") != "upgrade":
         return inventory
@@ -198,15 +205,15 @@
         stdout = result.stdout.lower()
 
         version = None
         lines = ''
 
         version_regex = re.compile("\\s\\d*\\.\\d*", re.M)
         for line in stdout.split("\n"):
-            if 'centos' in line or 'rhel' in line:
+            if 'centos' in line or 'rhel' or 'rocky' in line:
                 # CentOS and Red Hat have a major version in VERSION_ID string
                 matches = re.findall(version_regex, line)
                 if matches:
                     version = matches[0].strip()
             if '=' in line:
                 lines += line + "\n"
 
@@ -277,46 +284,34 @@
         buffer.write("search %s\n" % config["search"])
     if config.get("nameservers") is not None:
         for address in config.get("nameservers"):
             buffer.write("nameserver %s\n" % address)
     return buffer
 
 
-def generate_etc_hosts_config(inventory, cluster=None):
+def generate_etc_hosts_config(inventory, cluster=None, etc_hosts_part='etc_hosts_generated'):
+# generate records for /etc/hosts from services.etc_hosts or services.etc_hosts_generated
+
     result = ""
 
     max_len_ip = 0
 
-    ignore_ips = []
-    if cluster and cluster.context['initial_procedure'] == 'remove_node':
-        for removal_node in cluster.procedure_inventory.get("nodes"):
-            removal_node_name = removal_node['name']
-            for node in inventory['nodes']:
-                if node['name'] == removal_node_name:
-                    if node.get('address'):
-                        ignore_ips.append(node['address'])
-                    if node.get('internal_address'):
-                        ignore_ips.append(node['internal_address'])
-
-    ignore_ips = list(set(ignore_ips))
-
-    for ip in list(inventory['services']['etc_hosts'].keys()):
+    for ip in list(inventory['services'][etc_hosts_part].keys()):
         if len(ip) > max_len_ip:
             max_len_ip = len(ip)
 
-    for ip, names in inventory['services']['etc_hosts'].items():
+    for ip, names in inventory['services'][etc_hosts_part].items():
         if isinstance(names, list):
             # remove records with empty values from list
             names = list(filter(len, names))
             # if list is empty, then skip
             if not names:
                 continue
             names = " ".join(names)
-        if ip not in ignore_ips:
-            result += "%s%s  %s\n" % (ip, " " * (max_len_ip - len(ip)), names)
+        result += "%s%s  %s\n" % (ip, " " * (max_len_ip - len(ip)), names)
 
     return result
 
 
 def update_etc_hosts(group, config=None):
     if config is None:
         raise Exception("Data can't be empty")
```

### Comparing `kubemarine-0.16.0/kubemarine/templates/__init__.py` & `kubemarine-0.17.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.17.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.17.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.17.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.17.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.17.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/testsuite.py` & `kubemarine-0.17.0/kubemarine/testsuite.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/thirdparties.py` & `kubemarine-0.17.0/kubemarine/thirdparties.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine/yum.py` & `kubemarine-0.17.0/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.16.0/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.17.0/kubemarine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.16.0
+Version: 0.17.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
+Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
 Keywords: kubernetes,devops,administration,helm
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -79,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -98,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -127,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.16.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.17.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -172,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.17.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.17.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.17.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.16.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.17.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.16.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.17.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.16.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.17.0/LICENSE)
```

### Comparing `kubemarine-0.16.0/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.17.0/kubemarine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,30 +59,32 @@
 kubemarine/kubernetes/__init__.py
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
-kubemarine/patches/p1_helm_values.py
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
 kubemarine/plugins/nginx_ingress.py
 kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
 kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
 kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
 kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
 kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
 kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
 kubemarine/procedures/__init__.py
 kubemarine/procedures/add_node.py
 kubemarine/procedures/backup.py
 kubemarine/procedures/cert_renew.py
 kubemarine/procedures/check_iaas.py
 kubemarine/procedures/check_paas.py
 kubemarine/procedures/do.py
```

### Comparing `kubemarine-0.16.0/pyproject.toml` & `kubemarine-0.17.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 dependencies = [
     "PyYAML==6.0",
     "deepmerge==1.0.*",
     "fabric==2.6.*",
     "jinja2==3.1.*",
     "MarkupSafe==2.1.*",
     "invoke==1.6.*",
-    "ruamel.yaml==0.17.*",
+    "ruamel.yaml==0.17.22",
     "pygelf==0.4.*",
     "toml==0.10.*",
     "python-dateutil==2.8.*",
     "deepdiff==6.2.*",
     "ordered-set==4.1.*",
     # cryptography is a transitive dependency of paramiko. Fix version to avoid unexpected deprecation warnings.
     "cryptography==39.0.*",
@@ -60,15 +60,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "0.16.0"
+current_version = "0.17.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.16.0/setup.py` & `kubemarine-0.17.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,9 +41,10 @@
 # Though deprecated, it seems to be the only way to provide shell scripts.
 SCRIPTS=["bin/kubemarine.cmd", "bin/kubemarine"]
 
 setup(
     scripts=SCRIPTS,
     version=VERSION,
     long_description=README,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    url='https://github.com/Netcracker/KubeMarine'
 )
```

