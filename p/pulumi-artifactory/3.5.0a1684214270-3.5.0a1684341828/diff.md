# Comparing `tmp/pulumi_artifactory-3.5.0a1684214270.tar.gz` & `tmp/pulumi_artifactory-3.5.0a1684341828.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_artifactory-3.5.0a1684214270.tar", last modified: Tue May 16 05:25:25 2023, max compression
+gzip compressed data, was "pulumi_artifactory-3.5.0a1684341828.tar", last modified: Wed May 17 16:48:19 2023, max compression
```

## Comparing `pulumi_artifactory-3.5.0a1684214270.tar` & `pulumi_artifactory-3.5.0a1684341828.tar`

### file list

```diff
@@ -1,308 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:25.565105 pulumi_artifactory-3.5.0a1684214270/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-16 05:25:25.565105 pulumi_artifactory-3.5.0a1684214270/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:25.561104 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/
--rw-r--r--   0 runner    (1001) docker     (123)    45570 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    26856 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    54037 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/anonymous_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/artifact_property_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/artifact_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/artifactory_release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/build_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:25.565105 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/distribution_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/docker_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/general_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_terraformbackend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    29850 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/ldap_group_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/ldap_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_repository_multi_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_repository_single_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_terraform_backend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    24136 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/managed_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/oauth_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18740 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/permission_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/property_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/pull_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/push_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_repository_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24828 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/repository_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/saml_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35645 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/scoped_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/single_replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25463 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/unmanaged_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    27110 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44685 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_terraform_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:25:25.565105 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:25:25.565105 pulumi_artifactory-3.5.0a1684214270/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-16 05:25:25.000000 pulumi_artifactory-3.5.0a1684214270/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:48:19.338317 pulumi_artifactory-3.5.0a1684341828/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 16:48:19.338317 pulumi_artifactory-3.5.0a1684341828/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:48:19.334317 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (123)    45822 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33734 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/anonymous_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/artifact_property_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/artifact_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/artifactory_release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/build_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:48:19.338317 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/distribution_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/distribution_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/docker_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/general_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_terraformbackend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/ldap_group_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/ldap_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_repository_multi_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_repository_single_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_terraform_backend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/managed_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/oauth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/permission_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/pull_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/push_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_repository_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/repository_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/saml_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41731 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/scoped_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/single_replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/unmanaged_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_terraform_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:48:19.334317 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-17 16:48:19.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-17 16:48:19.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:48:19.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:48:19.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 16:48:19.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 16:48:19.000000 pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 16:48:19.338317 pulumi_artifactory-3.5.0a1684341828/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-17 16:48:18.000000 pulumi_artifactory-3.5.0a1684341828/setup.py
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/PKG-INFO` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_artifactory
-Version: 3.5.0a1684214270
+Name: pulumi-artifactory
+Version: 3.5.0a1684341828
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/README.md` & `pulumi_artifactory-3.5.0a1684341828/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/__init__.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .artifact_property_webhook import *
 from .artifact_webhook import *
 from .artifactory_release_bundle_webhook import *
 from .backup import *
 from .build_webhook import *
 from .certificate import *
 from .debian_repository import *
+from .distribution_public_key import *
 from .distribution_webhook import *
 from .docker_v1_repository import *
 from .docker_v2_repository import *
 from .docker_webhook import *
 from .federated_alpine_repository import *
 from .federated_bower_repository import *
 from .federated_cargo_repository import *
@@ -390,14 +391,22 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/debianRepository:DebianRepository": "DebianRepository"
   }
  },
  {
   "pkg": "artifactory",
+  "mod": "index/distributionPublicKey",
+  "fqn": "pulumi_artifactory",
+  "classes": {
+   "artifactory:index/distributionPublicKey:DistributionPublicKey": "DistributionPublicKey"
+  }
+ },
+ {
+  "pkg": "artifactory",
   "mod": "index/distributionWebhook",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/distributionWebhook:DistributionWebhook": "DistributionWebhook"
   }
  },
  {
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/_inputs.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/_utilities.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/access_token.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/access_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -294,14 +294,115 @@
                  end_date: Optional[pulumi.Input[str]] = None,
                  end_date_relative: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  refreshable: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Provides an Artifactory Access Token resource. This can be used to create and manage Artifactory Access Tokens.
+
+        > **Note:** Access Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
+        state.
+
+        ## Example Usage
+
+        ### S
+        ### Create a new Artifactory Access Token for an existing user
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        exising_user = artifactory.AccessToken("exisingUser",
+            end_date_relative="5m",
+            username="existing-user")
+        ```
+
+        Note: This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
+        ### Create a new Artifactory User and Access token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        new_user_user = artifactory.User("newUserUser",
+            email="new_user@somewhere.com",
+            groups=["readers"])
+        new_user_access_token = artifactory.AccessToken("newUserAccessToken",
+            username=new_user_user.name,
+            end_date_relative="5m")
+        ```
+        ### Creates a new token for groups
+        This creates a transient user called `temporary-user`.
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        temporary_user = artifactory.AccessToken("temporaryUser",
+            end_date_relative="1h",
+            groups=["readers"],
+            username="temporary-user")
+        ```
+        ### Create token with no expiry
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        no_expiry = artifactory.AccessToken("noExpiry",
+            end_date_relative="0s",
+            username="existing-user")
+        ```
+        ### Creates a refreshable token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        refreshable = artifactory.AccessToken("refreshable",
+            end_date_relative="1m",
+            groups=["readers"],
+            refreshable=True,
+            username="refreshable")
+        ```
+        ### Creates an administrator token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        admin = artifactory.AccessToken("admin",
+            admin_token=artifactory.AccessTokenAdminTokenArgs(
+                instance_id="<instance id>",
+            ),
+            end_date_relative="1m",
+            username="admin")
+        ```
+        ### Creates a token with an audience
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        audience = artifactory.AccessToken("audience",
+            audience="jfrt@*",
+            end_date_relative="1m",
+            refreshable=True,
+            username="audience")
+        ```
+        ### Creates a token with a fixed end date
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        fixeddate = artifactory.AccessToken("fixeddate",
+            end_date="2018-01-01T01:02:03Z",
+            groups=["readers"],
+            username="fixeddate")
+        ```
+        ## References
+
+        - https://www.jfrog.com/confluence/display/ACC1X/Access+Tokens
+        - https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateToken
+
         ## Import
 
         Artifactory **does not** retain access tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['AccessTokenAdminTokenArgs']] admin_token: (Optional) Specify the `instance_id` in this block to grant this token admin privileges. This can only be created when the authenticated user is an admin. `admin_token` cannot be specified with `groups`.
@@ -315,14 +416,115 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AccessTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides an Artifactory Access Token resource. This can be used to create and manage Artifactory Access Tokens.
+
+        > **Note:** Access Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
+        state.
+
+        ## Example Usage
+
+        ### S
+        ### Create a new Artifactory Access Token for an existing user
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        exising_user = artifactory.AccessToken("exisingUser",
+            end_date_relative="5m",
+            username="existing-user")
+        ```
+
+        Note: This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
+        ### Create a new Artifactory User and Access token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        new_user_user = artifactory.User("newUserUser",
+            email="new_user@somewhere.com",
+            groups=["readers"])
+        new_user_access_token = artifactory.AccessToken("newUserAccessToken",
+            username=new_user_user.name,
+            end_date_relative="5m")
+        ```
+        ### Creates a new token for groups
+        This creates a transient user called `temporary-user`.
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        temporary_user = artifactory.AccessToken("temporaryUser",
+            end_date_relative="1h",
+            groups=["readers"],
+            username="temporary-user")
+        ```
+        ### Create token with no expiry
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        no_expiry = artifactory.AccessToken("noExpiry",
+            end_date_relative="0s",
+            username="existing-user")
+        ```
+        ### Creates a refreshable token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        refreshable = artifactory.AccessToken("refreshable",
+            end_date_relative="1m",
+            groups=["readers"],
+            refreshable=True,
+            username="refreshable")
+        ```
+        ### Creates an administrator token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        admin = artifactory.AccessToken("admin",
+            admin_token=artifactory.AccessTokenAdminTokenArgs(
+                instance_id="<instance id>",
+            ),
+            end_date_relative="1m",
+            username="admin")
+        ```
+        ### Creates a token with an audience
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        audience = artifactory.AccessToken("audience",
+            audience="jfrt@*",
+            end_date_relative="1m",
+            refreshable=True,
+            username="audience")
+        ```
+        ### Creates a token with a fixed end date
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        fixeddate = artifactory.AccessToken("fixeddate",
+            end_date="2018-01-01T01:02:03Z",
+            groups=["readers"],
+            username="fixeddate")
+        ```
+        ## References
+
+        - https://www.jfrog.com/confluence/display/ACC1X/Access+Tokens
+        - https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateToken
+
         ## Import
 
         Artifactory **does not** retain access tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param AccessTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/alpine_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         :param pulumi.Input[bool] download_direct: When set, download requests to this repository will redirect the client to download the artifact directly from the cloud
                storage provider. Available in Enterprise+ and Edge licenses only.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*. By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When used, only
                artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: The RSA key to be used to sign alpine indices.
+        :param pulumi.Input[str] primary_keypair_ref: Used to sign index files in Alpine Linux repositories. See:
+               https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         :param pulumi.Input[bool] priority_resolution: Setting repositories with priority will cause metadata to be merged only from repositories set with this field
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
@@ -218,15 +219,16 @@
     def notes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notes", value)
 
     @property
     @pulumi.getter(name="primaryKeypairRef")
     def primary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        The RSA key to be used to sign alpine indices.
+        Used to sign index files in Alpine Linux repositories. See:
+        https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         """
         return pulumi.get(self, "primary_keypair_ref")
 
     @primary_keypair_ref.setter
     def primary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "primary_keypair_ref", value)
 
@@ -342,15 +344,16 @@
                storage provider. Available in Enterprise+ and Edge licenses only.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*. By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When used, only
                artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] key: the identity key of the repo.
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: The RSA key to be used to sign alpine indices.
+        :param pulumi.Input[str] primary_keypair_ref: Used to sign index files in Alpine Linux repositories. See:
+               https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         :param pulumi.Input[bool] priority_resolution: Setting repositories with priority will cause metadata to be merged only from repositories set with this field
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
@@ -528,15 +531,16 @@
     def package_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "package_type", value)
 
     @property
     @pulumi.getter(name="primaryKeypairRef")
     def primary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        The RSA key to be used to sign alpine indices.
+        Used to sign index files in Alpine Linux repositories. See:
+        https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         """
         return pulumi.get(self, "primary_keypair_ref")
 
     @primary_keypair_ref.setter
     def primary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "primary_keypair_ref", value)
 
@@ -683,15 +687,16 @@
                storage provider. Available in Enterprise+ and Edge licenses only.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*. By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When used, only
                artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] key: the identity key of the repo.
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: The RSA key to be used to sign alpine indices.
+        :param pulumi.Input[str] primary_keypair_ref: Used to sign index files in Alpine Linux repositories. See:
+               https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         :param pulumi.Input[bool] priority_resolution: Setting repositories with priority will cause metadata to be merged only from repositories set with this field
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
@@ -842,15 +847,16 @@
                storage provider. Available in Enterprise+ and Edge licenses only.
         :param pulumi.Input[str] excludes_pattern: List of artifact patterns to exclude when evaluating artifact requests, in the form of x/y/**/z/*. By default no
                artifacts are excluded.
         :param pulumi.Input[str] includes_pattern: List of artifact patterns to include when evaluating artifact requests in the form of x/y/**/z/*. When used, only
                artifacts matching one of the include patterns are served. By default, all artifacts are included (**/*).
         :param pulumi.Input[str] key: the identity key of the repo.
         :param pulumi.Input[str] notes: Internal description.
-        :param pulumi.Input[str] primary_keypair_ref: The RSA key to be used to sign alpine indices.
+        :param pulumi.Input[str] primary_keypair_ref: Used to sign index files in Alpine Linux repositories. See:
+               https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         :param pulumi.Input[bool] priority_resolution: Setting repositories with priority will cause metadata to be merged only from repositories set with this field
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_environments: Project environment for assigning this repository to. Allow values: "DEV", "PROD", or one of custom environment. Before
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
@@ -971,15 +977,16 @@
     def package_type(self) -> pulumi.Output[str]:
         return pulumi.get(self, "package_type")
 
     @property
     @pulumi.getter(name="primaryKeypairRef")
     def primary_keypair_ref(self) -> pulumi.Output[Optional[str]]:
         """
-        The RSA key to be used to sign alpine indices.
+        Used to sign index files in Alpine Linux repositories. See:
+        https://www.jfrog.com/confluence/display/JFROG/Alpine+Linux+Repositories#AlpineLinuxRepositories-SigningAlpineLinuxIndex
         """
         return pulumi.get(self, "primary_keypair_ref")
 
     @property
     @pulumi.getter(name="priorityResolution")
     def priority_resolution(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/anonymous_user.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/anonymous_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,48 +13,52 @@
 
 @pulumi.input_type
 class AnonymousUserArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a AnonymousUser resource.
-        :param pulumi.Input[str] name: Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        :param pulumi.Input[str] name: Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+               set or updated in the HCL.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+        set or updated in the HCL.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class _AnonymousUserState:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering AnonymousUser resources.
-        :param pulumi.Input[str] name: Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        :param pulumi.Input[str] name: Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+               set or updated in the HCL.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+        set or updated in the HCL.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -75,23 +79,22 @@
 
         # Define a new Artifactory 'anonymous' user for import
         anonymous = artifactory.AnonymousUser("anonymous")
         ```
 
         ## Import
 
