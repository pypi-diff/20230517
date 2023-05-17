# Comparing `tmp/apicurio_registry_python_sdk_preview-2.4.2.tar.gz` & `tmp/apicurio_registry_python_sdk_preview-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.2.tar", max compression
+gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.3.tar", max compression
```

## Comparing `apicurio_registry_python_sdk_preview-2.4.2.tar` & `apicurio_registry_python_sdk_preview-2.4.3.tar`

### file list

```diff
@@ -1,5 +1,86 @@
--rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurio_registry_python_sdk_preview-2.4.2/README.md
--rw-r--r--   0        0        0     2207 2023-05-16 11:09:16.402810 apicurio_registry_python_sdk_preview-2.4.2/kiota-gen.py
--rw-r--r--   0        0        0     1041 2023-05-16 11:21:23.307748 apicurio_registry_python_sdk_preview-2.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurio_registry_python_sdk_preview-2.4.2/python_sdk/__init__.py
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0      368 2023-05-17 11:57:07.580710 apicurio_registry_python_sdk_preview-2.4.3/README.md
+-rw-r--r--   0        0        0     2224 2023-05-17 11:57:07.580853 apicurio_registry_python_sdk_preview-2.4.3/kiota-gen.py
+-rw-r--r--   0        0        0     1133 2023-05-17 11:59:12.179901 apicurio_registry_python_sdk_preview-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 11:57:07.581617 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/__init__.py
+-rw-r--r--   0        0        0     6316 2023-05-17 11:58:03.965323 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/admin_request_builder.py
+-rw-r--r--   0        0        0     4141 2023-05-17 11:58:03.988283 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/artifact_types/artifact_types_request_builder.py
+-rw-r--r--   0        0        0     2509 2023-05-17 11:58:03.969731 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/config_request_builder.py
+-rw-r--r--   0        0        0     9895 2023-05-17 11:58:03.973749 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
+-rw-r--r--   0        0        0     4230 2023-05-17 11:58:03.971418 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/properties/properties_request_builder.py
+-rw-r--r--   0        0        0     4497 2023-05-17 11:58:03.991072 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/export/export_request_builder.py
+-rw-r--r--   0        0        0     4016 2023-05-17 11:58:03.989723 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/import_/import_request_builder.py
+-rw-r--r--   0        0        0     9210 2023-05-17 11:58:03.986822 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/loggers/item/with_logger_item_request_builder.py
+-rw-r--r--   0        0        0     3970 2023-05-17 11:58:03.984865 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/loggers/loggers_request_builder.py
+-rw-r--r--   0        0        0     9490 2023-05-17 11:58:03.983360 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
+-rw-r--r--   0        0        0     6823 2023-05-17 11:58:03.975845 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/role_mappings/role_mappings_request_builder.py
+-rw-r--r--   0        0        0     9847 2023-05-17 11:58:03.968546 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0     9029 2023-05-17 11:58:03.966798 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     7675 2023-05-17 11:58:03.895749 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/groups_request_builder.py
+-rw-r--r--   0        0        0    17933 2023-05-17 11:58:03.893278 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0    12567 2023-05-17 11:58:03.886788 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6977 2023-05-17 11:58:03.878777 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
+-rw-r--r--   0        0        0    11150 2023-05-17 11:58:03.890714 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0    10297 2023-05-17 11:58:03.889210 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     4942 2023-05-17 11:58:03.887760 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/state/state_request_builder.py
+-rw-r--r--   0        0        0     6104 2023-05-17 11:58:03.891646 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/test/test_request_builder.py
+-rw-r--r--   0        0        0    10548 2023-05-17 11:58:03.881391 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6008 2023-05-17 11:58:03.879938 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4767 2023-05-17 11:58:03.883765 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
+-rw-r--r--   0        0        0    10171 2023-05-17 11:58:03.882732 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
+-rw-r--r--   0        0        0     9632 2023-05-17 11:58:03.885032 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
+-rw-r--r--   0        0        0    16487 2023-05-17 11:58:03.877530 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
+-rw-r--r--   0        0        0     7662 2023-05-17 11:58:03.894579 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/with_group_item_request_builder.py
+-rw-r--r--   0        0        0     1299 2023-05-17 11:58:03.961423 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/content_hashes_request_builder.py
+-rw-r--r--   0        0        0     4122 2023-05-17 11:58:03.960005 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4828 2023-05-17 11:58:03.960895 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
+-rw-r--r--   0        0        0     1287 2023-05-17 11:58:03.957929 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/content_ids_request_builder.py
+-rw-r--r--   0        0        0     4108 2023-05-17 11:58:03.956443 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4820 2023-05-17 11:58:03.957362 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/item/with_content_item_request_builder.py
+-rw-r--r--   0        0        0     1283 2023-05-17 11:58:03.962038 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/global_ids_request_builder.py
+-rw-r--r--   0        0        0     4807 2023-05-17 11:58:03.963054 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     5362 2023-05-17 11:58:03.964005 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/item/with_global_item_request_builder.py
+-rw-r--r--   0        0        0     4913 2023-05-17 11:58:03.958932 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/ids_request_builder.py
+-rw-r--r--   0        0        0     1160 2023-05-17 11:58:04.053648 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/kiota-lock.json
+-rw-r--r--   0        0        0     4573 2023-05-17 11:58:03.943710 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_content.py
+-rw-r--r--   0        0        0    15041 2023-05-17 11:58:03.908896 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_meta_data.py
+-rw-r--r--   0        0        0     3253 2023-05-17 11:58:03.939926 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_owner.py
+-rw-r--r--   0        0        0     5461 2023-05-17 11:58:03.903898 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_reference.py
+-rw-r--r--   0        0        0     4781 2023-05-17 11:58:03.950660 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_search_results.py
+-rw-r--r--   0        0        0      134 2023-05-17 11:58:03.918704 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_state.py
+-rw-r--r--   0        0        0     3192 2023-05-17 11:58:03.919539 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_type_info.py
+-rw-r--r--   0        0        0     5921 2023-05-17 11:58:03.953433 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/configuration_property.py
+-rw-r--r--   0        0        0     4961 2023-05-17 11:58:03.905804 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/create_group_meta_data.py
+-rw-r--r--   0        0        0     3989 2023-05-17 11:58:03.912876 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/download_ref.py
+-rw-r--r--   0        0        0     5719 2023-05-17 11:58:03.928803 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/editable_meta_data.py
+-rw-r--r--   0        0        0     5777 2023-05-17 11:58:03.945068 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/error.py
+-rw-r--r--   0        0        0     8023 2023-05-17 11:58:03.948338 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/group_meta_data.py
+-rw-r--r--   0        0        0     4661 2023-05-17 11:58:03.902712 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/group_search_results.py
+-rw-r--r--   0        0        0    14563 2023-05-17 11:58:03.923761 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/limits.py
+-rw-r--r--   0        0        0     2597 2023-05-17 11:58:03.933727 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/log_configuration.py
+-rw-r--r--   0        0        0      281 2023-05-17 11:58:03.919936 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/log_level.py
+-rw-r--r--   0        0        0     3217 2023-05-17 11:58:03.913704 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/named_log_configuration.py
+-rw-r--r--   0        0        0     2605 2023-05-17 11:58:03.909685 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/properties.py
+-rw-r--r--   0        0        0     4978 2023-05-17 11:58:03.935563 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/role_mapping.py
+-rw-r--r--   0        0        0      125 2023-05-17 11:58:03.910824 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/role_type.py
+-rw-r--r--   0        0        0     3964 2023-05-17 11:58:03.936706 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule.py
+-rw-r--r--   0        0        0      110 2023-05-17 11:58:03.924553 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule_type.py
+-rw-r--r--   0        0        0     2301 2023-05-17 11:58:03.918175 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule_violation_error.py
+-rw-r--r--   0        0        0    11035 2023-05-17 11:58:03.932367 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_artifact.py
+-rw-r--r--   0        0        0     7087 2023-05-17 11:58:03.938505 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_group.py
+-rw-r--r--   0        0        0    12237 2023-05-17 11:58:03.942119 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_version.py
+-rw-r--r--   0        0        0     5359 2023-05-17 11:58:03.926428 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/system_info.py
+-rw-r--r--   0        0        0     3263 2023-05-17 11:58:03.949597 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_configuration_property.py
+-rw-r--r--   0        0        0     3322 2023-05-17 11:58:03.904847 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_role.py
+-rw-r--r--   0        0        0     3712 2023-05-17 11:58:03.946103 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_state.py
+-rw-r--r--   0        0        0     6096 2023-05-17 11:58:03.951886 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/user_info.py
+-rw-r--r--   0        0        0    12512 2023-05-17 11:58:03.917536 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/version_meta_data.py
+-rw-r--r--   0        0        0     4748 2023-05-17 11:58:03.911864 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/version_search_results.py
+-rw-r--r--   0        0        0     4683 2023-05-17 11:58:03.955217 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/registry_client.py
+-rw-r--r--   0        0        0    10097 2023-05-17 11:58:03.871355 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/search/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0     1669 2023-05-17 11:58:03.871996 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/search/search_request_builder.py
+-rw-r--r--   0        0        0     3945 2023-05-17 11:58:03.868581 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/info/info_request_builder.py
+-rw-r--r--   0        0        0     3913 2023-05-17 11:58:03.869805 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/limits/limits_request_builder.py
+-rw-r--r--   0        0        0     1973 2023-05-17 11:58:03.858339 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/system_request_builder.py
+-rw-r--r--   0        0        0     3793 2023-05-17 11:58:03.873399 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/users/me/me_request_builder.py
+-rw-r--r--   0        0        0     1609 2023-05-17 11:58:03.872606 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/users/users_request_builder.py
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.3/PKG-INFO
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.2/kiota-gen.py` & `apicurio_registry_python_sdk_preview-2.4.3/kiota-gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import zipfile
 import io
 import os
