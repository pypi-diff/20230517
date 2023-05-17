# Comparing `tmp/azure-keyvault-certificates-4.7.0.zip` & `tmp/azure-keyvault-certificates-4.8.0b1.zip`

## zipinfo {}

```diff
@@ -1,256 +1,256 @@
-Zip file size: 533075 bytes, number of entries: 254
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/
--rw-rw-r--  2.0 unx    21358 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/README.md
--rw-rw-r--  2.0 unx     2477 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/setup.py
--rw-rw-r--  2.0 unx    11900 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/migration_guide.md
--rw-rw-r--  2.0 unx    34806 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/PKG-INFO
--rw-rw-r--  2.0 unx     1073 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/LICENSE
--rw-rw-r--  2.0 unx      195 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/MANIFEST.in
--rw-rw-r--  2.0 unx      285 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/setup.cfg
--rw-rw-r--  2.0 unx       86 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/pyproject.toml
--rw-rw-r--  2.0 unx    12508 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/CHANGELOG.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/tests/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     2191 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_test_case.py
--rw-rw-r--  2.0 unx     2544 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_merge_certificate.py
--rw-rw-r--  2.0 unx     2778 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_merge_certificate_async.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_context_manager.py
--rw-rw-r--  2.0 unx    33352 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_certificates_client_async.py
--rw-rw-r--  2.0 unx    14239 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_examples_certificates.py
--rw-rw-r--  2.0 unx    32695 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_certificates_client.py
--rw-rw-r--  2.0 unx      959 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_context_manager_async.py
--rw-rw-r--  2.0 unx     2258 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_async_test_case.py
--rw-rw-r--  2.0 unx     3411 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_parse_id.py
--rw-rw-r--  2.0 unx     2847 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/conftest.py
--rw-rw-r--  2.0 unx    14389 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/certs.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_multi_api.py
--rw-rw-r--  2.0 unx    14130 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/test_examples_certificates_async.py
--rw-rw-r--  2.0 unx      578 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/json_attribute_matcher.py
--rw-rw-r--  2.0 unx     1094 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/preparer.py
--rw-rw-r--  2.0 unx     1639 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/test_case.py
--rw-rw-r--  2.0 unx      151 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/__init__.py
--rw-rw-r--  2.0 unx     1909 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/test_case_async.py
--rw-rw-r--  2.0 unx     3935 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/helpers.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/preparer_async.py
--rw-rw-r--  2.0 unx     1407 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/_shared/helpers_async.py
--rw-rw-r--  2.0 unx     2077 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/perfstress_tests/get_certificate.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     3826 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/backup_restore_operations.py
--rw-rw-r--  2.0 unx     5032 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/list_operations.py
--rw-rw-r--  2.0 unx     3549 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/import_certificate_async.py
--rw-rw-r--  2.0 unx     4103 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/recover_purge_operations_async.py
--rw-rw-r--  2.0 unx     3452 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/issuers.py
--rw-rw-r--  2.0 unx     4946 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/parse_certificate_async.py
--rw-rw-r--  2.0 unx     5000 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/list_operations_async.py
--rw-rw-r--  2.0 unx     3790 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/backup_restore_operations_async.py
--rw-rw-r--  2.0 unx     2272 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/contacts.py
--rw-rw-r--  2.0 unx     2461 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/contacts_async.py
--rw-rw-r--  2.0 unx     4089 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/recover_purge_operations.py
--rw-rw-r--  2.0 unx     4491 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/hello_world_async.py
--rw-rw-r--  2.0 unx     4810 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/parse_certificate.py
--rw-rw-r--  2.0 unx     3766 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/issuers_async.py
--rw-rw-r--  2.0 unx     3235 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/import_certificate.py
--rw-rw-r--  2.0 unx     4453 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/samples/hello_world.py
--rw-rw-r--  2.0 unx        6 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/top_level.txt
--rw-rw-r--  2.0 unx       84 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/requires.txt
--rw-rw-r--  2.0 unx    34806 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    11428 b- defN 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/SOURCES.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/
--rw-rw-r--  2.0 unx      267 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/
--rw-rw-r--  2.0 unx      267 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/
--rw-rw-r--  2.0 unx    50144 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_models.py
--rw-rw-r--  2.0 unx     2437 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_polling.py
--rw-rw-r--  2.0 unx    71756 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated_models.py
--rw-rw-r--  2.0 unx     1350 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/__init__.py
--rw-rw-r--  2.0 unx    47947 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_client.py
--rw-rw-r--  2.0 unx      170 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_version.py
--rw-rw-r--  2.0 unx      231 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_sdk_moniker.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/py.typed
--rw-rw-r--  2.0 unx     2861 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_enums.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/
--rw-rw-r--  2.0 unx   191906 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_operations_mixin.py
--rw-rw-r--  2.0 unx      353 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/models.py
--rw-rw-r--  2.0 unx      698 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/__init__.py
--rw-rw-r--  2.0 unx     4616 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_key_vault_client.py
--rw-rw-r--  2.0 unx      344 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_version.py
--rw-rw-r--  2.0 unx    78842 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_serialization.py
--rw-rw-r--  2.0 unx     1993 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
--rw-rw-r--  2.0 unx     3138 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
--rw-rw-r--  2.0 unx     2532 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
--rw-rw-r--  2.0 unx     7089 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
--rw-rw-r--  2.0 unx   135465 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     3896 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
--rw-rw-r--  2.0 unx   408005 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
--rw-rw-r--  2.0 unx     3243 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2542 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   339680 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
--rw-rw-r--  2.0 unx    65953 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
--rw-rw-r--  2.0 unx     5068 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
--rw-rw-r--  2.0 unx   156980 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   130676 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
--rw-rw-r--  2.0 unx     7985 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
--rw-rw-r--  2.0 unx   156906 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
--rw-rw-r--  2.0 unx     7788 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
--rw-rw-r--  2.0 unx   461426 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   382727 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
--rw-rw-r--  2.0 unx    65498 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
--rw-rw-r--  2.0 unx     5011 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
--rw-rw-r--  2.0 unx   155108 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   128804 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx   194271 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
--rw-rw-r--  2.0 unx      543 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     4685 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2020 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
--rw-rw-r--  2.0 unx    66011 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
--rw-rw-r--  2.0 unx     5035 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
--rw-rw-r--  2.0 unx   154948 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   128644 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/__init__.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
--rw-rw-r--  2.0 unx     2511 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_configuration.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
--rw-rw-r--  2.0 unx    65586 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
--rw-rw-r--  2.0 unx     5035 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
--rw-rw-r--  2.0 unx   155108 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-16 19:44 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
--rw-rw-r--  2.0 unx      829 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx     2521 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   128804 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx     2113 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/exceptions.py
--rw-rw-r--  2.0 unx     4913 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
--rw-rw-r--  2.0 unx     4775 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/_polling.py
--rw-rw-r--  2.0 unx     2390 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/__init__.py
--rw-rw-r--  2.0 unx     2579 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/http_challenge_cache.py
--rw-rw-r--  2.0 unx     5690 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/challenge_auth_policy.py
--rw-rw-r--  2.0 unx     4968 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/async_client_base.py
--rw-rw-r--  2.0 unx     4939 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/http_challenge.py
--rw-rw-r--  2.0 unx     6247 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/client_base.py
--rw-rw-r--  2.0 unx     2702 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/_polling_async.py
--rw-rw-r--  2.0 unx      224 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/__init__.py
--rw-rw-r--  2.0 unx    46900 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/_client.py
--rw-rw-r--  2.0 unx     2311 b- defN 23-Mar-16 19:43 azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/_polling_async.py
-254 files, 4558332 bytes uncompressed, 470275 bytes compressed:  89.7%
+Zip file size: 534642 bytes, number of entries: 254
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/setup.cfg
+-rw-rw-r--  2.0 unx    35007 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/pyproject.toml
+-rw-rw-r--  2.0 unx      195 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx    21358 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/README.md
+-rw-rw-r--  2.0 unx    12720 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2464 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/setup.py
+-rw-rw-r--  2.0 unx      285 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/LICENSE
+-rw-rw-r--  2.0 unx    11900 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/migration_guide.md
+-rw-rw-r--  2.0 unx     3235 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/import_certificate.py
+-rw-rw-r--  2.0 unx     2461 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/contacts_async.py
+-rw-rw-r--  2.0 unx     3549 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/import_certificate_async.py
+-rw-rw-r--  2.0 unx     4103 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations_async.py
+-rw-rw-r--  2.0 unx     4810 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/parse_certificate.py
+-rw-rw-r--  2.0 unx     4946 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/parse_certificate_async.py
+-rw-rw-r--  2.0 unx     3452 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/issuers.py
+-rw-rw-r--  2.0 unx     3790 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations_async.py
+-rw-rw-r--  2.0 unx     5000 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/list_operations_async.py
+-rw-rw-r--  2.0 unx     4491 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/hello_world_async.py
+-rw-rw-r--  2.0 unx     2272 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/contacts.py
+-rw-rw-r--  2.0 unx     4089 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations.py
+-rw-rw-r--  2.0 unx     3766 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/issuers_async.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/list_operations.py
+-rw-rw-r--  2.0 unx     3826 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations.py
+-rw-rw-r--  2.0 unx     4453 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/hello_world.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx    35007 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    11428 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/tests/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx     2258 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_async_test_case.py
+-rw-rw-r--  2.0 unx    33352 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client_async.py
+-rw-rw-r--  2.0 unx     2778 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate_async.py
+-rw-rw-r--  2.0 unx     2191 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_test_case.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_multi_api.py
+-rw-rw-r--  2.0 unx     2544 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate.py
+-rw-rw-r--  2.0 unx     3411 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_parse_id.py
+-rw-rw-r--  2.0 unx     2847 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/conftest.py
+-rw-rw-r--  2.0 unx    14239 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates.py
+-rw-rw-r--  2.0 unx      959 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_context_manager_async.py
+-rw-rw-r--  2.0 unx    14130 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates_async.py
+-rw-rw-r--  2.0 unx    14389 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/certs.py
+-rw-rw-r--  2.0 unx    32695 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_context_manager.py
+-rw-rw-r--  2.0 unx     3935 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers.py
+-rw-rw-r--  2.0 unx      578 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/json_attribute_matcher.py
+-rw-rw-r--  2.0 unx     1407 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers_async.py
+-rw-rw-r--  2.0 unx     1094 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer.py
+-rw-rw-r--  2.0 unx     1909 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case_async.py
+-rw-rw-r--  2.0 unx     1639 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer_async.py
+-rw-rw-r--  2.0 unx      151 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/__init__.py
+-rw-rw-r--  2.0 unx     2077 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/get_certificate.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/
+-rw-rw-r--  2.0 unx      267 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/
+-rw-rw-r--  2.0 unx      267 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/
+-rw-rw-r--  2.0 unx    47947 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_client.py
+-rw-rw-r--  2.0 unx     2437 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_polling.py
+-rw-rw-r--  2.0 unx      172 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_version.py
+-rw-rw-r--  2.0 unx    50258 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_models.py
+-rw-rw-r--  2.0 unx     2861 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_enums.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/py.typed
+-rw-rw-r--  2.0 unx      231 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_sdk_moniker.py
+-rw-rw-r--  2.0 unx    71756 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated_models.py
+-rw-rw-r--  2.0 unx     1350 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/__init__.py
+-rw-rw-r--  2.0 unx     4939 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge.py
+-rw-rw-r--  2.0 unx     4775 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling.py
+-rw-rw-r--  2.0 unx     2702 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling_async.py
+-rw-rw-r--  2.0 unx     2113 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/exceptions.py
+-rw-rw-r--  2.0 unx     6078 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/challenge_auth_policy.py
+-rw-rw-r--  2.0 unx     4968 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_client_base.py
+-rw-rw-r--  2.0 unx     2579 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge_cache.py
+-rw-rw-r--  2.0 unx     5307 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
+-rw-rw-r--  2.0 unx     2390 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/__init__.py
+-rw-rw-r--  2.0 unx     6247 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/client_base.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/
+-rw-rw-r--  2.0 unx   191906 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_operations_mixin.py
+-rw-rw-r--  2.0 unx     1993 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      344 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_version.py
+-rw-rw-r--  2.0 unx     4616 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_key_vault_client.py
+-rw-rw-r--  2.0 unx      353 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/models.py
+-rw-rw-r--  2.0 unx    78842 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_serialization.py
+-rw-rw-r--  2.0 unx      698 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_vendor.py
+-rw-rw-r--  2.0 unx   461426 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
+-rw-rw-r--  2.0 unx     7788 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx   156906 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
+-rw-rw-r--  2.0 unx     7985 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
+-rw-rw-r--  2.0 unx   382727 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_vendor.py
+-rw-rw-r--  2.0 unx   155108 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
+-rw-rw-r--  2.0 unx     5011 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    65498 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
+-rw-rw-r--  2.0 unx   128804 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_vendor.py
+-rw-rw-r--  2.0 unx   155108 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
+-rw-rw-r--  2.0 unx     5035 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    65586 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
+-rw-rw-r--  2.0 unx   128804 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_vendor.py
+-rw-rw-r--  2.0 unx   156980 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
+-rw-rw-r--  2.0 unx     5068 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    65953 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
+-rw-rw-r--  2.0 unx   130676 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/
+-rw-rw-r--  2.0 unx     2532 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
+-rw-rw-r--  2.0 unx     3138 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
+-rw-rw-r--  2.0 unx   408005 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
+-rw-rw-r--  2.0 unx     3896 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx   135465 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     7089 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
+-rw-rw-r--  2.0 unx     2542 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
+-rw-rw-r--  2.0 unx     3243 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
+-rw-rw-r--  2.0 unx   339680 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   194271 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
+-rw-rw-r--  2.0 unx     2020 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     4685 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      543 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/
+-rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_patch.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_vendor.py
+-rw-rw-r--  2.0 unx   154948 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
+-rw-rw-r--  2.0 unx     5035 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx    66011 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/
+-rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
+-rw-rw-r--  2.0 unx   128644 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    46900 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_client.py
+-rw-rw-r--  2.0 unx     2311 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_polling_async.py
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/__init__.py
+254 files, 4559831 bytes uncompressed, 470826 bytes compressed:  89.7%
```

