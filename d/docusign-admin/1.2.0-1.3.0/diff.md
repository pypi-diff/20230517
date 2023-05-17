# Comparing `tmp/docusign-admin-1.2.0.tar.gz` & `tmp/docusign-admin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docusign-admin-1.2.0.tar", last modified: Fri Apr  7 14:21:42 2023, max compression
+gzip compressed data, was "dist/docusign-admin-1.3.0.tar", last modified: Wed May 17 18:56:48 2023, max compression
```

## Comparing `docusign-admin-1.2.0.tar` & `docusign-admin-1.3.0.tar`

### file list

```diff
@@ -1,141 +1,147 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/
--rwxr-xr-x   0 root         (0) root         (0)     1102 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3742 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3507 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin/
--rw-r--r--   0 root         (0) root         (0)    10185 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin/apis/
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16921 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/accounts_api.py
--rw-r--r--   0 root         (0) root         (0)    42743 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/bulk_exports_api.py
--rw-r--r--   0 root         (0) root         (0)    77072 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/bulk_imports_api.py
--rw-r--r--   0 root         (0) root         (0)    43217 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/ds_groups_api.py
--rw-r--r--   0 root         (0) root         (0)     5808 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/identity_providers_api.py
--rw-r--r--   0 root         (0) root         (0)    38443 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/product_permission_profiles_api.py
--rw-r--r--   0 root         (0) root         (0)     5732 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/reserved_domains_api.py
--rw-r--r--   0 root         (0) root         (0)    69337 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/apis/users_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin/client/
--rwxr-xr-x   0 root         (0) root         (0)      283 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    35251 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/api_client.py
--rwxr-xr-x   0 root         (0) root         (0)     1503 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/api_exception.py
--rwxr-xr-x   0 root         (0) root         (0)    11576 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin/client/auth/
--rwxr-xr-x   0 root         (0) root         (0)      219 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/auth/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14756 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/auth/oauth.py
--rwxr-xr-x   0 root         (0) root         (0)     7297 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/client/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin/models/
--rw-r--r--   0 root         (0) root         (0)     9339 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/add_ds_group_and_users_response.py
--rw-r--r--   0 root         (0) root         (0)     5015 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/add_ds_group_users_response.py
--rw-r--r--   0 root         (0) root         (0)     9032 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/add_user_response.py
--rw-r--r--   0 root         (0) root         (0)     7737 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/add_user_response_account_properties.py
--rw-r--r--   0 root         (0) root         (0)     6904 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/certificate_response.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/delete_membership_request.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/delete_membership_response.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/delete_memberships_request.py
--rw-r--r--   0 root         (0) root         (0)     4309 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/delete_memberships_response.py
--rw-r--r--   0 root         (0) root         (0)     4190 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/delete_response.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/delete_user_identity_request.py
--rw-r--r--   0 root         (0) root         (0)     7543 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/domain_response.py
--rw-r--r--   0 root         (0) root         (0)     3646 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/domains_response.py
--rw-r--r--   0 root         (0) root         (0)     4404 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_add_request.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_and_users_response.py
--rw-r--r--   0 root         (0) root         (0)     6307 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_list_response.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_request.py
--rw-r--r--   0 root         (0) root         (0)    10917 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_response.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_user_response.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_users_add_request.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_users_remove_request.py
--rw-r--r--   0 root         (0) root         (0)     5554 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/ds_group_users_response.py
--rw-r--r--   0 root         (0) root         (0)     4182 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/force_activate_membership_request.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/group_request.py
--rw-r--r--   0 root         (0) root         (0)     7202 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/identity_provider_response.py
--rw-r--r--   0 root         (0) root         (0)     3802 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/identity_providers_response.py
--rw-r--r--   0 root         (0) root         (0)     3912 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/link_response.py
--rw-r--r--   0 root         (0) root         (0)     4591 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/member_group_response.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/member_groups_response.py
--rw-r--r--   0 root         (0) root         (0)    10291 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/membership_response.py
--rw-r--r--   0 root         (0) root         (0)    12497 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/new_account_user_request.py
--rw-r--r--   0 root         (0) root         (0)    12493 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/new_multi_product_user_add_request.py
--rw-r--r--   0 root         (0) root         (0)    11489 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/new_user_request.py
--rw-r--r--   0 root         (0) root         (0)     6892 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/new_user_request_account_properties.py
--rw-r--r--   0 root         (0) root         (0)     9032 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/new_user_response.py
--rw-r--r--   0 root         (0) root         (0)     7494 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/new_user_response_account_properties.py
--rw-r--r--   0 root         (0) root         (0)     4260 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/oasirr_error_details.py
--rw-r--r--   0 root         (0) root         (0)     7100 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/oasirr_organization_account_settings_error_data_response.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/oetr_error_details.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_export_selected_account.py
--rw-r--r--   0 root         (0) root         (0)     3487 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_export_selected_domain.py
--rw-r--r--   0 root         (0) root         (0)     5792 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_report_configuration_response.py
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_report_create_response.py
--rw-r--r--   0 root         (0) root         (0)     3586 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_report_list_response.py
--rw-r--r--   0 root         (0) root         (0)    12629 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_report_list_response_org_report.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_report_list_response_requestor.py
--rw-r--r--   0 root         (0) root         (0)     6730 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/org_report_request.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_account_request.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_account_response.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_account_settings_import_requestor_response.py
--rw-r--r--   0 root         (0) root         (0)    15930 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_account_settings_import_response.py
--rw-r--r--   0 root         (0) root         (0)     9565 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_account_settings_import_result_response.py
--rw-r--r--   0 root         (0) root         (0)     3646 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_accounts_request.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_export_account.py
--rw-r--r--   0 root         (0) root         (0)     3496 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_export_domain.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_export_request.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_export_requestor_response.py
--rw-r--r--   0 root         (0) root         (0)    15025 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_export_response.py
--rw-r--r--   0 root         (0) root         (0)     7199 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_export_task_response.py
--rw-r--r--   0 root         (0) root         (0)     3628 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_exports_response.py
--rw-r--r--   0 root         (0) root         (0)    26879 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_import_response.py
--rw-r--r--   0 root         (0) root         (0)     4381 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_import_response_error_rollup.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_import_response_requestor.py
--rw-r--r--   0 root         (0) root         (0)     4443 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_import_response_warning_rollup.py
--rw-r--r--   0 root         (0) root         (0)     3628 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_imports_response.py
--rw-r--r--   0 root         (0) root         (0)    13757 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_response.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_salesforce_account_managers_response.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_simple_id_object.py
--rw-r--r--   0 root         (0) root         (0)    11100 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_user_response.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organization_users_response.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/organizations_response.py
--rw-r--r--   0 root         (0) root         (0)     4544 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/osamr_contact.py
--rw-r--r--   0 root         (0) root         (0)     7760 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/paging_response_properties.py
--rw-r--r--   0 root         (0) root         (0)     4209 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/permission_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     4063 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/permission_profile_response.py
--rw-r--r--   0 root         (0) root         (0)     4773 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/permission_profile_response21.py
--rw-r--r--   0 root         (0) root         (0)     3625 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/permissions_response.py
--rw-r--r--   0 root         (0) root         (0)     4963 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/product_permission_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6280 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/product_permission_profile_response.py
--rw-r--r--   0 root         (0) root         (0)     4257 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/product_permission_profiles_request.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/product_permission_profiles_response.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/remove_ds_group_users_response.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/remove_user_products_response.py
--rw-r--r--   0 root         (0) root         (0)     7036 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/required_attribute_mapping_response.py
--rw-r--r--   0 root         (0) root         (0)     6172 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/saml2_identity_provider_response.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/setting_response.py
--rw-r--r--   0 root         (0) root         (0)     8423 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/update_membership_request.py
--rw-r--r--   0 root         (0) root         (0)     3406 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/update_response.py
--rw-r--r--   0 root         (0) root         (0)     5207 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/update_user_email_request.py
--rw-r--r--   0 root         (0) root         (0)    13091 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     3544 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/update_users_email_request.py
--rw-r--r--   0 root         (0) root         (0)     3484 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/update_users_request.py
--rw-r--r--   0 root         (0) root         (0)    16955 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_drilldown_response.py
--rw-r--r--   0 root         (0) root         (0)     3379 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_identity_request.py
--rw-r--r--   0 root         (0) root         (0)     6341 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_identity_response.py
--rw-r--r--   0 root         (0) root         (0)     5150 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_product_permission_profiles_request.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_product_permission_profiles_response.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_product_profile_delete_request.py
--rw-r--r--   0 root         (0) root         (0)     5437 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/user_update_response.py
--rw-r--r--   0 root         (0) root         (0)     3532 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/users_drilldown_response.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/docusign_admin/models/users_update_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3742 2023-04-07 14:21:41.000000 docusign-admin-1.2.0/docusign_admin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6393 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 14:21:41.000000 docusign-admin-1.2.0/docusign_admin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/docusign_admin.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       79 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1615 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:42.000000 docusign-admin-1.2.0/test/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/test/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4772 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/test/test_oauth.py
--rwxr-xr-x   0 root         (0) root         (0)     6356 2023-04-07 14:21:38.000000 docusign-admin-1.2.0/test/unit_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1102 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3507 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin/
+-rw-r--r--   0 root         (0) root         (0)    10776 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin/apis/
+-rw-r--r--   0 root         (0) root         (0)      518 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22456 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/accounts_api.py
+-rw-r--r--   0 root         (0) root         (0)    42743 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/bulk_exports_api.py
+-rw-r--r--   0 root         (0) root         (0)    77072 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/bulk_imports_api.py
+-rw-r--r--   0 root         (0) root         (0)    43217 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/ds_groups_api.py
+-rw-r--r--   0 root         (0) root         (0)     5808 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/identity_providers_api.py
+-rw-r--r--   0 root         (0) root         (0)     6619 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/organizations_api.py
+-rw-r--r--   0 root         (0) root         (0)    38443 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/product_permission_profiles_api.py
+-rw-r--r--   0 root         (0) root         (0)     5732 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/reserved_domains_api.py
+-rw-r--r--   0 root         (0) root         (0)    69337 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/apis/users_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin/client/
+-rwxr-xr-x   0 root         (0) root         (0)      283 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    35251 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/api_client.py
+-rwxr-xr-x   0 root         (0) root         (0)     1503 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/api_exception.py
+-rwxr-xr-x   0 root         (0) root         (0)    11576 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin/client/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      219 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/auth/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14756 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/auth/oauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     7297 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/client/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin/models/
+-rw-r--r--   0 root         (0) root         (0)     9877 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/add_ds_group_and_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     5015 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/add_ds_group_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     9032 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/add_user_response.py
+-rw-r--r--   0 root         (0) root         (0)     7737 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/add_user_response_account_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6904 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/certificate_response.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/delete_membership_request.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/delete_membership_response.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/delete_memberships_request.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/delete_memberships_response.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/delete_response.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/delete_user_identity_request.py
+-rw-r--r--   0 root         (0) root         (0)     7543 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/domain_response.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/domains_response.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_add_request.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_and_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     6307 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_request.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_response.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_user_response.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_users_add_request.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_users_remove_request.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/ds_group_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     4182 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/force_activate_membership_request.py
+-rw-r--r--   0 root         (0) root         (0)     4631 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/group_request.py
+-rw-r--r--   0 root         (0) root         (0)     7202 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/identity_provider_response.py
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/identity_providers_response.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/individual_membership_data_redaction_request.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/individual_user_data_redaction_request.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/individual_user_data_redaction_response.py
+-rw-r--r--   0 root         (0) root         (0)     3912 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/link_response.py
+-rw-r--r--   0 root         (0) root         (0)     4591 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/member_group_response.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/member_groups_response.py
+-rw-r--r--   0 root         (0) root         (0)     3622 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/membership_data_redaction_request.py
+-rw-r--r--   0 root         (0) root         (0)     4708 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/membership_data_redaction_response.py
+-rw-r--r--   0 root         (0) root         (0)    10291 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/membership_response.py
+-rw-r--r--   0 root         (0) root         (0)    12497 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/new_account_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    12493 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/new_multi_product_user_add_request.py
+-rw-r--r--   0 root         (0) root         (0)    11489 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/new_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     6892 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/new_user_request_account_properties.py
+-rw-r--r--   0 root         (0) root         (0)     9032 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/new_user_response.py
+-rw-r--r--   0 root         (0) root         (0)     7494 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/new_user_response_account_properties.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/oasirr_error_details.py
+-rw-r--r--   0 root         (0) root         (0)     7100 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/oasirr_organization_account_settings_error_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/oetr_error_details.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_export_selected_account.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_export_selected_domain.py
+-rw-r--r--   0 root         (0) root         (0)     5792 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_report_configuration_response.py
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_report_create_response.py
+-rw-r--r--   0 root         (0) root         (0)     3586 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_report_list_response.py
+-rw-r--r--   0 root         (0) root         (0)    12629 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_report_list_response_org_report.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_report_list_response_requestor.py
+-rw-r--r--   0 root         (0) root         (0)     6730 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/org_report_request.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_account_request.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_account_response.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_account_settings_import_requestor_response.py
+-rw-r--r--   0 root         (0) root         (0)    15930 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_account_settings_import_response.py
+-rw-r--r--   0 root         (0) root         (0)     9565 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_account_settings_import_result_response.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_accounts_request.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_export_account.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_export_domain.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_export_request.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_export_requestor_response.py
+-rw-r--r--   0 root         (0) root         (0)    15025 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_export_response.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_export_task_response.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_exports_response.py
+-rw-r--r--   0 root         (0) root         (0)    26879 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_import_response.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_import_response_error_rollup.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_import_response_requestor.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_import_response_warning_rollup.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_imports_response.py
+-rw-r--r--   0 root         (0) root         (0)    13757 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_response.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_salesforce_account_managers_response.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_simple_id_object.py
+-rw-r--r--   0 root         (0) root         (0)    11100 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_user_response.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organization_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/organizations_response.py
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/osamr_contact.py
+-rw-r--r--   0 root         (0) root         (0)     7760 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/paging_response_properties.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/permission_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/permission_profile_response.py
+-rw-r--r--   0 root         (0) root         (0)     4773 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/permission_profile_response21.py
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/permissions_response.py
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/product_permission_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/product_permission_profile_response.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/product_permission_profiles_request.py
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/product_permission_profiles_response.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/remove_ds_group_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/remove_user_products_response.py
+-rw-r--r--   0 root         (0) root         (0)     7036 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/required_attribute_mapping_response.py
+-rw-r--r--   0 root         (0) root         (0)     6172 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/saml2_identity_provider_response.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/setting_response.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/update_membership_request.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/update_response.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/update_user_email_request.py
+-rw-r--r--   0 root         (0) root         (0)    13091 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     3544 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/update_users_email_request.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/update_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    16955 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_drilldown_response.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_identity_request.py
+-rw-r--r--   0 root         (0) root         (0)     6341 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_identity_response.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_product_permission_profiles_request.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_product_permission_profiles_response.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_product_profile_delete_request.py
+-rw-r--r--   0 root         (0) root         (0)     5437 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/user_update_response.py
+-rw-r--r--   0 root         (0) root         (0)     3532 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/users_drilldown_response.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/docusign_admin/models/users_update_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/docusign_admin.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       79 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1615 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:48.000000 docusign-admin-1.3.0/test/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/test/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4772 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/test/test_oauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     6356 2023-05-17 18:56:45.000000 docusign-admin-1.3.0/test/unit_tests.py
```

### Comparing `docusign-admin-1.2.0/LICENSE` & `docusign-admin-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/PKG-INFO` & `docusign-admin-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docusign-admin
-Version: 1.2.0
+Version: 1.3.0
 Summary: DocuSign Admin API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,DocuSign Admin API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docusign-admin Version: 1.2.0 Summary: DocuSign