-import shutil
 import stat
 import sys
 import platform
+from pathlib import Path
 
 KIOTA_VERSION = "1.1.3"
 
 KIOTA_OS_NAMES = {"Windows": "win", "Darwin": "osx", "Linux": "linux"}
 KIOTA_ARCH_NAMES = {"32bit": "x86", "64bit": "x64"}
 
 
@@ -53,15 +53,16 @@
         "common",
         "src",
         "main",
         "resources",
         "META-INF",
         "openapi.json",
     )
-    output = os.path.join(sys.path[0], "python_sdk", "client")
+    output = Path(__file__).parent.joinpath("python_sdk", "client")
+
     command = f'{kiota_bin} generate --language=python --openapi="{openapi_doc}" --output="{output}" --class-name=RegistryClient --namespace-name=client --clean-output --clear-cache'
     print(f"Executing kiota command: {command}")
 
     os.system(command)
     print("Kiota client generation has been successful")
     return setup_kwargs
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.2/pyproject.toml` & `apicurio_registry_python_sdk_preview-2.4.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "apicurio-registry-python-sdk-preview"
-version = "2.4.2"
+version = "2.4.3"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "python_sdk"}]
+include = [
+    { path = "python_sdk/client/*" },
+    { path = "python_sdk/client/**/*" }
+]
 license = "Apache 2.0"
 homepage = "https://github.com/apicurio/apicurio-registry"
 repository = "https://github.com/apicurio/apicurio-registry"
 keywords = ["apicurio", "registry"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.2/PKG-INFO` & `apicurio_registry_python_sdk_preview-2.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicurio-registry-python-sdk-preview
-Version: 2.4.2
+Version: 2.4.3
 Summary: 
 Home-page: https://github.com/apicurio/apicurio-registry
 License: Apache 2.0
 Keywords: apicurio,registry
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.11,<4.0
```