## zipnote {}

```diff
@@ -1,763 +1,763 @@
-Filename: azure-keyvault-certificates-4.7.0/
+Filename: azure-keyvault-certificates-4.8.0b1/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/
+Filename: azure-keyvault-certificates-4.8.0b1/samples/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/
+Filename: azure-keyvault-certificates-4.8.0b1/tests/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/README.md
+Filename: azure-keyvault-certificates-4.8.0b1/setup.cfg
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/setup.py
+Filename: azure-keyvault-certificates-4.8.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/migration_guide.md
+Filename: azure-keyvault-certificates-4.8.0b1/pyproject.toml
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/PKG-INFO
+Filename: azure-keyvault-certificates-4.8.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/LICENSE
+Filename: azure-keyvault-certificates-4.8.0b1/README.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/MANIFEST.in
+Filename: azure-keyvault-certificates-4.8.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/TROUBLESHOOTING.md
+Filename: azure-keyvault-certificates-4.8.0b1/setup.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/setup.cfg
+Filename: azure-keyvault-certificates-4.8.0b1/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/pyproject.toml
+Filename: azure-keyvault-certificates-4.8.0b1/LICENSE
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/CHANGELOG.md
+Filename: azure-keyvault-certificates-4.8.0b1/migration_guide.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/
+Filename: azure-keyvault-certificates-4.8.0b1/samples/import_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/perfstress_tests/
+Filename: azure-keyvault-certificates-4.8.0b1/samples/contacts_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_test_case.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/import_certificate_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_merge_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_merge_certificate_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/parse_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_context_manager.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/parse_certificate_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_certificates_client_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/issuers.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_examples_certificates.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_certificates_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/list_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_context_manager_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/hello_world_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_async_test_case.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/contacts.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_parse_id.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/conftest.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/issuers_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/certs.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/list_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_multi_api.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/test_examples_certificates_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/samples/hello_world.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/json_attribute_matcher.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/preparer.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/test_case.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/test_case_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/helpers.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/requires.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/preparer_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/_shared/helpers_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/perfstress_tests/get_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_async_test_case.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/tests/perfstress_tests/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/backup_restore_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/list_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_test_case.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/import_certificate_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_multi_api.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/recover_purge_operations_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/issuers.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_parse_id.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/parse_certificate_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/conftest.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/list_operations_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/backup_restore_operations_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_context_manager_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/contacts.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/contacts_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/certs.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/recover_purge_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/hello_world_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/test_context_manager.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/parse_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/issuers_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/json_attribute_matcher.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/import_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/samples/hello_world.py
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/top_level.txt
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/requires.txt
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/PKG-INFO
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/dependency_links.txt
+Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/not-zip-safe
+Filename: azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/get_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/SOURCES.txt
+Filename: azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_models.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_polling.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_polling.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated_models.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_version.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_models.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_version.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/py.typed
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_sdk_moniker.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_sdk_moniker.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/py.typed
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated_models.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/exceptions.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/challenge_auth_policy.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_client_base.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge_cache.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_operations_mixin.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/models.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/client_base.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_version.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_serialization.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_operations_mixin.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_version.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/models.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_serialization.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/exceptions.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/_polling.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/http_challenge_cache.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/challenge_auth_policy.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/async_client_base.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/http_challenge.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/client_base.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/_polling_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/_client.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_polling_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/_polling_async.py
+Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-keyvault-certificates-4.7.0/README.md` & `azure-keyvault-certificates-4.8.0b1/README.md`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/setup.py` & `azure-keyvault-certificates-4.8.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     long_description=README + "\n\n" + CHANGELOG,
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azurekeyvault@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-certificates",
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

