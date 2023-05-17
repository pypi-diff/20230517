# Comparing `tmp/azure-keyvault-secrets-4.7.0.zip` & `tmp/azure-keyvault-secrets-4.8.0b1.zip`

## zipinfo {}

```diff
@@ -1,245 +1,245 @@
-Zip file size: 423956 bytes, number of entries: 243
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/
--rw-rw-r--  2.0 unx    17595 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/README.md
--rw-rw-r--  2.0 unx     2462 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/setup.py
--rw-rw-r--  2.0 unx    10548 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/migration_guide.md
--rw-rw-r--  2.0 unx    28051 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/PKG-INFO
--rw-rw-r--  2.0 unx     1073 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/LICENSE
--rw-rw-r--  2.0 unx      190 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/MANIFEST.in
--rw-rw-r--  2.0 unx      280 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/setup.cfg
--rw-rw-r--  2.0 unx       86 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/pyproject.toml
--rw-rw-r--  2.0 unx     9531 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/CHANGELOG.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/tests/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     8249 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_samples_secrets_async.py
--rw-rw-r--  2.0 unx     2014 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_test_case.py
--rw-rw-r--  2.0 unx    15265 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_secrets_client.py
--rw-rw-r--  2.0 unx      821 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_context_manager.py
--rw-rw-r--  2.0 unx     7218 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_samples_secrets.py
--rw-rw-r--  2.0 unx     4689 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_polling_method.py
--rw-rw-r--  2.0 unx     5253 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_polling_method_async.py
--rw-rw-r--  2.0 unx    16679 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_secrets_async.py
--rw-rw-r--  2.0 unx      939 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_context_manager_async.py
--rw-rw-r--  2.0 unx     1826 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_async_test_case.py
--rw-rw-r--  2.0 unx     2908 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_parse_id.py
--rw-rw-r--  2.0 unx     2706 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/conftest.py
--rw-rw-r--  2.0 unx      849 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/test_multi_api.py
--rw-rw-r--  2.0 unx      578 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/json_attribute_matcher.py
--rw-rw-r--  2.0 unx     1094 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/preparer.py
--rw-rw-r--  2.0 unx     1649 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/test_case.py
--rw-rw-r--  2.0 unx      151 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/__init__.py
--rw-rw-r--  2.0 unx     1693 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/test_case_async.py
--rw-rw-r--  2.0 unx     3935 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/helpers.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/preparer_async.py
--rw-rw-r--  2.0 unx     1407 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/_shared/helpers_async.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1946 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/perfstress_tests/get_secret.py
--rw-rw-r--  2.0 unx     3359 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/tests/perfstress_tests/list_secrets.py
--rw-rw-r--  2.0 unx        6 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/top_level.txt
--rw-rw-r--  2.0 unx       84 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/requires.txt
--rw-rw-r--  2.0 unx    28051 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    10284 b- defN 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx     3182 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/backup_restore_operations.py
--rw-rw-r--  2.0 unx     4721 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/list_operations.py
--rw-rw-r--  2.0 unx     3702 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/recover_purge_operations_async.py
--rw-rw-r--  2.0 unx     4794 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/list_operations_async.py
--rw-rw-r--  2.0 unx     3391 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/backup_restore_operations_async.py
--rw-rw-r--  2.0 unx     3809 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/recover_purge_operations.py
--rw-rw-r--  2.0 unx     4125 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/hello_world_async.py
--rw-rw-r--  2.0 unx     3696 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/samples/hello_world.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/
--rw-rw-r--  2.0 unx      267 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/
--rw-rw-r--  2.0 unx      267 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/
--rw-rw-r--  2.0 unx    10894 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_models.py
--rw-rw-r--  2.0 unx    28832 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated_models.py
--rw-rw-r--  2.0 unx      528 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/__init__.py
--rw-rw-r--  2.0 unx    20202 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_client.py
--rw-rw-r--  2.0 unx      170 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_version.py
--rw-rw-r--  2.0 unx      226 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_sdk_moniker.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/py.typed
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/
--rw-rw-r--  2.0 unx   183141 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_operations_mixin.py
--rw-rw-r--  2.0 unx      380 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/models.py
--rw-rw-r--  2.0 unx      698 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/__init__.py
--rw-rw-r--  2.0 unx     7400 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_key_vault_client.py
--rw-rw-r--  2.0 unx      344 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_version.py
--rw-rw-r--  2.0 unx    78842 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_serialization.py
--rw-rw-r--  2.0 unx     1993 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/__init__.py
--rw-rw-r--  2.0 unx     3138 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_key_vault_client.py
--rw-rw-r--  2.0 unx     2532 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_patch.py
--rw-rw-r--  2.0 unx     7089 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/__init__.py
--rw-rw-r--  2.0 unx   135465 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     3896 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/__init__.py
--rw-rw-r--  2.0 unx   408005 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/__init__.py
--rw-rw-r--  2.0 unx     3243 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2542 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   339680 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_patch.py
--rw-rw-r--  2.0 unx     1783 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/__init__.py
--rw-rw-r--  2.0 unx    25244 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_models_py3.py
--rw-rw-r--  2.0 unx     3950 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/__init__.py
--rw-rw-r--  2.0 unx    66338 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    55088 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_patch.py
--rw-rw-r--  2.0 unx     7985 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/__init__.py
--rw-rw-r--  2.0 unx   156906 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_models_py3.py
--rw-rw-r--  2.0 unx     7788 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/__init__.py
--rw-rw-r--  2.0 unx   461426 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   382727 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_patch.py
--rw-rw-r--  2.0 unx     1783 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/__init__.py
--rw-rw-r--  2.0 unx    25244 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_models_py3.py
--rw-rw-r--  2.0 unx     3950 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/__init__.py
--rw-rw-r--  2.0 unx    65765 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    54515 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx   185197 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_operations_mixin.py
--rw-rw-r--  2.0 unx      543 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     7469 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2020 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_patch.py
--rw-rw-r--  2.0 unx     1783 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/__init__.py
--rw-rw-r--  2.0 unx    25244 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_models_py3.py
--rw-rw-r--  2.0 unx     3950 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/__init__.py
--rw-rw-r--  2.0 unx    64816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    53566 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_patch.py
--rw-rw-r--  2.0 unx     1783 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/__init__.py
--rw-rw-r--  2.0 unx    25244 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_models_py3.py
--rw-rw-r--  2.0 unx     3950 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/__init__.py
--rw-rw-r--  2.0 unx    65765 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    54515 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx     2113 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/exceptions.py
--rw-rw-r--  2.0 unx     4913 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/async_challenge_auth_policy.py
--rw-rw-r--  2.0 unx     4775 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/_polling.py
--rw-rw-r--  2.0 unx     2390 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/__init__.py
--rw-rw-r--  2.0 unx     2579 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/http_challenge_cache.py
--rw-rw-r--  2.0 unx     5690 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/challenge_auth_policy.py
--rw-rw-r--  2.0 unx     4968 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/async_client_base.py
--rw-rw-r--  2.0 unx     4939 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/http_challenge.py
--rw-rw-r--  2.0 unx     6247 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/client_base.py
--rw-rw-r--  2.0 unx     2702 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/_polling_async.py
--rw-rw-r--  2.0 unx      213 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/__init__.py
--rw-rw-r--  2.0 unx    18614 b- defN 23-Mar-16 19:43 azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/_client.py
-243 files, 3455900 bytes uncompressed, 367796 bytes compressed:  89.4%
+Zip file size: 425410 bytes, number of entries: 243
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/setup.cfg
+-rw-rw-r--  2.0 unx    28252 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/pyproject.toml
+-rw-rw-r--  2.0 unx      190 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx    17595 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/README.md
+-rw-rw-r--  2.0 unx     9743 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2449 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/setup.py
+-rw-rw-r--  2.0 unx      280 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/LICENSE
+-rw-rw-r--  2.0 unx    10548 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/migration_guide.md
+-rw-rw-r--  2.0 unx     3702 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/recover_purge_operations_async.py
+-rw-rw-r--  2.0 unx     3391 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/backup_restore_operations_async.py
+-rw-rw-r--  2.0 unx     4794 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/list_operations_async.py
+-rw-rw-r--  2.0 unx     4125 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/hello_world_async.py
+-rw-rw-r--  2.0 unx     3809 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/recover_purge_operations.py
+-rw-rw-r--  2.0 unx     4721 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/list_operations.py
+-rw-rw-r--  2.0 unx     3182 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/backup_restore_operations.py
+-rw-rw-r--  2.0 unx     3696 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/samples/hello_world.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx    28252 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    10284 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/tests/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx     1826 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_async_test_case.py
+-rw-rw-r--  2.0 unx     8249 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_samples_secrets_async.py
+-rw-rw-r--  2.0 unx     2014 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_test_case.py
+-rw-rw-r--  2.0 unx      849 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_multi_api.py
+-rw-rw-r--  2.0 unx     5253 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_polling_method_async.py
+-rw-rw-r--  2.0 unx     2908 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_parse_id.py
+-rw-rw-r--  2.0 unx     2706 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/conftest.py
+-rw-rw-r--  2.0 unx    16679 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_secrets_async.py
+-rw-rw-r--  2.0 unx      939 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_context_manager_async.py
+-rw-rw-r--  2.0 unx     4689 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_polling_method.py
+-rw-rw-r--  2.0 unx    15265 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_secrets_client.py
+-rw-rw-r--  2.0 unx     7218 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_samples_secrets.py
+-rw-rw-r--  2.0 unx      821 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/test_context_manager.py
+-rw-rw-r--  2.0 unx     3935 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/helpers.py
+-rw-rw-r--  2.0 unx      578 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/json_attribute_matcher.py
+-rw-rw-r--  2.0 unx     1407 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/helpers_async.py
+-rw-rw-r--  2.0 unx     1094 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/preparer.py
+-rw-rw-r--  2.0 unx     1693 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/test_case_async.py
+-rw-rw-r--  2.0 unx     1649 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/test_case.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/preparer_async.py
+-rw-rw-r--  2.0 unx      151 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/_shared/__init__.py
+-rw-rw-r--  2.0 unx     3359 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/list_secrets.py
+-rw-rw-r--  2.0 unx     1946 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/get_secret.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/
+-rw-rw-r--  2.0 unx      267 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/
+-rw-rw-r--  2.0 unx      267 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/
+-rw-rw-r--  2.0 unx    20202 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_client.py
+-rw-rw-r--  2.0 unx      172 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_version.py
+-rw-rw-r--  2.0 unx    10894 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_models.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/py.typed
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_sdk_moniker.py
+-rw-rw-r--  2.0 unx    28832 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated_models.py
+-rw-rw-r--  2.0 unx      528 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/__init__.py
+-rw-rw-r--  2.0 unx     4939 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/http_challenge.py
+-rw-rw-r--  2.0 unx     4775 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/_polling.py
+-rw-rw-r--  2.0 unx     2702 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/_polling_async.py
+-rw-rw-r--  2.0 unx     2113 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/exceptions.py
+-rw-rw-r--  2.0 unx     6078 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/challenge_auth_policy.py
+-rw-rw-r--  2.0 unx     4968 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/async_client_base.py
+-rw-rw-r--  2.0 unx     2579 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/http_challenge_cache.py
+-rw-rw-r--  2.0 unx     5307 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/async_challenge_auth_policy.py
+-rw-rw-r--  2.0 unx     2390 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/__init__.py
+-rw-rw-r--  2.0 unx     6247 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/client_base.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/
+-rw-rw-r--  2.0 unx   183141 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_operations_mixin.py
+-rw-rw-r--  2.0 unx     1993 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      344 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_version.py
+-rw-rw-r--  2.0 unx     7400 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_key_vault_client.py
+-rw-rw-r--  2.0 unx      380 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/models.py
+-rw-rw-r--  2.0 unx    78842 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_serialization.py
+-rw-rw-r--  2.0 unx      698 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_vendor.py
+-rw-rw-r--  2.0 unx   461426 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_patch.py
+-rw-rw-r--  2.0 unx     7788 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx   156906 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_models_py3.py
+-rw-rw-r--  2.0 unx     7985 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_vendor.py
+-rw-rw-r--  2.0 unx   382727 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_vendor.py
+-rw-rw-r--  2.0 unx    65765 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_patch.py
+-rw-rw-r--  2.0 unx     3950 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    25244 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_models_py3.py
+-rw-rw-r--  2.0 unx     1783 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_vendor.py
+-rw-rw-r--  2.0 unx    54515 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_vendor.py
+-rw-rw-r--  2.0 unx    65765 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_patch.py
+-rw-rw-r--  2.0 unx     3950 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    25244 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_models_py3.py
+-rw-rw-r--  2.0 unx     1783 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_vendor.py
+-rw-rw-r--  2.0 unx    54515 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_vendor.py
+-rw-rw-r--  2.0 unx    66338 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_patch.py
+-rw-rw-r--  2.0 unx     3950 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    25244 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_models_py3.py
+-rw-rw-r--  2.0 unx     1783 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_vendor.py
+-rw-rw-r--  2.0 unx    55088 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/
+-rw-rw-r--  2.0 unx     2532 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_patch.py
+-rw-rw-r--  2.0 unx     3138 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_vendor.py
+-rw-rw-r--  2.0 unx   408005 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_patch.py
+-rw-rw-r--  2.0 unx     3896 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx   135465 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     7089 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/
+-rw-rw-r--  2.0 unx     2542 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_patch.py
+-rw-rw-r--  2.0 unx     3243 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_vendor.py
+-rw-rw-r--  2.0 unx   339680 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   185197 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_operations_mixin.py
+-rw-rw-r--  2.0 unx     2020 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     7469 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      543 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_vendor.py
+-rw-rw-r--  2.0 unx    64816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_patch.py
+-rw-rw-r--  2.0 unx     3950 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    25244 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_models_py3.py
+-rw-rw-r--  2.0 unx     1783 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_vendor.py
+-rw-rw-r--  2.0 unx    53566 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    18614 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/_client.py
+-rw-rw-r--  2.0 unx      213 b- defN 23-May-16 23:24 azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/__init__.py
+243 files, 3457285 bytes uncompressed, 368278 bytes compressed:  89.4%
```