-        Anonymous user can be imported using their name, e.g.
-
         ```sh
          $ pulumi import artifactory:index/anonymousUser:AnonymousUser anonymous-user anonymous
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        :param pulumi.Input[str] name: Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+               set or updated in the HCL.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AnonymousUserArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -104,16 +107,14 @@
 
         # Define a new Artifactory 'anonymous' user for import
         anonymous = artifactory.AnonymousUser("anonymous")
         ```
 
         ## Import
 
-        Anonymous user can be imported using their name, e.g.
-
         ```sh
          $ pulumi import artifactory:index/anonymousUser:AnonymousUser anonymous-user anonymous
         ```
 
         :param str resource_name: The name of the resource.
         :param AnonymousUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -154,24 +155,26 @@
         """
         Get an existing AnonymousUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        :param pulumi.Input[str] name: Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+               set or updated in the HCL.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AnonymousUserState.__new__(_AnonymousUserState)
 
         __props__.__dict__["name"] = name
         return AnonymousUser(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Username for anonymous user. This should not be set in the HCL, or change after importing into Terraform state.
+        Username for anonymous user. This is only for ensuring resource schema is valid for Terraform. This is not meant to be
+        set or updated in the HCL.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/api_key.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/api_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 class ApiKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
         """
+        Provides an Artifactory API key resource. This can be used to create and manage Artifactory API keys.
+
+        > **Note:** API keys will be stored in the raw state as plain-text. Read more about sensitive data in state.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         # Create a new Artifactory API key for the configured user
@@ -83,14 +87,18 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ApiKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides an Artifactory API key resource. This can be used to create and manage Artifactory API keys.
+
+        > **Note:** API keys will be stored in the raw state as plain-text. Read more about sensitive data in state.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         # Create a new Artifactory API key for the configured user
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/artifact_property_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/artifact_property_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/artifact_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/artifact_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/artifactory_release_bundle_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/artifactory_release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/backup.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/build_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/build_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/certificate.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/config/vars.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/config/vars.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,9 +35,12 @@
         """
         Toggle for pre-flight checking of Artifactory Pro and Enterprise license. Default to `true`.
         """
         return __config__.get_bool('checkLicense') or False
 
     @property
     def url(self) -> Optional[str]:
+        """
+        Artifactory URL.
+        """
         return __config__.get('url')
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/distribution_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/distribution_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/docker_v1_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/docker_v2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/docker_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/docker_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_cargo_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_cocoapods_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_docker_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_docker_v1_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_docker_v2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_gitltfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_opkg_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_terraform_module_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_terraform_provider_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/federated_vagrant_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/general_security.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/general_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_cargo_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_cocoapods_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_docker_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_docker_v1_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_docker_v2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_gitlfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_opkg_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_terraform_module_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_terraform_provider_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_federated_vagrant_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_file.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_fileinfo.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_fileinfo.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_group.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_cargo_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_cocoapods_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_docker_v1_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_docker_v2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_gitlfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_opkg_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_pub_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_terraform_module_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_terraform_provider_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_terraformbackend_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_terraformbackend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_local_vagrant_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_permission_target.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_cargo_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_cocoapods_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_docker_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_gitlfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_opkg_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_p2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_pub_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_terraform_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_remote_vcs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_user.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_docker_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_gitlfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_p2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_pub_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/get_virtual_terraform_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/get_virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/group.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,77 +10,67 @@
 from . import _utilities
 
 __all__ = ['GroupArgs', 'Group']
 
 @pulumi.input_type
 class GroupArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
                  admin_privileges: Optional[pulumi.Input[bool]] = None,
                  auto_join: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  detach_all_users: Optional[pulumi.Input[bool]] = None,
                  external_id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  policy_manager: Optional[pulumi.Input[bool]] = None,
                  realm: Optional[pulumi.Input[str]] = None,
                  realm_attributes: Optional[pulumi.Input[str]] = None,
                  reports_manager: Optional[pulumi.Input[bool]] = None,
                  users_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  watch_manager: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Group resource.
-        :param pulumi.Input[str] name: Name of the group
         :param pulumi.Input[bool] admin_privileges: Any users added to this group will automatically be assigned with admin privileges in the system.
         :param pulumi.Input[bool] auto_join: When this parameter is set, any new users defined in the system are automatically assigned to this group.
-        :param pulumi.Input[str] description: A description for the group
-        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        :param pulumi.Input[str] description: A description for the group.
+        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         :param pulumi.Input[str] external_id: New external group ID used to configure the corresponding group in Azure AD.
+        :param pulumi.Input[str] name: Name of the group.
         :param pulumi.Input[bool] policy_manager: When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         :param pulumi.Input[str] realm: The realm for the group.
         :param pulumi.Input[str] realm_attributes: The realm attributes for the group.
         :param pulumi.Input[bool] reports_manager: When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_names: List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
         :param pulumi.Input[bool] watch_manager: When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
-        pulumi.set(__self__, "name", name)
         if admin_privileges is not None:
             pulumi.set(__self__, "admin_privileges", admin_privileges)
         if auto_join is not None:
             pulumi.set(__self__, "auto_join", auto_join)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if detach_all_users is not None:
             pulumi.set(__self__, "detach_all_users", detach_all_users)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if policy_manager is not None:
             pulumi.set(__self__, "policy_manager", policy_manager)
         if realm is not None:
             pulumi.set(__self__, "realm", realm)
         if realm_attributes is not None:
             pulumi.set(__self__, "realm_attributes", realm_attributes)
         if reports_manager is not None:
             pulumi.set(__self__, "reports_manager", reports_manager)
         if users_names is not None:
             pulumi.set(__self__, "users_names", users_names)
         if watch_manager is not None:
             pulumi.set(__self__, "watch_manager", watch_manager)
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of the group
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
     @pulumi.getter(name="adminPrivileges")
     def admin_privileges(self) -> Optional[pulumi.Input[bool]]:
         """
         Any users added to this group will automatically be assigned with admin privileges in the system.
         """
         return pulumi.get(self, "admin_privileges")
 
@@ -100,27 +90,27 @@
     def auto_join(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_join", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A description for the group
+        A description for the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="detachAllUsers")
     def detach_all_users(self) -> Optional[pulumi.Input[bool]]:
         """
-        When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         """
         return pulumi.get(self, "detach_all_users")
 
     @detach_all_users.setter
     def detach_all_users(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "detach_all_users", value)
 
@@ -133,14 +123,26 @@
         return pulumi.get(self, "external_id")
 
     @external_id.setter
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the group.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="policyManager")
     def policy_manager(self) -> Optional[pulumi.Input[bool]]:
         """
         When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         """
         return pulumi.get(self, "policy_manager")
 