## Comparing `azure-keyvault-certificates-4.7.0/migration_guide.md` & `azure-keyvault-certificates-4.8.0b1/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/PKG-INFO` & `azure-keyvault-certificates-4.8.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-certificates
-Version: 4.7.0
+Version: 4.8.0b1
 Summary: Microsoft Azure Key Vault Certificates Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-certificates
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
@@ -414,14 +414,20 @@
 [soft_delete]: https://docs.microsoft.com/azure/key-vault/general/soft-delete-overview
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fkeyvault%2Fazure-keyvault-certificates%2FREADME.png)
 
 
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

## Comparing `azure-keyvault-certificates-4.7.0/LICENSE` & `azure-keyvault-certificates-4.8.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/CHANGELOG.md` & `azure-keyvault-certificates-4.8.0b1/CHANGELOG.md`

 * *Files 1% similar despite different names*

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

## Comparing `azure-keyvault-certificates-4.7.0/tests/_test_case.py` & `azure-keyvault-certificates-4.8.0b1/tests/_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_merge_certificate.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_merge_certificate_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_context_manager.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_context_manager.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_certificates_client_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_examples_certificates.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_certificates_client.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_context_manager_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_context_manager_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_async_test_case.py` & `azure-keyvault-certificates-4.8.0b1/tests/_async_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_parse_id.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_parse_id.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/conftest.py` & `azure-keyvault-certificates-4.8.0b1/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/certs.py` & `azure-keyvault-certificates-4.8.0b1/tests/certs.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_multi_api.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_multi_api.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/test_examples_certificates_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/json_attribute_matcher.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/json_attribute_matcher.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/preparer.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/test_case.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/test_case_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/helpers.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/preparer_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/_shared/helpers_async.py` & `azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/tests/perfstress_tests/get_certificate.py` & `azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/get_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/backup_restore_operations.py` & `azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/list_operations.py` & `azure-keyvault-certificates-4.8.0b1/samples/list_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/import_certificate_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/import_certificate_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/recover_purge_operations_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/issuers.py` & `azure-keyvault-certificates-4.8.0b1/samples/issuers.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/parse_certificate_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/parse_certificate_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/list_operations_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/list_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/backup_restore_operations_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/contacts.py` & `azure-keyvault-certificates-4.8.0b1/samples/contacts.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/contacts_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/contacts_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/recover_purge_operations.py` & `azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/hello_world_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/hello_world_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/parse_certificate.py` & `azure-keyvault-certificates-4.8.0b1/samples/parse_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/issuers_async.py` & `azure-keyvault-certificates-4.8.0b1/samples/issuers_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/import_certificate.py` & `azure-keyvault-certificates-4.8.0b1/samples/import_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/samples/hello_world.py` & `azure-keyvault-certificates-4.8.0b1/samples/hello_world.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/PKG-INFO` & `azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-certificates
-Version: 4.7.0
+Version: 4.8.0b1
 Summary: Microsoft Azure Key Vault Certificates Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-certificates
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
@@ -414,14 +414,20 @@
 [soft_delete]: https://docs.microsoft.com/azure/key-vault/general/soft-delete-overview
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fkeyvault%2Fazure-keyvault-certificates%2FREADME.png)
 
 
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