## zipnote {}

```diff
@@ -1,730 +1,730 @@
-Filename: azure-keyvault-secrets-4.7.0/
+Filename: azure-keyvault-secrets-4.8.0b1/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/
+Filename: azure-keyvault-secrets-4.8.0b1/samples/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/
+Filename: azure-keyvault-secrets-4.8.0b1/tests/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/README.md
+Filename: azure-keyvault-secrets-4.8.0b1/setup.cfg
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/setup.py
+Filename: azure-keyvault-secrets-4.8.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/migration_guide.md
+Filename: azure-keyvault-secrets-4.8.0b1/pyproject.toml
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/PKG-INFO
+Filename: azure-keyvault-secrets-4.8.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/LICENSE
+Filename: azure-keyvault-secrets-4.8.0b1/README.md
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/MANIFEST.in
+Filename: azure-keyvault-secrets-4.8.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/TROUBLESHOOTING.md
+Filename: azure-keyvault-secrets-4.8.0b1/setup.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/setup.cfg
+Filename: azure-keyvault-secrets-4.8.0b1/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/pyproject.toml
+Filename: azure-keyvault-secrets-4.8.0b1/LICENSE
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/CHANGELOG.md
+Filename: azure-keyvault-secrets-4.8.0b1/migration_guide.md
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/
+Filename: azure-keyvault-secrets-4.8.0b1/samples/recover_purge_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/perfstress_tests/
+Filename: azure-keyvault-secrets-4.8.0b1/samples/backup_restore_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_samples_secrets_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/samples/list_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_test_case.py
+Filename: azure-keyvault-secrets-4.8.0b1/samples/hello_world_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_secrets_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/samples/recover_purge_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_context_manager.py
+Filename: azure-keyvault-secrets-4.8.0b1/samples/list_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_samples_secrets.py
+Filename: azure-keyvault-secrets-4.8.0b1/samples/backup_restore_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_polling_method.py
+Filename: azure-keyvault-secrets-4.8.0b1/samples/hello_world.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_polling_method_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_secrets_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_context_manager_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_async_test_case.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_parse_id.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/conftest.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/requires.txt
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/test_multi_api.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/json_attribute_matcher.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/preparer.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_async_test_case.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/test_case.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_samples_secrets_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_test_case.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/test_case_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_multi_api.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/helpers.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_polling_method_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/preparer_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_parse_id.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/_shared/helpers_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/conftest.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/perfstress_tests/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_secrets_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/perfstress_tests/get_secret.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_context_manager_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/tests/perfstress_tests/list_secrets.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_polling_method.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/top_level.txt
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_secrets_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/requires.txt
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_samples_secrets.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/PKG-INFO
+Filename: azure-keyvault-secrets-4.8.0b1/tests/test_context_manager.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/dependency_links.txt
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/helpers.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/not-zip-safe
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/json_attribute_matcher.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/SOURCES.txt
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/helpers_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/backup_restore_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/preparer.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/list_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/test_case_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/recover_purge_operations_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/test_case.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/list_operations_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/preparer_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/backup_restore_operations_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/_shared/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/recover_purge_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/list_secrets.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/hello_world_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/get_secret.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/samples/hello_world.py
+Filename: azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_models.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated_models.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_version.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_models.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/py.typed
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_version.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_sdk_moniker.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_sdk_moniker.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated_models.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/py.typed
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/http_challenge.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/_polling.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/_polling_async.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/exceptions.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/challenge_auth_policy.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/async_client_base.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/http_challenge_cache.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_operations_mixin.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/async_challenge_auth_policy.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/models.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/client_base.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_version.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_serialization.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_operations_mixin.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_version.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/models.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_serialization.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_models_py3.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_key_vault_client_enums.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_models_py3.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_key_vault_client_enums.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_models_py3.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_key_vault_client_enums.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_models_py3.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_key_vault_client_enums.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_operations_mixin.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_models_py3.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_key_vault_client_enums.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_operations_mixin.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_models_py3.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_key_vault_client_enums.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_key_vault_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_configuration.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_vendor.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/_patch.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/exceptions.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/async_challenge_auth_policy.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/_polling.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/http_challenge_cache.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/challenge_auth_policy.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/async_client_base.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/http_challenge.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/client_base.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/_polling_async.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/__init__.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/_client.py
 Comment: 
 
-Filename: azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/_client.py
+Filename: azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-keyvault-secrets-4.7.0/README.md` & `azure-keyvault-secrets-4.8.0b1/README.md`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/setup.py` & `azure-keyvault-secrets-4.8.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     long_description=README + "\n\n" + CHANGELOG,
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azurekeyvault@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-secrets",
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