@@ -183,14 +185,17 @@
     @reports_manager.setter
     def reports_manager(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reports_manager", value)
 
     @property
     @pulumi.getter(name="usersNames")
     def users_names(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
+        """
         return pulumi.get(self, "users_names")
 
     @users_names.setter
     def users_names(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users_names", value)
 
     @property
@@ -221,22 +226,23 @@
                  reports_manager: Optional[pulumi.Input[bool]] = None,
                  users_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  watch_manager: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Group resources.
         :param pulumi.Input[bool] admin_privileges: Any users added to this group will automatically be assigned with admin privileges in the system.
         :param pulumi.Input[bool] auto_join: When this parameter is set, any new users defined in the system are automatically assigned to this group.
-        :param pulumi.Input[str] description: A description for the group
-        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        :param pulumi.Input[str] description: A description for the group.
+        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         :param pulumi.Input[str] external_id: New external group ID used to configure the corresponding group in Azure AD.
-        :param pulumi.Input[str] name: Name of the group
+        :param pulumi.Input[str] name: Name of the group.
         :param pulumi.Input[bool] policy_manager: When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         :param pulumi.Input[str] realm: The realm for the group.
         :param pulumi.Input[str] realm_attributes: The realm attributes for the group.
         :param pulumi.Input[bool] reports_manager: When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_names: List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
         :param pulumi.Input[bool] watch_manager: When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
         if admin_privileges is not None:
             pulumi.set(__self__, "admin_privileges", admin_privileges)
         if auto_join is not None:
             pulumi.set(__self__, "auto_join", auto_join)
         if description is not None:
@@ -284,27 +290,27 @@
     def auto_join(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_join", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A description for the group
+        A description for the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="detachAllUsers")
     def detach_all_users(self) -> Optional[pulumi.Input[bool]]:
         """
-        When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         """
         return pulumi.get(self, "detach_all_users")
 
     @detach_all_users.setter
     def detach_all_users(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "detach_all_users", value)
 
@@ -320,15 +326,15 @@
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the group
+        Name of the group.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -379,14 +385,17 @@
     @reports_manager.setter
     def reports_manager(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reports_manager", value)
 
     @property
     @pulumi.getter(name="usersNames")
     def users_names(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
+        """
         return pulumi.get(self, "users_names")
 
     @users_names.setter
     def users_names(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users_names", value)
 
     @property
@@ -419,49 +428,50 @@
                  reports_manager: Optional[pulumi.Input[bool]] = None,
                  users_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  watch_manager: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         ## Import
 
-        Groups can be imported using their name, e.g.
-
         ```sh
          $ pulumi import artifactory:index/group:Group terraform-group mygroup
         ```
 
+         ~> `users_names` can't be imported due to API limitations.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin_privileges: Any users added to this group will automatically be assigned with admin privileges in the system.
         :param pulumi.Input[bool] auto_join: When this parameter is set, any new users defined in the system are automatically assigned to this group.
-        :param pulumi.Input[str] description: A description for the group
-        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        :param pulumi.Input[str] description: A description for the group.
+        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         :param pulumi.Input[str] external_id: New external group ID used to configure the corresponding group in Azure AD.
-        :param pulumi.Input[str] name: Name of the group
+        :param pulumi.Input[str] name: Name of the group.
         :param pulumi.Input[bool] policy_manager: When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         :param pulumi.Input[str] realm: The realm for the group.
         :param pulumi.Input[str] realm_attributes: The realm attributes for the group.
         :param pulumi.Input[bool] reports_manager: When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_names: List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
         :param pulumi.Input[bool] watch_manager: When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GroupArgs,
+                 args: Optional[GroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Import
 
-        Groups can be imported using their name, e.g.
-
         ```sh
          $ pulumi import artifactory:index/group:Group terraform-group mygroup
         ```
 
+         ~> `users_names` can't be imported due to API limitations.
+
         :param str resource_name: The name of the resource.
         :param GroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(GroupArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -495,16 +505,14 @@
             __props__ = GroupArgs.__new__(GroupArgs)
 
             __props__.__dict__["admin_privileges"] = admin_privileges
             __props__.__dict__["auto_join"] = auto_join
             __props__.__dict__["description"] = description
             __props__.__dict__["detach_all_users"] = detach_all_users
             __props__.__dict__["external_id"] = external_id
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["policy_manager"] = policy_manager
             __props__.__dict__["realm"] = realm
             __props__.__dict__["realm_attributes"] = realm_attributes
             __props__.__dict__["reports_manager"] = reports_manager
             __props__.__dict__["users_names"] = users_names
             __props__.__dict__["watch_manager"] = watch_manager
@@ -535,22 +543,23 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin_privileges: Any users added to this group will automatically be assigned with admin privileges in the system.
         :param pulumi.Input[bool] auto_join: When this parameter is set, any new users defined in the system are automatically assigned to this group.
-        :param pulumi.Input[str] description: A description for the group
-        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        :param pulumi.Input[str] description: A description for the group.
+        :param pulumi.Input[bool] detach_all_users: When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         :param pulumi.Input[str] external_id: New external group ID used to configure the corresponding group in Azure AD.
-        :param pulumi.Input[str] name: Name of the group
+        :param pulumi.Input[str] name: Name of the group.
         :param pulumi.Input[bool] policy_manager: When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         :param pulumi.Input[str] realm: The realm for the group.
         :param pulumi.Input[str] realm_attributes: The realm attributes for the group.
         :param pulumi.Input[bool] reports_manager: When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users_names: List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
         :param pulumi.Input[bool] watch_manager: When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupState.__new__(_GroupState)
 
         __props__.__dict__["admin_privileges"] = admin_privileges
@@ -583,23 +592,23 @@
         """
         return pulumi.get(self, "auto_join")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A description for the group
+        A description for the group.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="detachAllUsers")
-    def detach_all_users(self) -> pulumi.Output[Optional[bool]]:
+    def detach_all_users(self) -> pulumi.Output[bool]:
         """
-        When this is set to `true`, an empty or missing usernames array will detach all users from the group
+        When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         """
         return pulumi.get(self, "detach_all_users")
 
     @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> pulumi.Output[Optional[str]]:
         """
@@ -607,21 +616,21 @@
         """
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the group
+        Name of the group.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="policyManager")
-    def policy_manager(self) -> pulumi.Output[Optional[bool]]:
+    def policy_manager(self) -> pulumi.Output[bool]:
         """
         When this override is set, User in the group can set Xray security and compliance policies. Default value is `false`.
         """
         return pulumi.get(self, "policy_manager")
 
     @property
     @pulumi.getter
@@ -637,26 +646,29 @@
         """
         The realm attributes for the group.
         """
         return pulumi.get(self, "realm_attributes")
 
     @property
     @pulumi.getter(name="reportsManager")
-    def reports_manager(self) -> pulumi.Output[Optional[bool]]:
+    def reports_manager(self) -> pulumi.Output[bool]:
         """
         When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
         """
         return pulumi.get(self, "reports_manager")
 
     @property
     @pulumi.getter(name="usersNames")
     def users_names(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
+        """
         return pulumi.get(self, "users_names")
 
     @property
     @pulumi.getter(name="watchManager")
-    def watch_manager(self) -> pulumi.Output[Optional[bool]]:
+    def watch_manager(self) -> pulumi.Output[bool]:
         """
         When this override is set, User in the group can manage Xray Watches on any resource type. Default value is `false`.
         """
         return pulumi.get(self, "watch_manager")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/keypair.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/keypair.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
         :param pulumi.Input[str] alias: Will be used as a filename when retrieving the public key via REST API.
         :param pulumi.Input[str] pair_name: A unique identifier for the Key Pair record.
         :param pulumi.Input[str] pair_type: Key Pair type. Supported types - GPG and RSA.
         :param pulumi.Input[str] passphrase: Passphrase will be used to decrypt the private key. Validated server side.
         :param pulumi.Input[str] private_key: Private key. PEM format will be validated.
         :param pulumi.Input[str] public_key: Public key. PEM format will be validated.
         :param pulumi.Input[bool] unavailable: Unknown usage. Returned in the json payload and cannot be set.
+               
+               Artifactory REST API call Get Key Pair doesn't return keys `private_key` and `passphrase`, but consumes these keys in the POST call.
         """
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if pair_name is not None:
             pulumi.set(__self__, "pair_name", pair_name)
         if pair_type is not None:
             pulumi.set(__self__, "pair_type", pair_type)
@@ -218,14 +220,16 @@
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter
     def unavailable(self) -> Optional[pulumi.Input[bool]]:
         """
         Unknown usage. Returned in the json payload and cannot be set.
+
+        Artifactory REST API call Get Key Pair doesn't return keys `private_key` and `passphrase`, but consumes these keys in the POST call.
         """
         return pulumi.get(self, "unavailable")
 
     @unavailable.setter
     def unavailable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "unavailable", value)
 
@@ -393,14 +397,16 @@
         :param pulumi.Input[str] alias: Will be used as a filename when retrieving the public key via REST API.
         :param pulumi.Input[str] pair_name: A unique identifier for the Key Pair record.
         :param pulumi.Input[str] pair_type: Key Pair type. Supported types - GPG and RSA.
         :param pulumi.Input[str] passphrase: Passphrase will be used to decrypt the private key. Validated server side.
         :param pulumi.Input[str] private_key: Private key. PEM format will be validated.
         :param pulumi.Input[str] public_key: Public key. PEM format will be validated.
         :param pulumi.Input[bool] unavailable: Unknown usage. Returned in the json payload and cannot be set.
+               
+               Artifactory REST API call Get Key Pair doesn't return keys `private_key` and `passphrase`, but consumes these keys in the POST call.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _KeypairState.__new__(_KeypairState)
 
         __props__.__dict__["alias"] = alias
         __props__.__dict__["pair_name"] = pair_name
@@ -460,10 +466,12 @@
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter
     def unavailable(self) -> pulumi.Output[bool]:
         """
         Unknown usage. Returned in the json payload and cannot be set.
+
+        Artifactory REST API call Get Key Pair doesn't return keys `private_key` and `passphrase`, but consumes these keys in the POST call.
         """
         return pulumi.get(self, "unavailable")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/ldap_group_setting.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/ldap_group_setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,42 +15,43 @@
 class LdapGroupSettingArgs:
     def __init__(__self__, *,
                  description_attribute: pulumi.Input[str],
                  filter: pulumi.Input[str],
                  group_member_attribute: pulumi.Input[str],
                  group_name_attribute: pulumi.Input[str],
                  ldap_setting_key: pulumi.Input[str],
-                 name: pulumi.Input[str],
                  strategy: pulumi.Input[str],
                  group_base_dn: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  sub_tree: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a LdapGroupSetting resource.
         :param pulumi.Input[str] description_attribute: An attribute on the group entry which denoting the group description. Used when importing groups.
         :param pulumi.Input[str] filter: The LDAP filter used to search for group entries. Used for importing groups.
         :param pulumi.Input[str] group_member_attribute: A multi-value attribute on the group entry containing user DNs or IDs of the group members (e.g., uniqueMember,member).
         :param pulumi.Input[str] group_name_attribute: Attribute on the group entry denoting the group name. Used when importing groups.
         :param pulumi.Input[str] ldap_setting_key: The LDAP setting key you want to use for group retrieval. The value for this field corresponds to 'enabledLdap' field of the ldap group setting XML block of system configuration.
-        :param pulumi.Input[str] name: Ldap group setting name.
         :param pulumi.Input[str] strategy: The JFrog Platform Deployment (JPD) supports three ways of mapping groups to LDAP schemas:
                - STATIC: Group objects are aware of their members, however, the users are not aware of the groups they belong to. Each group object such as groupOfNames or groupOfUniqueNames holds its respective member attributes, typically member or uniqueMember, which is a user DN.
                - DYNAMIC: User objects are aware of what groups they belong to, but the group objects are not aware of their members. Each user object contains a custom attribute, such as group, that holds the group DNs or group names of which the user is a member.
                - HIERARCHICAL: The user's DN is indicative of the groups the user belongs to by using group names as part of user DN hierarchy. Each user DN contains a list of ou's or custom attributes that make up the group association. For example, uid=user1,ou=developers,ou=uk,dc=jfrog,dc=org indicates that user1 belongs to two groups: uk and developers.
         :param pulumi.Input[str] group_base_dn: A search base for group entry DNs, relative to the DN on the LDAP server’s URL (and not relative to the LDAP Setting’s “Search Base”). Used when importing groups.
+        :param pulumi.Input[str] name: Ldap group setting name.
         :param pulumi.Input[bool] sub_tree: When set, enables deep search through the sub-tree of the LDAP URL + Search Base. True by default.
         """
         pulumi.set(__self__, "description_attribute", description_attribute)
         pulumi.set(__self__, "filter", filter)
         pulumi.set(__self__, "group_member_attribute", group_member_attribute)
         pulumi.set(__self__, "group_name_attribute", group_name_attribute)
         pulumi.set(__self__, "ldap_setting_key", ldap_setting_key)
-        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "strategy", strategy)
         if group_base_dn is not None:
             pulumi.set(__self__, "group_base_dn", group_base_dn)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if sub_tree is not None:
             pulumi.set(__self__, "sub_tree", sub_tree)
 
     @property
     @pulumi.getter(name="descriptionAttribute")
     def description_attribute(self) -> pulumi.Input[str]:
         """
@@ -108,26 +109,14 @@
 
     @ldap_setting_key.setter
     def ldap_setting_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "ldap_setting_key", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Ldap group setting name.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def strategy(self) -> pulumi.Input[str]:
         """
         The JFrog Platform Deployment (JPD) supports three ways of mapping groups to LDAP schemas:
         - STATIC: Group objects are aware of their members, however, the users are not aware of the groups they belong to. Each group object such as groupOfNames or groupOfUniqueNames holds its respective member attributes, typically member or uniqueMember, which is a user DN.
         - DYNAMIC: User objects are aware of what groups they belong to, but the group objects are not aware of their members. Each user object contains a custom attribute, such as group, that holds the group DNs or group names of which the user is a member.
         - HIERARCHICAL: The user's DN is indicative of the groups the user belongs to by using group names as part of user DN hierarchy. Each user DN contains a list of ou's or custom attributes that make up the group association. For example, uid=user1,ou=developers,ou=uk,dc=jfrog,dc=org indicates that user1 belongs to two groups: uk and developers.
         """
@@ -146,14 +135,26 @@
         return pulumi.get(self, "group_base_dn")
 
     @group_base_dn.setter
     def group_base_dn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_base_dn", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Ldap group setting name.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="subTree")
     def sub_tree(self) -> Optional[pulumi.Input[bool]]:
         """
         When set, enables deep search through the sub-tree of the LDAP URL + Search Base. True by default.
         """
         return pulumi.get(self, "sub_tree")
 
@@ -353,15 +354,14 @@
         ldap_group_name = artifactory.LdapGroupSetting("ldapGroupName",
             description_attribute="description",
             filter="(objectClass=groupOfNames)",
             group_base_dn="",
             group_member_attribute="uniqueMember",
             group_name_attribute="cn",
             ldap_setting_key="ldap_name",
-            name="ldap_group_name",
             strategy="STATIC",
             sub_tree=True)
         ```
         Note: `Name` argument has to match to the resource name.\\
         Reference Link: [JFrog LDAP](https://www.jfrog.com/confluence/display/JFROG/LDAP)
 
         ## Import
@@ -411,15 +411,14 @@
         ldap_group_name = artifactory.LdapGroupSetting("ldapGroupName",
             description_attribute="description",
             filter="(objectClass=groupOfNames)",
             group_base_dn="",
             group_member_attribute="uniqueMember",
             group_name_attribute="cn",
             ldap_setting_key="ldap_name",
-            name="ldap_group_name",
             strategy="STATIC",
             sub_tree=True)
         ```
         Note: `Name` argument has to match to the resource name.\\
         Reference Link: [JFrog LDAP](https://www.jfrog.com/confluence/display/JFROG/LDAP)
 
         ## Import
@@ -475,16 +474,14 @@
             __props__.__dict__["group_member_attribute"] = group_member_attribute
             if group_name_attribute is None and not opts.urn:
                 raise TypeError("Missing required property 'group_name_attribute'")
             __props__.__dict__["group_name_attribute"] = group_name_attribute
             if ldap_setting_key is None and not opts.urn:
                 raise TypeError("Missing required property 'ldap_setting_key'")
             __props__.__dict__["ldap_setting_key"] = ldap_setting_key
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if strategy is None and not opts.urn:
                 raise TypeError("Missing required property 'strategy'")
             __props__.__dict__["strategy"] = strategy
             __props__.__dict__["sub_tree"] = sub_tree
         super(LdapGroupSetting, __self__).__init__(
             'artifactory:index/ldapGroupSetting:LdapGroupSetting',
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/ldap_setting.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/ldap_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_cargo_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_cocoapods_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_gitltfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_opkg_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_pub_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_repository_multi_replication.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_repository_multi_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_repository_single_replication.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_repository_single_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_terraform_backend_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_terraform_backend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_terraform_module_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_terraform_provider_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/local_vagrant_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/managed_user.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/unmanaged_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,49 +5,51 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ManagedUserArgs', 'ManagedUser']
+__all__ = ['UnmanagedUserArgs', 'UnmanagedUser']
 
 @pulumi.input_type
-class ManagedUserArgs:
+class UnmanagedUserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 password: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a ManagedUser resource.
+        The set of arguments for constructing a UnmanagedUser resource.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[str] name: Username for user.
+        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         pulumi.set(__self__, "email", email)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "password", password)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
         """
@@ -57,38 +59,14 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Username for user.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def password(self) -> pulumi.Input[str]:
-        """
-        Password for the user.
-        """
-        return pulumi.get(self, "password")
-
-    @password.setter
-    def password(self, value: pulumi.Input[str]):
-        pulumi.set(self, "password", value)
-
-    @property
-    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
@@ -128,46 +106,70 @@
         return pulumi.get(self, "internal_password_disabled")
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Username for user.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
+        """
+        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
+
+    @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
         When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
 @pulumi.input_type
-class _ManagedUserState:
+class _UnmanagedUserState:
     def __init__(__self__, *,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering ManagedUser resources.
+        Input properties used for looking up and filtering UnmanagedUser resources.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user.
+        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if email is not None:
@@ -255,15 +257,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the user.
+        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -276,104 +278,124 @@
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
-class ManagedUser(pulumi.CustomResource):
+class UnmanagedUser(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
+        Provides an Artifactory unmanaged user resource. This can be used to create and manage Artifactory users.
+        The password is a required field by the [Artifactory API](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateorReplaceUser), but we made it optional in this resource to accommodate the scenario where the password is not needed and will be reset by the actual user later.\\
+        When the optional attribute `password` is omitted, a random password is generated according to current Artifactory password policy.
+
+        > The generated password won't be stored in the TF state and can not be recovered. The user must reset the password to be able to log in. An admin can always generate the access key for the user as well. The password change won't trigger state drift.
+
+        > This resource is an alias for `User` resource, it is identical and was added for clarity and compatibility purposes. We don't recommend to use this resource unless there is a specific use case for it. Recommended resource is `ManagedUser`.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         # Create a new Artifactory user called terraform
-        test_user = artifactory.ManagedUser("test-user",
+        test_user = artifactory.UnmanagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
-            name="terraform",
             password="my super secret password")
         ```
+        ## Managing groups relationship
+
+        See our recommendation on how to manage user-group relationship.
 
         ## Import
 
         Users can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
+         $ pulumi import artifactory:index/unmanagedUser:UnmanagedUser test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user.
+        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ManagedUserArgs,
+                 args: UnmanagedUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides an Artifactory unmanaged user resource. This can be used to create and manage Artifactory users.
+        The password is a required field by the [Artifactory API](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-CreateorReplaceUser), but we made it optional in this resource to accommodate the scenario where the password is not needed and will be reset by the actual user later.\\
+        When the optional attribute `password` is omitted, a random password is generated according to current Artifactory password policy.
+
+        > The generated password won't be stored in the TF state and can not be recovered. The user must reset the password to be able to log in. An admin can always generate the access key for the user as well. The password change won't trigger state drift.
+
+        > This resource is an alias for `User` resource, it is identical and was added for clarity and compatibility purposes. We don't recommend to use this resource unless there is a specific use case for it. Recommended resource is `ManagedUser`.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         # Create a new Artifactory user called terraform
-        test_user = artifactory.ManagedUser("test-user",
+        test_user = artifactory.UnmanagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
                 "logged-in-users",
                 "readers",
             ],
-            name="terraform",
             password="my super secret password")
         ```
+        ## Managing groups relationship
+
+        See our recommendation on how to manage user-group relationship.
 
         ## Import
 
         Users can be imported using their name, e.g.
 
         ```sh
-         $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
+         $ pulumi import artifactory:index/unmanagedUser:UnmanagedUser test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
-        :param ManagedUserArgs args: The arguments to use to populate this resource's properties.
+        :param UnmanagedUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ManagedUserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UnmanagedUserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -389,34 +411,30 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ManagedUserArgs.__new__(ManagedUserArgs)
+            __props__ = UnmanagedUserArgs.__new__(UnmanagedUserArgs)
 
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
-            if password is None and not opts.urn:
-                raise TypeError("Missing required property 'password'")
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(ManagedUser, __self__).__init__(
-            'artifactory:index/managedUser:ManagedUser',
+        super(UnmanagedUser, __self__).__init__(
+            'artifactory:index/unmanagedUser:UnmanagedUser',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -424,44 +442,44 @@
             admin: Optional[pulumi.Input[bool]] = None,
             disable_ui_access: Optional[pulumi.Input[bool]] = None,
             email: Optional[pulumi.Input[str]] = None,
             groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             internal_password_disabled: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             password: Optional[pulumi.Input[str]] = None,
-            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'ManagedUser':
+            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'UnmanagedUser':
         """
-        Get an existing ManagedUser resource's state with the given name, id, and optional extra
+        Get an existing UnmanagedUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
         :param pulumi.Input[str] email: Email for user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
         :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user.
+        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ManagedUserState.__new__(_ManagedUserState)
+        __props__ = _UnmanagedUserState.__new__(_UnmanagedUserState)
 
         __props__.__dict__["admin"] = admin
         __props__.__dict__["disable_ui_access"] = disable_ui_access
         __props__.__dict__["email"] = email
         __props__.__dict__["groups"] = groups
         __props__.__dict__["internal_password_disabled"] = internal_password_disabled
         __props__.__dict__["name"] = name
         __props__.__dict__["password"] = password
         __props__.__dict__["profile_updatable"] = profile_updatable
-        return ManagedUser(resource_name, opts=opts, __props__=__props__)
+        return UnmanagedUser(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def admin(self) -> pulumi.Output[Optional[bool]]:
         """
         When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
         """
@@ -505,17 +523,17 @@
         """
         Username for user.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def password(self) -> pulumi.Output[str]:
+    def password(self) -> pulumi.Output[Optional[str]]:
         """
-        Password for the user.
+        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/oauth_settings.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/oauth_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             persist_users=True)
         ```
 
         ## Import
 
         Current OAuth SSO settings can be imported using `oauth_settings` as the `ID`. If the resource is being imported, there will be a state drift, because `client_secret` can't be known. There are two options on how to approach this:
 
-        1) Don't set `client_secret` initially, import, then update the config with actual secret; 2) Accept that there is a drift initially and run `terraform apply` twice;
+        1) Don't set `client_secret` initially, import, then update the config with actual secret; 2) Accept that there is a drift initially and run `pulumi up` twice;
 
         ```sh
          $ pulumi import artifactory:index/oauthSettings:OauthSettings oauth oauth_settings
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -249,15 +249,15 @@
             persist_users=True)
         ```
 
         ## Import
 
         Current OAuth SSO settings can be imported using `oauth_settings` as the `ID`. If the resource is being imported, there will be a state drift, because `client_secret` can't be known. There are two options on how to approach this:
 
-        1) Don't set `client_secret` initially, import, then update the config with actual secret; 2) Accept that there is a drift initially and run `terraform apply` twice;
+        1) Don't set `client_secret` initially, import, then update the config with actual secret; 2) Accept that there is a drift initially and run `pulumi up` twice;
 
         ```sh
          $ pulumi import artifactory:index/oauthSettings:OauthSettings oauth oauth_settings
         ```
 
         :param str resource_name: The name of the resource.
         :param OauthSettingsArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/outputs.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/permission_target.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/permission_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,58 +12,59 @@
 from ._inputs import *
 
 __all__ = ['PermissionTargetArgs', 'PermissionTarget']
 
 @pulumi.input_type
 class PermissionTargetArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
                  build: Optional[pulumi.Input['PermissionTargetBuildArgs']] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  release_bundle: Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']] = None,
                  repo: Optional[pulumi.Input['PermissionTargetRepoArgs']] = None):
         """
         The set of arguments for constructing a PermissionTarget resource.
-        :param pulumi.Input[str] name: Name of permission.
         :param pulumi.Input['PermissionTargetBuildArgs'] build: As for repo but for artifactory-build-info permissions.
+        :param pulumi.Input[str] name: Name of permission.
         :param pulumi.Input['PermissionTargetReleaseBundleArgs'] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input['PermissionTargetRepoArgs'] repo: Repository permission configuration.
         """
-        pulumi.set(__self__, "name", name)
         if build is not None:
             pulumi.set(__self__, "build", build)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if release_bundle is not None:
             pulumi.set(__self__, "release_bundle", release_bundle)
         if repo is not None:
             pulumi.set(__self__, "repo", repo)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def build(self) -> Optional[pulumi.Input['PermissionTargetBuildArgs']]:
         """
         As for repo but for artifactory-build-info permissions.
         """
         return pulumi.get(self, "build")
 
     @build.setter
     def build(self, value: Optional[pulumi.Input['PermissionTargetBuildArgs']]):
         pulumi.set(self, "build", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of permission.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="releaseBundle")
     def release_bundle(self) -> Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']]:
         """
         As for repo for for release-bundles permissions.
         """
         return pulumi.get(self, "release_bundle")
 
@@ -186,15 +187,14 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
-            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -257,15 +257,15 @@
         :param pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']] repo: Repository permission configuration.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PermissionTargetArgs,
+                 args: Optional[PermissionTargetArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Artifactory permission target resource. This can be used to create and manage Artifactory permission targets.
 
         ## Example Usage
 
         ```python
@@ -283,15 +283,14 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
-            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -372,16 +371,14 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PermissionTargetArgs.__new__(PermissionTargetArgs)
 
             __props__.__dict__["build"] = build
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["release_bundle"] = release_bundle
             __props__.__dict__["repo"] = repo
         super(PermissionTarget, __self__).__init__(
             'artifactory:index/permissionTarget:PermissionTarget',
             resource_name,
             __props__,
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/permission_targets.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/permission_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,58 +12,59 @@
 from ._inputs import *
 
 __all__ = ['PermissionTargetsArgs', 'PermissionTargets']
 
 @pulumi.input_type
 class PermissionTargetsArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
                  build: Optional[pulumi.Input['PermissionTargetsBuildArgs']] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  release_bundle: Optional[pulumi.Input['PermissionTargetsReleaseBundleArgs']] = None,
                  repo: Optional[pulumi.Input['PermissionTargetsRepoArgs']] = None):
         """
         The set of arguments for constructing a PermissionTargets resource.
-        :param pulumi.Input[str] name: Name of permission.
         :param pulumi.Input['PermissionTargetsBuildArgs'] build: As for repo but for artifactory-build-info permissions.
+        :param pulumi.Input[str] name: Name of permission.
         :param pulumi.Input['PermissionTargetsReleaseBundleArgs'] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input['PermissionTargetsRepoArgs'] repo: Repository permission configuration.
         """
-        pulumi.set(__self__, "name", name)
         if build is not None:
             pulumi.set(__self__, "build", build)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if release_bundle is not None:
             pulumi.set(__self__, "release_bundle", release_bundle)
         if repo is not None:
             pulumi.set(__self__, "repo", repo)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def build(self) -> Optional[pulumi.Input['PermissionTargetsBuildArgs']]:
         """
         As for repo but for artifactory-build-info permissions.
         """
         return pulumi.get(self, "build")
 
     @build.setter
     def build(self, value: Optional[pulumi.Input['PermissionTargetsBuildArgs']]):
         pulumi.set(self, "build", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of permission.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="releaseBundle")
     def release_bundle(self) -> Optional[pulumi.Input['PermissionTargetsReleaseBundleArgs']]:
         """
         As for repo for for release-bundles permissions.
         """
         return pulumi.get(self, "release_bundle")
 
@@ -186,15 +187,14 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
-            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -257,15 +257,15 @@
         :param pulumi.Input[pulumi.InputType['PermissionTargetsReleaseBundleArgs']] release_bundle: As for repo for for release-bundles permissions.
         :param pulumi.Input[pulumi.InputType['PermissionTargetsRepoArgs']] repo: Repository permission configuration.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PermissionTargetsArgs,
+                 args: Optional[PermissionTargetsArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Artifactory permission target resource. This can be used to create and manage Artifactory permission targets.
 
         ## Example Usage
 
         ```python
@@ -283,15 +283,14 @@
                             "write",
                         ],
                     )],
                 ),
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
             ),
-            name="test-perm",
             release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
                 actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
                     users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
                 ),
@@ -372,16 +371,14 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PermissionTargetsArgs.__new__(PermissionTargetsArgs)
 
             __props__.__dict__["build"] = build
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["release_bundle"] = release_bundle
             __props__.__dict__["repo"] = repo
         super(PermissionTargets, __self__).__init__(
             'artifactory:index/permissionTargets:PermissionTargets',
             resource_name,
             __props__,
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/property_set.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/property_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,54 +12,55 @@
 from ._inputs import *
 
 __all__ = ['PropertySetArgs', 'PropertySet']
 
 @pulumi.input_type
 class PropertySetArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
                  properties: pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]],
+                 name: Optional[pulumi.Input[str]] = None,
                  visible: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a PropertySet resource.
-        :param pulumi.Input[str] name: Predefined property name.
         :param pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]] properties: A list of properties that will be part of the property set.
+        :param pulumi.Input[str] name: Predefined property name.
         :param pulumi.Input[bool] visible: Defines if the list visible and assignable to the repository or artifact. Default value is `true`.
         """
-        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "properties", properties)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if visible is not None:
             pulumi.set(__self__, "visible", visible)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Predefined property name.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def properties(self) -> pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]]:
         """
         A list of properties that will be part of the property set.
         """
         return pulumi.get(self, "properties")
 
     @properties.setter
     def properties(self, value: pulumi.Input[Sequence[pulumi.Input['PropertySetPropertyArgs']]]):
         pulumi.set(self, "properties", value)
 
     @property
     @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Predefined property name.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def visible(self) -> Optional[pulumi.Input[bool]]:
         """
         Defines if the list visible and assignable to the repository or artifact. Default value is `true`.
         """
         return pulumi.get(self, "visible")
 
     @visible.setter
@@ -142,15 +143,14 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         foo = artifactory.PropertySet("foo",
-            name="property-set1",
             properties=[
                 artifactory.PropertySetPropertyArgs(
                     closed_predefined_values=True,
                     multiple_choice=True,
                     name="set1property1",
                     predefined_values=[
                         artifactory.PropertySetPropertyPredefinedValueArgs(
@@ -212,15 +212,14 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         foo = artifactory.PropertySet("foo",
-            name="property-set1",
             properties=[
                 artifactory.PropertySetPropertyArgs(
                     closed_predefined_values=True,
                     multiple_choice=True,
                     name="set1property1",
                     predefined_values=[
                         artifactory.PropertySetPropertyPredefinedValueArgs(
@@ -283,16 +282,14 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PropertySetArgs.__new__(PropertySetArgs)
 
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if properties is None and not opts.urn:
                 raise TypeError("Missing required property 'properties'")
             __props__.__dict__["properties"] = properties
             __props__.__dict__["visible"] = visible
         super(PropertySet, __self__).__init__(
             'artifactory:index/propertySet:PropertySet',
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/provider.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                  url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] access_token: This is a access token that can be given to you by your admin under `Identity and Access`. If not set, the 'api_key'
                attribute value will be used.
         :param pulumi.Input[str] api_key: API token. Projects functionality will not work with any auth method other than access tokens
         :param pulumi.Input[bool] check_license: Toggle for pre-flight checking of Artifactory Pro and Enterprise license. Default to `true`.
+        :param pulumi.Input[str] url: Artifactory URL.
         """
         if access_token is not None:
             pulumi.set(__self__, "access_token", access_token)
         if api_key is not None:
             warnings.warn("""An upcoming version will support the option to block the usage/creation of API Keys (for admins to set on their platform).
 In September 2022, the option to block the usage/creation of API Keys will be enabled by default, with the option for admins to change it back to enable API Keys.
 In January 2023, API Keys will be deprecated all together and the option to use them will no longer be available.""", DeprecationWarning)
@@ -79,14 +80,17 @@
     @check_license.setter
     def check_license(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "check_license", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
+        """
+        Artifactory URL.
+        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
@@ -108,14 +112,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_token: This is a access token that can be given to you by your admin under `Identity and Access`. If not set, the 'api_key'
                attribute value will be used.
         :param pulumi.Input[str] api_key: API token. Projects functionality will not work with any auth method other than access tokens
         :param pulumi.Input[bool] check_license: Toggle for pre-flight checking of Artifactory Pro and Enterprise license. Default to `true`.
+        :param pulumi.Input[str] url: Artifactory URL.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -190,9 +195,12 @@
         API token. Projects functionality will not work with any auth method other than access tokens
         """
         return pulumi.get(self, "api_key")
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Output[Optional[str]]:
+        """
+        Artifactory URL.
+        """
         return pulumi.get(self, "url")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/proxy.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/pull_replication.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/pull_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/push_replication.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/push_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/release_bundle_webhook.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_cargo_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_cocoapods_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_docker_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_gitlfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_go_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_maven_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_opkg_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_p2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_pub_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_repository_replication.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_repository_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_terraform_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/remote_vcs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/replication_config.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/repository_layout.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/repository_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 
 @pulumi.input_type
 class RepositoryLayoutArgs:
     def __init__(__self__, *,
                  artifact_path_pattern: pulumi.Input[str],
                  file_integration_revision_regexp: pulumi.Input[str],
                  folder_integration_revision_regexp: pulumi.Input[str],
-                 name: pulumi.Input[str],
                  descriptor_path_pattern: Optional[pulumi.Input[str]] = None,
-                 distinctive_descriptor_path_pattern: Optional[pulumi.Input[bool]] = None):
+                 distinctive_descriptor_path_pattern: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RepositoryLayout resource.
         :param pulumi.Input[str] artifact_path_pattern: Please refer to: [Path
                Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-ModulesandPathPatternsusedbyRepositoryLayouts)
                in the Artifactory Wiki documentation.
         :param pulumi.Input[str] file_integration_revision_regexp: A regular expression matching the integration revision string appearing in a file name as part of the artifact's path.
                For example, 'SNAPSHOT|(?:(?:[0-9]{8}.[0-9]{6})-(?:[0-9]+))', in Maven. Note! Take care not to introduce any regexp
                capturing groups within this expression. If not applicable use '.*'
         :param pulumi.Input[str] folder_integration_revision_regexp: A regular expression matching the integration revision string appearing in a folder name as part of the artifact's path.
                For example, 'SNAPSHOT', in Maven. Note! Take care not to introduce any regexp capturing groups within this expression.
                If not applicable use '.*'
-        :param pulumi.Input[str] name: Layout name
         :param pulumi.Input[str] descriptor_path_pattern: Please refer to: [Descriptor Path
                Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-DescriptorPathPatterns) in
                the Artifactory Wiki documentation.
         :param pulumi.Input[bool] distinctive_descriptor_path_pattern: When set, 'descriptor_path_pattern' will be used. Default to 'false'.
+        :param pulumi.Input[str] name: Layout name
         """
         pulumi.set(__self__, "artifact_path_pattern", artifact_path_pattern)
         pulumi.set(__self__, "file_integration_revision_regexp", file_integration_revision_regexp)
         pulumi.set(__self__, "folder_integration_revision_regexp", folder_integration_revision_regexp)
-        pulumi.set(__self__, "name", name)
         if descriptor_path_pattern is not None:
             pulumi.set(__self__, "descriptor_path_pattern", descriptor_path_pattern)
         if distinctive_descriptor_path_pattern is not None:
             pulumi.set(__self__, "distinctive_descriptor_path_pattern", distinctive_descriptor_path_pattern)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="artifactPathPattern")
     def artifact_path_pattern(self) -> pulumi.Input[str]:
         """
         Please refer to: [Path
         Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-ModulesandPathPatternsusedbyRepositoryLayouts)
@@ -85,26 +86,14 @@
         return pulumi.get(self, "folder_integration_revision_regexp")
 
     @folder_integration_revision_regexp.setter
     def folder_integration_revision_regexp(self, value: pulumi.Input[str]):
         pulumi.set(self, "folder_integration_revision_regexp", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Layout name
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
     @pulumi.getter(name="descriptorPathPattern")
     def descriptor_path_pattern(self) -> Optional[pulumi.Input[str]]:
         """
         Please refer to: [Descriptor Path
         Patterns](https://www.jfrog.com/confluence/display/JFROG/Repository+Layouts#RepositoryLayouts-DescriptorPathPatterns) in
         the Artifactory Wiki documentation.
         """
@@ -122,14 +111,26 @@
         """
         return pulumi.get(self, "distinctive_descriptor_path_pattern")
 
     @distinctive_descriptor_path_pattern.setter
     def distinctive_descriptor_path_pattern(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "distinctive_descriptor_path_pattern", value)
 
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Layout name
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
 
 @pulumi.input_type
 class _RepositoryLayoutState:
     def __init__(__self__, *,
                  artifact_path_pattern: Optional[pulumi.Input[str]] = None,
                  descriptor_path_pattern: Optional[pulumi.Input[str]] = None,
                  distinctive_descriptor_path_pattern: Optional[pulumi.Input[bool]] = None,
@@ -323,16 +324,14 @@
             __props__.__dict__["distinctive_descriptor_path_pattern"] = distinctive_descriptor_path_pattern
             if file_integration_revision_regexp is None and not opts.urn:
                 raise TypeError("Missing required property 'file_integration_revision_regexp'")
             __props__.__dict__["file_integration_revision_regexp"] = file_integration_revision_regexp
             if folder_integration_revision_regexp is None and not opts.urn:
                 raise TypeError("Missing required property 'folder_integration_revision_regexp'")
             __props__.__dict__["folder_integration_revision_regexp"] = folder_integration_revision_regexp
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
         super(RepositoryLayout, __self__).__init__(
             'artifactory:index/repositoryLayout:RepositoryLayout',
             resource_name,
             __props__,
             opts)
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/saml_settings.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/saml_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/scoped_token.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/scoped_token.py`

 * *Files 11% similar despite different names*

```diff
@@ -385,14 +385,93 @@
                  expires_in: Optional[pulumi.Input[int]] = None,
                  include_reference_token: Optional[pulumi.Input[bool]] = None,
                  refreshable: Optional[pulumi.Input[bool]] = None,
                  scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Provides an Artifactory Scoped Token resource. This can be used to create and manage Artifactory Scoped Tokens.
+
+        !>Scoped Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
+        state.
+
+        ~>Token would not be saved by Artifactory if `expires_in` is less than the persistency threshold value (default to 10800 seconds) set in Access configuration. See [Persistency Threshold](https://www.jfrog.com/confluence/display/JFROG/Access+Tokens#AccessTokens-PersistencyThreshold) for details.
+
+        ## Example Usage
+
+        ### S
+        ### Create a new Artifactory scoped token for an existing user
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token = artifactory.ScopedToken("scopedToken", username="existing-user")
+        ```
+
+        **Note:** This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
+        ### Create a new Artifactory user and scoped token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        new_user = artifactory.User("newUser",
+            email="new_user@somewhere.com",
+            groups=["readers"])
+        scoped_token_user = artifactory.ScopedToken("scopedTokenUser", username=new_user.name)
+        ```
+        ### Creates a new token for groups
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token_group = artifactory.ScopedToken("scopedTokenGroup", scopes=["applied-permissions/groups:readers"])
+        ```
+        ### Create token with expiry
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token_no_expiry = artifactory.ScopedToken("scopedTokenNoExpiry",
+            expires_in=7200,
+            username="existing-user")
+        ```
+        ### Creates a refreshable token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token_refreshable = artifactory.ScopedToken("scopedTokenRefreshable",
+            refreshable=True,
+            username="existing-user")
+        ```
+        ### Creates an administrator token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        admin = artifactory.ScopedToken("admin",
+            scopes=["applied-permissions/admin"],
+            username="admin-user")
+        ```
+        ### Creates a token with an audience
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        audience = artifactory.ScopedToken("audience",
+            audiences=["jfrt@*"],
+            scopes=["applied-permissions/admin"],
+            username="admin-user")
+        ```
+        ## References
+
+        - https://www.jfrog.com/confluence/display/JFROG/Access+Tokens
+        - https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-AccessTokens
+
         ## Import
 
         Artifactory **does not** retain scoped tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: (Optional) A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to `*@*` if not set. Service ID must begin with `jfrt@`. For instructions to retrieve the Artifactory Service ID see this [documentation](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-GetServiceID).
@@ -406,14 +485,93 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ScopedTokenArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides an Artifactory Scoped Token resource. This can be used to create and manage Artifactory Scoped Tokens.
+
+        !>Scoped Tokens will be stored in the raw state as plain-text. Read more about sensitive data in
+        state.
+
+        ~>Token would not be saved by Artifactory if `expires_in` is less than the persistency threshold value (default to 10800 seconds) set in Access configuration. See [Persistency Threshold](https://www.jfrog.com/confluence/display/JFROG/Access+Tokens#AccessTokens-PersistencyThreshold) for details.
+
+        ## Example Usage
+
+        ### S
+        ### Create a new Artifactory scoped token for an existing user
+
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token = artifactory.ScopedToken("scopedToken", username="existing-user")
+        ```
+
+        **Note:** This assumes that the user `existing-user` has already been created in Artifactory by different means, i.e. manually or in a separate pulumi up.
+        ### Create a new Artifactory user and scoped token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        new_user = artifactory.User("newUser",
+            email="new_user@somewhere.com",
+            groups=["readers"])
+        scoped_token_user = artifactory.ScopedToken("scopedTokenUser", username=new_user.name)
+        ```
+        ### Creates a new token for groups
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token_group = artifactory.ScopedToken("scopedTokenGroup", scopes=["applied-permissions/groups:readers"])
+        ```
+        ### Create token with expiry
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token_no_expiry = artifactory.ScopedToken("scopedTokenNoExpiry",
+            expires_in=7200,
+            username="existing-user")
+        ```
+        ### Creates a refreshable token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        scoped_token_refreshable = artifactory.ScopedToken("scopedTokenRefreshable",
+            refreshable=True,
+            username="existing-user")
+        ```
+        ### Creates an administrator token
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        admin = artifactory.ScopedToken("admin",
+            scopes=["applied-permissions/admin"],
+            username="admin-user")
+        ```
+        ### Creates a token with an audience
+        ```python
+        import pulumi
+        import pulumi_artifactory as artifactory
+
+        audience = artifactory.ScopedToken("audience",
+            audiences=["jfrt@*"],
+            scopes=["applied-permissions/admin"],
+            username="admin-user")
+        ```
+        ## References
+
+        - https://www.jfrog.com/confluence/display/JFROG/Access+Tokens
+        - https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-AccessTokens
+
         ## Import
 
         Artifactory **does not** retain scoped tokens and cannot be imported into state.
 
         :param str resource_name: The name of the resource.
         :param ScopedTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/single_replication_config.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/single_replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/unmanaged_user.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/managed_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['UnmanagedUserArgs', 'UnmanagedUser']
+__all__ = ['ManagedUserArgs', 'ManagedUser']
 
 @pulumi.input_type
-class UnmanagedUserArgs:
+class ManagedUserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
-                 name: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a UnmanagedUser resource.
+        The set of arguments for constructing a ManagedUser resource.
         :param pulumi.Input[str] email: Email for user.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         pulumi.set(__self__, "email", email)
-        pulumi.set(__self__, "name", name)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
@@ -58,118 +59,118 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Username for user.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
-        When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
+        (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
     def admin(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "admin", value)
 
     @property
     @pulumi.getter(name="disableUiAccess")
     def disable_ui_access(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         """
         return pulumi.get(self, "disable_ui_access")
 
     @disable_ui_access.setter
     def disable_ui_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_ui_access", value)
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
+        List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter(name="internalPasswordDisabled")
     def internal_password_disabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         """
         return pulumi.get(self, "internal_password_disabled")
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
     @property
     @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Username for user.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
 @pulumi.input_type
-class _UnmanagedUserState:
+class _ManagedUserState:
     def __init__(__self__, *,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering UnmanagedUser resources.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        Input properties used for looking up and filtering ManagedUser resources.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if email is not None:
             pulumi.set(__self__, "email", email)
@@ -184,27 +185,27 @@
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
-        When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
+        (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
     def admin(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "admin", value)
 
     @property
     @pulumi.getter(name="disableUiAccess")
     def disable_ui_access(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         """
         return pulumi.get(self, "disable_ui_access")
 
     @disable_ui_access.setter
     def disable_ui_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_ui_access", value)
 
@@ -220,27 +221,27 @@
     def email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
+        List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter(name="internalPasswordDisabled")
     def internal_password_disabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         """
         return pulumi.get(self, "internal_password_disabled")
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
@@ -256,36 +257,36 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
 
-class UnmanagedUser(pulumi.CustomResource):
+class ManagedUser(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  email: Optional[pulumi.Input[str]] = None,
@@ -298,89 +299,75 @@
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        # Create a new Artifactory user called terraform
-        test_user = artifactory.UnmanagedUser("test-user",
+        test_user = artifactory.ManagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
-                "logged-in-users",
                 "readers",
+                "logged-in-users",
             ],
-            name="terraform",
             password="my super secret password")
         ```
-        ## Managing groups relationship
-
-        See our recommendation on how to manage user-group relationship.
 
         ## Import
 
-        Users can be imported using their name, e.g.
-
         ```sh
-         $ pulumi import artifactory:index/unmanagedUser:UnmanagedUser test-user myusername
+         $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: UnmanagedUserArgs,
+                 args: ManagedUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        # Create a new Artifactory user called terraform
-        test_user = artifactory.UnmanagedUser("test-user",
+        test_user = artifactory.ManagedUser("test-user",
             email="test-user@artifactory-terraform.com",
             groups=[
-                "logged-in-users",
                 "readers",
+                "logged-in-users",
             ],
-            name="terraform",
             password="my super secret password")
         ```
-        ## Managing groups relationship
-
-        See our recommendation on how to manage user-group relationship.
 
         ## Import
 
-        Users can be imported using their name, e.g.
-
         ```sh
-         $ pulumi import artifactory:index/unmanagedUser:UnmanagedUser test-user myusername
+         $ pulumi import artifactory:index/managedUser:ManagedUser test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
-        :param UnmanagedUserArgs args: The arguments to use to populate this resource's properties.
+        :param ManagedUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(UnmanagedUserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ManagedUserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -396,32 +383,30 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = UnmanagedUserArgs.__new__(UnmanagedUserArgs)
+            __props__ = ManagedUserArgs.__new__(ManagedUserArgs)
 
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(UnmanagedUser, __self__).__init__(
-            'artifactory:index/unmanagedUser:UnmanagedUser',
+        super(ManagedUser, __self__).__init__(
+            'artifactory:index/managedUser:ManagedUser',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -429,82 +414,82 @@
             admin: Optional[pulumi.Input[bool]] = None,
             disable_ui_access: Optional[pulumi.Input[bool]] = None,
             email: Optional[pulumi.Input[str]] = None,
             groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             internal_password_disabled: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             password: Optional[pulumi.Input[str]] = None,
-            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'UnmanagedUser':
+            profile_updatable: Optional[pulumi.Input[bool]] = None) -> 'ManagedUser':
         """
-        Get an existing UnmanagedUser resource's state with the given name, id, and optional extra
+        Get an existing ManagedUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _UnmanagedUserState.__new__(_UnmanagedUserState)
+        __props__ = _ManagedUserState.__new__(_ManagedUserState)
 
         __props__.__dict__["admin"] = admin
         __props__.__dict__["disable_ui_access"] = disable_ui_access
         __props__.__dict__["email"] = email
         __props__.__dict__["groups"] = groups
         __props__.__dict__["internal_password_disabled"] = internal_password_disabled
         __props__.__dict__["name"] = name
         __props__.__dict__["password"] = password
         __props__.__dict__["profile_updatable"] = profile_updatable
-        return UnmanagedUser(resource_name, opts=opts, __props__=__props__)
+        return ManagedUser(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def admin(self) -> pulumi.Output[Optional[bool]]:
+    def admin(self) -> pulumi.Output[bool]:
         """
-        When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
+        (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @property
     @pulumi.getter(name="disableUiAccess")
-    def disable_ui_access(self) -> pulumi.Output[Optional[bool]]:
+    def disable_ui_access(self) -> pulumi.Output[bool]:
         """
-        When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         """
         return pulumi.get(self, "disable_ui_access")
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Output[str]:
         """
         Email for user.
         """
         return pulumi.get(self, "email")
 
     @property
     @pulumi.getter
-    def groups(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def groups(self) -> pulumi.Output[Sequence[str]]:
         """
-        List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership is set to empty. User will not be part of default "readers" group automatically.
+        List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter(name="internalPasswordDisabled")
-    def internal_password_disabled(self) -> pulumi.Output[Optional[bool]]:
+    def internal_password_disabled(self) -> pulumi.Output[bool]:
         """
-        When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         """
         return pulumi.get(self, "internal_password_disabled")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -512,19 +497,19 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[Optional[str]]:
         """
-        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="profileUpdatable")
-    def profile_updatable(self) -> pulumi.Output[Optional[bool]]:
+    def profile_updatable(self) -> pulumi.Output[bool]:
         """
-        When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/user.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,42 +11,43 @@
 
 __all__ = ['UserArgs', 'User']
 
 @pulumi.input_type
 class UserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
-                 name: pulumi.Input[str],
                  admin: Optional[pulumi.Input[bool]] = None,
                  disable_ui_access: Optional[pulumi.Input[bool]] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a User resource.
         :param pulumi.Input[str] email: Email for user.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         pulumi.set(__self__, "email", email)
-        pulumi.set(__self__, "name", name)
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if internal_password_disabled is not None:
             pulumi.set(__self__, "internal_password_disabled", internal_password_disabled)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
@@ -58,89 +59,89 @@
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Username for user.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
-        When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
+        (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
     def admin(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "admin", value)
 
     @property
     @pulumi.getter(name="disableUiAccess")
     def disable_ui_access(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         """
         return pulumi.get(self, "disable_ui_access")
 
     @disable_ui_access.setter
     def disable_ui_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_ui_access", value)
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
+        List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter(name="internalPasswordDisabled")
     def internal_password_disabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         """
         return pulumi.get(self, "internal_password_disabled")
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
     @property
     @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Username for user.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
@@ -154,22 +155,22 @@
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  internal_password_disabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  profile_updatable: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering User resources.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         if admin is not None:
             pulumi.set(__self__, "admin", admin)
         if disable_ui_access is not None:
             pulumi.set(__self__, "disable_ui_access", disable_ui_access)
         if email is not None:
             pulumi.set(__self__, "email", email)
@@ -184,27 +185,27 @@
         if profile_updatable is not None:
             pulumi.set(__self__, "profile_updatable", profile_updatable)
 
     @property
     @pulumi.getter
     def admin(self) -> Optional[pulumi.Input[bool]]:
         """
-        When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
+        (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @admin.setter
     def admin(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "admin", value)
 
     @property
     @pulumi.getter(name="disableUiAccess")
     def disable_ui_access(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         """
         return pulumi.get(self, "disable_ui_access")
 
     @disable_ui_access.setter
     def disable_ui_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_ui_access", value)
 
@@ -220,27 +221,27 @@
     def email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "email", value)
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
+        List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter(name="internalPasswordDisabled")
     def internal_password_disabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         """
         return pulumi.get(self, "internal_password_disabled")
 
     @internal_password_disabled.setter
     def internal_password_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal_password_disabled", value)
 
@@ -256,27 +257,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter(name="profileUpdatable")
     def profile_updatable(self) -> Optional[pulumi.Input[bool]]:
         """
-        When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
 
     @profile_updatable.setter
     def profile_updatable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "profile_updatable", value)
 
@@ -304,46 +305,46 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        # Create a new Artifactory user called terraform
         test_user = artifactory.User("test-user",
+            admin=False,
+            disable_ui_access=False,
             email="test-user@artifactory-terraform.com",
             groups=[
-                "logged-in-users",
                 "readers",
+                "logged-in-users",
             ],
-            name="terraform",
-            password="my super secret password")
+            internal_password_disabled=False,
+            password="my super secret password",
+            profile_updatable=True)
         ```
         ## Managing groups relationship
 
         See our recommendation on how to manage user-group relationship.
 
         ## Import
 
-        Users can be imported using their name, e.g.
-
         ```sh
          $ pulumi import artifactory:index/user:User test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -356,32 +357,32 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
-        # Create a new Artifactory user called terraform
         test_user = artifactory.User("test-user",
+            admin=False,
+            disable_ui_access=False,
             email="test-user@artifactory-terraform.com",
             groups=[
-                "logged-in-users",
                 "readers",
+                "logged-in-users",
             ],
-            name="terraform",
-            password="my super secret password")
+            internal_password_disabled=False,
+            password="my super secret password",
+            profile_updatable=True)
         ```
         ## Managing groups relationship
 
         See our recommendation on how to manage user-group relationship.
 
         ## Import
 
-        Users can be imported using their name, e.g.
-
         ```sh
          $ pulumi import artifactory:index/user:User test-user myusername
         ```
 
         :param str resource_name: The name of the resource.
         :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -417,16 +418,14 @@
             __props__.__dict__["admin"] = admin
             __props__.__dict__["disable_ui_access"] = disable_ui_access
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
             __props__.__dict__["groups"] = groups
             __props__.__dict__["internal_password_disabled"] = internal_password_disabled
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["profile_updatable"] = profile_updatable
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(User, __self__).__init__(
             'artifactory:index/user:User',
@@ -449,22 +448,22 @@
         """
         Get an existing User resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] admin: When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
-        :param pulumi.Input[bool] disable_ui_access: When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        :param pulumi.Input[bool] admin: (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
+        :param pulumi.Input[bool] disable_ui_access: (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         :param pulumi.Input[str] email: Email for user.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
-        :param pulumi.Input[bool] internal_password_disabled: When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
+        :param pulumi.Input[bool] internal_password_disabled: (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         :param pulumi.Input[str] name: Username for user.
-        :param pulumi.Input[str] password: Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
-        :param pulumi.Input[bool] profile_updatable: When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        :param pulumi.Input[str] password: (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
+        :param pulumi.Input[bool] profile_updatable: (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UserState.__new__(_UserState)
 
         __props__.__dict__["admin"] = admin
         __props__.__dict__["disable_ui_access"] = disable_ui_access
@@ -474,49 +473,49 @@
         __props__.__dict__["name"] = name
         __props__.__dict__["password"] = password
         __props__.__dict__["profile_updatable"] = profile_updatable
         return User(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def admin(self) -> pulumi.Output[Optional[bool]]:
+    def admin(self) -> pulumi.Output[bool]:
         """
-        When enabled, this user is an administrator with all the ensuing privileges. Default value is `false`.
+        (Optional, Default: false) When enabled, this user is an administrator with all the ensuing privileges.
         """
         return pulumi.get(self, "admin")
 
     @property
     @pulumi.getter(name="disableUiAccess")
-    def disable_ui_access(self) -> pulumi.Output[Optional[bool]]:
+    def disable_ui_access(self) -> pulumi.Output[bool]:
         """
-        When set, this user can only access Artifactory through the REST API. This option cannot be set if the user has Admin privileges. Default value is `true`.
+        (Optional, Default: true) When enabled, this user can only access the system through the REST API. This option cannot be set if the user has Admin privileges.
         """
         return pulumi.get(self, "disable_ui_access")
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Output[str]:
         """
         Email for user.
         """
         return pulumi.get(self, "email")
 
     @property
     @pulumi.getter
-    def groups(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def groups(self) -> pulumi.Output[Sequence[str]]:
         """
-        List of groups this user is a part of. **Notes:** If this attribute is not specified then user's group membership set to empty. User will not be part of default "readers" group automatically.
+        List of groups this user is a part of. If no groups set, `readers` group will be added by default. If other groups are assigned, `readers` must be added to the list manually to avoid state drift.
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter(name="internalPasswordDisabled")
-    def internal_password_disabled(self) -> pulumi.Output[Optional[bool]]:
+    def internal_password_disabled(self) -> pulumi.Output[bool]:
         """
-        When set, disables the fallback of using an internal password when external authentication (such as LDAP) is enabled.
+        (Optional, Default: false) When enabled, disables the fallback mechanism for using an internal password when external authentication (such as LDAP) is enabled.
         """
         return pulumi.get(self, "internal_password_disabled")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -524,19 +523,19 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[Optional[str]]:
         """
-        Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters.
+        (Optional, Sensitive) Password for the user. When omitted, a random password is generated using the following password policy: 12 characters with 1 digit, 1 symbol, with upper and lower case letters
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="profileUpdatable")
-    def profile_updatable(self) -> pulumi.Output[Optional[bool]]:
+    def profile_updatable(self) -> pulumi.Output[bool]:
         """
-        When set, this user can update his profile details (except for the password. Only an administrator can update the password). Default value is `true`.
+        (Optional, Default: true) When enabled, this user can update their profile details (except for the password. Only an administrator can update the password). There may be cases in which you want to leave this unset to prevent users from updating their profile. For example, a departmental user with a single password shared between all department members.
         """
         return pulumi.get(self, "profile_updatable")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_alpine_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_bower_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_chef_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_composer_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_conan_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_conda_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_cran_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_debian_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_docker_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_gems_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_generic_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_gitlfs_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_gradle_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_helm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_ivy_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_npm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_nuget_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_p2_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_pub_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_puppet_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_pypi_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_rpm_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_rpm_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[str] secondary_keypair_ref: The secondary GPG key to be used to sign packages.
+        :param pulumi.Input[str] secondary_keypair_ref: Secondary keypair used to sign artifacts.
         """
         pulumi.set(__self__, "key", key)
         if artifactory_requests_can_retrieve_remote_artifacts is not None:
             pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
         if default_deployment_repo is not None:
             pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
@@ -229,15 +229,15 @@
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
     @property
     @pulumi.getter(name="secondaryKeypairRef")
     def secondary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        The secondary GPG key to be used to sign packages.
+        Secondary keypair used to sign artifacts.
         """
         return pulumi.get(self, "secondary_keypair_ref")
 
     @secondary_keypair_ref.setter
     def secondary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secondary_keypair_ref", value)
 
@@ -277,15 +277,15 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[str] secondary_keypair_ref: The secondary GPG key to be used to sign packages.
+        :param pulumi.Input[str] secondary_keypair_ref: Secondary keypair used to sign artifacts.
         """
         if artifactory_requests_can_retrieve_remote_artifacts is not None:
             pulumi.set(__self__, "artifactory_requests_can_retrieve_remote_artifacts", artifactory_requests_can_retrieve_remote_artifacts)
         if default_deployment_repo is not None:
             pulumi.set(__self__, "default_deployment_repo", default_deployment_repo)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -473,15 +473,15 @@
     def repositories(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "repositories", value)
 
     @property
     @pulumi.getter(name="secondaryKeypairRef")
     def secondary_keypair_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        The secondary GPG key to be used to sign packages.
+        Secondary keypair used to sign artifacts.
         """
         return pulumi.get(self, "secondary_keypair_ref")
 
     @secondary_keypair_ref.setter
     def secondary_keypair_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secondary_keypair_ref", value)
 
@@ -563,15 +563,15 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[str] secondary_keypair_ref: The secondary GPG key to be used to sign packages.
+        :param pulumi.Input[str] secondary_keypair_ref: Secondary keypair used to sign artifacts.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VirtualRpmRepositoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -715,15 +715,15 @@
                Artifactory 7.53.1, up to 2 values ("DEV" and "PROD") are allowed. From 7.53.1 onward, only one value is allowed. The
                attribute should only be used if the repository is already assigned to the existing project. If not, the attribute will
                be ignored by Artifactory, but will remain in the Terraform state, which will create state drift during the update.
         :param pulumi.Input[str] project_key: Project key for assigning this repository to. Must be 2 - 20 lowercase alphanumeric and hyphen characters. When
                assigning repository to a project, repository key must be prefixed with project key, separated by a dash.
         :param pulumi.Input[str] repo_layout_ref: Repository layout key for the local repository
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: The effective list of actual repositories included in this virtual repository.
-        :param pulumi.Input[str] secondary_keypair_ref: The secondary GPG key to be used to sign packages.
+        :param pulumi.Input[str] secondary_keypair_ref: Secondary keypair used to sign artifacts.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VirtualRpmRepositoryState.__new__(_VirtualRpmRepositoryState)
 
         __props__.__dict__["artifactory_requests_can_retrieve_remote_artifacts"] = artifactory_requests_can_retrieve_remote_artifacts
         __props__.__dict__["default_deployment_repo"] = default_deployment_repo
@@ -850,11 +850,11 @@
         """
         return pulumi.get(self, "repositories")
 
     @property
     @pulumi.getter(name="secondaryKeypairRef")
     def secondary_keypair_ref(self) -> pulumi.Output[Optional[str]]:
         """
-        The secondary GPG key to be used to sign packages.
+        Secondary keypair used to sign artifacts.
         """
         return pulumi.get(self, "secondary_keypair_ref")
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_sbt_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_swift_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory/virtual_terraform_repository.py` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory/virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/PKG-INFO` & `pulumi_artifactory-3.5.0a1684341828/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-artifactory
-Version: 3.5.0a1684214270
+Name: pulumi_artifactory
+Version: 3.5.0a1684341828
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/pulumi_artifactory.egg-info/SOURCES.txt` & `pulumi_artifactory-3.5.0a1684341828/pulumi_artifactory.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pulumi_artifactory/artifact_property_webhook.py
 pulumi_artifactory/artifact_webhook.py
 pulumi_artifactory/artifactory_release_bundle_webhook.py
 pulumi_artifactory/backup.py
 pulumi_artifactory/build_webhook.py
 pulumi_artifactory/certificate.py
 pulumi_artifactory/debian_repository.py
+pulumi_artifactory/distribution_public_key.py
 pulumi_artifactory/distribution_webhook.py
 pulumi_artifactory/docker_v1_repository.py
 pulumi_artifactory/docker_v2_repository.py
 pulumi_artifactory/docker_webhook.py
 pulumi_artifactory/federated_alpine_repository.py
 pulumi_artifactory/federated_bower_repository.py
 pulumi_artifactory/federated_cargo_repository.py
```

### Comparing `pulumi_artifactory-3.5.0a1684214270/setup.py` & `pulumi_artifactory-3.5.0a1684341828/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.5.0a1684214270"
-PLUGIN_VERSION = "3.5.0-alpha.1684214270+54534913"
+VERSION = "3.5.0a1684341828"
+PLUGIN_VERSION = "3.5.0-alpha.1684341828+1bf77a59"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'artifactory', PLUGIN_VERSION])
         except OSError as error:
```