## Comparing `azure-keyvault-certificates-4.7.0/azure_keyvault_certificates.egg-info/SOURCES.txt` & `azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_models.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1101,14 +1101,15 @@
     """
 
     def __init__(
         self,
         provider: "Optional[str]",
         attributes: "Optional[models.IssuerAttributes]" = None,
         account_id: "Optional[str]" = None,
+        # [SuppressMessage("Microsoft.Security", "CS002:SecretInNextLine", Justification="Typedef, not string.")]
         password: "Optional[str]" = None,
         organization_id: "Optional[str]" = None,
         admin_contacts: "Optional[List[AdministratorContact]]" = None,
         **kwargs,
     ) -> None:
         self._provider = provider
         self._attributes = attributes
```

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_polling.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_polling.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated_models.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated_models.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_operations_mixin.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_operations_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_serialization.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_operations_mixin.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_operations_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/exceptions.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py`

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

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/_polling.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/__init__.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/http_challenge_cache.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge_cache.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/challenge_auth_policy.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/challenge_auth_policy.py`

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

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/async_client_base.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_client_base.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/http_challenge.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/client_base.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/client_base.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/_shared/_polling_async.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/_client.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.7.0/azure/keyvault/certificates/aio/_polling_async.py` & `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_polling_async.py`

 * *Files identical despite different names*