+Metadata-Version: 2.1 Name: docusign-admin Version: 1.3.0 Summary: DocuSign
 Admin API Home-page: Author-email: devcenter@docusign.com Keywords:
 Swagger,DocuSign Admin API Description-Content-Type: text/markdown License-
 File: LICENSE # The Official DocuSign OrgAdmin Python Client [![PyPI version]
 [pypi-image]][pypi-url]  [![Build status][travis-image]][travis-url] [PyPI
 module](https://pypi.python.org/pypi/docusign_admin) that wraps the DocuSign
 OrgAdmin API [Documentation about the DocuSign OrgAdmin API](https://
 developers.docusign.com/) ## Requirements - Python 2.7 (3.7+ recommended) -
```

### Comparing `docusign-admin-1.2.0/README.md` & `docusign-admin-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/__init__.py` & `docusign-admin-1.3.0/docusign_admin/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 # import apis into sdk package
 from .apis.accounts_api import AccountsApi
 from .apis.bulk_exports_api import BulkExportsApi
 from .apis.bulk_imports_api import BulkImportsApi
 from .apis.ds_groups_api import DSGroupsApi
 from .apis.identity_providers_api import IdentityProvidersApi
+from .apis.organizations_api import OrganizationsApi
 from .apis.product_permission_profiles_api import ProductPermissionProfilesApi
 from .apis.reserved_domains_api import ReservedDomainsApi
 from .apis.users_api import UsersApi
 
 # import ApiClient
 from .client.api_client import ApiClient
 from .client.configuration import Configuration
@@ -60,17 +61,22 @@
 from docusign_admin.models.domain_response import DomainResponse
 from docusign_admin.models.domains_response import DomainsResponse
 from docusign_admin.models.error_details import ErrorDetails
 from docusign_admin.models.force_activate_membership_request import ForceActivateMembershipRequest
 from docusign_admin.models.group_request import GroupRequest
 from docusign_admin.models.identity_provider_response import IdentityProviderResponse
 from docusign_admin.models.identity_providers_response import IdentityProvidersResponse
+from docusign_admin.models.individual_membership_data_redaction_request import IndividualMembershipDataRedactionRequest
+from docusign_admin.models.individual_user_data_redaction_request import IndividualUserDataRedactionRequest
+from docusign_admin.models.individual_user_data_redaction_response import IndividualUserDataRedactionResponse
 from docusign_admin.models.link_response import LinkResponse
 from docusign_admin.models.member_group_response import MemberGroupResponse
 from docusign_admin.models.member_groups_response import MemberGroupsResponse
+from docusign_admin.models.membership_data_redaction_request import MembershipDataRedactionRequest
+from docusign_admin.models.membership_data_redaction_response import MembershipDataRedactionResponse
 from docusign_admin.models.membership_response import MembershipResponse
 from docusign_admin.models.new_account_user_request import NewAccountUserRequest
 from docusign_admin.models.new_multi_product_user_add_request import NewMultiProductUserAddRequest
 from docusign_admin.models.new_user_request import NewUserRequest
 from docusign_admin.models.new_user_request_account_properties import NewUserRequestAccountProperties
 from docusign_admin.models.new_user_response import NewUserResponse
 from docusign_admin.models.new_user_response_account_properties import NewUserResponseAccountProperties
```

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/accounts_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/accounts_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -379,7 +379,121 @@
                                         response_type='PermissionsResponse',
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
+
+    def redact_individual_membership_data(self, account_id, request_model, **kwargs):
+        """
+        Redacts membership data for users with memberships in an account.
+        Required scopes: user_data_redact
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.redact_individual_membership_data(account_id, request_model, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param str account_id: The account ID Guid (required)
+        :param IndividualMembershipDataRedactionRequest request_model: The request body describing the membership to be redacted (required)
+        :return: IndividualUserDataRedactionResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.redact_individual_membership_data_with_http_info(account_id, request_model, **kwargs)
+        else:
+            (data) = self.redact_individual_membership_data_with_http_info(account_id, request_model, **kwargs)
+            return data
+
+    def redact_individual_membership_data_with_http_info(self, account_id, request_model, **kwargs):
+        """
+        Redacts membership data for users with memberships in an account.
+        Required scopes: user_data_redact
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.redact_individual_membership_data_with_http_info(account_id, request_model, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param str account_id: The account ID Guid (required)
+        :param IndividualMembershipDataRedactionRequest request_model: The request body describing the membership to be redacted (required)
+        :return: IndividualUserDataRedactionResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['account_id', 'request_model']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method redact_individual_membership_data" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'account_id' is set
+        if ('account_id' not in params) or (params['account_id'] is None):
+            raise ValueError("Missing the required parameter `account_id` when calling `redact_individual_membership_data`")
+        # verify the required parameter 'request_model' is set
+        if ('request_model' not in params) or (params['request_model'] is None):
+            raise ValueError("Missing the required parameter `request_model` when calling `redact_individual_membership_data`")
+
+
+        collection_formats = {}
+
+        resource_path = '/v2/data_redaction/accounts/{accountId}/user'.replace('{format}', 'json')
+        path_params = {}
+        if 'account_id' in params:
+            path_params['accountId'] = params['account_id']
+
+        query_params = {}
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'request_model' in params:
+            body_params = params['request_model']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/json'])
+
+        # Authentication setting
+        auth_settings = []
+
+        return self.api_client.call_api(resource_path, 'POST',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type='IndividualUserDataRedactionResponse',
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=collection_formats)
```

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/bulk_exports_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/bulk_exports_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/bulk_imports_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/bulk_imports_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/ds_groups_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/ds_groups_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/identity_providers_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/identity_providers_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/product_permission_profiles_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/product_permission_profiles_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/reserved_domains_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/reserved_domains_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/apis/users_api.py` & `docusign-admin-1.3.0/docusign_admin/apis/users_api.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/client/api_client.py` & `docusign-admin-1.3.0/docusign_admin/client/api_client.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/client/api_exception.py` & `docusign-admin-1.3.0/docusign_admin/client/api_exception.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/client/api_response.py` & `docusign-admin-1.3.0/docusign_admin/client/api_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/client/auth/oauth.py` & `docusign-admin-1.3.0/docusign_admin/client/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/client/configuration.py` & `docusign-admin-1.3.0/docusign_admin/client/configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/__init__.py` & `docusign-admin-1.3.0/docusign_admin/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,22 @@
 from docusign_admin.models.domain_response import DomainResponse
 from docusign_admin.models.domains_response import DomainsResponse
 from docusign_admin.models.error_details import ErrorDetails
 from docusign_admin.models.force_activate_membership_request import ForceActivateMembershipRequest
 from docusign_admin.models.group_request import GroupRequest
 from docusign_admin.models.identity_provider_response import IdentityProviderResponse
 from docusign_admin.models.identity_providers_response import IdentityProvidersResponse
+from docusign_admin.models.individual_membership_data_redaction_request import IndividualMembershipDataRedactionRequest
+from docusign_admin.models.individual_user_data_redaction_request import IndividualUserDataRedactionRequest
+from docusign_admin.models.individual_user_data_redaction_response import IndividualUserDataRedactionResponse
 from docusign_admin.models.link_response import LinkResponse
 from docusign_admin.models.member_group_response import MemberGroupResponse
 from docusign_admin.models.member_groups_response import MemberGroupsResponse
+from docusign_admin.models.membership_data_redaction_request import MembershipDataRedactionRequest
+from docusign_admin.models.membership_data_redaction_response import MembershipDataRedactionResponse
 from docusign_admin.models.membership_response import MembershipResponse
 from docusign_admin.models.new_account_user_request import NewAccountUserRequest
 from docusign_admin.models.new_multi_product_user_add_request import NewMultiProductUserAddRequest
 from docusign_admin.models.new_user_request import NewUserRequest
 from docusign_admin.models.new_user_request_account_properties import NewUserRequestAccountProperties
 from docusign_admin.models.new_user_response import NewUserResponse
 from docusign_admin.models.new_user_response_account_properties import NewUserResponseAccountProperties
```

### Comparing `docusign-admin-1.2.0/docusign_admin/models/add_ds_group_and_users_response.py` & `docusign-admin-1.3.0/docusign_admin/models/add_ds_group_and_users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/add_ds_group_users_response.py` & `docusign-admin-1.3.0/docusign_admin/models/add_ds_group_users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/add_user_response.py` & `docusign-admin-1.3.0/docusign_admin/models/add_user_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/add_user_response_account_properties.py` & `docusign-admin-1.3.0/docusign_admin/models/add_user_response_account_properties.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/certificate_response.py` & `docusign-admin-1.3.0/docusign_admin/models/certificate_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/delete_membership_request.py` & `docusign-admin-1.3.0/docusign_admin/models/delete_membership_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/delete_membership_response.py` & `docusign-admin-1.3.0/docusign_admin/models/delete_membership_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/delete_memberships_request.py` & `docusign-admin-1.3.0/docusign_admin/models/delete_memberships_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/delete_memberships_response.py` & `docusign-admin-1.3.0/docusign_admin/models/delete_memberships_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/delete_response.py` & `docusign-admin-1.3.0/docusign_admin/models/delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/delete_user_identity_request.py` & `docusign-admin-1.3.0/docusign_admin/models/delete_user_identity_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/domain_response.py` & `docusign-admin-1.3.0/docusign_admin/models/domain_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/domains_response.py` & `docusign-admin-1.3.0/docusign_admin/models/domains_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_add_request.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_add_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_and_users_response.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_and_users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_list_response.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_list_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_request.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_response.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_user_response.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_user_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_users_add_request.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_users_add_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_users_remove_request.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_users_remove_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/ds_group_users_response.py` & `docusign-admin-1.3.0/docusign_admin/models/ds_group_users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/error_details.py` & `docusign-admin-1.3.0/docusign_admin/models/error_details.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/force_activate_membership_request.py` & `docusign-admin-1.3.0/docusign_admin/models/force_activate_membership_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/group_request.py` & `docusign-admin-1.3.0/docusign_admin/models/group_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/identity_provider_response.py` & `docusign-admin-1.3.0/docusign_admin/models/identity_provider_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/identity_providers_response.py` & `docusign-admin-1.3.0/docusign_admin/models/identity_providers_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/link_response.py` & `docusign-admin-1.3.0/docusign_admin/models/link_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/member_group_response.py` & `docusign-admin-1.3.0/docusign_admin/models/member_group_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/member_groups_response.py` & `docusign-admin-1.3.0/docusign_admin/models/member_groups_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/membership_response.py` & `docusign-admin-1.3.0/docusign_admin/models/membership_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/new_account_user_request.py` & `docusign-admin-1.3.0/docusign_admin/models/new_account_user_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/new_multi_product_user_add_request.py` & `docusign-admin-1.3.0/docusign_admin/models/new_multi_product_user_add_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/new_user_request.py` & `docusign-admin-1.3.0/docusign_admin/models/new_user_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/new_user_request_account_properties.py` & `docusign-admin-1.3.0/docusign_admin/models/new_user_request_account_properties.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/new_user_response.py` & `docusign-admin-1.3.0/docusign_admin/models/new_user_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/new_user_response_account_properties.py` & `docusign-admin-1.3.0/docusign_admin/models/new_user_response_account_properties.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/oasirr_error_details.py` & `docusign-admin-1.3.0/docusign_admin/models/oasirr_error_details.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/oasirr_organization_account_settings_error_data_response.py` & `docusign-admin-1.3.0/docusign_admin/models/oasirr_organization_account_settings_error_data_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/oetr_error_details.py` & `docusign-admin-1.3.0/docusign_admin/models/oetr_error_details.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_export_selected_account.py` & `docusign-admin-1.3.0/docusign_admin/models/org_export_selected_account.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_export_selected_domain.py` & `docusign-admin-1.3.0/docusign_admin/models/org_export_selected_domain.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_report_configuration_response.py` & `docusign-admin-1.3.0/docusign_admin/models/org_report_configuration_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_report_create_response.py` & `docusign-admin-1.3.0/docusign_admin/models/org_report_create_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_report_list_response.py` & `docusign-admin-1.3.0/docusign_admin/models/org_report_list_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_report_list_response_org_report.py` & `docusign-admin-1.3.0/docusign_admin/models/org_report_list_response_org_report.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_report_list_response_requestor.py` & `docusign-admin-1.3.0/docusign_admin/models/org_report_list_response_requestor.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/org_report_request.py` & `docusign-admin-1.3.0/docusign_admin/models/org_report_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_account_request.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_account_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_account_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_account_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_account_settings_import_requestor_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_account_settings_import_requestor_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_account_settings_import_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_account_settings_import_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_account_settings_import_result_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_account_settings_import_result_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_accounts_request.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_accounts_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_export_account.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_export_account.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_export_domain.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_export_domain.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_export_request.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_export_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_export_requestor_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_export_requestor_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_export_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_export_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_export_task_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_export_task_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_exports_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_exports_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_import_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_import_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_import_response_error_rollup.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_import_response_error_rollup.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_import_response_requestor.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_import_response_requestor.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_import_response_warning_rollup.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_import_response_warning_rollup.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_imports_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_imports_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_salesforce_account_managers_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_salesforce_account_managers_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_simple_id_object.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_simple_id_object.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_user_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_user_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organization_users_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organization_users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/organizations_response.py` & `docusign-admin-1.3.0/docusign_admin/models/organizations_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/osamr_contact.py` & `docusign-admin-1.3.0/docusign_admin/models/osamr_contact.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/paging_response_properties.py` & `docusign-admin-1.3.0/docusign_admin/models/paging_response_properties.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/permission_profile_request.py` & `docusign-admin-1.3.0/docusign_admin/models/permission_profile_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/permission_profile_response.py` & `docusign-admin-1.3.0/docusign_admin/models/permission_profile_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/permission_profile_response21.py` & `docusign-admin-1.3.0/docusign_admin/models/permission_profile_response21.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/permissions_response.py` & `docusign-admin-1.3.0/docusign_admin/models/permissions_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/product_permission_profile_request.py` & `docusign-admin-1.3.0/docusign_admin/models/product_permission_profile_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/product_permission_profile_response.py` & `docusign-admin-1.3.0/docusign_admin/models/product_permission_profile_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/product_permission_profiles_request.py` & `docusign-admin-1.3.0/docusign_admin/models/product_permission_profiles_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/product_permission_profiles_response.py` & `docusign-admin-1.3.0/docusign_admin/models/product_permission_profiles_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/remove_ds_group_users_response.py` & `docusign-admin-1.3.0/docusign_admin/models/remove_ds_group_users_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/remove_user_products_response.py` & `docusign-admin-1.3.0/docusign_admin/models/remove_user_products_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/required_attribute_mapping_response.py` & `docusign-admin-1.3.0/docusign_admin/models/required_attribute_mapping_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/saml2_identity_provider_response.py` & `docusign-admin-1.3.0/docusign_admin/models/saml2_identity_provider_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/setting_response.py` & `docusign-admin-1.3.0/docusign_admin/models/setting_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/update_membership_request.py` & `docusign-admin-1.3.0/docusign_admin/models/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/update_response.py` & `docusign-admin-1.3.0/docusign_admin/models/update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/update_user_email_request.py` & `docusign-admin-1.3.0/docusign_admin/models/update_user_email_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/update_user_request.py` & `docusign-admin-1.3.0/docusign_admin/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/update_users_email_request.py` & `docusign-admin-1.3.0/docusign_admin/models/update_users_email_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/update_users_request.py` & `docusign-admin-1.3.0/docusign_admin/models/update_users_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_drilldown_response.py` & `docusign-admin-1.3.0/docusign_admin/models/user_drilldown_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_identity_request.py` & `docusign-admin-1.3.0/docusign_admin/models/user_identity_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_identity_response.py` & `docusign-admin-1.3.0/docusign_admin/models/user_identity_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_product_permission_profiles_request.py` & `docusign-admin-1.3.0/docusign_admin/models/user_product_permission_profiles_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_product_permission_profiles_response.py` & `docusign-admin-1.3.0/docusign_admin/models/user_product_permission_profiles_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_product_profile_delete_request.py` & `docusign-admin-1.3.0/docusign_admin/models/user_product_profile_delete_request.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/user_update_response.py` & `docusign-admin-1.3.0/docusign_admin/models/user_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/users_drilldown_response.py` & `docusign-admin-1.3.0/docusign_admin/models/users_drilldown_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin/models/users_update_response.py` & `docusign-admin-1.3.0/docusign_admin/models/users_update_response.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/docusign_admin.egg-info/PKG-INFO` & `docusign-admin-1.3.0/docusign_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docusign-admin
-Version: 1.2.0
+Version: 1.3.0
 Summary: DocuSign Admin API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,DocuSign Admin API
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docusign-admin Version: 1.2.0 Summary: DocuSign
+Metadata-Version: 2.1 Name: docusign-admin Version: 1.3.0 Summary: DocuSign
 Admin API Home-page: Author-email: devcenter@docusign.com Keywords:
 Swagger,DocuSign Admin API Description-Content-Type: text/markdown License-
 File: LICENSE # The Official DocuSign OrgAdmin Python Client [![PyPI version]
 [pypi-image]][pypi-url]  [![Build status][travis-image]][travis-url] [PyPI
 module](https://pypi.python.org/pypi/docusign_admin) that wraps the DocuSign
 OrgAdmin API [Documentation about the DocuSign OrgAdmin API](https://
 developers.docusign.com/) ## Requirements - Python 2.7 (3.7+ recommended) -
```

### Comparing `docusign-admin-1.2.0/docusign_admin.egg-info/SOURCES.txt` & `docusign-admin-1.3.0/docusign_admin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docusign_admin.egg-info/top_level.txt
 docusign_admin/apis/__init__.py
 docusign_admin/apis/accounts_api.py
 docusign_admin/apis/bulk_exports_api.py
 docusign_admin/apis/bulk_imports_api.py
 docusign_admin/apis/ds_groups_api.py
 docusign_admin/apis/identity_providers_api.py
+docusign_admin/apis/organizations_api.py
 docusign_admin/apis/product_permission_profiles_api.py
 docusign_admin/apis/reserved_domains_api.py
 docusign_admin/apis/users_api.py
 docusign_admin/client/__init__.py
 docusign_admin/client/api_client.py
 docusign_admin/client/api_exception.py
 docusign_admin/client/api_response.py
@@ -48,17 +49,22 @@
 docusign_admin/models/ds_group_users_remove_request.py
 docusign_admin/models/ds_group_users_response.py
 docusign_admin/models/error_details.py
 docusign_admin/models/force_activate_membership_request.py
 docusign_admin/models/group_request.py
 docusign_admin/models/identity_provider_response.py
 docusign_admin/models/identity_providers_response.py
+docusign_admin/models/individual_membership_data_redaction_request.py
+docusign_admin/models/individual_user_data_redaction_request.py
+docusign_admin/models/individual_user_data_redaction_response.py
 docusign_admin/models/link_response.py
 docusign_admin/models/member_group_response.py
 docusign_admin/models/member_groups_response.py
+docusign_admin/models/membership_data_redaction_request.py
+docusign_admin/models/membership_data_redaction_response.py
 docusign_admin/models/membership_response.py
 docusign_admin/models/new_account_user_request.py
 docusign_admin/models/new_multi_product_user_add_request.py
 docusign_admin/models/new_user_request.py
 docusign_admin/models/new_user_request_account_properties.py
 docusign_admin/models/new_user_response.py
 docusign_admin/models/new_user_response_account_properties.py
```

### Comparing `docusign-admin-1.2.0/setup.py` & `docusign-admin-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages, Command, os  # noqa: H301	
 
 NAME = "docusign-admin"
-VERSION = "1.2.0"
+VERSION = "1.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `docusign-admin-1.2.0/test/test_oauth.py` & `docusign-admin-1.3.0/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-admin-1.2.0/test/unit_tests.py` & `docusign-admin-1.3.0/test/unit_tests.py`

 * *Files identical despite different names*

