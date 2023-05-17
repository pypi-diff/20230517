# Comparing `tmp/azure-confidentialledger-1.0.0b1.zip` & `tmp/azure-confidentialledger-1.1.0.zip`

## zipinfo {}

```diff
@@ -1,101 +1,105 @@
-Zip file size: 104773 bytes, number of entries: 99
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/
--rw-rw-r--  2.0 unx    27640 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/PKG-INFO
--rw-rw-r--  2.0 unx      115 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     2872 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/setup.py
--rw-rw-r--  2.0 unx    22853 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/README.md
--rw-rw-r--  2.0 unx       67 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/setup.cfg
--rw-rw-r--  2.0 unx      185 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx    27640 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     4610 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      165 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/tests/_shared/
--rw-rw-r--  2.0 unx      776 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_certificate_async.py
--rw-rw-r--  2.0 unx     1317 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/test_identity_service_client_async.py
--rw-rw-r--  2.0 unx      703 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_certificate.py
--rw-rw-r--  2.0 unx     1243 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_aad.py
--rw-rw-r--  2.0 unx      164 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/conftest.py
--rw-rw-r--  2.0 unx     1301 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/test_identity_service_client.py
--rw-rw-r--  2.0 unx     1473 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_aad_async.py
--rw-rw-r--  2.0 unx      221 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/_shared/testcase_async.py
--rw-rw-r--  2.0 unx    11357 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/_shared/client_test_common_async.py
--rw-rw-r--  2.0 unx    10554 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/_shared/client_test_common.py
--rw-rw-r--  2.0 unx      211 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/_shared/testcase.py
--rw-rw-r--  2.0 unx        0 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/_shared/__init__.py
--rw-rw-r--  2.0 unx     3971 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/tests/_shared/constants.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/
--rw-rw-r--  2.0 unx       66 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_shared/
--rw-rw-r--  2.0 unx      172 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_version.py
--rw-rw-r--  2.0 unx     4238 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_client_base.py
--rw-rw-r--  2.0 unx        0 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/py.typed
--rw-rw-r--  2.0 unx      487 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_enums.py
--rw-rw-r--  2.0 unx    17421 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_client.py
--rw-rw-r--  2.0 unx      251 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_user_agent.py
--rw-rw-r--  2.0 unx      994 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/__init__.py
--rw-rw-r--  2.0 unx     8865 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_models.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/
--rw-rw-r--  2.0 unx        0 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/
--rw-rw-r--  2.0 unx        0 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/
--rw-rw-r--  2.0 unx     3766 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_confidential_ledger_identity_service_client.py
--rw-rw-r--  2.0 unx      484 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_version.py
--rw-rw-r--  2.0 unx     2665 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_configuration.py
--rw-rw-r--  2.0 unx      774 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/__init__.py
--rw-rw-r--  2.0 unx      640 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/operations/__init__.py
--rw-rw-r--  2.0 unx     4717 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/operations/_confidential_ledger_identity_service_operations.py
--rw-rw-r--  2.0 unx     3454 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/_models_py3.py
--rw-rw-r--  2.0 unx      988 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/__init__.py
--rw-rw-r--  2.0 unx     3416 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/_models.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/operations/
--rw-rw-r--  2.0 unx     3620 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/_confidential_ledger_identity_service_client.py
--rw-rw-r--  2.0 unx     2498 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/_configuration.py
--rw-rw-r--  2.0 unx      620 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/__init__.py
--rw-rw-r--  2.0 unx      640 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     4585 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/operations/_confidential_ledger_identity_service_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/
--rw-rw-r--  2.0 unx        0 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/
--rw-rw-r--  2.0 unx      484 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_version.py
--rw-rw-r--  2.0 unx     3498 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_confidential_ledger_client.py
--rw-rw-r--  2.0 unx     2561 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_configuration.py
--rw-rw-r--  2.0 unx      727 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/__init__.py
--rw-rw-r--  2.0 unx    36917 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/operations/_confidential_ledger_operations.py
--rw-rw-r--  2.0 unx      593 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/operations/__init__.py
--rw-rw-r--  2.0 unx     1730 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/_confidential_ledger_client_enums.py
--rw-rw-r--  2.0 unx    19156 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/_models_py3.py
--rw-rw-r--  2.0 unx     2968 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/__init__.py
--rw-rw-r--  2.0 unx    18086 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/_models.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/operations/
--rw-rw-r--  2.0 unx     3352 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/_confidential_ledger_client.py
--rw-rw-r--  2.0 unx     2394 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/_configuration.py
--rw-rw-r--  2.0 unx      573 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/__init__.py
--rw-rw-r--  2.0 unx    36499 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/operations/_confidential_ledger_operations.py
--rw-rw-r--  2.0 unx      593 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     4416 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/_client_base.py
--rw-rw-r--  2.0 unx    17582 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/_client.py
--rw-rw-r--  2.0 unx      271 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-12 16:54 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/aio/
--rw-rw-r--  2.0 unx     4051 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/_client.py
--rw-rw-r--  2.0 unx      379 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/__init__.py
--rw-rw-r--  2.0 unx     1169 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/_models.py
--rw-rw-r--  2.0 unx     4533 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/aio/_client.py
--rw-rw-r--  2.0 unx      308 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/aio/__init__.py
--rw-rw-r--  2.0 unx      917 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_shared/credential.py
--rw-rw-r--  2.0 unx      280 b- defN 21-May-12 16:51 azure-confidentialledger-1.0.0b1/azure/confidentialledger/_shared/__init__.py
-99 files, 348844 bytes uncompressed, 79335 bytes compressed:  77.3%
+Zip file size: 174363 bytes, number of entries: 103
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/
+-rw-rw-r--  2.0 unx    31138 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/README.md
+-rw-rw-r--  2.0 unx     2784 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/setup.py
+-rw-rw-r--  2.0 unx    34119 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/setup.cfg
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/LICENSE
+-rw-rw-r--  2.0 unx       99 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/pyproject.toml
+-rw-rw-r--  2.0 unx     1999 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx      202 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/MANIFEST.in
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/py.typed
+-rw-rw-r--  2.0 unx    77452 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_serialization.py
+-rw-rw-r--  2.0 unx      900 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/__init__.py
+-rw-rw-r--  2.0 unx     2730 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_configuration.py
+-rw-rw-r--  2.0 unx     3670 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_client.py
+-rw-rw-r--  2.0 unx     4619 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_patch.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_vendor.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/
+-rw-rw-r--  2.0 unx    77452 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_serialization.py
+-rw-rw-r--  2.0 unx      923 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/__init__.py
+-rw-rw-r--  2.0 unx     2868 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_configuration.py
+-rw-rw-r--  2.0 unx     3884 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_client.py
+-rw-rw-r--  2.0 unx     1806 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_patch.py
+-rw-rw-r--  2.0 unx     1395 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_vendor.py
+-rw-rw-r--  2.0 unx     4886 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/_operations.py
+-rw-rw-r--  2.0 unx      856 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/
+-rw-rw-r--  2.0 unx      869 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/__init__.py
+-rw-rw-r--  2.0 unx     2835 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3925 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_client.py
+-rw-rw-r--  2.0 unx     1810 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_patch.py
+-rw-rw-r--  2.0 unx     1015 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3911 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/_operations.py
+-rw-rw-r--  2.0 unx      856 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/_patch.py
+-rw-rw-r--  2.0 unx    58233 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/_operations.py
+-rw-rw-r--  2.0 unx      834 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/__init__.py
+-rw-rw-r--  2.0 unx    12371 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/_patch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/
+-rw-rw-r--  2.0 unx      847 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/__init__.py
+-rw-rw-r--  2.0 unx     2697 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3711 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_client.py
+-rw-rw-r--  2.0 unx     4366 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_patch.py
+-rw-rw-r--  2.0 unx      993 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_vendor.py
+-rw-rw-r--  2.0 unx    46971 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/_operations.py
+-rw-rw-r--  2.0 unx      834 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/__init__.py
+-rw-rw-r--  2.0 unx    11339 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/_patch.py
+-rw-rw-r--  2.0 unx     8022 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_claims_digest_computation.py
+-rw-rw-r--  2.0 unx     1573 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_utils.py
+-rw-rw-r--  2.0 unx      492 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/__init__.py
+-rw-rw-r--  2.0 unx     3434 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_claims_models.py
+-rw-rw-r--  2.0 unx     6663 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_receipt_models.py
+-rw-rw-r--  2.0 unx    12609 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_receipt_verification.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/tests/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/tests/receipt/
+-rw-rw-r--  2.0 unx      256 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/conftest.py
+-rw-rw-r--  2.0 unx    21313 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/test_confidential_ledger_client.py
+-rw-rw-r--  2.0 unx      881 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/test_identity_service_client.py
+-rw-rw-r--  2.0 unx     1034 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/test_identity_service_client_async.py
+-rw-rw-r--  2.0 unx    22340 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/test_confidential_ledger_client_async.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/_shared/__init__.py
+-rw-rw-r--  2.0 unx     3932 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/_shared/constants.py
+-rw-rw-r--  2.0 unx     3659 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/_shared/testcase.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:51 azure-confidentialledger-1.1.0/tests/receipt/_shared/
+-rw-rw-r--  2.0 unx    16670 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/test_receipt_verification.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/__init__.py
+-rw-rw-r--  2.0 unx     3530 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/test_claims_models.py
+-rw-rw-r--  2.0 unx     3717 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/test_receipt_models.py
+-rw-rw-r--  2.0 unx     6468 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/test_claims_digest_computation.py
+-rw-rw-r--  2.0 unx     1698 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/_shared/claims_constants.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/_shared/__init__.py
+-rw-rw-r--  2.0 unx    10384 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/tests/receipt/_shared/receipt_constants.py
+-rw-rw-r--  2.0 unx     4998 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/verify_service_async.py
+-rw-rw-r--  2.0 unx     4403 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/verify_service.py
+-rw-rw-r--  2.0 unx     5670 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/get_and_verify_receipt.py
+-rw-rw-r--  2.0 unx     7498 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/use_collections_async.py
+-rw-rw-r--  2.0 unx     6333 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/use_collections.py
+-rw-rw-r--  2.0 unx     4723 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/list_ledger_entries_async.py
+-rw-rw-r--  2.0 unx     5214 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/manage_users_async.py
+-rw-rw-r--  2.0 unx     4408 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/get_receipt.py
+-rw-rw-r--  2.0 unx     4567 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/manage_users.py
+-rw-rw-r--  2.0 unx     6177 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/write_to_ledger.py
+-rw-rw-r--  2.0 unx     7338 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/write_to_ledger_async.py
+-rw-rw-r--  2.0 unx     5018 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/get_receipt_async.py
+-rw-rw-r--  2.0 unx     3998 b- defN 23-May-12 16:50 azure-confidentialledger-1.1.0/samples/list_ledger_entries.py
+-rw-rw-r--  2.0 unx    34119 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       68 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     3409 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-12 16:51 azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/not-zip-safe
+103 files, 653232 bytes uncompressed, 152543 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -1,298 +1,310 @@
-Filename: azure-confidentialledger-1.0.0b1/
+Filename: azure-confidentialledger-1.1.0/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/
+Filename: azure-confidentialledger-1.1.0/azure/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/
+Filename: azure-confidentialledger-1.1.0/tests/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/
+Filename: azure-confidentialledger-1.1.0/samples/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/PKG-INFO
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/CHANGELOG.md
+Filename: azure-confidentialledger-1.1.0/README.md
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/setup.py
+Filename: azure-confidentialledger-1.1.0/setup.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/README.md
+Filename: azure-confidentialledger-1.1.0/PKG-INFO
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/setup.cfg
+Filename: azure-confidentialledger-1.1.0/setup.cfg
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/MANIFEST.in
+Filename: azure-confidentialledger-1.1.0/LICENSE
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/PKG-INFO
+Filename: azure-confidentialledger-1.1.0/pyproject.toml
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/dependency_links.txt
+Filename: azure-confidentialledger-1.1.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/not-zip-safe
+Filename: azure-confidentialledger-1.1.0/MANIFEST.in
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/SOURCES.txt
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/requires.txt
+Filename: azure-confidentialledger-1.1.0/azure/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/top_level.txt
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_certificate_async.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/test_identity_service_client_async.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_certificate.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/py.typed
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_aad.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_serialization.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/conftest.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/test_identity_service_client.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_configuration.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_aad_async.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_client.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/testcase_async.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/client_test_common_async.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_vendor.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/client_test_common.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_version.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/testcase.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/tests/_shared/constants.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_serialization.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_configuration.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_client.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_vendor.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_shared/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/_operations.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_version.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_client_base.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/py.typed
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_enums.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_client.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_configuration.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_user_agent.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_client.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_models.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_vendor.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/_operations.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/aio/_operations/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/_operations.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/operations/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/_operations/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_confidential_ledger_identity_service_client.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_configuration.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_version.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_client.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_configuration.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_vendor.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/operations/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/_operations.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/operations/_confidential_ledger_identity_service_operations.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/_models_py3.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_operations/_patch.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_claims_digest_computation.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/models/_models.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_utils.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/operations/
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/_confidential_ledger_identity_service_client.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_claims_models.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/_configuration.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_receipt_models.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure/confidentialledger/receipt/_receipt_verification.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/operations/__init__.py
+Filename: azure-confidentialledger-1.1.0/tests/_shared/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/operations/_confidential_ledger_identity_service_operations.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/
+Filename: azure-confidentialledger-1.1.0/tests/conftest.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/__init__.py
+Filename: azure-confidentialledger-1.1.0/tests/test_confidential_ledger_client.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/operations/
+Filename: azure-confidentialledger-1.1.0/tests/test_identity_service_client.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/
+Filename: azure-confidentialledger-1.1.0/tests/test_identity_service_client_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/
+Filename: azure-confidentialledger-1.1.0/tests/test_confidential_ledger_client_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_version.py
+Filename: azure-confidentialledger-1.1.0/tests/_shared/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_confidential_ledger_client.py
+Filename: azure-confidentialledger-1.1.0/tests/_shared/constants.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_configuration.py
+Filename: azure-confidentialledger-1.1.0/tests/_shared/testcase.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/__init__.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/_shared/
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/operations/_confidential_ledger_operations.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/test_receipt_verification.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/operations/__init__.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/_confidential_ledger_client_enums.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/test_claims_models.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/_models_py3.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/test_receipt_models.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/__init__.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/test_claims_digest_computation.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/models/_models.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/_shared/claims_constants.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/operations/
+Filename: azure-confidentialledger-1.1.0/tests/receipt/_shared/__init__.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/_confidential_ledger_client.py
+Filename: azure-confidentialledger-1.1.0/tests/receipt/_shared/receipt_constants.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/_configuration.py
+Filename: azure-confidentialledger-1.1.0/samples/verify_service_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/__init__.py
+Filename: azure-confidentialledger-1.1.0/samples/verify_service.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/operations/_confidential_ledger_operations.py
+Filename: azure-confidentialledger-1.1.0/samples/get_and_verify_receipt.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/aio/operations/__init__.py
+Filename: azure-confidentialledger-1.1.0/samples/use_collections_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/_client_base.py
+Filename: azure-confidentialledger-1.1.0/samples/use_collections.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/_client.py
+Filename: azure-confidentialledger-1.1.0/samples/list_ledger_entries_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/__init__.py
+Filename: azure-confidentialledger-1.1.0/samples/manage_users_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/aio/
+Filename: azure-confidentialledger-1.1.0/samples/get_receipt.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/_client.py
+Filename: azure-confidentialledger-1.1.0/samples/manage_users.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/__init__.py
+Filename: azure-confidentialledger-1.1.0/samples/write_to_ledger.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/_models.py
+Filename: azure-confidentialledger-1.1.0/samples/write_to_ledger_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/aio/_client.py
+Filename: azure-confidentialledger-1.1.0/samples/get_receipt_async.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/identity_service/aio/__init__.py
+Filename: azure-confidentialledger-1.1.0/samples/list_ledger_entries.py
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_shared/credential.py
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-confidentialledger-1.0.0b1/azure/confidentialledger/_shared/__init__.py
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/requires.txt
+Comment: 
+
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/not-zip-safe
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-confidentialledger-1.0.0b1/PKG-INFO` & `azure-confidentialledger-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,499 +1,670 @@
 Metadata-Version: 2.1
 Name: azure-confidentialledger
-Version: 1.0.0b1
+Version: 1.1.0
 Summary: Microsoft Azure Confidential Ledger Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: accledgerdevs@microsoft.com
 License: MIT License
-Description: # Azure Confidential Ledger client library for Python
-        
-        Azure Confidential Ledger provides a service for logging to an immutable, tamper-proof ledger. As part of the [Azure Confidential Computing][azure_confidential_computing] portfolio, Azure Confidential Ledger runs in secure, hardware-based trusted execution environments, also known as enclaves. It is built on Microsoft Research's [Confidential Consortium Framework][ccf].
-        
-        [Source code][confidential_ledger_client_src] | [Package (PyPI)][pypi_package_confidential_ledger] | [API reference documentation][reference_docs] | [Product documentation][confidential_ledger_docs]
-        
-        ## Getting started
-        ### Install packages
-        Install [azure-confidentialledger][pypi_package_confidential_ledger] and [azure-identity][azure_identity_pypi] with [pip][pip]:
-        ```Bash
-        pip install azure-identity azure-confidentialledger
-        ```
-        [azure-identity][azure_identity] is used for Azure Active Directory
-        authentication as demonstrated below.
-        
-        ### Prerequisites
-        * An [Azure subscription][azure_sub]
-        * Python 2.7, 3.5.3, or later
-        * A running instance of Azure Confidential Ledger.
-        * A registered user in the Confidential Ledger, typically assigned during [ARM][azure_resource_manager] resource creation, with `Administrator` privileges.
-        
-        ### Authenticate the client
-        #### Using Azure Active Directory
-        This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate to the Confidential Ledger via Azure Active Directory. However, `ConfidentialLedgerClient` accepts any [azure-identity][azure_identity] credential. See the [azure-identity][azure_identity] documentation for more information about other credentials.
-        
-        #### Using a client certificate
-        As an alternative to Azure Active Directory, clients may choose to use a client certificate to authenticate via mutual TLS. `azure.confidentialledger.ConfidentialLedgerCertificateCredential` may be used for this purpose.
-        
-        ### Create a client
-        `DefaultAzureCredential` will automatically handle most Azure SDK client scenarios. To get started, set environment variables for the AAD identity registered with your Confidential Ledger.
-        ```bash
-        export AZURE_CLIENT_ID="generated app id"
-        export AZURE_CLIENT_SECRET="random password"
-        export AZURE_TENANT_ID="tenant id"
-        ```
-        Then, `DefaultAzureCredential` will be able to authenticate the `ConfidentialLedgerClient`.
-        
-        Constructing the client also requires your Confidential Ledger's URL and id, which you can get from the Azure CLI or the Azure Portal. When you have retrieved those values, please replace instances of `"my-ledger-id"` and `"https://my-ledger-url.confidential-ledger.azure.com"` in the examples below. You may also need to replace `"https://identity.accledger.azure.com"` with the hostname from the `identityServiceUri` in the ARM description of your ledger.
-        
-        Because Confidential Ledgers use self-signed certificates securely generated and stored in an enclave, the signing certificate for each Confidential Ledger must first be retrieved from the Confidential Ledger Identity Service.
-        
-        ```python
-        from azure.identity import DefaultAzureCredential
-        from azure.confidentialledger import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        ```
-        
-        ## Key concepts
-        ### Ledger entries and transactions
-        Every write to Azure Confidential Ledger generates an immutable ledger entry in the service. Writes, also referred to as transactions, are uniquely identified by transaction ids that increment with each write. Once written, ledger entries may be retrieved at any time.
-        
-        ### Receipts
-        State changes to the Confidential Ledger are saved in a data structure called a Merkle tree. To cryptographically verify that writes were correctly saved, a Merkle proof, or receipt, can be retrieved for any transaction id.
-        
-        ### Sub-ledgers
-        While most use cases will involve one ledger, we provide the sub-ledger feature in case semantically or logically different groups of data need to be stored in the same Confidential Ledger.
-        
-        Ledger entries are retrieved by their sub-ledger identifier. The Confidential Ledger will always assume a constant, service-determined sub-ledger id for entries submitted without a sub-ledger specified.
-        
-        ### Users
-        Users are managed directly with the Confidential Ledger instead of through Azure. Users may be AAD-based, identified by their AAD object id, or certificate-based, identified by their PEM certificate fingerprint.
-        
-        ### Confidential computing
-        [Azure Confidential Computing][azure_confidential_computing] allows you to isolate and protect your data while it is being processed in the cloud. Azure Confidential Ledger runs on Azure Confidential Computing virtual machines, thus providing stronger data protection with encryption of data in use.
-        
-        ### Confidential Consortium Framework
-        Azure Confidential Ledger is built on Microsoft Research's open-source [Confidential Consortium Framework (CCF)][ccf]. Under CCF, applications are managed by a consortium of members with the ability to submit proposals to modify and govern application operation. In Azure Confidential Ledger, Microsoft Azure owns a member identity, allowing it to perform governance actions like replacing unhealthy nodes in the Confidential Ledger, or upgrading the enclave code.
-        
-        ## Examples
-        This section contains code snippets covering common tasks:
-        * [Append a ledger entry](#append-entry "Append a ledger entry")
-        * [Get a receipt](#get-receipt "Get a receipt")
-        * [Using sub-ledgers](#using-sub-ledgers "Using sub-ledgers")
-        * [Retrieving ledger entries](#retrieving-ledger-entries "Retrieving ledger entries")
-        * [Making a ranged query](#making-a-ranged-query "Making a ranged query")
-        * [Managing users](#managing-users "Managing users")
-        * [Using certificate authentication](#using-certificate-authentication "Using certificate authentication")
-        * [Verifying service details](#verifying-service-details "Verifying service details")
-        * [Asynchronously get a ledger entry](#asynchronously-get-a-ledger-entry "Asynchronously get a ledger entry")
-        * [Asynchronously get a range of ledger entries](#asynchronously-get-a-range-of-ledger-entries "Asynchronously get a range of ledger entries")
-        
-        
-        ### Append entry
-        Data that needs to be stored immutably in a tamper-proof manner can be saved to Azure Confidential Ledger by appending an entry to the ledger.
-        
-        ```python
-        first_append_result = ledger_client.append_to_ledger(entry_contents="Hello world!")
-        print(first_append_result.transaction_id)
-        ```
-        
-        Since Confidential Ledger is a distributed system, rare transient failures may cause writes to be lost. For entries that must be preserved, it is advisable to verify that the write became durable. Waits are blocking calls.
-        ```python
-        from azure.confidentialledger import TransactionState
-        ledger_client.wait_until_durable(transaction_id=first_append_result.transaction_id)
-        assert ledger_client.get_transaction_status(
-            transaction_id=first_append_result.transaction_id
-        ).state is TransactionState.COMMITTED
-        
-        # Alternatively, a client may wait when appending.
-        append_result = ledger_client.append_to_ledger(
-            entry_contents="Hello world, again!", wait_for_commit=True
-        )
-        assert ledger_client.get_transaction_status(
-            transaction_id=append_result.transaction_id
-        ).state is TransactionState.COMMITTED
-        ```
-        
-        ### Get receipt
-        A receipt can be retrieved for any transaction id to provide cryptographic proof of the contents of the transaction.
-        ```python
-        receipt = ledger_client.get_transaction_receipt(
-            transaction_id=append_result.transaction_id
-        )
-        print(receipt.contents)
-        ```
-        
-        ### Using sub-ledgers
-        Clients can write to different sub-ledgers to separate logically-distinct data.
-        ```python
-        ledger_client.append_to_ledger(
-            entry_contents="Hello from Alice", sub_ledger_id="Alice"
-        )
-        ledger_client.append_to_ledger(
-            entry_contents="Hello from Bob", sub_ledger_id="Bob"
-        )
-        ```
-        
-        When no sub-ledger id is specified on method calls, the Confidential Ledger service will assume a constant, service-determined sub-ledger id.
-        ```python
-        append_result = ledger_client.append_to_ledger(entry_contents="Hello world?", wait_for_commit=True)
-        
-        # The append result contains the sub-ledger id assigned.
-        entry_by_subledger = ledger_client.get_ledger_entry(
-            transaction_id=append_result.transaction_id,
-            sub_ledger_id=append_result.sub_ledger_id
-        )
-        assert entry_by_subledger.contents == "Hello world?"
-        
-        # When a ledger entry is retrieved without a sub-ledger specified,
-        # the service default is used.
-        entry = ledger_client.get_ledger_entry(transaction_id=append_result.transaction_id)
-        assert entry.contents == entry_by_subledger.contents
-        assert entry.sub_ledger_id == entry_by_subledger.sub_ledger_id
-        ```
-        
-        ### Retrieving ledger entries
-        Ledger entries are retrieved from sub-ledgers. When a transaction id is specified, the returned value is the value contained in the specified sub-ledger at the point in time identified by the transaction id. If no transaction id is specified, the latest available value is returned.
-        ```python
-        append_result = ledger_client.append_to_ledger(entry_contents="Hello world 0")
-        ledger_client.append_to_ledger(entry_contents="Hello world 1")
-        
-        subledger_append_result = ledger_client.append_to_ledger(
-            entry_contents="Hello world sub-ledger 0",
-            sub_ledger_id="sub-ledger"
-        )
-        ledger_client.append_to_ledger(
-            entry_contents="Hello world sub-ledger 1",
-            sub_ledger_id="sub-ledger",
-            wait_for_commit=True
-        )
-        
-        # The ledger entry written at 'append_result.transaction_id'
-        # is retrieved from the default sub-ledger.
-        entry = ledger_client.get_ledger_entry(transaction_id=append_result.transaction_id)
-        assert entry.contents == "Hello world 0"
-        
-        # This is the latest entry available in the default sub-ledger.
-        latest_entry = ledger_client.get_ledger_entry()
-        assert latest_entry.contents == "Hello world 1"
-        
-        # The ledger entry written at 'subledger_append_result.transaction_id'
-        # is retrieved from the sub-ledger 'sub-ledger'.
-        subledger_entry = ledger_client.get_ledger_entry(
-            transaction_id=subledger_append_result.transaction_id,
-            sub_ledger_id="sub-ledger"
-        )
-        assert subledger_entry.contents == "Hello world sub-ledger 0"
-        
-        # This is the latest entry available in the sub-ledger 'sub-ledger'.
-        subledger_latest_entry = ledger_client.get_ledger_entry(
-            sub_ledger_id="sub-ledger"
-        )
-        assert subledger_latest_entry.contents == "Hello world sub-ledger 1"
-        ```
-        
-        ### Making a ranged query
-        Ledger entries in a sub-ledger may be retrieved over a range of transaction ids.
-        ```python
-        ranged_result = ledger_client.get_ledger_entries(
-            from_transaction_id=first_append_result.transaction_id
-        )
-        for entry in ranged_result:
-            print(f"Transaction id {entry.transaction_id} contents: {entry.contents}")
-        ```
-        
-        ### Managing users
-        Users with `Administrator` privileges can manage users of the Confidential Ledger directly with the Confidential Ledger itself. Available roles are `Reader` (read-only), `Contributor` (read and write), and `Administrator` (read, write, and add or remove users).
-        
-        ```python
-        from azure.confidentialledger import LedgerUserRole
-        user_id = "some AAD object id"
-        user = ledger_client.create_or_update_user(
-            user_id, LedgerUserRole.CONTRIBUTOR
-        )
-        # A client may now be created and used with AAD credentials for the user identified by `user_id`.
-        
-        user = ledger_client.get_user(user_id)
-        assert user.id == user_id
-        assert user.role == LedgerUserRole.CONTRIBUTOR
-        
-        ledger_client.delete_user(user_id)
-        
-        # For a certificate-based user, their user ID is the fingerprint for their PEM certificate.
-        user_id = "PEM certificate fingerprint"
-        user = ledger_client.create_or_update_user(
-            user_id, LedgerUserRole.READER
-        )
-        ```
-        
-        ### Using certificate authentication
-        Clients may authenticate with a client certificate in mutual TLS instead of via an Azure Active Directory token. `ConfidentialLedgerCertificateCredential` is provided for such clients.
-        ```python
-        from azure.confidentialledger import ConfidentialLedgerClient, ConfidentialLedgerCertificateCredential
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = ConfidentialLedgerCertificateCredential("path to user certificate PEM")
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        ```
-        
-        ### Verifying service details
-        One may want to validate details about the Confidential Ledger for a variety of reasons. For example, you may want to view details about how Microsoft may manage your Confidential Ledger as part of [Confidential Consortium Framework governance](https://microsoft.github.io/CCF/main/governance/index.html), or verify that your Confidential Ledger is indeed running in a secure enclave. A number of client methods are provided for these use cases.
-        ```python
-        consortium = ledger_client.get_consortium()
-        # Consortium members can manage and alter the Confidential Ledger,
-        # such as by replacing unhealthy nodes.
-        for member in consortium.members:
-            print(member.certificate)
-            print(member.id)
-        
-        import hashlib
-        # The constitution is a collection of JavaScript code that
-        # defines actions available to members,
-        # and vets proposals by members to execute those actions.
-        constitution = ledger_client.get_constitution()
-        assert constitution.digest.lower() == \
-            hashlib.sha256(constitution.contents.encode()).hexdigest().lower()
-        print(constitution.contents)
-        print(constitution.digest)
-        
-        # Enclave quotes contain material that can be used to
-        # cryptographically verify the validity and contents
-        # of an enclave.
-        ledger_enclaves = ledger_client.get_enclave_quotes()
-        assert ledger_enclaves.source_node in ledger_enclaves.quotes
-        for node_id, quote in ledger_enclaves.quotes.items():
-            assert node_id == quote.node_id
-            print(quote.node_id)
-            print(quote.mrenclave)
-            print(quote.raw_quote)
-            print(quote.version)
-        ```
-        
-        [Microsoft Azure Attestation Service](https://azure.microsoft.com/services/azure-attestation/) is one provider of enclave quotes.
-        
-        ### Async API
-        This library includes a complete async API supported on Python 3.5+. To use it, you must first install an async transport, such as [aiohttp](https://pypi.org/project/aiohttp). See the [azure-core documentation](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#transport) for more information.
-        
-        An async client is obtained from `azure.confidentialledger.aio`. Methods have the same names and signatures as the synchronous client.
-        
-        Async clients should be closed when they're no longer needed. These objects are async context managers and define async `close` methods. For example:
-        
-        ```python
-        from azure.identity.aio import DefaultAzureCredential
-        from azure.confidentialledger.aio import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service.aio import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = await identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        
-        # Call close when the client and credential are no longer needed.
-        await client.close()
-        await credential.close()
-        
-        # Alternatively, use them as async context managers (contextlib.AsyncExitStack can help).
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        async with client:
-            async with credential:
-                pass
-        ```
-        
-        #### Asynchronously get a ledger entry
-        Ledger entries may be retrieved with the async client.
-        ```python
-        entry = await self.client.get_ledger_entry()
-        print(entry.contents)
-        print(entry.sub_ledger_id)
-        ```
-        
-        #### Asynchronously get a range of ledger entries
-        Ledger entries may be retrieved over a range with the async client.
-        ```python
-        query_result = client.get_ledger_entries(
-            from_transaction_id="12.3"
-        )
-        async for entry in query_result:
-            print(entry.transaction_id)
-            print(entry.contents)
-        ```
-        
-        ## Troubleshooting
-        ### General
-        Confidential Ledger clients raise exceptions defined in [azure-core][azure_core_exceptions]. For example, if you try to get a transaction that doesn't exist, `ConfidentialLedgerClient` raises [ResourceNotFoundError](https://aka.ms/azsdk-python-core-exceptions-resource-not-found-error):
-        
-        ```python
-        from azure.core.exceptions import ResourceNotFoundError
-        from azure.identity import DefaultAzureCredential
-        from azure.confidentialledger import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        
-        try:
-            ledger_client.get_ledger_entry(transaction_id="10000.100000")
-        except ResourceNotFoundError as e:
-            print(e.message)
-        ```
-        
-        ### Logging
-        This library uses the standard
-        [logging](https://docs.python.org/3.5/library/logging.html) library for logging. Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO level.
-        
-        Detailed DEBUG level logging, including request/response bodies and unredacted headers, can be enabled on a client with the `logging_enable` argument:
-        ```python
-        import logging
-        import sys
-        
-        from azure.identity import DefaultAzureCredential
-        from azure.confidentialledger import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        # Create a logger for the 'azure' SDK
-        logger = logging.getLogger('azure')
-        logger.setLevel(logging.DEBUG)
-        
-        # Configure a console output
-        handler = logging.StreamHandler(stream=sys.stdout)
-        logger.addHandler(handler)
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        
-        # This client will log detailed information about its HTTP sessions, at DEBUG level
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name,
-            logging_enable=True
-        )
-        ```
-        
-        Similarly, `logging_enable` can enable detailed logging for a single operation, even when it isn't enabled for the client:
-        ```python
-        ledger_client.get_ledger_entry(transaction_id="12.3", logging_enable=True)
-        ```
-        
-        ## Next steps
-        ###  Additional Documentation
-        For more extensive documentation on Azure Confidential Ledger, see the
-        [API reference documentation][reference_docs]. You may also read more about Microsoft Research's open-source [Confidential Consortium Framework][ccf].
-        
-        ## Contributing
-        This project welcomes contributions and suggestions. Most contributions require
-        you to agree to a Contributor License Agreement (CLA) declaring that you have
-        the right to, and actually do, grant us the rights to use your contribution.
-        For details, visit https://cla.microsoft.com.
-        
-        When you submit a pull request, a CLA-bot will automatically determine whether
-        you need to provide a CLA and decorate the PR appropriately (e.g., label,
-        comment). Simply follow the instructions provided by the bot. You will only
-        need to do this once across all repos using our CLA.
-        
-        This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct].
-        For more information, see the
-        [Code of Conduct FAQ][code_of_conduct_faq] or
-        contact opencode@microsoft.com with any additional questions or comments.
-        
-        
-        [azure_cli]: https://docs.microsoft.com/cli/azure
-        [azure_cloud_shell]: https://shell.azure.com/bash
-        [azure_confidential_computing]: https://azure.microsoft.com/solutions/confidential-compute
-        [azure_core_exceptions]: https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core#azure-core-library-exceptions
-        [azure_identity]: https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/identity/azure-identity
-        [azure_identity_pypi]: https://pypi.org/project/azure-identity/
-        [azure_resource_manager]: https://docs.microsoft.com/azure/azure-resource-manager/management/overview
-        [azure_sub]: https://azure.microsoft.com/free
-        [ccf]: https://github.com/Microsoft/CCF
-        [code_of_conduct]: https://opensource.microsoft.com/codeofconduct
-        [code_of_conduct_faq]: https://opensource.microsoft.com/codeofconduct/faq
-        [confidential_ledger_client_src]: https://aka.ms/azsdk/python/confidentialledger/src
-        [confidential_ledger_docs]: https://aka.ms/confidentialledger-servicedocs
-        [default_cred_ref]: https://aka.ms/azsdk/python/identity/docs#azure.identity.DefaultAzureCredential
-        [pip]: https://pypi.org/project/pip/
-        [pypi_package_confidential_ledger]: https://aka.ms/azsdk/python/confidentialledger/pypi
-        [reference_docs]: https://aka.ms/azsdk/python/confidentialledger/ref-docs
-        
-        
-        # Release History
-        
-        ## 1.0.0b1 (2021-05-12)
-        
-        - This is the initial release of the Azure Confidential Ledger library.
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Project-URL: Bug Reports, https://github.com/Azure/azure-sdk-for-python/issues
+Project-URL: Source, https://github.com/Azure/azure-sdk-python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Azure Confidential Ledger client library for Python
+
+Azure Confidential Ledger provides a service for logging to an immutable, tamper-proof ledger. As part of the [Azure Confidential Computing][azure_confidential_computing] portfolio, Azure Confidential Ledger runs in secure, hardware-based trusted execution environments, also known as enclaves. It is built on Microsoft Research's [Confidential Consortium Framework][ccf].
+
+[Source code][confidential_ledger_client_src]
+| [Package (PyPI)][pypi_package_confidential_ledger]
+| [Package (Conda)](https://anaconda.org/microsoft/azure-confidentialledger/)
+| [API reference documentation][reference_docs]
+| [Product documentation][confidential_ledger_docs]
+
+## Getting started
+### Install packages
+Install [azure-confidentialledger][pypi_package_confidential_ledger] and [azure-identity][azure_identity_pypi] with [pip][pip]:
+```Bash
+pip install azure-identity azure-confidentialledger
+```
+[azure-identity][azure_identity] is used for Azure Active Directory
+authentication as demonstrated below.
+
+### Prerequisites
+* An [Azure subscription][azure_sub]
+* Python 3.6 or later
+* A running instance of Azure Confidential Ledger.
+* A registered user in the Confidential Ledger, typically assigned during [ARM][azure_resource_manager] resource creation, with `Administrator` privileges.
+
+### Authenticate the client
+#### Using Azure Active Directory
+This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate to the Confidential Ledger via Azure Active Directory. However, `ConfidentialLedgerClient` accepts any [azure-identity][azure_identity] credential. See the [azure-identity][azure_identity] documentation for more information about other credentials.
+
+#### Using a client certificate
+As an alternative to Azure Active Directory, clients may choose to use a client certificate to authenticate via mutual TLS. `azure.confidentialledger.ConfidentialLedgerCertificateCredential` may be used for this purpose.
+
+### Create a client
+`DefaultAzureCredential` will automatically handle most Azure SDK client scenarios. To get started, set environment variables for the AAD identity registered with your Confidential Ledger.
+```bash
+export AZURE_CLIENT_ID="generated app id"
+export AZURE_CLIENT_SECRET="random password"
+export AZURE_TENANT_ID="tenant id"
+```
+Then, `DefaultAzureCredential` will be able to authenticate the `ConfidentialLedgerClient`.
+
+Constructing the client also requires your Confidential Ledger's URL and id, which you can get from the Azure CLI or the Azure Portal. When you have retrieved those values, please replace instances of `"my-ledger-id"` and `"https://my-ledger-id.confidential-ledger.azure.com"` in the examples below. You may also need to replace `"https://identity.confidential-ledger.core.azure.com"` with the hostname from the `identityServiceUri` in the ARM description of your ledger.
+
+Because Confidential Ledgers use self-signed certificates securely generated and stored in an enclave, the signing certificate for each Confidential Ledger must first be retrieved from the Confidential Ledger Identity Service.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+```
+
+Conveniently, the `ConfidentialLedgerClient` constructor will fetch the ledger TLS certificate (and write it to the specified file) if it is provided with a non-existent file. The user is responsible for removing the created file as needed.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.identity import DefaultAzureCredential
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path="ledger_certificate.pem"
+)
+
+# The ledger TLS certificate is written to `ledger_certificate.pem`.
+```
+
+To make it clear that a file is being used for the ledger TLS certificate, subsequent examples will explicitly write the ledger TLS certificate to a file.
+
+## Key concepts
+### Ledger entries and transactions
+Every write to Azure Confidential Ledger generates an immutable ledger entry in the service. Writes, also referred to as transactions, are uniquely identified by transaction ids that increment with each write. Once written, ledger entries may be retrieved at any time.
+
+### Collections
+While most use cases involve just one collection per Confidential Ledger, we provide the collection id feature in case semantically or logically different groups of data need to be stored in the same Confidential Ledger.
+
+Ledger entries are retrieved by their `collectionId`. The Confidential Ledger will always assume a constant, service-determined `collectionId` for entries written without a `collectionId` specified.
+
+### Users
+Users are managed directly with the Confidential Ledger instead of through Azure. Users may be AAD-based, identified by their AAD object id, or certificate-based, identified by their PEM certificate fingerprint.
+
+### Receipts
+
+To enforce transaction integrity guarantees, an Azure Confidential Ledger uses a [Merkle tree][merkle_tree_wiki] data structure to record the hash of all transactions blocks that are appended to the immutable ledger. After a write transaction is committed, Azure Confidential Ledger users can get a cryptographic Merkle proof, or receipt, over the entry produced in a Confidential Ledger to verify that the write operation was correctly saved. A write transaction receipt is proof that the system has committed the corresponding transaction and can be used to verify that the entry has been effectively appended to the ledger.
+
+Please refer to the following [article](https://learn.microsoft.com/azure/confidential-ledger/write-transaction-receipts) for more information about Azure Confidential Ledger write transaction receipts.
+
+### Receipt Verification
+
+After getting a receipt for a write transaction, Azure Confidential Ledger users can verify the contents of the fetched receipt following a verification algorithm. The success of the verification is proof that the write operation associated to the receipt was correctly appended into the immutable ledger.
+
+Please refer to the following [article](https://learn.microsoft.com/azure/confidential-ledger/verify-write-transaction-receipts) for more information about the verification process for Azure Confidential Ledger write transaction receipts.
+
+### Application Claims
+Azure Confidential Ledger applications can attach arbitrary data, called application claims, to write transactions. These claims represent the actions executed during a write operation. When attached to a transaction, the SHA-256 digest of the claims object is included in the ledger and committed as part of the write transaction. This guarantees that the digest is signed in place and cannot be tampered with.
+
+Later, application claims can be revealed in their un-digested form in the receipt payload corresponding to the same transaction where they were added. This allows users to leverage the information in the receipt to re-compute the same claims digest that was attached and signed in place by the Azure Confidential Ledger instance during the transaction. The claims digest can be used as part of the write transaction receipt verification process, providing an offline way for users to fully verify the authenticity of the recorded claims.
+
+More details on the application claims format and the digest computation algorithm can be found at the following links:
+
+- [Azure Confidential Ledger application claims](https://learn.microsoft.com/azure/confidential-ledger/write-transaction-receipts#application-claims)
+- [Azure Confidential Ledger application claims digest verification](https://learn.microsoft.com/azure/confidential-ledger/verify-write-transaction-receipts#verify-application-claims-digest)
+
+Please refer to the following CCF documentation pages for more information about CCF Application claims:
+
+- [Application Claims](https://microsoft.github.io/CCF/main/use_apps/verify_tx.html#application-claims)
+- [User-Defined Claims in Receipts](https://microsoft.github.io/CCF/main/build_apps/example_cpp.html#user-defined-claims-in-receipts)
+
+### Confidential computing
+[Azure Confidential Computing][azure_confidential_computing] allows you to isolate and protect your data while it is being processed in the cloud. Azure Confidential Ledger runs on Azure Confidential Computing virtual machines, thus providing stronger data protection with encryption of data in use.
+
+### Confidential Consortium Framework
+Azure Confidential Ledger is built on Microsoft Research's open-source [Confidential Consortium Framework (CCF)][ccf]. Under CCF, applications are managed by a consortium of members with the ability to submit proposals to modify and govern application operation. In Azure Confidential Ledger, Microsoft Azure owns an operator member identity that allows it to perform governance and maintenance actions like replacing unhealthy nodes in the Confidential Ledger and upgrading the enclave code.
+
+## Examples
+This section contains code snippets covering common tasks, including:
+- [Append entry](#append-entry)
+- [Retrieving ledger entries](#retrieving-ledger-entries)
+- [Making a ranged query](#making-a-ranged-query)
+- [Managing users](#managing-users)
+- [Using certificate authentication](#using-certificate-authentication)
+- [Verify write transaction receipts](#verify-write-transaction-receipts)
+
+### Append entry
+Data that needs to be stored immutably in a tamper-proof manner can be saved to Azure Confidential Ledger by appending an entry to the ledger.
+
+Since Confidential Ledger is a distributed system, rare transient failures may cause writes to be lost. For entries that must be preserved, it is advisable to verify that the write became durable. For less important writes where higher client throughput is preferred, the wait step may be skipped.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_entry_result = ledger_client.create_ledger_entry(
+        {"contents": "Hello world!"}
+    )
+transaction_id = post_entry_result["transactionId"]
+
+wait_poller = ledger_client.begin_wait_for_commit(transaction_id)
+wait_poller.wait()
+print(f'Ledger entry at transaction id {transaction_id} has been committed successfully')
+```
+
+Alternatively, the client may wait for commit when writing a ledger entry.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Hello world again!"}
+)
+new_post_result = post_poller.result()
+print(
+    'The new ledger entry has been committed successfully at transaction id '
+    f'{new_post_result["transactionId"]}'
+)
+```
+
+### Retrieving ledger entries
+Getting ledger entries older than the latest may take some time as the service is loading historical entries, so a poller is provided.
+
+Ledger entries are retrieved by collection. The returned value is the value contained in the specified collection at the point in time identified by the transaction id.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Original hello"}
+)
+post_result = post_poller.result()
+
+post_transaction_id = post_result["transactionId"]
+
+latest_entry = ledger_client.get_current_ledger_entry()
+print(
+    f'Current entry (transaction id = {latest_entry["transactionId"]}) '
+    f'in collection {latest_entry["collectionId"]}: {latest_entry["contents"]}'
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Hello!"}
+)
+post_result = post_poller.result()
+
+get_entry_poller = ledger_client.begin_get_ledger_entry(post_transaction_id)
+older_entry = get_entry_poller.result()
+print(
+    f'Contents of {older_entry["entry"]["collectionId"]} at {post_transaction_id}: {older_entry["entry"]["contents"]}'
+)
+```
+
+### Making a ranged query
+Ledger entries may be retrieved over a range of transaction ids. Entries will only be returned from the default or specified collection.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "First message"}
+)
+first_transaction_id = post_poller.result()["transactionId"]
+
+for i in range(10):
+    ledger_client.create_ledger_entry(
+        {"contents": f"Message {i}"}
+    )
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Last message"}
+)
+last_transaction_id = post_poller.result()["transactionId"]
+
+ranged_result = ledger_client.list_ledger_entries(
+    from_transaction_id=first_transaction_id,
+    to_transaction_id=last_transaction_id,
+)
+for entry in ranged_result:
+    print(f'Contents at {entry["transactionId"]}: {entry["contents"]}')
+```
+
+### Managing users
+Users with `Administrator` privileges can manage users of the Confidential Ledger directly with the Confidential Ledger itself. Available roles are `Reader` (read-only), `Contributor` (read and write), and `Administrator` (read, write, and add or remove users).
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+user_id = "some AAD object id"
+user = ledger_client.create_or_update_user(
+    user_id, {"assignedRole": "Contributor"}
+)
+# A client may now be created and used with AAD credentials (i.e. AAD-issued JWT tokens) for the user identified by `user_id`.
+
+user = ledger_client.get_user(user_id)
+assert user["userId"] == user_id
+assert user["assignedRole"] == "Contributor"
+
+ledger_client.delete_user(user_id)
+
+# For a certificate-based user, their user ID is the fingerprint for their PEM certificate.
+user_id = "PEM certificate fingerprint"
+user = ledger_client.create_or_update_user(
+    user_id, {"assignedRole": "Reader"}
+)
+
+user = ledger_client.get_user(user_id)
+assert user["userId"] == user_id
+assert user["assignedRole"] == "Reader"
+
+ledger_client.delete_user(user_id)
+```
+
+### Using certificate authentication
+Clients may authenticate with a client certificate in mutual TLS instead of via an Azure Active Directory token. `ConfidentialLedgerCertificateCredential` is provided for such clients.
+
+```python
+from azure.confidentialledger import (
+    ConfidentialLedgerCertificateCredential,
+    ConfidentialLedgerClient,
+)
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = ConfidentialLedgerCertificateCredential(
+    certificate_path="Path to user certificate PEM file"
+)
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+```
+
+### Verify write transaction receipts
+
+Clients can leverage the receipt verification library in the SDK to verify write transaction receipts issued by Azure Confidential Legder instances. The utility can be used to fully verify receipts offline as the verification algorithm does not require to be connected to a Confidential ledger or any other Azure service.
+
+Once a new entry has been appended to the ledger (please refer to [this example](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/confidentialledger/azure-confidentialledger#append-entry)), it is possible to get a receipt for the committed write transaction.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+# Replace this with the Confidential Ledger ID 
+ledger_id = "my-ledger-id"
+
+# Setup authentication
+credential = DefaultAzureCredential()
+
+# Create a Ledger Certificate client and use it to
+# retrieve the service identity for our ledger
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id=ledger_id
+)
+
+# Save ledger service certificate into a file for later use
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+# Create Confidential Ledger client
+ledger_client = ConfidentialLedgerClient(
+    endpoint=f"https://{ledger_id}.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+# The method begin_get_receipt returns a poller that
+# we can use to wait for the receipt to be available for retrieval 
+get_receipt_poller = ledger_client.begin_get_receipt(transaction_id)
+get_receipt_result = get_receipt_poller.result()
+
+print(f"Write receipt for transaction id {transaction_id} was successfully retrieved: {get_receipt_result}")
+```
+
+After fetching a receipt for a write transaction, it is possible to call the `verify_receipt` function to verify that the receipt is valid. The function can accept an optional list of application claims to verify against the receipt claims digest.
+
+```python
+from azure.confidentialledger.receipt import (
+    verify_receipt,
+)
+
+# Read contents of service certificate file saved in previous step.
+with open(ledger_tls_cert_file_name, "r") as service_cert_file:
+    service_cert_content = service_cert_file.read()
+
+# Optionally read application claims, if any
+application_claims = get_receipt_result.get("applicationClaims", None) 
+
+try:
+    # Verify the contents of the receipt.
+    verify_receipt(get_receipt_result["receipt"], service_cert_content, application_claims=application_claims)
+    print(f"Receipt for transaction id {transaction_id} successfully verified")
+except ValueError:
+    print(f"Receipt verification for transaction id {transaction_id} failed")
+```
+
+A full sample Python program that shows how to append a new entry to a running Confidential Ledger instance, get a receipt for the committed transaction, and verify the receipt contents can be found under the [samples](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples) folder: [get_and_verify_receipt.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/get_and_verify_receipt.py).
+
+### Async API
+This library includes a complete async API supported on Python 3.5+. To use it, you must first install an async transport, such as [aiohttp](https://pypi.org/project/aiohttp). See the [azure-core documentation](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#transport) for more information.
+
+An async client is obtained from `azure.confidentialledger.aio`. Methods have the same names and signatures as the synchronous client. Samples may be found [here](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples).
+
+## Troubleshooting
+### General
+Confidential Ledger clients raise exceptions defined in [azure-core][azure_core_exceptions]. For example, if you try to get a transaction that doesn't exist, `ConfidentialLedgerClient` raises [ResourceNotFoundError](https://aka.ms/azsdk-python-core-exceptions-resource-not-found-error):
+
+```python
+from azure.core.exceptions import ResourceNotFoundError
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+try:
+    ledger_client.begin_get_ledger_entry(
+        transaction_id="10000.100000"  # Using a very high id that probably doesn't exist in the ledger if it's relatively new.
+    )
+except ResourceNotFoundError as e:
+    print(e.message)
+```
+
+### Logging
+This library uses the standard
+[logging](https://docs.python.org/3.5/library/logging.html) library for logging. Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO level.
+
+Detailed DEBUG level logging, including request/response bodies and unredacted headers, can be enabled on a client with the `logging_enable` argument:
+```python
+import logging
+import sys
+
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+# Create a logger for the 'azure' SDK
+logger = logging.getLogger('azure')
+logger.setLevel(logging.DEBUG)
+
+# Configure a console output
+handler = logging.StreamHandler(stream=sys.stdout)
+logger.addHandler(handler)
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+
+# This client will log detailed information about its HTTP sessions, at DEBUG level.
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name,
+    logging_enable=True,
+)
+```
+
+Similarly, `logging_enable` can enable detailed logging for a single operation, even when it isn't enabled for the client:
+```python
+ledger_client.get_current_ledger_entry(logging_enable=True)
+```
+
+## Next steps
+### More sample code
+These code samples show common scenario operations with the Azure Confidential Ledger client library.
+
+#### Common scenarios
+
+- Writing to the ledger:
+  - [write_to_ledger.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/write_to_ledger.py) 
+  - [write_to_ledger_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/write_to_ledger_async.py) (async version)
+
+- Write many ledger entries and retrieve them all afterwards:
+  - [list_ledger_entries.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/list_ledger_entries.py)
+  - [list_ledger_entries_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/list_ledger_entries_async.py) (async version)
+
+- Manage users using service-implemented role-based access control: 
+  - [manage_users.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/manage_users.py)
+  - [manage_users_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/manage_users_async.py) (async version)
+
+#### Advanced scenarios
+
+- Using collections: 
+  - [use_collections.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/use_collections.py)
+  - [use_collections_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/use_collections_async.py) (async version)
+  
+- Getting receipts for ledger writes: 
+  - [get_receipt.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/get_receipt.py)
+  - [get_receipt_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/get_receipt_async.py) (async version)
+  
+- Verifying service details: 
+  - [verify_service.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/verify_service.py) 
+  - [verify_service_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/verify_service_async.py) (async version)
+
+###  Additional Documentation
+For more extensive documentation on Azure Confidential Ledger, see the
+[API reference documentation][reference_docs]. You may also read more about Microsoft Research's open-source [Confidential Consortium Framework][ccf].
+
+## Contributing
+This project welcomes contributions and suggestions. Most contributions require
+you to agree to a Contributor License Agreement (CLA) declaring that you have
+the right to, and actually do, grant us the rights to use your contribution.
+For details, visit https://cla.microsoft.com.
+
+When you submit a pull request, a CLA-bot will automatically determine whether
+you need to provide a CLA and decorate the PR appropriately (e.g., label,
+comment). Simply follow the instructions provided by the bot. You will only
+need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct].
+For more information, see the
+[Code of Conduct FAQ][code_of_conduct_faq] or
+contact opencode@microsoft.com with any additional questions or comments.
+
+
+[azure_cli]: https://docs.microsoft.com/cli/azure
+[azure_cloud_shell]: https://shell.azure.com/bash
+[azure_confidential_computing]: https://azure.microsoft.com/solutions/confidential-compute
+[azure_core_exceptions]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core#azure-core-library-exceptions
+[azure_identity]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity
+[azure_identity_pypi]: https://pypi.org/project/azure-identity/
+[azure_resource_manager]: https://docs.microsoft.com/azure/azure-resource-manager/management/overview
+[azure_sub]: https://azure.microsoft.com/free
+[ccf]: https://github.com/Microsoft/CCF
+[code_of_conduct]: https://opensource.microsoft.com/codeofconduct
+[code_of_conduct_faq]: https://opensource.microsoft.com/codeofconduct/faq
+[confidential_ledger_client_src]: https://aka.ms/azsdk/python/confidentialledger/src
+[confidential_ledger_docs]: https://aka.ms/confidentialledger-servicedocs
+[default_cred_ref]: https://aka.ms/azsdk/python/identity/docs#azure.identity.DefaultAzureCredential
+[pip]: https://pypi.org/project/pip/
+[pypi_package_confidential_ledger]: https://aka.ms/azsdk/python/confidentialledger/pypi
+[reference_docs]: https://aka.ms/azsdk/python/confidentialledger/ref-docs
+
+
+# Release History
+
+## 1.1.0 (2023-05-09)
+
+### Features Added
+- Add `azure.confidentialledger.receipt` module for Azure Confidential Ledger write transaction receipt verification.
+- Add `verify_receipt` function to verify write transaction receipts from a receipt JSON object. The function accepts an optional, keyword-only, list of application claims parameter, which can be used to compute the claims digest from the given claims: the verification would fail if the computed digest value does not match the `claimsDigest` value present in the receipt.
+- Add `compute_claims_digest` function to compute the claims digest from a list of application claims JSON objects. 
+- Add sample code to get and verify a write receipt from a running Confidential Ledger instance.
+- Update README with examples and documentation for receipt verification and application claims.
+
+### Other Changes
+- Add dependency on Python `cryptography` library (`>= 2.1.4`)
+- Add tests for receipt verification models and receipt verification public method.
+- Add tests for application claims models and digest computation public method.
+
+## 1.0.0 (2022-07-19)
+
+GA Data Plane Python SDK for Confidential Ledger.
+
+### Bugs Fixed
+- User ids that are certificate fingerprints are no longer URL-encoded in the request URI.
+
+### Breaking Changes
+- Removed all models. Methods now return JSON directly.
+- `sub_ledger_id` fields are now named `collection_id`.
+- `azure.confidentialledger.identity_service` has been renamed to `azure.confidentialledger.certificate`.
+- `ConfidentialLedgerIdentityServiceClient` is now `ConfidentialLedgerCertificateClient`.
+- `post_ledger_entry` has been renamed to `create_ledger_entry`.
+
+### Other Changes
+- Python 2.7 is no longer supported. Please use Python version 3.7 or later.
+- Convenience poller methods added for certain long-running operations.
+- Add new supported API version: `2022-05-13`.
+
+## 1.0.0b1 (2021-05-12)
+
+- This is the initial release of the Azure Confidential Ledger library.
```

## Comparing `azure-confidentialledger-1.0.0b1/setup.py` & `azure-confidentialledger-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,73 +11,76 @@
 import re
 from setuptools import setup, find_packages
 
 # example setup.py Feel free to copy the entire "azure-template" folder into a package folder named
 # with "azure-<yourpackagename>". Ensure that the below arguments to setup() are updated to reflect
 # your package.
 
-# this setup.py is set up in a specific way to keep the azure* and azure-mgmt-* namespaces WORKING
-# all the way up from python 2.7.
-# Reference here: https://github.com/Azure/azure-sdk-for-python/wiki/Azure-packaging
-
 PACKAGE_NAME = "azure-confidentialledger"
 PACKAGE_PPRINT_NAME = "Confidential Ledger"
 
 # a-b-c => a/b/c
 PACKAGE_FOLDER_PATH = PACKAGE_NAME.replace("-", "/")
 # a-b-c => a.b.c
 NAMESPACE_NAME = PACKAGE_NAME.replace("-", ".")
 
 # Version extraction inspired from 'requests'
 with open(os.path.join(PACKAGE_FOLDER_PATH, "_version.py"), "r") as fd:
-    VERSION = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
+    VERSION = re.search(
+        r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
+    ).group(1)
 
 if not VERSION:
     raise RuntimeError("Cannot find version information")
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 with open("CHANGELOG.md", encoding="utf-8") as f:
     CHANGELOG = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     include_package_data=True,
-    description="Microsoft Azure {} Client Library for Python".format(PACKAGE_PPRINT_NAME),
-
+    description="Microsoft Azure {} Client Library for Python".format(
+        PACKAGE_PPRINT_NAME
+    ),
     # ensure that these are updated to reflect the package owners' information
     long_description=README + "\n\n" + CHANGELOG,
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="accledgerdevs@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python",
     classifiers=[
-        "Development Status :: 4 - Beta",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
+        "Development Status :: 5 - Production/Stable",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
+    python_requires=">=3.7",
     zip_safe=False,
-    packages=find_packages(exclude=[
-        "tests",
-        # Exclude packages that will be covered by PEP420 or nspkg
-        "azure"
-    ]),
+    packages=find_packages(
+        exclude=[
+            "tests",
+            # Exclude packages that will be covered by PEP420 or nspkg
+            "azure",
+        ]
+    ),
+    package_data={
+        'pytyped': ['py.typed'],
+    },
     install_requires=[
-        "azure-common~=1.1",
-        "azure-core<2.0.0,>=1.2.2",
-        "msrest>=0.5.0",
+        "azure-core<2.0.0,>=1.24.0",
+        "isodate<1.0.0,>=0.6.1",
+        "cryptography>=2.1.4",
     ],
-    extras_require={
-        ":python_version<'3.0'": ["azure-nspkg"],
-        ":python_version<'3.4'": ["enum34>=1.0.4"],
-        ":python_version<'3.5'": ["typing"],
+    project_urls={
+        'Bug Reports': 'https://github.com/Azure/azure-sdk-for-python/issues',
+        'Source': 'https://github.com/Azure/azure-sdk-python',
     }
 )
```

## Comparing `azure-confidentialledger-1.0.0b1/azure_confidentialledger.egg-info/PKG-INFO` & `azure-confidentialledger-1.1.0/azure_confidentialledger.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,499 +1,670 @@
 Metadata-Version: 2.1
 Name: azure-confidentialledger
-Version: 1.0.0b1
+Version: 1.1.0
 Summary: Microsoft Azure Confidential Ledger Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: accledgerdevs@microsoft.com
 License: MIT License
-Description: # Azure Confidential Ledger client library for Python
-        
-        Azure Confidential Ledger provides a service for logging to an immutable, tamper-proof ledger. As part of the [Azure Confidential Computing][azure_confidential_computing] portfolio, Azure Confidential Ledger runs in secure, hardware-based trusted execution environments, also known as enclaves. It is built on Microsoft Research's [Confidential Consortium Framework][ccf].
-        
-        [Source code][confidential_ledger_client_src] | [Package (PyPI)][pypi_package_confidential_ledger] | [API reference documentation][reference_docs] | [Product documentation][confidential_ledger_docs]
-        
-        ## Getting started
-        ### Install packages
-        Install [azure-confidentialledger][pypi_package_confidential_ledger] and [azure-identity][azure_identity_pypi] with [pip][pip]:
-        ```Bash
-        pip install azure-identity azure-confidentialledger
-        ```
-        [azure-identity][azure_identity] is used for Azure Active Directory
-        authentication as demonstrated below.
-        
-        ### Prerequisites
-        * An [Azure subscription][azure_sub]
-        * Python 2.7, 3.5.3, or later
-        * A running instance of Azure Confidential Ledger.
-        * A registered user in the Confidential Ledger, typically assigned during [ARM][azure_resource_manager] resource creation, with `Administrator` privileges.
-        
-        ### Authenticate the client
-        #### Using Azure Active Directory
-        This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate to the Confidential Ledger via Azure Active Directory. However, `ConfidentialLedgerClient` accepts any [azure-identity][azure_identity] credential. See the [azure-identity][azure_identity] documentation for more information about other credentials.
-        
-        #### Using a client certificate
-        As an alternative to Azure Active Directory, clients may choose to use a client certificate to authenticate via mutual TLS. `azure.confidentialledger.ConfidentialLedgerCertificateCredential` may be used for this purpose.
-        
-        ### Create a client
-        `DefaultAzureCredential` will automatically handle most Azure SDK client scenarios. To get started, set environment variables for the AAD identity registered with your Confidential Ledger.
-        ```bash
-        export AZURE_CLIENT_ID="generated app id"
-        export AZURE_CLIENT_SECRET="random password"
-        export AZURE_TENANT_ID="tenant id"
-        ```
-        Then, `DefaultAzureCredential` will be able to authenticate the `ConfidentialLedgerClient`.
-        
-        Constructing the client also requires your Confidential Ledger's URL and id, which you can get from the Azure CLI or the Azure Portal. When you have retrieved those values, please replace instances of `"my-ledger-id"` and `"https://my-ledger-url.confidential-ledger.azure.com"` in the examples below. You may also need to replace `"https://identity.accledger.azure.com"` with the hostname from the `identityServiceUri` in the ARM description of your ledger.
-        
-        Because Confidential Ledgers use self-signed certificates securely generated and stored in an enclave, the signing certificate for each Confidential Ledger must first be retrieved from the Confidential Ledger Identity Service.
-        
-        ```python
-        from azure.identity import DefaultAzureCredential
-        from azure.confidentialledger import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        ```
-        
-        ## Key concepts
-        ### Ledger entries and transactions
-        Every write to Azure Confidential Ledger generates an immutable ledger entry in the service. Writes, also referred to as transactions, are uniquely identified by transaction ids that increment with each write. Once written, ledger entries may be retrieved at any time.
-        
-        ### Receipts
-        State changes to the Confidential Ledger are saved in a data structure called a Merkle tree. To cryptographically verify that writes were correctly saved, a Merkle proof, or receipt, can be retrieved for any transaction id.
-        
-        ### Sub-ledgers
-        While most use cases will involve one ledger, we provide the sub-ledger feature in case semantically or logically different groups of data need to be stored in the same Confidential Ledger.
-        
-        Ledger entries are retrieved by their sub-ledger identifier. The Confidential Ledger will always assume a constant, service-determined sub-ledger id for entries submitted without a sub-ledger specified.
-        
-        ### Users
-        Users are managed directly with the Confidential Ledger instead of through Azure. Users may be AAD-based, identified by their AAD object id, or certificate-based, identified by their PEM certificate fingerprint.
-        
-        ### Confidential computing
-        [Azure Confidential Computing][azure_confidential_computing] allows you to isolate and protect your data while it is being processed in the cloud. Azure Confidential Ledger runs on Azure Confidential Computing virtual machines, thus providing stronger data protection with encryption of data in use.
-        
-        ### Confidential Consortium Framework
-        Azure Confidential Ledger is built on Microsoft Research's open-source [Confidential Consortium Framework (CCF)][ccf]. Under CCF, applications are managed by a consortium of members with the ability to submit proposals to modify and govern application operation. In Azure Confidential Ledger, Microsoft Azure owns a member identity, allowing it to perform governance actions like replacing unhealthy nodes in the Confidential Ledger, or upgrading the enclave code.
-        
-        ## Examples
-        This section contains code snippets covering common tasks:
-        * [Append a ledger entry](#append-entry "Append a ledger entry")
-        * [Get a receipt](#get-receipt "Get a receipt")
-        * [Using sub-ledgers](#using-sub-ledgers "Using sub-ledgers")
-        * [Retrieving ledger entries](#retrieving-ledger-entries "Retrieving ledger entries")
-        * [Making a ranged query](#making-a-ranged-query "Making a ranged query")
-        * [Managing users](#managing-users "Managing users")
-        * [Using certificate authentication](#using-certificate-authentication "Using certificate authentication")
-        * [Verifying service details](#verifying-service-details "Verifying service details")
-        * [Asynchronously get a ledger entry](#asynchronously-get-a-ledger-entry "Asynchronously get a ledger entry")
-        * [Asynchronously get a range of ledger entries](#asynchronously-get-a-range-of-ledger-entries "Asynchronously get a range of ledger entries")
-        
-        
-        ### Append entry
-        Data that needs to be stored immutably in a tamper-proof manner can be saved to Azure Confidential Ledger by appending an entry to the ledger.
-        
-        ```python
-        first_append_result = ledger_client.append_to_ledger(entry_contents="Hello world!")
-        print(first_append_result.transaction_id)
-        ```
-        
-        Since Confidential Ledger is a distributed system, rare transient failures may cause writes to be lost. For entries that must be preserved, it is advisable to verify that the write became durable. Waits are blocking calls.
-        ```python
-        from azure.confidentialledger import TransactionState
-        ledger_client.wait_until_durable(transaction_id=first_append_result.transaction_id)
-        assert ledger_client.get_transaction_status(
-            transaction_id=first_append_result.transaction_id
-        ).state is TransactionState.COMMITTED
-        
-        # Alternatively, a client may wait when appending.
-        append_result = ledger_client.append_to_ledger(
-            entry_contents="Hello world, again!", wait_for_commit=True
-        )
-        assert ledger_client.get_transaction_status(
-            transaction_id=append_result.transaction_id
-        ).state is TransactionState.COMMITTED
-        ```
-        
-        ### Get receipt
-        A receipt can be retrieved for any transaction id to provide cryptographic proof of the contents of the transaction.
-        ```python
-        receipt = ledger_client.get_transaction_receipt(
-            transaction_id=append_result.transaction_id
-        )
-        print(receipt.contents)
-        ```
-        
-        ### Using sub-ledgers
-        Clients can write to different sub-ledgers to separate logically-distinct data.
-        ```python
-        ledger_client.append_to_ledger(
-            entry_contents="Hello from Alice", sub_ledger_id="Alice"
-        )
-        ledger_client.append_to_ledger(
-            entry_contents="Hello from Bob", sub_ledger_id="Bob"
-        )
-        ```
-        
-        When no sub-ledger id is specified on method calls, the Confidential Ledger service will assume a constant, service-determined sub-ledger id.
-        ```python
-        append_result = ledger_client.append_to_ledger(entry_contents="Hello world?", wait_for_commit=True)
-        
-        # The append result contains the sub-ledger id assigned.
-        entry_by_subledger = ledger_client.get_ledger_entry(
-            transaction_id=append_result.transaction_id,
-            sub_ledger_id=append_result.sub_ledger_id
-        )
-        assert entry_by_subledger.contents == "Hello world?"
-        
-        # When a ledger entry is retrieved without a sub-ledger specified,
-        # the service default is used.
-        entry = ledger_client.get_ledger_entry(transaction_id=append_result.transaction_id)
-        assert entry.contents == entry_by_subledger.contents
-        assert entry.sub_ledger_id == entry_by_subledger.sub_ledger_id
-        ```
-        
-        ### Retrieving ledger entries
-        Ledger entries are retrieved from sub-ledgers. When a transaction id is specified, the returned value is the value contained in the specified sub-ledger at the point in time identified by the transaction id. If no transaction id is specified, the latest available value is returned.
-        ```python
-        append_result = ledger_client.append_to_ledger(entry_contents="Hello world 0")
-        ledger_client.append_to_ledger(entry_contents="Hello world 1")
-        
-        subledger_append_result = ledger_client.append_to_ledger(
-            entry_contents="Hello world sub-ledger 0",
-            sub_ledger_id="sub-ledger"
-        )
-        ledger_client.append_to_ledger(
-            entry_contents="Hello world sub-ledger 1",
-            sub_ledger_id="sub-ledger",
-            wait_for_commit=True
-        )
-        
-        # The ledger entry written at 'append_result.transaction_id'
-        # is retrieved from the default sub-ledger.
-        entry = ledger_client.get_ledger_entry(transaction_id=append_result.transaction_id)
-        assert entry.contents == "Hello world 0"
-        
-        # This is the latest entry available in the default sub-ledger.
-        latest_entry = ledger_client.get_ledger_entry()
-        assert latest_entry.contents == "Hello world 1"
-        
-        # The ledger entry written at 'subledger_append_result.transaction_id'
-        # is retrieved from the sub-ledger 'sub-ledger'.
-        subledger_entry = ledger_client.get_ledger_entry(
-            transaction_id=subledger_append_result.transaction_id,
-            sub_ledger_id="sub-ledger"
-        )
-        assert subledger_entry.contents == "Hello world sub-ledger 0"
-        
-        # This is the latest entry available in the sub-ledger 'sub-ledger'.
-        subledger_latest_entry = ledger_client.get_ledger_entry(
-            sub_ledger_id="sub-ledger"
-        )
-        assert subledger_latest_entry.contents == "Hello world sub-ledger 1"
-        ```
-        
-        ### Making a ranged query
-        Ledger entries in a sub-ledger may be retrieved over a range of transaction ids.
-        ```python
-        ranged_result = ledger_client.get_ledger_entries(
-            from_transaction_id=first_append_result.transaction_id
-        )
-        for entry in ranged_result:
-            print(f"Transaction id {entry.transaction_id} contents: {entry.contents}")
-        ```
-        
-        ### Managing users
-        Users with `Administrator` privileges can manage users of the Confidential Ledger directly with the Confidential Ledger itself. Available roles are `Reader` (read-only), `Contributor` (read and write), and `Administrator` (read, write, and add or remove users).
-        
-        ```python
-        from azure.confidentialledger import LedgerUserRole
-        user_id = "some AAD object id"
-        user = ledger_client.create_or_update_user(
-            user_id, LedgerUserRole.CONTRIBUTOR
-        )
-        # A client may now be created and used with AAD credentials for the user identified by `user_id`.
-        
-        user = ledger_client.get_user(user_id)
-        assert user.id == user_id
-        assert user.role == LedgerUserRole.CONTRIBUTOR
-        
-        ledger_client.delete_user(user_id)
-        
-        # For a certificate-based user, their user ID is the fingerprint for their PEM certificate.
-        user_id = "PEM certificate fingerprint"
-        user = ledger_client.create_or_update_user(
-            user_id, LedgerUserRole.READER
-        )
-        ```
-        
-        ### Using certificate authentication
-        Clients may authenticate with a client certificate in mutual TLS instead of via an Azure Active Directory token. `ConfidentialLedgerCertificateCredential` is provided for such clients.
-        ```python
-        from azure.confidentialledger import ConfidentialLedgerClient, ConfidentialLedgerCertificateCredential
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = ConfidentialLedgerCertificateCredential("path to user certificate PEM")
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        ```
-        
-        ### Verifying service details
-        One may want to validate details about the Confidential Ledger for a variety of reasons. For example, you may want to view details about how Microsoft may manage your Confidential Ledger as part of [Confidential Consortium Framework governance](https://microsoft.github.io/CCF/main/governance/index.html), or verify that your Confidential Ledger is indeed running in a secure enclave. A number of client methods are provided for these use cases.
-        ```python
-        consortium = ledger_client.get_consortium()
-        # Consortium members can manage and alter the Confidential Ledger,
-        # such as by replacing unhealthy nodes.
-        for member in consortium.members:
-            print(member.certificate)
-            print(member.id)
-        
-        import hashlib
-        # The constitution is a collection of JavaScript code that
-        # defines actions available to members,
-        # and vets proposals by members to execute those actions.
-        constitution = ledger_client.get_constitution()
-        assert constitution.digest.lower() == \
-            hashlib.sha256(constitution.contents.encode()).hexdigest().lower()
-        print(constitution.contents)
-        print(constitution.digest)
-        
-        # Enclave quotes contain material that can be used to
-        # cryptographically verify the validity and contents
-        # of an enclave.
-        ledger_enclaves = ledger_client.get_enclave_quotes()
-        assert ledger_enclaves.source_node in ledger_enclaves.quotes
-        for node_id, quote in ledger_enclaves.quotes.items():
-            assert node_id == quote.node_id
-            print(quote.node_id)
-            print(quote.mrenclave)
-            print(quote.raw_quote)
-            print(quote.version)
-        ```
-        
-        [Microsoft Azure Attestation Service](https://azure.microsoft.com/services/azure-attestation/) is one provider of enclave quotes.
-        
-        ### Async API
-        This library includes a complete async API supported on Python 3.5+. To use it, you must first install an async transport, such as [aiohttp](https://pypi.org/project/aiohttp). See the [azure-core documentation](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#transport) for more information.
-        
-        An async client is obtained from `azure.confidentialledger.aio`. Methods have the same names and signatures as the synchronous client.
-        
-        Async clients should be closed when they're no longer needed. These objects are async context managers and define async `close` methods. For example:
-        
-        ```python
-        from azure.identity.aio import DefaultAzureCredential
-        from azure.confidentialledger.aio import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service.aio import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = await identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        
-        # Call close when the client and credential are no longer needed.
-        await client.close()
-        await credential.close()
-        
-        # Alternatively, use them as async context managers (contextlib.AsyncExitStack can help).
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        async with client:
-            async with credential:
-                pass
-        ```
-        
-        #### Asynchronously get a ledger entry
-        Ledger entries may be retrieved with the async client.
-        ```python
-        entry = await self.client.get_ledger_entry()
-        print(entry.contents)
-        print(entry.sub_ledger_id)
-        ```
-        
-        #### Asynchronously get a range of ledger entries
-        Ledger entries may be retrieved over a range with the async client.
-        ```python
-        query_result = client.get_ledger_entries(
-            from_transaction_id="12.3"
-        )
-        async for entry in query_result:
-            print(entry.transaction_id)
-            print(entry.contents)
-        ```
-        
-        ## Troubleshooting
-        ### General
-        Confidential Ledger clients raise exceptions defined in [azure-core][azure_core_exceptions]. For example, if you try to get a transaction that doesn't exist, `ConfidentialLedgerClient` raises [ResourceNotFoundError](https://aka.ms/azsdk-python-core-exceptions-resource-not-found-error):
-        
-        ```python
-        from azure.core.exceptions import ResourceNotFoundError
-        from azure.identity import DefaultAzureCredential
-        from azure.confidentialledger import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name
-        )
-        
-        try:
-            ledger_client.get_ledger_entry(transaction_id="10000.100000")
-        except ResourceNotFoundError as e:
-            print(e.message)
-        ```
-        
-        ### Logging
-        This library uses the standard
-        [logging](https://docs.python.org/3.5/library/logging.html) library for logging. Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO level.
-        
-        Detailed DEBUG level logging, including request/response bodies and unredacted headers, can be enabled on a client with the `logging_enable` argument:
-        ```python
-        import logging
-        import sys
-        
-        from azure.identity import DefaultAzureCredential
-        from azure.confidentialledger import ConfidentialLedgerClient
-        from azure.confidentialledger.identity_service import ConfidentialLedgerIdentityServiceClient
-        
-        # Create a logger for the 'azure' SDK
-        logger = logging.getLogger('azure')
-        logger.setLevel(logging.DEBUG)
-        
-        # Configure a console output
-        handler = logging.StreamHandler(stream=sys.stdout)
-        logger.addHandler(handler)
-        
-        identity_client = ConfidentialLedgerIdentityServiceClient("https://identity.accledger.azure.com")
-        network_identity = identity_client.get_ledger_identity(
-            ledger_id="my-ledger-id"
-        )
-        
-        ledger_tls_cert_file_name = "ledger_certificate.pem"
-        with open(ledger_tls_cert_file_name, "w") as cert_file:
-            cert_file.write(network_identity.ledger_tls_certificate)
-        
-        credential = DefaultAzureCredential()
-        
-        # This client will log detailed information about its HTTP sessions, at DEBUG level
-        ledger_client = ConfidentialLedgerClient(
-            endpoint="https://my-ledger-url.confidential-ledger.azure.com", 
-            credential=credential,
-            ledger_certificate_path=ledger_tls_cert_file_name,
-            logging_enable=True
-        )
-        ```
-        
-        Similarly, `logging_enable` can enable detailed logging for a single operation, even when it isn't enabled for the client:
-        ```python
-        ledger_client.get_ledger_entry(transaction_id="12.3", logging_enable=True)
-        ```
-        
-        ## Next steps
-        ###  Additional Documentation
-        For more extensive documentation on Azure Confidential Ledger, see the
-        [API reference documentation][reference_docs]. You may also read more about Microsoft Research's open-source [Confidential Consortium Framework][ccf].
-        
-        ## Contributing
-        This project welcomes contributions and suggestions. Most contributions require
-        you to agree to a Contributor License Agreement (CLA) declaring that you have
-        the right to, and actually do, grant us the rights to use your contribution.
-        For details, visit https://cla.microsoft.com.
-        
-        When you submit a pull request, a CLA-bot will automatically determine whether
-        you need to provide a CLA and decorate the PR appropriately (e.g., label,
-        comment). Simply follow the instructions provided by the bot. You will only
-        need to do this once across all repos using our CLA.
-        
-        This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct].
-        For more information, see the
-        [Code of Conduct FAQ][code_of_conduct_faq] or
-        contact opencode@microsoft.com with any additional questions or comments.
-        
-        
-        [azure_cli]: https://docs.microsoft.com/cli/azure
-        [azure_cloud_shell]: https://shell.azure.com/bash
-        [azure_confidential_computing]: https://azure.microsoft.com/solutions/confidential-compute
-        [azure_core_exceptions]: https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core#azure-core-library-exceptions
-        [azure_identity]: https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/identity/azure-identity
-        [azure_identity_pypi]: https://pypi.org/project/azure-identity/
-        [azure_resource_manager]: https://docs.microsoft.com/azure/azure-resource-manager/management/overview
-        [azure_sub]: https://azure.microsoft.com/free
-        [ccf]: https://github.com/Microsoft/CCF
-        [code_of_conduct]: https://opensource.microsoft.com/codeofconduct
-        [code_of_conduct_faq]: https://opensource.microsoft.com/codeofconduct/faq
-        [confidential_ledger_client_src]: https://aka.ms/azsdk/python/confidentialledger/src
-        [confidential_ledger_docs]: https://aka.ms/confidentialledger-servicedocs
-        [default_cred_ref]: https://aka.ms/azsdk/python/identity/docs#azure.identity.DefaultAzureCredential
-        [pip]: https://pypi.org/project/pip/
-        [pypi_package_confidential_ledger]: https://aka.ms/azsdk/python/confidentialledger/pypi
-        [reference_docs]: https://aka.ms/azsdk/python/confidentialledger/ref-docs
-        
-        
-        # Release History
-        
-        ## 1.0.0b1 (2021-05-12)
-        
-        - This is the initial release of the Azure Confidential Ledger library.
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Project-URL: Bug Reports, https://github.com/Azure/azure-sdk-for-python/issues
+Project-URL: Source, https://github.com/Azure/azure-sdk-python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Azure Confidential Ledger client library for Python
+
+Azure Confidential Ledger provides a service for logging to an immutable, tamper-proof ledger. As part of the [Azure Confidential Computing][azure_confidential_computing] portfolio, Azure Confidential Ledger runs in secure, hardware-based trusted execution environments, also known as enclaves. It is built on Microsoft Research's [Confidential Consortium Framework][ccf].
+
+[Source code][confidential_ledger_client_src]
+| [Package (PyPI)][pypi_package_confidential_ledger]
+| [Package (Conda)](https://anaconda.org/microsoft/azure-confidentialledger/)
+| [API reference documentation][reference_docs]
+| [Product documentation][confidential_ledger_docs]
+
+## Getting started
+### Install packages
+Install [azure-confidentialledger][pypi_package_confidential_ledger] and [azure-identity][azure_identity_pypi] with [pip][pip]:
+```Bash
+pip install azure-identity azure-confidentialledger
+```
+[azure-identity][azure_identity] is used for Azure Active Directory
+authentication as demonstrated below.
+
+### Prerequisites
+* An [Azure subscription][azure_sub]
+* Python 3.6 or later
+* A running instance of Azure Confidential Ledger.
+* A registered user in the Confidential Ledger, typically assigned during [ARM][azure_resource_manager] resource creation, with `Administrator` privileges.
+
+### Authenticate the client
+#### Using Azure Active Directory
+This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate to the Confidential Ledger via Azure Active Directory. However, `ConfidentialLedgerClient` accepts any [azure-identity][azure_identity] credential. See the [azure-identity][azure_identity] documentation for more information about other credentials.
+
+#### Using a client certificate
+As an alternative to Azure Active Directory, clients may choose to use a client certificate to authenticate via mutual TLS. `azure.confidentialledger.ConfidentialLedgerCertificateCredential` may be used for this purpose.
+
+### Create a client
+`DefaultAzureCredential` will automatically handle most Azure SDK client scenarios. To get started, set environment variables for the AAD identity registered with your Confidential Ledger.
+```bash
+export AZURE_CLIENT_ID="generated app id"
+export AZURE_CLIENT_SECRET="random password"
+export AZURE_TENANT_ID="tenant id"
+```
+Then, `DefaultAzureCredential` will be able to authenticate the `ConfidentialLedgerClient`.
+
+Constructing the client also requires your Confidential Ledger's URL and id, which you can get from the Azure CLI or the Azure Portal. When you have retrieved those values, please replace instances of `"my-ledger-id"` and `"https://my-ledger-id.confidential-ledger.azure.com"` in the examples below. You may also need to replace `"https://identity.confidential-ledger.core.azure.com"` with the hostname from the `identityServiceUri` in the ARM description of your ledger.
+
+Because Confidential Ledgers use self-signed certificates securely generated and stored in an enclave, the signing certificate for each Confidential Ledger must first be retrieved from the Confidential Ledger Identity Service.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+```
+
+Conveniently, the `ConfidentialLedgerClient` constructor will fetch the ledger TLS certificate (and write it to the specified file) if it is provided with a non-existent file. The user is responsible for removing the created file as needed.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.identity import DefaultAzureCredential
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path="ledger_certificate.pem"
+)
+
+# The ledger TLS certificate is written to `ledger_certificate.pem`.
+```
+
+To make it clear that a file is being used for the ledger TLS certificate, subsequent examples will explicitly write the ledger TLS certificate to a file.
+
+## Key concepts
+### Ledger entries and transactions
+Every write to Azure Confidential Ledger generates an immutable ledger entry in the service. Writes, also referred to as transactions, are uniquely identified by transaction ids that increment with each write. Once written, ledger entries may be retrieved at any time.
+
+### Collections
+While most use cases involve just one collection per Confidential Ledger, we provide the collection id feature in case semantically or logically different groups of data need to be stored in the same Confidential Ledger.
+
+Ledger entries are retrieved by their `collectionId`. The Confidential Ledger will always assume a constant, service-determined `collectionId` for entries written without a `collectionId` specified.
+
+### Users
+Users are managed directly with the Confidential Ledger instead of through Azure. Users may be AAD-based, identified by their AAD object id, or certificate-based, identified by their PEM certificate fingerprint.
+
+### Receipts
+
+To enforce transaction integrity guarantees, an Azure Confidential Ledger uses a [Merkle tree][merkle_tree_wiki] data structure to record the hash of all transactions blocks that are appended to the immutable ledger. After a write transaction is committed, Azure Confidential Ledger users can get a cryptographic Merkle proof, or receipt, over the entry produced in a Confidential Ledger to verify that the write operation was correctly saved. A write transaction receipt is proof that the system has committed the corresponding transaction and can be used to verify that the entry has been effectively appended to the ledger.
+
+Please refer to the following [article](https://learn.microsoft.com/azure/confidential-ledger/write-transaction-receipts) for more information about Azure Confidential Ledger write transaction receipts.
+
+### Receipt Verification
+
+After getting a receipt for a write transaction, Azure Confidential Ledger users can verify the contents of the fetched receipt following a verification algorithm. The success of the verification is proof that the write operation associated to the receipt was correctly appended into the immutable ledger.
+
+Please refer to the following [article](https://learn.microsoft.com/azure/confidential-ledger/verify-write-transaction-receipts) for more information about the verification process for Azure Confidential Ledger write transaction receipts.
+
+### Application Claims
+Azure Confidential Ledger applications can attach arbitrary data, called application claims, to write transactions. These claims represent the actions executed during a write operation. When attached to a transaction, the SHA-256 digest of the claims object is included in the ledger and committed as part of the write transaction. This guarantees that the digest is signed in place and cannot be tampered with.
+
+Later, application claims can be revealed in their un-digested form in the receipt payload corresponding to the same transaction where they were added. This allows users to leverage the information in the receipt to re-compute the same claims digest that was attached and signed in place by the Azure Confidential Ledger instance during the transaction. The claims digest can be used as part of the write transaction receipt verification process, providing an offline way for users to fully verify the authenticity of the recorded claims.
+
+More details on the application claims format and the digest computation algorithm can be found at the following links:
+
+- [Azure Confidential Ledger application claims](https://learn.microsoft.com/azure/confidential-ledger/write-transaction-receipts#application-claims)
+- [Azure Confidential Ledger application claims digest verification](https://learn.microsoft.com/azure/confidential-ledger/verify-write-transaction-receipts#verify-application-claims-digest)
+
+Please refer to the following CCF documentation pages for more information about CCF Application claims:
+
+- [Application Claims](https://microsoft.github.io/CCF/main/use_apps/verify_tx.html#application-claims)
+- [User-Defined Claims in Receipts](https://microsoft.github.io/CCF/main/build_apps/example_cpp.html#user-defined-claims-in-receipts)
+
+### Confidential computing
+[Azure Confidential Computing][azure_confidential_computing] allows you to isolate and protect your data while it is being processed in the cloud. Azure Confidential Ledger runs on Azure Confidential Computing virtual machines, thus providing stronger data protection with encryption of data in use.
+
+### Confidential Consortium Framework
+Azure Confidential Ledger is built on Microsoft Research's open-source [Confidential Consortium Framework (CCF)][ccf]. Under CCF, applications are managed by a consortium of members with the ability to submit proposals to modify and govern application operation. In Azure Confidential Ledger, Microsoft Azure owns an operator member identity that allows it to perform governance and maintenance actions like replacing unhealthy nodes in the Confidential Ledger and upgrading the enclave code.
+
+## Examples
+This section contains code snippets covering common tasks, including:
+- [Append entry](#append-entry)
+- [Retrieving ledger entries](#retrieving-ledger-entries)
+- [Making a ranged query](#making-a-ranged-query)
+- [Managing users](#managing-users)
+- [Using certificate authentication](#using-certificate-authentication)
+- [Verify write transaction receipts](#verify-write-transaction-receipts)
+
+### Append entry
+Data that needs to be stored immutably in a tamper-proof manner can be saved to Azure Confidential Ledger by appending an entry to the ledger.
+
+Since Confidential Ledger is a distributed system, rare transient failures may cause writes to be lost. For entries that must be preserved, it is advisable to verify that the write became durable. For less important writes where higher client throughput is preferred, the wait step may be skipped.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_entry_result = ledger_client.create_ledger_entry(
+        {"contents": "Hello world!"}
+    )
+transaction_id = post_entry_result["transactionId"]
+
+wait_poller = ledger_client.begin_wait_for_commit(transaction_id)
+wait_poller.wait()
+print(f'Ledger entry at transaction id {transaction_id} has been committed successfully')
+```
+
+Alternatively, the client may wait for commit when writing a ledger entry.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Hello world again!"}
+)
+new_post_result = post_poller.result()
+print(
+    'The new ledger entry has been committed successfully at transaction id '
+    f'{new_post_result["transactionId"]}'
+)
+```
+
+### Retrieving ledger entries
+Getting ledger entries older than the latest may take some time as the service is loading historical entries, so a poller is provided.
+
+Ledger entries are retrieved by collection. The returned value is the value contained in the specified collection at the point in time identified by the transaction id.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Original hello"}
+)
+post_result = post_poller.result()
+
+post_transaction_id = post_result["transactionId"]
+
+latest_entry = ledger_client.get_current_ledger_entry()
+print(
+    f'Current entry (transaction id = {latest_entry["transactionId"]}) '
+    f'in collection {latest_entry["collectionId"]}: {latest_entry["contents"]}'
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Hello!"}
+)
+post_result = post_poller.result()
+
+get_entry_poller = ledger_client.begin_get_ledger_entry(post_transaction_id)
+older_entry = get_entry_poller.result()
+print(
+    f'Contents of {older_entry["entry"]["collectionId"]} at {post_transaction_id}: {older_entry["entry"]["contents"]}'
+)
+```
+
+### Making a ranged query
+Ledger entries may be retrieved over a range of transaction ids. Entries will only be returned from the default or specified collection.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "First message"}
+)
+first_transaction_id = post_poller.result()["transactionId"]
+
+for i in range(10):
+    ledger_client.create_ledger_entry(
+        {"contents": f"Message {i}"}
+    )
+
+post_poller = ledger_client.begin_create_ledger_entry(
+    {"contents": "Last message"}
+)
+last_transaction_id = post_poller.result()["transactionId"]
+
+ranged_result = ledger_client.list_ledger_entries(
+    from_transaction_id=first_transaction_id,
+    to_transaction_id=last_transaction_id,
+)
+for entry in ranged_result:
+    print(f'Contents at {entry["transactionId"]}: {entry["contents"]}')
+```
+
+### Managing users
+Users with `Administrator` privileges can manage users of the Confidential Ledger directly with the Confidential Ledger itself. Available roles are `Reader` (read-only), `Contributor` (read and write), and `Administrator` (read, write, and add or remove users).
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+user_id = "some AAD object id"
+user = ledger_client.create_or_update_user(
+    user_id, {"assignedRole": "Contributor"}
+)
+# A client may now be created and used with AAD credentials (i.e. AAD-issued JWT tokens) for the user identified by `user_id`.
+
+user = ledger_client.get_user(user_id)
+assert user["userId"] == user_id
+assert user["assignedRole"] == "Contributor"
+
+ledger_client.delete_user(user_id)
+
+# For a certificate-based user, their user ID is the fingerprint for their PEM certificate.
+user_id = "PEM certificate fingerprint"
+user = ledger_client.create_or_update_user(
+    user_id, {"assignedRole": "Reader"}
+)
+
+user = ledger_client.get_user(user_id)
+assert user["userId"] == user_id
+assert user["assignedRole"] == "Reader"
+
+ledger_client.delete_user(user_id)
+```
+
+### Using certificate authentication
+Clients may authenticate with a client certificate in mutual TLS instead of via an Azure Active Directory token. `ConfidentialLedgerCertificateCredential` is provided for such clients.
+
+```python
+from azure.confidentialledger import (
+    ConfidentialLedgerCertificateCredential,
+    ConfidentialLedgerClient,
+)
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = ConfidentialLedgerCertificateCredential(
+    certificate_path="Path to user certificate PEM file"
+)
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+```
+
+### Verify write transaction receipts
+
+Clients can leverage the receipt verification library in the SDK to verify write transaction receipts issued by Azure Confidential Legder instances. The utility can be used to fully verify receipts offline as the verification algorithm does not require to be connected to a Confidential ledger or any other Azure service.
+
+Once a new entry has been appended to the ledger (please refer to [this example](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/confidentialledger/azure-confidentialledger#append-entry)), it is possible to get a receipt for the committed write transaction.
+
+```python
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+# Replace this with the Confidential Ledger ID 
+ledger_id = "my-ledger-id"
+
+# Setup authentication
+credential = DefaultAzureCredential()
+
+# Create a Ledger Certificate client and use it to
+# retrieve the service identity for our ledger
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id=ledger_id
+)
+
+# Save ledger service certificate into a file for later use
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+# Create Confidential Ledger client
+ledger_client = ConfidentialLedgerClient(
+    endpoint=f"https://{ledger_id}.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+# The method begin_get_receipt returns a poller that
+# we can use to wait for the receipt to be available for retrieval 
+get_receipt_poller = ledger_client.begin_get_receipt(transaction_id)
+get_receipt_result = get_receipt_poller.result()
+
+print(f"Write receipt for transaction id {transaction_id} was successfully retrieved: {get_receipt_result}")
+```
+
+After fetching a receipt for a write transaction, it is possible to call the `verify_receipt` function to verify that the receipt is valid. The function can accept an optional list of application claims to verify against the receipt claims digest.
+
+```python
+from azure.confidentialledger.receipt import (
+    verify_receipt,
+)
+
+# Read contents of service certificate file saved in previous step.
+with open(ledger_tls_cert_file_name, "r") as service_cert_file:
+    service_cert_content = service_cert_file.read()
+
+# Optionally read application claims, if any
+application_claims = get_receipt_result.get("applicationClaims", None) 
+
+try:
+    # Verify the contents of the receipt.
+    verify_receipt(get_receipt_result["receipt"], service_cert_content, application_claims=application_claims)
+    print(f"Receipt for transaction id {transaction_id} successfully verified")
+except ValueError:
+    print(f"Receipt verification for transaction id {transaction_id} failed")
+```
+
+A full sample Python program that shows how to append a new entry to a running Confidential Ledger instance, get a receipt for the committed transaction, and verify the receipt contents can be found under the [samples](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples) folder: [get_and_verify_receipt.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/get_and_verify_receipt.py).
+
+### Async API
+This library includes a complete async API supported on Python 3.5+. To use it, you must first install an async transport, such as [aiohttp](https://pypi.org/project/aiohttp). See the [azure-core documentation](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#transport) for more information.
+
+An async client is obtained from `azure.confidentialledger.aio`. Methods have the same names and signatures as the synchronous client. Samples may be found [here](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples).
+
+## Troubleshooting
+### General
+Confidential Ledger clients raise exceptions defined in [azure-core][azure_core_exceptions]. For example, if you try to get a transaction that doesn't exist, `ConfidentialLedgerClient` raises [ResourceNotFoundError](https://aka.ms/azsdk-python-core-exceptions-resource-not-found-error):
+
+```python
+from azure.core.exceptions import ResourceNotFoundError
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name
+)
+
+try:
+    ledger_client.begin_get_ledger_entry(
+        transaction_id="10000.100000"  # Using a very high id that probably doesn't exist in the ledger if it's relatively new.
+    )
+except ResourceNotFoundError as e:
+    print(e.message)
+```
+
+### Logging
+This library uses the standard
+[logging](https://docs.python.org/3.5/library/logging.html) library for logging. Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO level.
+
+Detailed DEBUG level logging, including request/response bodies and unredacted headers, can be enabled on a client with the `logging_enable` argument:
+```python
+import logging
+import sys
+
+from azure.confidentialledger import ConfidentialLedgerClient
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.identity import DefaultAzureCredential
+
+# Create a logger for the 'azure' SDK
+logger = logging.getLogger('azure')
+logger.setLevel(logging.DEBUG)
+
+# Configure a console output
+handler = logging.StreamHandler(stream=sys.stdout)
+logger.addHandler(handler)
+
+identity_client = ConfidentialLedgerCertificateClient()
+network_identity = identity_client.get_ledger_identity(
+    ledger_id="my-ledger-id"
+)
+
+ledger_tls_cert_file_name = "ledger_certificate.pem"
+with open(ledger_tls_cert_file_name, "w") as cert_file:
+    cert_file.write(network_identity["ledgerTlsCertificate"])
+
+credential = DefaultAzureCredential()
+
+# This client will log detailed information about its HTTP sessions, at DEBUG level.
+ledger_client = ConfidentialLedgerClient(
+    endpoint="https://my-ledger-id.confidential-ledger.azure.com",
+    credential=credential,
+    ledger_certificate_path=ledger_tls_cert_file_name,
+    logging_enable=True,
+)
+```
+
+Similarly, `logging_enable` can enable detailed logging for a single operation, even when it isn't enabled for the client:
+```python
+ledger_client.get_current_ledger_entry(logging_enable=True)
+```
+
+## Next steps
+### More sample code
+These code samples show common scenario operations with the Azure Confidential Ledger client library.
+
+#### Common scenarios
+
+- Writing to the ledger:
+  - [write_to_ledger.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/write_to_ledger.py) 
+  - [write_to_ledger_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/write_to_ledger_async.py) (async version)
+
+- Write many ledger entries and retrieve them all afterwards:
+  - [list_ledger_entries.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/list_ledger_entries.py)
+  - [list_ledger_entries_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/list_ledger_entries_async.py) (async version)
+
+- Manage users using service-implemented role-based access control: 
+  - [manage_users.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/manage_users.py)
+  - [manage_users_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/manage_users_async.py) (async version)
+
+#### Advanced scenarios
+
+- Using collections: 
+  - [use_collections.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/use_collections.py)
+  - [use_collections_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/use_collections_async.py) (async version)
+  
+- Getting receipts for ledger writes: 
+  - [get_receipt.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/get_receipt.py)
+  - [get_receipt_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/get_receipt_async.py) (async version)
+  
+- Verifying service details: 
+  - [verify_service.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/verify_service.py) 
+  - [verify_service_async.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/confidentialledger/azure-confidentialledger/samples/verify_service_async.py) (async version)
+
+###  Additional Documentation
+For more extensive documentation on Azure Confidential Ledger, see the
+[API reference documentation][reference_docs]. You may also read more about Microsoft Research's open-source [Confidential Consortium Framework][ccf].
+
+## Contributing
+This project welcomes contributions and suggestions. Most contributions require
+you to agree to a Contributor License Agreement (CLA) declaring that you have
+the right to, and actually do, grant us the rights to use your contribution.
+For details, visit https://cla.microsoft.com.
+
+When you submit a pull request, a CLA-bot will automatically determine whether
+you need to provide a CLA and decorate the PR appropriately (e.g., label,
+comment). Simply follow the instructions provided by the bot. You will only
+need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct].
+For more information, see the
+[Code of Conduct FAQ][code_of_conduct_faq] or
+contact opencode@microsoft.com with any additional questions or comments.
+
+
+[azure_cli]: https://docs.microsoft.com/cli/azure
+[azure_cloud_shell]: https://shell.azure.com/bash
+[azure_confidential_computing]: https://azure.microsoft.com/solutions/confidential-compute
+[azure_core_exceptions]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core#azure-core-library-exceptions
+[azure_identity]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity
+[azure_identity_pypi]: https://pypi.org/project/azure-identity/
+[azure_resource_manager]: https://docs.microsoft.com/azure/azure-resource-manager/management/overview
+[azure_sub]: https://azure.microsoft.com/free
+[ccf]: https://github.com/Microsoft/CCF
+[code_of_conduct]: https://opensource.microsoft.com/codeofconduct
+[code_of_conduct_faq]: https://opensource.microsoft.com/codeofconduct/faq
+[confidential_ledger_client_src]: https://aka.ms/azsdk/python/confidentialledger/src
+[confidential_ledger_docs]: https://aka.ms/confidentialledger-servicedocs
+[default_cred_ref]: https://aka.ms/azsdk/python/identity/docs#azure.identity.DefaultAzureCredential
+[pip]: https://pypi.org/project/pip/
+[pypi_package_confidential_ledger]: https://aka.ms/azsdk/python/confidentialledger/pypi
+[reference_docs]: https://aka.ms/azsdk/python/confidentialledger/ref-docs
+
+
+# Release History
+
+## 1.1.0 (2023-05-09)
+
+### Features Added
+- Add `azure.confidentialledger.receipt` module for Azure Confidential Ledger write transaction receipt verification.
+- Add `verify_receipt` function to verify write transaction receipts from a receipt JSON object. The function accepts an optional, keyword-only, list of application claims parameter, which can be used to compute the claims digest from the given claims: the verification would fail if the computed digest value does not match the `claimsDigest` value present in the receipt.
+- Add `compute_claims_digest` function to compute the claims digest from a list of application claims JSON objects. 
+- Add sample code to get and verify a write receipt from a running Confidential Ledger instance.
+- Update README with examples and documentation for receipt verification and application claims.
+
+### Other Changes
+- Add dependency on Python `cryptography` library (`>= 2.1.4`)
+- Add tests for receipt verification models and receipt verification public method.
+- Add tests for application claims models and digest computation public method.
+
+## 1.0.0 (2022-07-19)
+
+GA Data Plane Python SDK for Confidential Ledger.
+
+### Bugs Fixed
+- User ids that are certificate fingerprints are no longer URL-encoded in the request URI.
+
+### Breaking Changes
+- Removed all models. Methods now return JSON directly.
+- `sub_ledger_id` fields are now named `collection_id`.
+- `azure.confidentialledger.identity_service` has been renamed to `azure.confidentialledger.certificate`.
+- `ConfidentialLedgerIdentityServiceClient` is now `ConfidentialLedgerCertificateClient`.
+- `post_ledger_entry` has been renamed to `create_ledger_entry`.
+
+### Other Changes
+- Python 2.7 is no longer supported. Please use Python version 3.7 or later.
+- Convenience poller methods added for certain long-running operations.
+- Add new supported API version: `2022-05-13`.
+
+## 1.0.0b1 (2021-05-12)
+
+- This is the initial release of the Azure Confidential Ledger library.
```

## Comparing `azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_certificate_async.py` & `azure-confidentialledger-1.1.0/tests/test_identity_service_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from azure.confidentialledger import (
-    ConfidentialLedgerCertificateCredential,
+from devtools_testutils import AzureRecordedTestCase, recorded_by_proxy
+
+from azure.confidentialledger.certificate import (
+    ConfidentialLedgerCertificateClient,
 )
-from azure.confidentialledger.aio import ConfidentialLedgerClient
 
-from _shared.client_test_common_async import AsyncConfidentialLedgerClientTestMixin
+from _shared.testcase import ConfidentialLedgerPreparer
+
 
+class TestConfidentialLedgerCertificateClient(AzureRecordedTestCase):
+    @ConfidentialLedgerPreparer()
+    @recorded_by_proxy
+    def test_get_ledger_identity(self, **kwargs):
+        confidentialledger_id = kwargs.pop("confidentialledger_id")
 
-class AsyncCertificateCredentialClientTest(
-    AsyncConfidentialLedgerClientTestMixin.AsyncBaseTest
-):
-    def setUp(self):
-        super(AsyncCertificateCredentialClientTest, self).setUp()
-        self.client = self.create_client_from_credential(
-            ConfidentialLedgerClient,
-            credential=ConfidentialLedgerCertificateCredential(
-                self.user_certificate_path
-            ),
-            ledger_certificate_path=self.network_certificate_path,
-            endpoint=self.confidential_ledger_url,
+        client = self.create_client_from_credential(
+            ConfidentialLedgerCertificateClient,
+            credential=None,
         )
+
+        network_identity = (
+            client.get_ledger_identity(
+                ledger_id=confidentialledger_id
+            )
+        )
+
+        assert network_identity["ledgerId"] == confidentialledger_id
+        assert network_identity["ledgerTlsCertificate"]
```

## Comparing `azure-confidentialledger-1.0.0b1/tests/test_confidential_ledger_client_aad.py` & `azure-confidentialledger-1.1.0/tests/test_identity_service_client_async.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from azure.confidentialledger import (
-    ConfidentialLedgerClient,
-    ConfidentialLedgerCertificateCredential,
-    LedgerUserRole,
-)
+from devtools_testutils import AzureRecordedTestCase
+from devtools_testutils.aio import recorded_by_proxy_async
 
-from _shared.client_test_common import ConfidentialLedgerClientTestMixin
+from azure.confidentialledger.certificate.aio import (
+    ConfidentialLedgerCertificateClient,
+)
 
-AAD_USER_OBJECT_ID = "a" * 36
+from _shared.testcase import ConfidentialLedgerPreparer
 
 
-class AadCredentialClientTest(ConfidentialLedgerClientTestMixin.BaseTest):
-    def setUp(self):
-        super(AadCredentialClientTest, self).setUp()
-        self.client = self.create_client_from_credential(
-            ConfidentialLedgerClient,
-            credential=self.get_credential(ConfidentialLedgerClient),
-            ledger_certificate_path=self.network_certificate_path,
-            endpoint=self.confidential_ledger_url,
-        )
+class TestConfidentialLedgerCertificateClient(AzureRecordedTestCase):
+    @ConfidentialLedgerPreparer()
+    @recorded_by_proxy_async
+    async def test_get_ledger_identity(self, **kwargs):
+        confidentialledger_id = kwargs.pop("confidentialledger_id")
 
         client = self.create_client_from_credential(
-            ConfidentialLedgerClient,
-            credential=ConfidentialLedgerCertificateCredential(
-                self.user_certificate_path
-            ),
-            ledger_certificate_path=self.network_certificate_path,
-            endpoint=self.confidential_ledger_url,
+            ConfidentialLedgerCertificateClient,
+            credential=None,
         )
 
-        aad_object_id = self.set_value_to_scrub(
-            "CONFIDENTIAL_LEDGER_AAD_USER_OBJECT_ID", AAD_USER_OBJECT_ID
-        )
-        client.create_or_update_user(aad_object_id, LedgerUserRole.ADMINISTRATOR)
+        try:
+            network_identity = (
+                await client.get_ledger_identity(
+                    ledger_id=confidentialledger_id
+                )
+            )
+
+            assert network_identity["ledgerId"] == confidentialledger_id
+            assert network_identity["ledgerTlsCertificate"]
+        finally:
+            await client.close()
```

## Comparing `azure-confidentialledger-1.0.0b1/tests/_shared/constants.py` & `azure-confidentialledger-1.1.0/tests/_shared/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 
-NETWORK_CERTIFICATE = """-----BEGIN CERTIFICATE-----
-MIIBezCCASGgAwIBAgIRAL/+TT7iOY+UWa5Uh484vRYwCgYIKoZIzj0EAwIwFjEU
-MBIGA1UEAwwLQ0NGIE5ldHdvcmswHhcNMjEwMzExMDAwMDAwWhcNMjMwNjExMjM1
-OTU5WjAWMRQwEgYDVQQDDAtDQ0YgTmV0d29yazBZMBMGByqGSM49AgEGCCqGSM49
-AwEHA0IABG4t5blH9yUsJB4Ywm0VcsxxiFTdiWffd4w+m8r3GRfV0i6qaHT44dVK
-rMQH7ymSGCtz5PHqUQhy8ZJWAepDDKijUDBOMAwGA1UdEwQFMAMBAf8wHQYDVR0O
-BBYEFD+OVuRiS6dJICYtesS2Shx/KIEEMB8GA1UdIwQYMBaAFD+OVuRiS6dJICYt
-esS2Shx/KIEEMAoGCCqGSM49BAMCA0gAMEUCICrLXfKPC1DmKdcTKnZwhiEoPvMi
-RboMeODv/0hlL67gAiEA5gvNwskSiYefETGihWTouTqL+uyhDb4s3/R5XcIHaQQ=
------END CERTIFICATE-----"""
+import os
+
+TEST_PROXY_CERT = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "..", "..", "..", "..", 'eng', 'common', 'testproxy', 'dotnet-devcert.crt'))
 
 # Duplicate certificate from KeyVault.
-# https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/keyvault/azure-keyvault-certificates/tests/ca.crt
-# https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/keyvault/azure-keyvault-certificates/tests/ca.key
-USER_CERTIFICATE = """-----BEGIN CERTIFICATE-----
+# https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/keyvault/azure-keyvault-certificates/tests/ca.crt
+USER_CERTIFICATE_PUBLIC_KEY = """-----BEGIN CERTIFICATE-----
 MIIDazCCAlOgAwIBAgIUYju9zymmCCF7rCaROzfZs0pNgmkwDQYJKoZIhvcNAQEL
 BQAwRTELMAkGA1UEBhMCQVUxEzARBgNVBAgMClNvbWUtU3RhdGUxITAfBgNVBAoM
 GEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZDAeFw0xOTA4MjgyMjU0MTNaFw0xOTA5
 MjcyMjU0MTNaMEUxCzAJBgNVBAYTAkFVMRMwEQYDVQQIDApTb21lLVN0YXRlMSEw
 HwYDVQQKDBhJbnRlcm5ldCBXaWRnaXRzIFB0eSBMdGQwggEiMA0GCSqGSIb3DQEB
 AQUAA4IBDwAwggEKAoIBAQD0YrMz5atoPmTTxLtCO69kM3E97bdjJgyAVZJS9mP3
 HQyHkFNb09eDeAAzcZLR5nYXX7yweowTWVcIe3k9+Z/tUeVrAlOVe2COaIHAUZIh
@@ -33,17 +25,19 @@
 fFNfTnqFggB0gzAPBgNVHRMBAf8EBTADAQH/MA0GCSqGSIb3DQEBCwUAA4IBAQAr
 +RM7gbqWRXnWJwE/hV/ZI2hXAhDN4RYQ4fWMJfg/E9wcLeqqRtJhXbqpJW08IZWp
 QKcWfrFcfZ3ZxVAi5Ey+iuvD2VeBf9v5RZI4c9JqswS9xG2A1x/BeGcUk1y/q9E5
 4whf5fLSJQVxK+C53yemoHPrBg8zVhLJv5SG7Uw7jcqiQvu2aHGGWPLiO7mmMPtP
 qO/I+6FjXuBpNomTqM897MY3Qzg43rpoCilpOpkRtMHknfhFxt05p+Fn73Fb60ru
 ZsFRA52lsEBxGmI0QmXGjwkUZFwQTXEDUWwId3VJxoHRZwv1gmHfwhkYt+mNWJDa
 mU7AMDzlQRwGC8hpWJRT
------END CERTIFICATE-----
------BEGIN RSA PRIVATE KEY-----
-MIIEpQIBAAKCAQEA9GKzM+WraD5k08S7QjuvZDNxPe23YyYMgFWSUvZj9x0Mh5BT
+-----END CERTIFICATE-----"""
+
+# https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/keyvault/azure-keyvault-certificates/tests/ca.key
+USER_CERTIFICATE_PRIVATE_KEY = ("-----BEGIN RSA PRIVATE KEY-----\n"  #[SuppressMessage("Microsoft.Security", "CS001:SecretInline", Justification="Test secret that is found elsewhere in this repo")]
+"""MIIEpQIBAAKCAQEA9GKzM+WraD5k08S7QjuvZDNxPe23YyYMgFWSUvZj9x0Mh5BT
 W9PXg3gAM3GS0eZ2F1+8sHqME1lXCHt5Pfmf7VHlawJTlXtgjmiBwFGSIYxC6v7v
 Nue//DKqmyl4bMq1jQFQ8ip3Q4L224MTbFE2zKAHvQQi/+X86MLJzy2giDAmEWkC
 VMkmyKE5iotdYRdPQhRUpC/Z730DgxchHXuiRz1q1UbHtpYqDyyXgvS6FBjTWZ26
 q8vlGx6eLzkT6ejkE6gU5tWVVj8wrmLllJhHtuyu84IRCa/2MdDi6vZCOR/etAkj
 pHYbDk3AZDkX4Yr0kJ5jp9kZwjyBLFE848FzWQIDAQABAoIBAHrhegv5SrOy083r
 mODX0/wFJcam1dRD2HtbC6UtgNxLPfaYKmH85duUJj23uMRUJkLgf6cZJ3+/J1T7
 iN4Ru0mAKWQiGlcKX2WbxMon+dtmhGtW3n90DgPIkiJMuuGxF5Kb+9CYa7mFi4ya
@@ -60,8 +54,12 @@
 /L9pt8kVqiY2Zw3C49h3gVdR6hKD/Z3AZhKdfDJHEbfd7sHTCRgykQmQXFgBI2QK
 pguboJ627atjODB3sGWrqMUCgYEA2QoJ3lsNYqM/8TpaQQGuOaSPVK+5uOyakyLN
 XqzGwGFWXiFfEz2u/m+wfpZCPIQLV4WuAYAbrb+1D6WmYwPiLESVs8DKwY2Vt3tg
 mc9SIC5CdqRKqIkoto264Qf82En6xXB2Q0qxe2+z8ZWhNfv1nDYEE9FeevNCx76F
 VCVbHXkCgYEA4+FD1q6iwl9wsAOKFVo+W044/MhKHDsyIED3YOzeRTAWRl2w/KX0
 c5ty2KecGu0cVXoAv2YUttHsuMZfm/QdosZr9UB4CR2lmzRys3LSx6QzCkZeMb/s
 QOMs6SYCPXggdXCAu9EVf5+TtYQg7aQNTTuYErlyq2g/tk3un8bHTwI=
------END RSA PRIVATE KEY-----"""
+-----END RSA PRIVATE KEY-----""")
+
+USER_CERTIFICATE = f"{USER_CERTIFICATE_PUBLIC_KEY}\n{USER_CERTIFICATE_PRIVATE_KEY}"
+
+USER_CERTIFICATE_THUMBPRINT = "5F:23:3D:26:E2:28:88:9C:06:E0:88:21:FA:C7:B2:9A:F8:81:30:6B:F9:15:41:F2:34:05:05:44:4C:AD:5A:B5"
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_client_base.py` & `azure-confidentialledger-1.1.0/samples/list_ledger_entries_async.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,120 @@
-# ------------------------------------
-# Copyright (c) Microsoft Corporation.
-# Licensed under the MIT License.
-# ------------------------------------
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+"""
+FILE: list_ledger_entries_async.py
+DESCRIPTION:
+    This sample demonstrates how to iteratively retrieve a batch of ledger entries. In this sample,
+    we write many ledger entries before retrieving them at once.
+USAGE:
+    python list_ledger_entries_async.py
+    Set the environment variables with your own values before running the sample:
+    1) CONFIDENTIALLEDGER_ENDPOINT - the endpoint of the Confidential Ledger.
+"""
+
+import asyncio
+import logging
+import os
+import sys
+import tempfile
+
+from azure.confidentialledger.aio import ConfidentialLedgerClient
+from azure.confidentialledger.certificate.aio import (
+    ConfidentialLedgerCertificateClient,
+)
+from azure.identity.aio import DefaultAzureCredential
 
-from azure.core.pipeline.policies import BearerTokenCredentialPolicy, HttpLoggingPolicy
 
-from ._generated._generated_ledger.v0_1_preview import (
-    ConfidentialLedgerClient as _ConfidentialLedgerClient,
-)
-from ._shared import ConfidentialLedgerCertificateCredential, DEFAULT_VERSION
-from ._user_agent import USER_AGENT
+logging.basicConfig(level=logging.ERROR)
+LOG = logging.getLogger()
+
+
+async def main():
+    # Set the values of the client ID, tenant ID, and client secret of the AAD application as
+    # environment variables:
+    #   AZURE_CLIENT_ID, AZURE_TENANT_ID, AZURE_CLIENT_SECRET, CONFIDENTIALLEDGER_ENDPOINT
+    try:
+        ledger_endpoint = os.environ["CONFIDENTIALLEDGER_ENDPOINT"]
+    except KeyError:
+        LOG.error(
+            "Missing environment variable 'CONFIDENTIALLEDGER_ENDPOINT' - "
+            "please set it before running the example"
+        )
+        sys.exit(1)
 
-try:
-    from typing import TYPE_CHECKING
-except ImportError:
-    TYPE_CHECKING = False
-
-if TYPE_CHECKING:
-    from azure.core.credentials import TokenCredential
-    from typing import Any, Union
-
-
-class ConfidentialLedgerClientBase(object):
-    def __init__(self, endpoint, credential, ledger_certificate_path, **kwargs):
-        # type: (str, Union[ConfidentialLedgerCertificateCredential, TokenCredential], str, Any) -> None
-
-        client = kwargs.get("generated_client")
-        if client:
-            # caller provided a configured client -> nothing left to initialize
-            self._client = client
-            return
-
-        if not endpoint:
-            raise ValueError("Expected endpoint to be a non-empty string")
-
-        if not credential:
-            raise ValueError("Expected credential to not be None")
-
-        if not isinstance(ledger_certificate_path, str):
-            raise TypeError("ledger_certificate_path must be a string")
-
-        if ledger_certificate_path == "":
-            raise ValueError(
-                "If not None, ledger_certificate_path must be a non-empty string"
-            )
-
-        try:
-            endpoint = endpoint.strip(" /")
-            if not endpoint.startswith("https://"):
-                self._endpoint = "https://" + endpoint
-            else:
-                self._endpoint = endpoint
-        except AttributeError:
-            raise ValueError("Confidential Ledger URL must be a string.")
-
-        self.api_version = kwargs.pop("api_version", DEFAULT_VERSION)
-
-        if not kwargs.get("transport", None):
-            # Customize the transport layer to use client certificate authentication and validate
-            # a self-signed TLS certificate.
-            if isinstance(credential, ConfidentialLedgerCertificateCredential):
-                kwargs["connection_cert"] = credential.certificate_path
-
-            kwargs["connection_verify"] = ledger_certificate_path
-
-        http_logging_policy = HttpLoggingPolicy(**kwargs)
-        http_logging_policy.allowed_header_names.update(
-            {
-                "x-ms-keyvault-network-info",
-                "x-ms-keyvault-region",
-                "x-ms-keyvault-service-version",
-            }
+    # Under the current URI format, the ledger id is the first part of the ledger endpoint.
+    # i.e. https://<ledger id>.confidential-ledger.azure.com
+    ledger_id = ledger_endpoint.replace("https://", "").split(".")[0]
+
+    identity_service_client = ConfidentialLedgerCertificateClient()
+    async with identity_service_client:
+        ledger_certificate = await identity_service_client.get_ledger_identity(
+            ledger_id
         )
 
-        if not isinstance(credential, ConfidentialLedgerCertificateCredential):
-            kwargs["authentication_policy"] = kwargs.pop(
-                "authentication_policy",
-                BearerTokenCredentialPolicy(
-                    credential,
-                    "https://confidential-ledger.azure.com/.default",
-                    **kwargs
-                ),
-            )
-
-        try:
-            self._client = _ConfidentialLedgerClient(
-                self._endpoint,
-                api_version=self.api_version,
-                http_logging_policy=http_logging_policy,
-                sdk_moniker=USER_AGENT,
-                **kwargs
-            )
-        except NotImplementedError:
-            raise NotImplementedError(
-                "This package doesn't support API version '{}'. ".format(
-                    self.api_version
+    # The Confidential Ledger's TLS certificate must be written to a file to be used by the
+    # ConfidentialLedgerClient. Here, we write it to a temporary file so that is is cleaned up
+    # automatically when the program exits.
+    with tempfile.TemporaryDirectory() as tempdir:
+        ledger_cert_file = os.path.join(tempdir, f"{ledger_id}.pem")
+        with open(ledger_cert_file, "w") as outfile:
+            outfile.write(ledger_certificate["ledgerTlsCertificate"])
+
+        print(
+            f"Ledger certificate has been written to {ledger_cert_file}. "
+            "It will be deleted when the script completes."
+        )
+
+        # Build a client through AAD
+        credential = DefaultAzureCredential()
+        ledger_client = ConfidentialLedgerClient(
+            ledger_endpoint,
+            credential=credential,
+            ledger_certificate_path=ledger_cert_file,
+        )
+
+        # Using the async objects as a context manager ensures they are properly closed after use.
+        async with credential:
+            async with ledger_client:
+                post_poller = await ledger_client.begin_create_ledger_entry(
+                    {"contents": "First message"}
                 )
-                + "Supported versions: 0.1-preview"
-            )
+                poller_result = await post_poller.result()
+                first_transaction_id = poller_result["transactionId"]
+
+                print(
+                    "Wrote 'First message' to the ledger. It is recorded at transaction id "
+                    f"{first_transaction_id}."
+                )
+
+                for i in range(10):
+                    entry_contents = f"Message {i}"
+                    print(
+                        f"Writing '{entry_contents}' to the ledger."
+                    )
+                    await ledger_client.create_ledger_entry({"contents": entry_contents})
+
+                post_poller = await ledger_client.begin_create_ledger_entry(
+                    {"contents": "Last message"}
+                )
+                poller_result = await post_poller.result()
+                last_transaction_id = poller_result["transactionId"]
+
+                print(
+                    "Wrote 'Last message' to the ledger. It is recorded at transaction id "
+                    f"{last_transaction_id}."
+                )
+
+                ranged_result = ledger_client.list_ledger_entries(
+                    from_transaction_id=first_transaction_id,
+                    to_transaction_id=last_transaction_id,
+                )
+                async for entry in ranged_result:
+                    print(f'Contents at {entry["transactionId"]}: {entry["contents"]}')
+
 
-    @property
-    def endpoint(self):
-        # type: () -> str
-        """The URL this client is connected to."""
-        return self._endpoint
-
-    def __enter__(self):
-        # type: () -> ConfidentialLedgerClientBase
-        self._client.__enter__()
-        return self
-
-    def __exit__(self, *args):
-        # type: (Any) -> None
-        self._client.__exit__(*args)
-
-    def close(self):
-        # type: () -> None
-        """Close sockets opened by the client.
-
-        Calling this method is unnecessary when using the client as a context manager.
-        """
-        self._client.close()
+if __name__ == "__main__":
+    asyncio.run(main())
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_confidential_ledger_identity_service_client.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,80 +2,87 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from copy import deepcopy
+from typing import Any, TYPE_CHECKING
 
 from azure.core import PipelineClient
-from msrest import Deserializer, Serializer
+from azure.core.rest import HttpRequest, HttpResponse
+
+from ._configuration import ConfidentialLedgerClientConfiguration
+from ._operations import ConfidentialLedgerClientOperationsMixin
+from ._serialization import Deserializer, Serializer
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any
-
-    from azure.core.pipeline.transport import HttpRequest, HttpResponse
-
-from ._configuration import ConfidentialLedgerIdentityServiceClientConfiguration
-from .operations import ConfidentialLedgerIdentityServiceOperations
-from . import models
-
+    from typing import Dict
 
-class ConfidentialLedgerIdentityServiceClient(object):
-    """The ConfidentialLedgerIdentityServiceClient is used to retrieve the TLS certificate required for connecting to a Confidential Ledger.
 
-    :ivar confidential_ledger_identity_service: ConfidentialLedgerIdentityServiceOperations operations
-    :vartype confidential_ledger_identity_service: azure.confidentialledger._generated/_generated_identity.v0_1_preview.operations.ConfidentialLedgerIdentityServiceOperations
-    :param identity_service_uri: The Identity Service URL, for example https://identity.accledger.azure.com.
-    :type identity_service_uri: str
+class ConfidentialLedgerClient(
+    ConfidentialLedgerClientOperationsMixin
+):  # pylint: disable=client-accepts-api-version-keyword
+    """The ConfidentialLedgerClient writes and retrieves ledger entries against the Confidential
+    Ledger service.
+
+    :param ledger_endpoint: The Confidential Ledger URL, for example
+     https://contoso.confidentialledger.azure.com. Required.
+    :type ledger_endpoint: str
+    :keyword api_version: Api Version. Default value is "2022-05-13". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        identity_service_uri,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        base_url = '{identityServiceUri}'
-        self._config = ConfidentialLedgerIdentityServiceClientConfiguration(identity_service_uri, **kwargs)
-        self._client = PipelineClient(base_url=base_url, config=self._config, **kwargs)
+    def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
+        self, ledger_endpoint: str, **kwargs: Any
+    ) -> None:
+        _endpoint = "{ledgerEndpoint}"
+        self._config = ConfidentialLedgerClientConfiguration(ledger_endpoint=ledger_endpoint, **kwargs)
+        self._client = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
-        self._serialize = Serializer(client_models)
+        self._serialize = Serializer()
+        self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
-        self._deserialize = Deserializer(client_models)
 
-        self.confidential_ledger_identity_service = ConfidentialLedgerIdentityServiceOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-
-    def _send_request(self, http_request, **kwargs):
-        # type: (HttpRequest, Any) -> HttpResponse
+    def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
-        :param http_request: The network request you want to make. Required.
-        :type http_request: ~azure.core.pipeline.transport.HttpRequest
-        :keyword bool stream: Whether the response payload will be streamed. Defaults to True.
+        >>> from azure.core.rest import HttpRequest
+        >>> request = HttpRequest("GET", "https://www.example.org/")
+        <HttpRequest [GET], url: 'https://www.example.org/'>
+        >>> response = client.send_request(request)
+        <HttpResponse: 200 OK>
+
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
+
+        :param request: The network request you want to make. Required.
+        :type request: ~azure.core.rest.HttpRequest
+        :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.pipeline.transport.HttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
+
+        request_copy = deepcopy(request)
         path_format_arguments = {
-            'identityServiceUri': self._serialize.url("self._config.identity_service_uri", self._config.identity_service_uri, 'str', skip_quote=True),
+            "ledgerEndpoint": self._serialize.url(
+                "self._config.ledger_endpoint", self._config.ledger_endpoint, "str", skip_quote=True
+            ),
         }
-        http_request.url = self._client.format_url(http_request.url, **path_format_arguments)
-        stream = kwargs.pop("stream", True)
-        pipeline_response = self._client._pipeline.run(http_request, stream=stream, **kwargs)
-        return pipeline_response.http_response
+
+        request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
+        return self._client.send_request(request_copy, **kwargs)
 
     def close(self):
         # type: () -> None
         self._client.close()
 
     def __enter__(self):
-        # type: () -> ConfidentialLedgerIdentityServiceClient
+        # type: () -> ConfidentialLedgerClient
         self._client.__enter__()
         return self
 
     def __exit__(self, *exc_details):
         # type: (Any) -> None
         self._client.__exit__(*exc_details)
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/_configuration.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,58 +2,54 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
 from ._version import VERSION
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any
 
-
-class ConfidentialLedgerIdentityServiceClientConfiguration(Configuration):
-    """Configuration for ConfidentialLedgerIdentityServiceClient.
+class ConfidentialLedgerClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ConfidentialLedgerClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
-    :param identity_service_uri: The Identity Service URL, for example https://identity.accledger.azure.com.
-    :type identity_service_uri: str
+    :param ledger_endpoint: The Confidential Ledger URL, for example
+     https://contoso.confidentialledger.azure.com. Required.
+    :type ledger_endpoint: str
+    :keyword api_version: Api Version. Default value is "2022-05-13". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        identity_service_uri,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        if identity_service_uri is None:
-            raise ValueError("Parameter 'identity_service_uri' must not be None.")
-        super(ConfidentialLedgerIdentityServiceClientConfiguration, self).__init__(**kwargs)
-
-        self.identity_service_uri = identity_service_uri
-        self.api_version = "0.1-preview"
-        kwargs.setdefault('sdk_moniker', 'confidentialledger/{}'.format(VERSION))
+    def __init__(self, ledger_endpoint: str, **kwargs: Any) -> None:
+        super(ConfidentialLedgerClientConfiguration, self).__init__(**kwargs)
+        api_version = kwargs.pop("api_version", "2022-05-13")  # type: str
+
+        if ledger_endpoint is None:
+            raise ValueError("Parameter 'ledger_endpoint' must not be None.")
+
+        self.ledger_endpoint = ledger_endpoint
+        self.api_version = api_version
+        kwargs.setdefault("sdk_moniker", "confidentialledger/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
-        self,
-        **kwargs  # type: Any
+        self, **kwargs  # type: Any
     ):
         # type: (...) -> None
-        self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
-        self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get('http_logging_policy') or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
-        self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
-        self.authentication_policy = kwargs.get('authentication_policy')
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
+        self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/__init__.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._confidential_ledger_identity_service_client import ConfidentialLedgerIdentityServiceClient
-from ._version import VERSION
+from ._client import ConfidentialLedgerCertificateClient
+from .._version import VERSION
 
 __version__ = VERSION
-__all__ = ['ConfidentialLedgerIdentityServiceClient']
 
 try:
-    from ._patch import patch_sdk  # type: ignore
-    patch_sdk()
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
 except ImportError:
-    pass
+    _patch_all = []
+from ._patch import patch_sdk as _patch_sdk
+
+__all__ = ["ConfidentialLedgerCertificateClient"]
+__all__.extend([p for p in _patch_all if p not in __all__])
+
+_patch_sdk()
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_identity/v0_1_preview/aio/_configuration.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,44 +10,46 @@
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
 from .._version import VERSION
 
 
-class ConfidentialLedgerIdentityServiceClientConfiguration(Configuration):
-    """Configuration for ConfidentialLedgerIdentityServiceClient.
+class ConfidentialLedgerCertificateClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+    """Configuration for ConfidentialLedgerCertificateClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
-    :param identity_service_uri: The Identity Service URL, for example https://identity.accledger.azure.com.
-    :type identity_service_uri: str
+    :param certificate_endpoint: The certificate endpoint (or "Identity Service Endpoint" in the
+     Azure portal), for example https://identity.confidential-ledger.core.azure.com. Required.
+    :type certificate_endpoint: str
+    :keyword api_version: Api Version. Default value is "2022-05-13". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        identity_service_uri: str,
-        **kwargs: Any
-    ) -> None:
-        if identity_service_uri is None:
-            raise ValueError("Parameter 'identity_service_uri' must not be None.")
-        super(ConfidentialLedgerIdentityServiceClientConfiguration, self).__init__(**kwargs)
-
-        self.identity_service_uri = identity_service_uri
-        self.api_version = "0.1-preview"
-        kwargs.setdefault('sdk_moniker', 'confidentialledger/{}'.format(VERSION))
+    def __init__(self, certificate_endpoint: str, **kwargs: Any) -> None:
+        super(ConfidentialLedgerCertificateClientConfiguration, self).__init__(**kwargs)
+        api_version = kwargs.pop("api_version", "2022-05-13")  # type: str
+
+        if certificate_endpoint is None:
+            raise ValueError("Parameter 'certificate_endpoint' must not be None.")
+
+        self.certificate_endpoint = certificate_endpoint
+        self.api_version = api_version
+        kwargs.setdefault("sdk_moniker", "confidentialledger-certificate/{}".format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
-        self,
-        **kwargs: Any
-    ) -> None:
-        self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
-        self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get('http_logging_policy') or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.AsyncRetryPolicy(**kwargs)
-        self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.AsyncRedirectPolicy(**kwargs)
-        self.authentication_policy = kwargs.get('authentication_policy')
+        self, **kwargs  # type: Any
+    ):
+        # type: (...) -> None
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
+        self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_confidential_ledger_client.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,80 +2,84 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from copy import deepcopy
+from typing import Any, Awaitable, TYPE_CHECKING
 
-from azure.core import PipelineClient
-from msrest import Deserializer, Serializer
-
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any
-
-    from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core import AsyncPipelineClient
+from azure.core.rest import AsyncHttpResponse, HttpRequest
 
+from .._serialization import Deserializer, Serializer
 from ._configuration import ConfidentialLedgerClientConfiguration
-from .operations import ConfidentialLedgerOperations
-from . import models
+from ._operations import ConfidentialLedgerClientOperationsMixin
 
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from typing import Dict
 
-class ConfidentialLedgerClient(object):
-    """The ConfidentialLedgerClient writes and retrieves ledger entries against the Confidential Ledger service.
 
-    :ivar confidential_ledger: ConfidentialLedgerOperations operations
-    :vartype confidential_ledger: azure.confidentialledger._generated/_generated_ledger.v0_1_preview.operations.ConfidentialLedgerOperations
-    :param ledger_uri: The Confidential Ledger URL, for example https://contoso.confidentialledger.azure.com.
-    :type ledger_uri: str
+class ConfidentialLedgerClient(
+    ConfidentialLedgerClientOperationsMixin
+):  # pylint: disable=client-accepts-api-version-keyword
+    """The ConfidentialLedgerClient writes and retrieves ledger entries against the Confidential
+    Ledger service.
+
+    :param ledger_endpoint: The Confidential Ledger URL, for example
+     https://contoso.confidentialledger.azure.com. Required.
+    :type ledger_endpoint: str
+    :keyword api_version: Api Version. Default value is "2022-05-13". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        ledger_uri,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        base_url = '{ledgerUri}'
-        self._config = ConfidentialLedgerClientConfiguration(ledger_uri, **kwargs)
-        self._client = PipelineClient(base_url=base_url, config=self._config, **kwargs)
+    def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
+        self, ledger_endpoint: str, **kwargs: Any
+    ) -> None:
+        _endpoint = "{ledgerEndpoint}"
+        self._config = ConfidentialLedgerClientConfiguration(ledger_endpoint=ledger_endpoint, **kwargs)
+        self._client = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
-        self._serialize = Serializer(client_models)
+        self._serialize = Serializer()
+        self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
-        self._deserialize = Deserializer(client_models)
 
-        self.confidential_ledger = ConfidentialLedgerOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-
-    def _send_request(self, http_request, **kwargs):
-        # type: (HttpRequest, Any) -> HttpResponse
+    def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
-        :param http_request: The network request you want to make. Required.
-        :type http_request: ~azure.core.pipeline.transport.HttpRequest
-        :keyword bool stream: Whether the response payload will be streamed. Defaults to True.
+        >>> from azure.core.rest import HttpRequest
+        >>> request = HttpRequest("GET", "https://www.example.org/")
+        <HttpRequest [GET], url: 'https://www.example.org/'>
+        >>> response = await client.send_request(request)
+        <AsyncHttpResponse: 200 OK>
+
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
+
+        :param request: The network request you want to make. Required.
+        :type request: ~azure.core.rest.HttpRequest
+        :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.pipeline.transport.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
+
+        request_copy = deepcopy(request)
         path_format_arguments = {
-            'ledgerUri': self._serialize.url("self._config.ledger_uri", self._config.ledger_uri, 'str', skip_quote=True),
+            "ledgerEndpoint": self._serialize.url(
+                "self._config.ledger_endpoint", self._config.ledger_endpoint, "str", skip_quote=True
+            ),
         }
-        http_request.url = self._client.format_url(http_request.url, **path_format_arguments)
-        stream = kwargs.pop("stream", True)
-        pipeline_response = self._client._pipeline.run(http_request, stream=stream, **kwargs)
-        return pipeline_response.http_response
-
-    def close(self):
-        # type: () -> None
-        self._client.close()
-
-    def __enter__(self):
-        # type: () -> ConfidentialLedgerClient
-        self._client.__enter__()
+
+        request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
+        return self._client.send_request(request_copy, **kwargs)
+
+    async def close(self) -> None:
+        await self._client.close()
+
+    async def __aenter__(self) -> "ConfidentialLedgerClient":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details) -> None:
+        await self._client.__aexit__(*exc_details)
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/_configuration.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,58 +2,51 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 
-from ._version import VERSION
+from .._version import VERSION
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any
 
-
-class ConfidentialLedgerClientConfiguration(Configuration):
+class ConfidentialLedgerClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for ConfidentialLedgerClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
-    :param ledger_uri: The Confidential Ledger URL, for example https://contoso.confidentialledger.azure.com.
-    :type ledger_uri: str
+    :param ledger_endpoint: The Confidential Ledger URL, for example
+     https://contoso.confidentialledger.azure.com. Required.
+    :type ledger_endpoint: str
+    :keyword api_version: Api Version. Default value is "2022-05-13". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        ledger_uri,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        if ledger_uri is None:
-            raise ValueError("Parameter 'ledger_uri' must not be None.")
+    def __init__(self, ledger_endpoint: str, **kwargs: Any) -> None:
         super(ConfidentialLedgerClientConfiguration, self).__init__(**kwargs)
+        api_version = kwargs.pop("api_version", "2022-05-13")  # type: str
+
+        if ledger_endpoint is None:
+            raise ValueError("Parameter 'ledger_endpoint' must not be None.")
 
-        self.ledger_uri = ledger_uri
-        self.api_version = "0.1-preview"
-        kwargs.setdefault('sdk_moniker', 'confidentialledger/{}'.format(VERSION))
+        self.ledger_endpoint = ledger_endpoint
+        self.api_version = api_version
+        kwargs.setdefault("sdk_moniker", "confidentialledger/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self,
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
-        self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get('http_logging_policy') or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
-        self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
-        self.authentication_policy = kwargs.get('authentication_policy')
+    def _configure(self, **kwargs: Any) -> None:
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
+        self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/_generated/_generated_ledger/v0_1_preview/__init__.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/certificate/_operations/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._confidential_ledger_client import ConfidentialLedgerClient
-from ._version import VERSION
+from ._operations import ConfidentialLedgerCertificateClientOperationsMixin
 
-__version__ = VERSION
-__all__ = ['ConfidentialLedgerClient']
+from ._patch import __all__ as _patch_all
+from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import patch_sdk as _patch_sdk
 
-try:
-    from ._patch import patch_sdk  # type: ignore
-    patch_sdk()
-except ImportError:
-    pass
+__all__ = [
+    "ConfidentialLedgerCertificateClientOperationsMixin",
+]
+__all__.extend([p for p in _patch_all if p not in __all__])
+_patch_sdk()
```

## Comparing `azure-confidentialledger-1.0.0b1/azure/confidentialledger/aio/_client_base.py` & `azure-confidentialledger-1.1.0/azure/confidentialledger/aio/_patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,97 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
+"""Customize generated code here.
 
-from typing import Any, TYPE_CHECKING, Union
+Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
+"""
+import os
+from typing import Any, List, Union
 
-from azure.core.pipeline.policies import (
-    AsyncBearerTokenCredentialPolicy,
-    HttpLoggingPolicy,
-)
+from azure.core.credentials_async import AsyncTokenCredential
+from azure.core.pipeline import policies
 
-from .._user_agent import USER_AGENT
-from .._generated._generated_ledger.v0_1_preview.aio import (
-    ConfidentialLedgerClient as _ConfidentialLedgerClient,
+from azure.confidentialledger.aio._client import (
+    ConfidentialLedgerClient as GeneratedClient,
 )
-from .._shared import ConfidentialLedgerCertificateCredential, DEFAULT_VERSION
-
-if TYPE_CHECKING:
-    from azure.core.credentials import TokenCredential
 
+# Since we can't `await` in __init__, use the sync client for the Identity Service.
+from azure.confidentialledger.certificate import ConfidentialLedgerCertificateClient
+from azure.confidentialledger._patch import ConfidentialLedgerCertificateCredential
+
+__all__: List[str] = [
+    "ConfidentialLedgerClient",
+]  # Add all objects you want publicly available to users at this package level
+
+
+def patch_sdk():
+    """Do not remove from this file.
+
+    `patch_sdk` is a last resort escape hatch that allows you to do customizations
+    you can't accomplish using the techniques described in
+    https://aka.ms/azsdk/python/dpcodegen/python/customize
+    """
+
+
+class ConfidentialLedgerClient(GeneratedClient):
+    """The ConfidentialLedgerClient writes and retrieves ledger entries against the Confidential
+    Ledger service.
+
+    :param endpoint: The Confidential Ledger URL, for example
+     https://contoso.confidentialledger.azure.com.
+    :type endpoint: str
+    :param credential: A credential object for authenticating with the Confidential Ledger.
+    :type credential: Union[
+        ~azure.confidentialledger.ConfidentialLedgerCertificateCredential,
+        ~azure.core.credentials_async.AsyncTokenCredential]
+    :keyword ledger_certificate_path: The path to the Confidential Ledger's TLS certificate. If this
+        file does not exist yet, the Confidential Ledger's TLS certificate will be fetched and saved
+        to this file.
+    :paramtype ledger_certificate_path: Union[bytes, str, os.PathLike]
+    :keyword api_version: Api Version. Default value is "2022-05-13". Note that overriding this
+     default value may result in unsupported behavior.
+    :paramtype api_version: str
+    """
 
-class AsyncConfidentialLedgerClientBase(object):
     def __init__(
         self,
-        *,
         endpoint: str,
-        credential: Union[ConfidentialLedgerCertificateCredential, "TokenCredential"],
-        ledger_certificate_path: str,
-        **kwargs: Any
+        credential: Union[ConfidentialLedgerCertificateCredential, AsyncTokenCredential],
+        *,
+        ledger_certificate_path: Union[bytes, str, os.PathLike],
+        **kwargs: Any,
     ) -> None:
-
-        client = kwargs.get("generated_client")
-        if client:
-            # caller provided a configured client -> nothing left to initialize
-            self._client = client
-            return
-
-        if not endpoint:
-            raise ValueError("Expected endpoint to be a non-empty string")
-
-        if not credential:
-            raise ValueError("Expected credential to not be None")
-
-        if not isinstance(ledger_certificate_path, str):
-            raise TypeError("ledger_certificate_path must be a string")
-
-        if ledger_certificate_path == "":
-            raise ValueError(
-                "If not None, ledger_certificate_path must be a non-empty string"
-            )
-
-        endpoint = endpoint.strip(" /")
-        try:
-            if not endpoint.startswith("https://"):
-                self._endpoint = "https://" + endpoint
-            else:
-                self._endpoint = endpoint
-        except AttributeError:
-            raise ValueError("Confidential Ledger URL must be a string.")
-
-        self.api_version = kwargs.pop("api_version", DEFAULT_VERSION)
-
-        if not kwargs.get("transport", None):
-            # Customize the transport layer to use client certificate authentication and validate
-            # a self-signed TLS certificate.
-            if isinstance(credential, ConfidentialLedgerCertificateCredential):
-                # The async version of the client seems to expect a sequence of filenames.
-                # azure/core/pipeline/transport/_aiohttp.py:163
-                # > ssl_ctx.load_cert_chain(*cert)
-                kwargs["connection_cert"] = (credential.certificate_path,)
-
-            kwargs["connection_verify"] = ledger_certificate_path
-
-        http_logging_policy = HttpLoggingPolicy(**kwargs)
-        http_logging_policy.allowed_header_names.update(
-            {
-                "x-ms-keyvault-network-info",
-                "x-ms-keyvault-region",
-                "x-ms-keyvault-service-version",
-            }
-        )
-
-        if not isinstance(credential, ConfidentialLedgerCertificateCredential):
-            kwargs["authentication_policy"] = kwargs.pop(
+        if os.path.isfile(ledger_certificate_path) is False:
+            # We'll need to fetch the TLS certificate.
+            identity_service_client = ConfidentialLedgerCertificateClient(**kwargs)
+
+            # Ledger URIs are of the form https://<ledger id>.confidential-ledger.azure.com.
+            ledger_id = endpoint.replace("https://", "").split(".")[0]
+            ledger_cert = identity_service_client.get_ledger_identity(ledger_id, **kwargs)
+
+            with open(ledger_certificate_path, "w", encoding="utf-8") as outfile:
+                outfile.write(ledger_cert["ledgerTlsCertificate"])
+
+        # For ConfidentialLedgerCertificateCredential, pass the path to the certificate down to the
+        # PipelineCLient.
+        if isinstance(credential, ConfidentialLedgerCertificateCredential):
+            # The async version of the client seems to expect a sequence of filenames.
+            # azure/core/pipeline/transport/_aiohttp.py:163
+            # > ssl_ctx.load_cert_chain(*cert)
+            kwargs["connection_cert"] = (credential.certificate_path,)
+
+        # The auto-generated client has authentication disabled so we can customize authentication.
+        # If the credential is the typical TokenCredential, then construct the authentication policy
+        # the normal way.
+        else:
+            credential_scopes = kwargs.pop("credential_scopes", ["https://confidential-ledger.azure.com/.default"])
+            kwargs["authentication_policy"] = kwargs.get(
                 "authentication_policy",
-                AsyncBearerTokenCredentialPolicy(
-                    credential,
-                    "https://confidential-ledger.azure.com/.default",
-                    **kwargs
-                ),
+                policies.AsyncBearerTokenCredentialPolicy(credential, *credential_scopes, **kwargs),
             )
 
-        try:
-            self._client = _ConfidentialLedgerClient(
-                self._endpoint,
-                api_version=self.api_version,
-                http_logging_policy=http_logging_policy,
-                sdk_moniker=USER_AGENT,
-                **kwargs
-            )
-        except NotImplementedError:
-            raise NotImplementedError(
-                "This package doesn't support API version '{}'. ".format(
-                    self.api_version
-                )
-                + "Supported versions: 0.1-preview"
-            )
+        # Customize the underlying client to use a self-signed TLS certificate.
+        kwargs["connection_verify"] = kwargs.get("connection_verify", ledger_certificate_path)
 
-    @property
-    def endpoint(self) -> str:
-        """The URL this client is connected to."""
-        return self._endpoint
-
-    async def __aenter__(self) -> "AsyncConfidentialLedgerClientBase":
-        await self._client.__aenter__()
-        return self
-
-    async def __aexit__(self, *args: Any) -> None:
-        await self._client.__aexit__(*args)
-
-    async def close(self) -> None:
-        """Close sockets opened by the client.
-
-        Calling this method is unnecessary when using the client as a context manager.
-        """
-        await self._client.close()
+        super().__init__(endpoint, **kwargs)
```