## Comparing `azure-keyvault-secrets-4.7.0/migration_guide.md` & `azure-keyvault-secrets-4.8.0b1/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/PKG-INFO` & `azure-keyvault-secrets-4.8.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-secrets
-Version: 4.7.0
+Version: 4.8.0b1
 Summary: Microsoft Azure Key Vault Secrets Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-secrets
 Author: Microsoft Corporation
 Author-email: azurekeyvault@microsoft.com
 License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -400,14 +400,20 @@
 [soft_delete]: https://docs.microsoft.com/azure/key-vault/general/soft-delete-overview
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fkeyvault%2Fazure-keyvault-secrets%2FREADME.png)
 
 
 # Release History
 
+## 4.8.0b1 (2023-05-16)
+
+### Bugs Fixed
+- Token requests made during AD FS authentication no longer specify an erroneous "adfs" tenant ID
+  ([#29888](https://github.com/Azure/azure-sdk-for-python/issues/29888))
+
 ## 4.7.0 (2023-03-16)
 
 ### Features Added
 - Added support for service API version `7.4`
 - Clients each have a `send_request` method that can be used to send custom requests using the
   client's existing pipeline ([#25172](https://github.com/Azure/azure-sdk-for-python/issues/25172))
```

## Comparing `azure-keyvault-secrets-4.7.0/LICENSE` & `azure-keyvault-secrets-4.8.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/CHANGELOG.md` & `azure-keyvault-secrets-4.8.0b1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 4.8.0b1 (2023-05-16)
+
+### Bugs Fixed
+- Token requests made during AD FS authentication no longer specify an erroneous "adfs" tenant ID
+  ([#29888](https://github.com/Azure/azure-sdk-for-python/issues/29888))
+
 ## 4.7.0 (2023-03-16)
 
 ### Features Added
 - Added support for service API version `7.4`
 - Clients each have a `send_request` method that can be used to send custom requests using the
   client's existing pipeline ([#25172](https://github.com/Azure/azure-sdk-for-python/issues/25172))
```

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_samples_secrets_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_samples_secrets_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_test_case.py` & `azure-keyvault-secrets-4.8.0b1/tests/_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_secrets_client.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_secrets_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_context_manager.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_context_manager.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_samples_secrets.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_samples_secrets.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_polling_method.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_polling_method.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_polling_method_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_polling_method_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_secrets_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_secrets_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_context_manager_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_context_manager_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_async_test_case.py` & `azure-keyvault-secrets-4.8.0b1/tests/_async_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_parse_id.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_parse_id.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/conftest.py` & `azure-keyvault-secrets-4.8.0b1/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/test_multi_api.py` & `azure-keyvault-secrets-4.8.0b1/tests/test_multi_api.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/json_attribute_matcher.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/json_attribute_matcher.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/preparer.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/preparer.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/test_case.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/test_case_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/test_case_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/helpers.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/helpers.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/preparer_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/preparer_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/_shared/helpers_async.py` & `azure-keyvault-secrets-4.8.0b1/tests/_shared/helpers_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/perfstress_tests/get_secret.py` & `azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/get_secret.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/tests/perfstress_tests/list_secrets.py` & `azure-keyvault-secrets-4.8.0b1/tests/perfstress_tests/list_secrets.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/PKG-INFO` & `azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-secrets
-Version: 4.7.0
+Version: 4.8.0b1
 Summary: Microsoft Azure Key Vault Secrets Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-secrets
 Author: Microsoft Corporation
 Author-email: azurekeyvault@microsoft.com
 License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -400,14 +400,20 @@
 [soft_delete]: https://docs.microsoft.com/azure/key-vault/general/soft-delete-overview
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fkeyvault%2Fazure-keyvault-secrets%2FREADME.png)
 
 
 # Release History
 
+## 4.8.0b1 (2023-05-16)
+
+### Bugs Fixed
+- Token requests made during AD FS authentication no longer specify an erroneous "adfs" tenant ID
+  ([#29888](https://github.com/Azure/azure-sdk-for-python/issues/29888))
+
 ## 4.7.0 (2023-03-16)
 
 ### Features Added
 - Added support for service API version `7.4`
 - Clients each have a `send_request` method that can be used to send custom requests using the
   client's existing pipeline ([#25172](https://github.com/Azure/azure-sdk-for-python/issues/25172))
```

## Comparing `azure-keyvault-secrets-4.7.0/azure_keyvault_secrets.egg-info/SOURCES.txt` & `azure-keyvault-secrets-4.8.0b1/azure_keyvault_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/backup_restore_operations.py` & `azure-keyvault-secrets-4.8.0b1/samples/backup_restore_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/list_operations.py` & `azure-keyvault-secrets-4.8.0b1/samples/list_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/recover_purge_operations_async.py` & `azure-keyvault-secrets-4.8.0b1/samples/recover_purge_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/list_operations_async.py` & `azure-keyvault-secrets-4.8.0b1/samples/list_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/backup_restore_operations_async.py` & `azure-keyvault-secrets-4.8.0b1/samples/backup_restore_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/recover_purge_operations.py` & `azure-keyvault-secrets-4.8.0b1/samples/recover_purge_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/hello_world_async.py` & `azure-keyvault-secrets-4.8.0b1/samples/hello_world_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/samples/hello_world.py` & `azure-keyvault-secrets-4.8.0b1/samples/hello_world.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_models.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_models.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated_models.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated_models.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_operations_mixin.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_operations_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_serialization.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_models_py3.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/models/_key_vault_client_enums.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_models_py3.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/models/_key_vault_client_enums.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_3/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_models_py3.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/models/_key_vault_client_enums.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_0/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_0/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_models_py3.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/models/_key_vault_client_enums.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_1/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_1/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_operations_mixin.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_operations_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_models_py3.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/models/_key_vault_client_enums.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_3/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v2016_10_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_4/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_models_py3.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/models/_key_vault_client_enums.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_key_vault_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_configuration.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/_vendor.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/_patch.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_4/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_generated/v7_2/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_generated/v7_2/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/exceptions.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/async_challenge_auth_policy.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/async_challenge_auth_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,13 +82,19 @@
                     f"The challenge resource '{resource_domain}' does not match the requested domain. Pass "
                     "`verify_challenge_resource=False` to your client's constructor to disable this verification. "
                     "See https://aka.ms/azsdk/blog/vault-uri for more information."
                 )
 
         body = request.context.pop("key_vault_request_data", None)
         request.http_request.set_text_body(body)  # no-op when text is None
-        await self.authorize_request(request, scope, tenant_id=challenge.tenant_id)
+
+        # The tenant parsed from AD FS challenges is "adfs"; we don't actually need a tenant for AD FS authentication
+        # For AD FS we skip cross-tenant authentication per https://github.com/Azure/azure-sdk-for-python/issues/28648
+        if challenge.tenant_id and challenge.tenant_id.lower().endswith("adfs"):
+            await self.authorize_request(request, scope)
+        else:
+            await self.authorize_request(request, scope, tenant_id=challenge.tenant_id)
 
         return True
 
     def _need_new_token(self) -> bool:
         return not self._token or self._token.expires_on - time.time() < 300
```

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/_polling.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/_polling.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/__init__.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/http_challenge_cache.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/http_challenge_cache.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/challenge_auth_policy.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/challenge_auth_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,20 @@
                     f"The challenge resource '{resource_domain}' does not match the requested domain. Pass "
                     "`verify_challenge_resource=False` to your client's constructor to disable this verification. "
                     "See https://aka.ms/azsdk/blog/vault-uri for more information."
                 )
 
         body = request.context.pop("key_vault_request_data", None)
         request.http_request.set_text_body(body)  # no-op when text is None
-        self.authorize_request(request, scope, tenant_id=challenge.tenant_id)
+
+        # The tenant parsed from AD FS challenges is "adfs"; we don't actually need a tenant for AD FS authentication
+        # For AD FS we skip cross-tenant authentication per https://github.com/Azure/azure-sdk-for-python/issues/28648
+        if challenge.tenant_id and challenge.tenant_id.lower().endswith("adfs"):
+            self.authorize_request(request, scope)
+        else:
+            self.authorize_request(request, scope, tenant_id=challenge.tenant_id)
 
         return True
 
     @property
     def _need_new_token(self) -> bool:
         return not self._token or self._token.expires_on - time.time() < 300
```

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/async_client_base.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/async_client_base.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/http_challenge.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/http_challenge.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/client_base.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/client_base.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/_shared/_polling_async.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/_shared/_polling_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-secrets-4.7.0/azure/keyvault/secrets/aio/_client.py` & `azure-keyvault-secrets-4.8.0b1/azure/keyvault/secrets/aio/_client.py`

 * *Files identical despite different names*

