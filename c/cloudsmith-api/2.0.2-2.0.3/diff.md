# Comparing `tmp/cloudsmith_api-2.0.2-py2.py3-none-any.whl.zip` & `tmp/cloudsmith_api-2.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,409 +1,413 @@
-Zip file size: 711364 bytes, number of entries: 407
--rw-r--r--  2.0 unx    15755 b- defN 23-May-01 11:28 cloudsmith_api/__init__.py
--rw-r--r--  2.0 unx    25067 b- defN 23-May-01 11:28 cloudsmith_api/api_client.py
--rw-r--r--  2.0 unx     8390 b- defN 23-May-01 11:28 cloudsmith_api/configuration.py
--rw-r--r--  2.0 unx    13166 b- defN 23-May-01 11:28 cloudsmith_api/rest.py
--rw-r--r--  2.0 unx     1131 b- defN 23-May-01 11:28 cloudsmith_api/api/__init__.py
--rw-r--r--  2.0 unx    11039 b- defN 23-May-01 11:28 cloudsmith_api/api/audit_log_api.py
--rw-r--r--  2.0 unx    11425 b- defN 23-May-01 11:28 cloudsmith_api/api/badges_api.py
--rw-r--r--  2.0 unx     7978 b- defN 23-May-01 11:28 cloudsmith_api/api/distros_api.py
--rw-r--r--  2.0 unx    54786 b- defN 23-May-01 11:28 cloudsmith_api/api/entitlements_api.py
--rw-r--r--  2.0 unx    26620 b- defN 23-May-01 11:28 cloudsmith_api/api/files_api.py
--rw-r--r--  2.0 unx     7930 b- defN 23-May-01 11:28 cloudsmith_api/api/formats_api.py
--rw-r--r--  2.0 unx    19214 b- defN 23-May-01 11:28 cloudsmith_api/api/metrics_api.py
--rw-r--r--  2.0 unx     8514 b- defN 23-May-01 11:28 cloudsmith_api/api/namespaces_api.py
--rw-r--r--  2.0 unx   195413 b- defN 23-May-01 11:28 cloudsmith_api/api/orgs_api.py
--rw-r--r--  2.0 unx   275618 b- defN 23-May-01 11:28 cloudsmith_api/api/packages_api.py
--rw-r--r--  2.0 unx    16386 b- defN 23-May-01 11:28 cloudsmith_api/api/quota_api.py
--rw-r--r--  2.0 unx     4157 b- defN 23-May-01 11:28 cloudsmith_api/api/rates_api.py
--rw-r--r--  2.0 unx    98642 b- defN 23-May-01 11:28 cloudsmith_api/api/repos_api.py
--rw-r--r--  2.0 unx     4118 b- defN 23-May-01 11:28 cloudsmith_api/api/status_api.py
--rw-r--r--  2.0 unx     8075 b- defN 23-May-01 11:28 cloudsmith_api/api/storage_regions_api.py
--rw-r--r--  2.0 unx     7631 b- defN 23-May-01 11:28 cloudsmith_api/api/user_api.py
--rw-r--r--  2.0 unx     4706 b- defN 23-May-01 11:28 cloudsmith_api/api/users_api.py
--rw-r--r--  2.0 unx    22056 b- defN 23-May-01 11:28 cloudsmith_api/api/vulnerabilities_api.py
--rw-r--r--  2.0 unx    26050 b- defN 23-May-01 11:28 cloudsmith_api/api/webhooks_api.py
--rw-r--r--  2.0 unx    14558 b- defN 23-May-01 11:28 cloudsmith_api/models/__init__.py
--rw-r--r--  2.0 unx     7305 b- defN 23-May-01 11:28 cloudsmith_api/models/allocated_limit.py
--rw-r--r--  2.0 unx     5410 b- defN 23-May-01 11:28 cloudsmith_api/models/allocated_limit_raw.py
--rw-r--r--  2.0 unx    58771 b- defN 23-May-01 11:28 cloudsmith_api/models/alpine_package_upload.py
--rw-r--r--  2.0 unx     7437 b- defN 23-May-01 11:28 cloudsmith_api/models/alpine_package_upload_request.py
--rw-r--r--  2.0 unx     4748 b- defN 23-May-01 11:28 cloudsmith_api/models/architecture.py
--rw-r--r--  2.0 unx    58494 b- defN 23-May-01 11:28 cloudsmith_api/models/cargo_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-May-01 11:28 cloudsmith_api/models/cargo_package_upload_request.py
--rw-r--r--  2.0 unx    59602 b- defN 23-May-01 11:28 cloudsmith_api/models/cocoapods_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-May-01 11:28 cloudsmith_api/models/cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx     6052 b- defN 23-May-01 11:28 cloudsmith_api/models/common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     5636 b- defN 23-May-01 11:28 cloudsmith_api/models/common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx     6052 b- defN 23-May-01 11:28 cloudsmith_api/models/common_downloads_metrics.py
--rw-r--r--  2.0 unx     3526 b- defN 23-May-01 11:28 cloudsmith_api/models/common_downloads_metrics_value.py
--rw-r--r--  2.0 unx     6129 b- defN 23-May-01 11:28 cloudsmith_api/models/common_metrics.py
--rw-r--r--  2.0 unx    59325 b- defN 23-May-01 11:28 cloudsmith_api/models/composer_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-May-01 11:28 cloudsmith_api/models/composer_package_upload_request.py
--rw-r--r--  2.0 unx    61539 b- defN 23-May-01 11:28 cloudsmith_api/models/conan_package_upload.py
--rw-r--r--  2.0 unx    14491 b- defN 23-May-01 11:28 cloudsmith_api/models/conan_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-May-01 11:28 cloudsmith_api/models/conda_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-May-01 11:28 cloudsmith_api/models/conda_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/cran_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/cran_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/dart_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/dart_package_upload_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-01 11:28 cloudsmith_api/models/deb_package_upload.py
--rw-r--r--  2.0 unx     9690 b- defN 23-May-01 11:28 cloudsmith_api/models/deb_package_upload_request.py
--rw-r--r--  2.0 unx     6159 b- defN 23-May-01 11:28 cloudsmith_api/models/distribution.py
--rw-r--r--  2.0 unx     8542 b- defN 23-May-01 11:28 cloudsmith_api/models/distribution_full.py
--rw-r--r--  2.0 unx     4497 b- defN 23-May-01 11:28 cloudsmith_api/models/distribution_version.py
--rw-r--r--  2.0 unx    58771 b- defN 23-May-01 11:28 cloudsmith_api/models/docker_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-May-01 11:28 cloudsmith_api/models/docker_package_upload_request.py
--rw-r--r--  2.0 unx     3541 b- defN 23-May-01 11:28 cloudsmith_api/models/entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     3729 b- defN 23-May-01 11:28 cloudsmith_api/models/error_detail.py
--rw-r--r--  2.0 unx     5590 b- defN 23-May-01 11:28 cloudsmith_api/models/eula.py
--rw-r--r--  2.0 unx    11287 b- defN 23-May-01 11:28 cloudsmith_api/models/format.py
--rw-r--r--  2.0 unx     7319 b- defN 23-May-01 11:28 cloudsmith_api/models/format_support.py
--rw-r--r--  2.0 unx     8615 b- defN 23-May-01 11:28 cloudsmith_api/models/geo_ip_location.py
--rw-r--r--  2.0 unx    57663 b- defN 23-May-01 11:28 cloudsmith_api/models/go_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-May-01 11:28 cloudsmith_api/models/go_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/helm_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/helm_package_upload_request.py
--rw-r--r--  2.0 unx     7028 b- defN 23-May-01 11:28 cloudsmith_api/models/history.py
--rw-r--r--  2.0 unx     5168 b- defN 23-May-01 11:28 cloudsmith_api/models/history_fieldset.py
--rw-r--r--  2.0 unx     5246 b- defN 23-May-01 11:28 cloudsmith_api/models/history_fieldset_raw.py
--rw-r--r--  2.0 unx    59325 b- defN 23-May-01 11:28 cloudsmith_api/models/luarocks_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-May-01 11:28 cloudsmith_api/models/luarocks_package_upload_request.py
--rw-r--r--  2.0 unx    61667 b- defN 23-May-01 11:28 cloudsmith_api/models/maven_package_upload.py
--rw-r--r--  2.0 unx    14513 b- defN 23-May-01 11:28 cloudsmith_api/models/maven_package_upload_request.py
--rw-r--r--  2.0 unx     5806 b- defN 23-May-01 11:28 cloudsmith_api/models/namespace.py
--rw-r--r--  2.0 unx    18223 b- defN 23-May-01 11:28 cloudsmith_api/models/namespace_audit_log.py
--rw-r--r--  2.0 unx    10461 b- defN 23-May-01 11:28 cloudsmith_api/models/nested_license_policy.py
--rw-r--r--  2.0 unx    11097 b- defN 23-May-01 11:28 cloudsmith_api/models/nested_vulnerability_policy.py
--rw-r--r--  2.0 unx     9219 b- defN 23-May-01 11:28 cloudsmith_api/models/nested_vulnerability_scan_results.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-01 11:28 cloudsmith_api/models/npm_package_upload.py
--rw-r--r--  2.0 unx     7663 b- defN 23-May-01 11:28 cloudsmith_api/models/npm_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-May-01 11:28 cloudsmith_api/models/nuget_package_upload.py
--rw-r--r--  2.0 unx     7272 b- defN 23-May-01 11:28 cloudsmith_api/models/nuget_package_upload_request.py
--rw-r--r--  2.0 unx     7918 b- defN 23-May-01 11:28 cloudsmith_api/models/organization.py
--rw-r--r--  2.0 unx     8391 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_group_sync.py
--rw-r--r--  2.0 unx     8223 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_group_sync_request.py
--rw-r--r--  2.0 unx    10169 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite.py
--rw-r--r--  2.0 unx    10519 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_extend.py
--rw-r--r--  2.0 unx     5661 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_request.py
--rw-r--r--  2.0 unx     3821 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_update.py
--rw-r--r--  2.0 unx     3929 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx    12300 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_membership.py
--rw-r--r--  2.0 unx    11008 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_license_policy.py
--rw-r--r--  2.0 unx     8427 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_license_policy_request.py
--rw-r--r--  2.0 unx     8280 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_license_policy_request_patch.py
--rw-r--r--  2.0 unx    11620 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_vulnerability_policy.py
--rw-r--r--  2.0 unx     8967 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
--rw-r--r--  2.0 unx     8962 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
--rw-r--r--  2.0 unx     8110 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team.py
--rw-r--r--  2.0 unx     3669 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_members.py
--rw-r--r--  2.0 unx     4783 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_membership.py
--rw-r--r--  2.0 unx     7065 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_request.py
--rw-r--r--  2.0 unx     7040 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_request_patch.py
--rw-r--r--  2.0 unx    57663 b- defN 23-May-01 11:28 cloudsmith_api/models/p2_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-May-01 11:28 cloudsmith_api/models/p2_package_upload_request.py
--rw-r--r--  2.0 unx    55965 b- defN 23-May-01 11:28 cloudsmith_api/models/package.py
--rw-r--r--  2.0 unx    57197 b- defN 23-May-01 11:28 cloudsmith_api/models/package_copy.py
--rw-r--r--  2.0 unx     4776 b- defN 23-May-01 11:28 cloudsmith_api/models/package_copy_request.py
--rw-r--r--  2.0 unx     3523 b- defN 23-May-01 11:28 cloudsmith_api/models/package_dependencies.py
--rw-r--r--  2.0 unx     7227 b- defN 23-May-01 11:28 cloudsmith_api/models/package_dependency.py
--rw-r--r--  2.0 unx    12968 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file.py
--rw-r--r--  2.0 unx     6108 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file_parts_upload.py
--rw-r--r--  2.0 unx     7841 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file_upload.py
--rw-r--r--  2.0 unx     7815 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file_upload_request.py
--rw-r--r--  2.0 unx     6035 b- defN 23-May-01 11:28 cloudsmith_api/models/package_license_policy_violation_log.py
--rw-r--r--  2.0 unx     5198 b- defN 23-May-01 11:28 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    57195 b- defN 23-May-01 11:28 cloudsmith_api/models/package_move.py
--rw-r--r--  2.0 unx     3820 b- defN 23-May-01 11:28 cloudsmith_api/models/package_move_request.py
--rw-r--r--  2.0 unx    58775 b- defN 23-May-01 11:28 cloudsmith_api/models/package_quarantine.py
--rw-r--r--  2.0 unx     3527 b- defN 23-May-01 11:28 cloudsmith_api/models/package_quarantine_request.py
--rw-r--r--  2.0 unx    57651 b- defN 23-May-01 11:28 cloudsmith_api/models/package_resync.py
--rw-r--r--  2.0 unx    15877 b- defN 23-May-01 11:28 cloudsmith_api/models/package_status.py
--rw-r--r--  2.0 unx    57199 b- defN 23-May-01 11:28 cloudsmith_api/models/package_tag.py
--rw-r--r--  2.0 unx     5352 b- defN 23-May-01 11:28 cloudsmith_api/models/package_tag_request.py
--rw-r--r--  2.0 unx     3547 b- defN 23-May-01 11:28 cloudsmith_api/models/package_usage_metrics.py
--rw-r--r--  2.0 unx     2740 b- defN 23-May-01 11:28 cloudsmith_api/models/package_version_badge.py
--rw-r--r--  2.0 unx     5707 b- defN 23-May-01 11:28 cloudsmith_api/models/package_vulnerability.py
--rw-r--r--  2.0 unx     7491 b- defN 23-May-01 11:28 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
--rw-r--r--  2.0 unx     5318 b- defN 23-May-01 11:28 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    58771 b- defN 23-May-01 11:28 cloudsmith_api/models/python_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-May-01 11:28 cloudsmith_api/models/python_package_upload_request.py
--rw-r--r--  2.0 unx     3358 b- defN 23-May-01 11:28 cloudsmith_api/models/quota.py
--rw-r--r--  2.0 unx     3463 b- defN 23-May-01 11:28 cloudsmith_api/models/quota_history.py
--rw-r--r--  2.0 unx     7675 b- defN 23-May-01 11:28 cloudsmith_api/models/rate_check.py
--rw-r--r--  2.0 unx    58899 b- defN 23-May-01 11:28 cloudsmith_api/models/raw_package_upload.py
--rw-r--r--  2.0 unx    11674 b- defN 23-May-01 11:28 cloudsmith_api/models/raw_package_upload_request.py
--rw-r--r--  2.0 unx    66229 b- defN 23-May-01 11:28 cloudsmith_api/models/repository.py
--rw-r--r--  2.0 unx    14861 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_audit_log.py
--rw-r--r--  2.0 unx    67555 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_create.py
--rw-r--r--  2.0 unx    52996 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_create_request.py
--rw-r--r--  2.0 unx     4365 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_cidr.py
--rw-r--r--  2.0 unx     4488 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_country_code.py
--rw-r--r--  2.0 unx     4424 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_rules.py
--rw-r--r--  2.0 unx     4515 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_rules_request.py
--rw-r--r--  2.0 unx     4312 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
--rw-r--r--  2.0 unx     3733 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_test_address.py
--rw-r--r--  2.0 unx     3906 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_test_address_response.py
--rw-r--r--  2.0 unx     7359 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
--rw-r--r--  2.0 unx     8734 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_gpg_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_gpg_key_create.py
--rw-r--r--  2.0 unx     7702 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_dict.py
--rw-r--r--  2.0 unx     3818 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_input.py
--rw-r--r--  2.0 unx     3881 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_input_request.py
--rw-r--r--  2.0 unx     3790 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx    51807 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_request_patch.py
--rw-r--r--  2.0 unx     7753 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_rsa_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_rsa_key_create.py
--rw-r--r--  2.0 unx    40222 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token.py
--rw-r--r--  2.0 unx     2750 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_action.py
--rw-r--r--  2.0 unx    41219 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_refresh.py
--rw-r--r--  2.0 unx    21868 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_refresh_request.py
--rw-r--r--  2.0 unx    22374 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_request.py
--rw-r--r--  2.0 unx    22569 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_request_patch.py
--rw-r--r--  2.0 unx     3505 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_sync.py
--rw-r--r--  2.0 unx     3904 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_sync_request.py
--rw-r--r--  2.0 unx    30400 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_webhook.py
--rw-r--r--  2.0 unx    18912 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_webhook_request.py
--rw-r--r--  2.0 unx    18774 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_webhook_request_patch.py
--rw-r--r--  2.0 unx     3523 b- defN 23-May-01 11:28 cloudsmith_api/models/resources_rate_check.py
--rw-r--r--  2.0 unx     2790 b- defN 23-May-01 11:28 cloudsmith_api/models/respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     2825 b- defN 23-May-01 11:28 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-01 11:28 cloudsmith_api/models/rpm_package_upload.py
--rw-r--r--  2.0 unx     7374 b- defN 23-May-01 11:28 cloudsmith_api/models/rpm_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/ruby_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/ruby_package_upload_request.py
--rw-r--r--  2.0 unx     8234 b- defN 23-May-01 11:28 cloudsmith_api/models/service.py
--rw-r--r--  2.0 unx     6726 b- defN 23-May-01 11:28 cloudsmith_api/models/service_request.py
--rw-r--r--  2.0 unx     6701 b- defN 23-May-01 11:28 cloudsmith_api/models/service_request_patch.py
--rw-r--r--  2.0 unx     4951 b- defN 23-May-01 11:28 cloudsmith_api/models/service_teams.py
--rw-r--r--  2.0 unx     4584 b- defN 23-May-01 11:28 cloudsmith_api/models/status_basic.py
--rw-r--r--  2.0 unx     8478 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_allocated_limit.py
--rw-r--r--  2.0 unx     6140 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_allocated_limit_raw.py
--rw-r--r--  2.0 unx     4670 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_region.py
--rw-r--r--  2.0 unx     6847 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_usage.py
--rw-r--r--  2.0 unx     5048 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_usage_raw.py
--rw-r--r--  2.0 unx     2665 b- defN 23-May-01 11:28 cloudsmith_api/models/tags.py
--rw-r--r--  2.0 unx    59602 b- defN 23-May-01 11:28 cloudsmith_api/models/terraform_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-May-01 11:28 cloudsmith_api/models/terraform_package_upload_request.py
--rw-r--r--  2.0 unx     5738 b- defN 23-May-01 11:28 cloudsmith_api/models/usage.py
--rw-r--r--  2.0 unx     4147 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_fieldset.py
--rw-r--r--  2.0 unx     4277 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_limits.py
--rw-r--r--  2.0 unx     4334 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_limits_raw.py
--rw-r--r--  2.0 unx     4382 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_raw.py
--rw-r--r--  2.0 unx     3590 b- defN 23-May-01 11:28 cloudsmith_api/models/user_auth_token.py
--rw-r--r--  2.0 unx     4612 b- defN 23-May-01 11:28 cloudsmith_api/models/user_auth_token_request.py
--rw-r--r--  2.0 unx     8019 b- defN 23-May-01 11:28 cloudsmith_api/models/user_brief.py
--rw-r--r--  2.0 unx    11110 b- defN 23-May-01 11:28 cloudsmith_api/models/user_profile.py
--rw-r--r--  2.0 unx    60899 b- defN 23-May-01 11:28 cloudsmith_api/models/vagrant_package_upload.py
--rw-r--r--  2.0 unx     9492 b- defN 23-May-01 11:28 cloudsmith_api/models/vagrant_package_upload_request.py
--rw-r--r--  2.0 unx    13112 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability.py
--rw-r--r--  2.0 unx     5400 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan.py
--rw-r--r--  2.0 unx    10040 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan_results.py
--rw-r--r--  2.0 unx     9417 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx     8443 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan_version.py
--rw-r--r--  2.0 unx     4751 b- defN 23-May-01 11:28 cloudsmith_api/models/webhook_template.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-01 11:28 test/__init__.py
--rw-r--r--  2.0 unx      900 b- defN 23-May-01 11:28 test/test_allocated_limit.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_allocated_limit_raw.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_alpine_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_alpine_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-May-01 11:28 test/test_architecture.py
--rw-r--r--  2.0 unx     1083 b- defN 23-May-01 11:28 test/test_audit_log_api.py
--rw-r--r--  2.0 unx      883 b- defN 23-May-01 11:28 test/test_badges_api.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_cargo_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_cargo_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_cocoapods_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_common_downloads_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_common_downloads_metrics_value.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_common_metrics.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_composer_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_composer_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_conan_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_conan_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_conda_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_conda_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_cran_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_cran_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_dart_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_dart_package_upload_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_deb_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_deb_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-May-01 11:28 test/test_distribution.py
--rw-r--r--  2.0 unx      916 b- defN 23-May-01 11:28 test/test_distribution_full.py
--rw-r--r--  2.0 unx      940 b- defN 23-May-01 11:28 test/test_distribution_version.py
--rw-r--r--  2.0 unx     1019 b- defN 23-May-01 11:28 test/test_distros_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_docker_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_docker_package_upload_request.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     2550 b- defN 23-May-01 11:28 test/test_entitlements_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_error_detail.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-01 11:28 test/test_eula.py
--rw-r--r--  2.0 unx     1503 b- defN 23-May-01 11:28 test/test_files_api.py
--rw-r--r--  2.0 unx      834 b- defN 23-May-01 11:28 test/test_format.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_format_support.py
--rw-r--r--  2.0 unx     1022 b- defN 23-May-01 11:28 test/test_formats_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-May-01 11:28 test/test_geo_ip_location.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-01 11:28 test/test_go_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_go_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_helm_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_helm_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-May-01 11:28 test/test_history.py
--rw-r--r--  2.0 unx      908 b- defN 23-May-01 11:28 test/test_history_fieldset.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_history_fieldset_raw.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_luarocks_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_luarocks_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_maven_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_maven_package_upload_request.py
--rw-r--r--  2.0 unx     1335 b- defN 23-May-01 11:28 test/test_metrics_api.py
--rw-r--r--  2.0 unx      858 b- defN 23-May-01 11:28 test/test_namespace.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_namespace_audit_log.py
--rw-r--r--  2.0 unx     1051 b- defN 23-May-01 11:28 test/test_namespaces_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_nested_license_policy.py
--rw-r--r--  2.0 unx      990 b- defN 23-May-01 11:28 test/test_nested_vulnerability_policy.py
--rw-r--r--  2.0 unx     1032 b- defN 23-May-01 11:28 test/test_nested_vulnerability_scan_results.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_npm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_npm_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_nuget_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_nuget_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-May-01 11:28 test/test_organization.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_organization_group_sync.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_organization_group_sync_request.py
--rw-r--r--  2.0 unx      932 b- defN 23-May-01 11:28 test/test_organization_invite.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_organization_invite_extend.py
--rw-r--r--  2.0 unx      990 b- defN 23-May-01 11:28 test/test_organization_invite_request.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_organization_invite_update.py
--rw-r--r--  2.0 unx     1082 b- defN 23-May-01 11:28 test/test_organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx      964 b- defN 23-May-01 11:28 test/test_organization_membership.py
--rw-r--r--  2.0 unx     1048 b- defN 23-May-01 11:28 test/test_organization_package_license_policy.py
--rw-r--r--  2.0 unx     1106 b- defN 23-May-01 11:28 test/test_organization_package_license_policy_request.py
--rw-r--r--  2.0 unx     1148 b- defN 23-May-01 11:28 test/test_organization_package_license_policy_request_patch.py
--rw-r--r--  2.0 unx     1096 b- defN 23-May-01 11:28 test/test_organization_package_vulnerability_policy.py
--rw-r--r--  2.0 unx     1154 b- defN 23-May-01 11:28 test/test_organization_package_vulnerability_policy_request.py
--rw-r--r--  2.0 unx     1196 b- defN 23-May-01 11:28 test/test_organization_package_vulnerability_policy_request_patch.py
--rw-r--r--  2.0 unx      916 b- defN 23-May-01 11:28 test/test_organization_team.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_organization_team_members.py
--rw-r--r--  2.0 unx      998 b- defN 23-May-01 11:28 test/test_organization_team_membership.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_organization_team_request.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_organization_team_request_patch.py
--rw-r--r--  2.0 unx     8724 b- defN 23-May-01 11:28 test/test_orgs_api.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-01 11:28 test/test_p2_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_p2_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-May-01 11:28 test/test_package.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_package_copy.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_package_copy_request.py
--rw-r--r--  2.0 unx      940 b- defN 23-May-01 11:28 test/test_package_dependencies.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_package_dependency.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_package_file.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_package_file_parts_upload.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_package_file_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_package_file_upload_request.py
--rw-r--r--  2.0 unx     1050 b- defN 23-May-01 11:28 test/test_package_license_policy_violation_log.py
--rw-r--r--  2.0 unx     1134 b- defN 23-May-01 11:28 test/test_package_license_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_package_move.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_package_move_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_package_quarantine.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_package_quarantine_request.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_package_resync.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_package_status.py
--rw-r--r--  2.0 unx      868 b- defN 23-May-01 11:28 test/test_package_tag.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_package_tag_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_package_usage_metrics.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_package_version_badge.py
--rw-r--r--  2.0 unx      948 b- defN 23-May-01 11:28 test/test_package_vulnerability.py
--rw-r--r--  2.0 unx     1098 b- defN 23-May-01 11:28 test/test_package_vulnerability_policy_violation_log.py
--rw-r--r--  2.0 unx     1182 b- defN 23-May-01 11:28 test/test_package_vulnerability_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    11023 b- defN 23-May-01 11:28 test/test_packages_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_python_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_python_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-May-01 11:28 test/test_quota.py
--rw-r--r--  2.0 unx     1364 b- defN 23-May-01 11:28 test/test_quota_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-01 11:28 test/test_quota_history.py
--rw-r--r--  2.0 unx      860 b- defN 23-May-01 11:28 test/test_rate_check.py
--rw-r--r--  2.0 unx      862 b- defN 23-May-01 11:28 test/test_rates_api.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_raw_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_raw_package_upload_request.py
--rw-r--r--  2.0 unx     4407 b- defN 23-May-01 11:28 test/test_repos_api.py
--rw-r--r--  2.0 unx      866 b- defN 23-May-01 11:28 test/test_repository.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_repository_audit_log.py
--rw-r--r--  2.0 unx      916 b- defN 23-May-01 11:28 test/test_repository_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_repository_create_request.py
--rw-r--r--  2.0 unx      944 b- defN 23-May-01 11:28 test/test_repository_geo_ip_cidr.py
--rw-r--r--  2.0 unx     1002 b- defN 23-May-01 11:28 test/test_repository_geo_ip_country_code.py
--rw-r--r--  2.0 unx      952 b- defN 23-May-01 11:28 test/test_repository_geo_ip_rules.py
--rw-r--r--  2.0 unx     1010 b- defN 23-May-01 11:28 test/test_repository_geo_ip_rules_request.py
--rw-r--r--  2.0 unx     1052 b- defN 23-May-01 11:28 test/test_repository_geo_ip_rules_request_patch.py
--rw-r--r--  2.0 unx     1002 b- defN 23-May-01 11:28 test/test_repository_geo_ip_test_address.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-01 11:28 test/test_repository_geo_ip_test_address_response.py
--rw-r--r--  2.0 unx     1102 b- defN 23-May-01 11:28 test/test_repository_geo_ip_test_address_response_dict.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_repository_gpg_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_repository_gpg_key_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_repository_privilege_dict.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_repository_privilege_input.py
--rw-r--r--  2.0 unx     1040 b- defN 23-May-01 11:28 test/test_repository_privilege_input_request.py
--rw-r--r--  2.0 unx     1082 b- defN 23-May-01 11:28 test/test_repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_repository_request_patch.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_repository_rsa_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_repository_rsa_key_create.py
--rw-r--r--  2.0 unx      908 b- defN 23-May-01 11:28 test/test_repository_token.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_repository_token_action.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_repository_token_refresh.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_repository_token_refresh_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_repository_token_request.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_repository_token_request_patch.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_repository_token_sync.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_repository_token_sync_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_repository_webhook.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_repository_webhook_request.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_repository_webhook_request_patch.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_resources_rate_check.py
--rw-r--r--  2.0 unx     1026 b- defN 23-May-01 11:28 test/test_respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     1084 b- defN 23-May-01 11:28 test/test_respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_rpm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_rpm_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_ruby_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_ruby_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-May-01 11:28 test/test_service.py
--rw-r--r--  2.0 unx      900 b- defN 23-May-01 11:28 test/test_service_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_service_request_patch.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-01 11:28 test/test_service_teams.py
--rw-r--r--  2.0 unx      864 b- defN 23-May-01 11:28 test/test_status_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_status_basic.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_storage_allocated_limit.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_storage_allocated_limit_raw.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_storage_region.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-01 11:28 test/test_storage_regions_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-01 11:28 test/test_storage_usage.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-01 11:28 test/test_storage_usage_raw.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-01 11:28 test/test_tags.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_terraform_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_terraform_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-May-01 11:28 test/test_usage.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_usage_fieldset.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_usage_limits.py
--rw-r--r--  2.0 unx      902 b- defN 23-May-01 11:28 test/test_usage_limits_raw.py
--rw-r--r--  2.0 unx      852 b- defN 23-May-01 11:28 test/test_usage_raw.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_user_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-May-01 11:28 test/test_user_auth_token.py
--rw-r--r--  2.0 unx      952 b- defN 23-May-01 11:28 test/test_user_auth_token_request.py
--rw-r--r--  2.0 unx      860 b- defN 23-May-01 11:28 test/test_user_brief.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_user_profile.py
--rw-r--r--  2.0 unx      865 b- defN 23-May-01 11:28 test/test_users_api.py
--rw-r--r--  2.0 unx      950 b- defN 23-May-01 11:28 test/test_vagrant_package_upload.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_vagrant_package_upload_request.py
--rw-r--r--  2.0 unx     1491 b- defN 23-May-01 11:28 test/test_vulnerabilities_api.py
--rw-r--r--  2.0 unx      890 b- defN 23-May-01 11:28 test/test_vulnerability.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_vulnerability_scan.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_vulnerability_scan_results.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_vulnerability_scan_version.py
--rw-r--r--  2.0 unx      908 b- defN 23-May-01 11:28 test/test_webhook_template.py
--rw-r--r--  2.0 unx     1557 b- defN 23-May-01 11:28 test/test_webhooks_api.py
--rw-r--r--  2.0 unx      457 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    39488 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/RECORD
-407 files, 4221278 bytes uncompressed, 647576 bytes compressed:  84.7%
+Zip file size: 723282 bytes, number of entries: 411
+-rw-r--r--  2.0 unx    15910 b- defN 23-May-17 09:26 cloudsmith_api/__init__.py
+-rw-r--r--  2.0 unx    25067 b- defN 23-May-17 09:26 cloudsmith_api/api_client.py
+-rw-r--r--  2.0 unx     8390 b- defN 23-May-17 09:26 cloudsmith_api/configuration.py
+-rw-r--r--  2.0 unx    13166 b- defN 23-May-17 09:26 cloudsmith_api/rest.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-May-17 09:26 cloudsmith_api/api/__init__.py
+-rw-r--r--  2.0 unx    11039 b- defN 23-May-17 09:26 cloudsmith_api/api/audit_log_api.py
+-rw-r--r--  2.0 unx    11425 b- defN 23-May-17 09:26 cloudsmith_api/api/badges_api.py
+-rw-r--r--  2.0 unx     7978 b- defN 23-May-17 09:26 cloudsmith_api/api/distros_api.py
+-rw-r--r--  2.0 unx    54786 b- defN 23-May-17 09:26 cloudsmith_api/api/entitlements_api.py
+-rw-r--r--  2.0 unx    26620 b- defN 23-May-17 09:26 cloudsmith_api/api/files_api.py
+-rw-r--r--  2.0 unx     7930 b- defN 23-May-17 09:26 cloudsmith_api/api/formats_api.py
+-rw-r--r--  2.0 unx    19214 b- defN 23-May-17 09:26 cloudsmith_api/api/metrics_api.py
+-rw-r--r--  2.0 unx     8514 b- defN 23-May-17 09:26 cloudsmith_api/api/namespaces_api.py
+-rw-r--r--  2.0 unx   195413 b- defN 23-May-17 09:26 cloudsmith_api/api/orgs_api.py
+-rw-r--r--  2.0 unx   284986 b- defN 23-May-17 09:26 cloudsmith_api/api/packages_api.py
+-rw-r--r--  2.0 unx    16386 b- defN 23-May-17 09:26 cloudsmith_api/api/quota_api.py
+-rw-r--r--  2.0 unx     4157 b- defN 23-May-17 09:26 cloudsmith_api/api/rates_api.py
+-rw-r--r--  2.0 unx    98642 b- defN 23-May-17 09:26 cloudsmith_api/api/repos_api.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-May-17 09:26 cloudsmith_api/api/status_api.py
+-rw-r--r--  2.0 unx     8075 b- defN 23-May-17 09:26 cloudsmith_api/api/storage_regions_api.py
+-rw-r--r--  2.0 unx     7631 b- defN 23-May-17 09:26 cloudsmith_api/api/user_api.py
+-rw-r--r--  2.0 unx     4706 b- defN 23-May-17 09:26 cloudsmith_api/api/users_api.py
+-rw-r--r--  2.0 unx    22091 b- defN 23-May-17 09:26 cloudsmith_api/api/vulnerabilities_api.py
+-rw-r--r--  2.0 unx    26050 b- defN 23-May-17 09:26 cloudsmith_api/api/webhooks_api.py
+-rw-r--r--  2.0 unx    14713 b- defN 23-May-17 09:26 cloudsmith_api/models/__init__.py
+-rw-r--r--  2.0 unx     7305 b- defN 23-May-17 09:26 cloudsmith_api/models/allocated_limit.py
+-rw-r--r--  2.0 unx     5410 b- defN 23-May-17 09:26 cloudsmith_api/models/allocated_limit_raw.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-17 09:26 cloudsmith_api/models/alpine_package_upload.py
+-rw-r--r--  2.0 unx     7437 b- defN 23-May-17 09:26 cloudsmith_api/models/alpine_package_upload_request.py
+-rw-r--r--  2.0 unx     4748 b- defN 23-May-17 09:26 cloudsmith_api/models/architecture.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-17 09:26 cloudsmith_api/models/cargo_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-May-17 09:26 cloudsmith_api/models/cargo_package_upload_request.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-May-17 09:26 cloudsmith_api/models/cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-May-17 09:26 cloudsmith_api/models/cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-17 09:26 cloudsmith_api/models/common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     5636 b- defN 23-May-17 09:26 cloudsmith_api/models/common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-17 09:26 cloudsmith_api/models/common_downloads_metrics.py
+-rw-r--r--  2.0 unx     3526 b- defN 23-May-17 09:26 cloudsmith_api/models/common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx     6129 b- defN 23-May-17 09:26 cloudsmith_api/models/common_metrics.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-May-17 09:26 cloudsmith_api/models/composer_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-May-17 09:26 cloudsmith_api/models/composer_package_upload_request.py
+-rw-r--r--  2.0 unx    61539 b- defN 23-May-17 09:26 cloudsmith_api/models/conan_package_upload.py
+-rw-r--r--  2.0 unx    14491 b- defN 23-May-17 09:26 cloudsmith_api/models/conan_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-17 09:26 cloudsmith_api/models/conda_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-May-17 09:26 cloudsmith_api/models/conda_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/cran_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/cran_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/dart_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/dart_package_upload_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/deb_package_upload.py
+-rw-r--r--  2.0 unx     9690 b- defN 23-May-17 09:26 cloudsmith_api/models/deb_package_upload_request.py
+-rw-r--r--  2.0 unx     6159 b- defN 23-May-17 09:26 cloudsmith_api/models/distribution.py
+-rw-r--r--  2.0 unx     8542 b- defN 23-May-17 09:26 cloudsmith_api/models/distribution_full.py
+-rw-r--r--  2.0 unx     4497 b- defN 23-May-17 09:26 cloudsmith_api/models/distribution_version.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-17 09:26 cloudsmith_api/models/docker_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-May-17 09:26 cloudsmith_api/models/docker_package_upload_request.py
+-rw-r--r--  2.0 unx     3541 b- defN 23-May-17 09:26 cloudsmith_api/models/entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     3729 b- defN 23-May-17 09:26 cloudsmith_api/models/error_detail.py
+-rw-r--r--  2.0 unx     5458 b- defN 23-May-17 09:26 cloudsmith_api/models/eula.py
+-rw-r--r--  2.0 unx    11287 b- defN 23-May-17 09:26 cloudsmith_api/models/format.py
+-rw-r--r--  2.0 unx     7319 b- defN 23-May-17 09:26 cloudsmith_api/models/format_support.py
+-rw-r--r--  2.0 unx     8615 b- defN 23-May-17 09:26 cloudsmith_api/models/geo_ip_location.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-May-17 09:26 cloudsmith_api/models/go_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-May-17 09:26 cloudsmith_api/models/go_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/helm_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/helm_package_upload_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/hex_package_upload.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-May-17 09:26 cloudsmith_api/models/hex_package_upload_request.py
+-rw-r--r--  2.0 unx     7028 b- defN 23-May-17 09:26 cloudsmith_api/models/history.py
+-rw-r--r--  2.0 unx     5168 b- defN 23-May-17 09:26 cloudsmith_api/models/history_fieldset.py
+-rw-r--r--  2.0 unx     5246 b- defN 23-May-17 09:26 cloudsmith_api/models/history_fieldset_raw.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-May-17 09:26 cloudsmith_api/models/luarocks_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-May-17 09:26 cloudsmith_api/models/luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx    61667 b- defN 23-May-17 09:26 cloudsmith_api/models/maven_package_upload.py
+-rw-r--r--  2.0 unx    14513 b- defN 23-May-17 09:26 cloudsmith_api/models/maven_package_upload_request.py
+-rw-r--r--  2.0 unx     5806 b- defN 23-May-17 09:26 cloudsmith_api/models/namespace.py
+-rw-r--r--  2.0 unx    18223 b- defN 23-May-17 09:26 cloudsmith_api/models/namespace_audit_log.py
+-rw-r--r--  2.0 unx    11620 b- defN 23-May-17 09:26 cloudsmith_api/models/nested_license_policy.py
+-rw-r--r--  2.0 unx    12280 b- defN 23-May-17 09:26 cloudsmith_api/models/nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     9527 b- defN 23-May-17 09:26 cloudsmith_api/models/nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/npm_package_upload.py
+-rw-r--r--  2.0 unx     7663 b- defN 23-May-17 09:26 cloudsmith_api/models/npm_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-17 09:26 cloudsmith_api/models/nuget_package_upload.py
+-rw-r--r--  2.0 unx     7272 b- defN 23-May-17 09:26 cloudsmith_api/models/nuget_package_upload_request.py
+-rw-r--r--  2.0 unx     7918 b- defN 23-May-17 09:26 cloudsmith_api/models/organization.py
+-rw-r--r--  2.0 unx     8391 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_group_sync.py
+-rw-r--r--  2.0 unx     8223 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_group_sync_request.py
+-rw-r--r--  2.0 unx    10169 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite.py
+-rw-r--r--  2.0 unx    10519 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_extend.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_request.py
+-rw-r--r--  2.0 unx     3821 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_update.py
+-rw-r--r--  2.0 unx     3929 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx    12300 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_membership.py
+-rw-r--r--  2.0 unx    12219 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_license_policy.py
+-rw-r--r--  2.0 unx     9666 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     9539 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx    12855 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx    10230 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx    10245 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx     8110 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team.py
+-rw-r--r--  2.0 unx     3669 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_members.py
+-rw-r--r--  2.0 unx     4783 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_membership.py
+-rw-r--r--  2.0 unx     7065 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_request.py
+-rw-r--r--  2.0 unx     7040 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_request_patch.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-May-17 09:26 cloudsmith_api/models/p2_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-May-17 09:26 cloudsmith_api/models/p2_package_upload_request.py
+-rw-r--r--  2.0 unx    55965 b- defN 23-May-17 09:26 cloudsmith_api/models/package.py
+-rw-r--r--  2.0 unx    57197 b- defN 23-May-17 09:26 cloudsmith_api/models/package_copy.py
+-rw-r--r--  2.0 unx     4776 b- defN 23-May-17 09:26 cloudsmith_api/models/package_copy_request.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-May-17 09:26 cloudsmith_api/models/package_dependencies.py
+-rw-r--r--  2.0 unx     7227 b- defN 23-May-17 09:26 cloudsmith_api/models/package_dependency.py
+-rw-r--r--  2.0 unx    12968 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file.py
+-rw-r--r--  2.0 unx     6108 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file_parts_upload.py
+-rw-r--r--  2.0 unx     7841 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file_upload.py
+-rw-r--r--  2.0 unx     7815 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file_upload_request.py
+-rw-r--r--  2.0 unx     6035 b- defN 23-May-17 09:26 cloudsmith_api/models/package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     5198 b- defN 23-May-17 09:26 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    57195 b- defN 23-May-17 09:26 cloudsmith_api/models/package_move.py
+-rw-r--r--  2.0 unx     3820 b- defN 23-May-17 09:26 cloudsmith_api/models/package_move_request.py
+-rw-r--r--  2.0 unx    58775 b- defN 23-May-17 09:26 cloudsmith_api/models/package_quarantine.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-May-17 09:26 cloudsmith_api/models/package_quarantine_request.py
+-rw-r--r--  2.0 unx    57651 b- defN 23-May-17 09:26 cloudsmith_api/models/package_resync.py
+-rw-r--r--  2.0 unx    15877 b- defN 23-May-17 09:26 cloudsmith_api/models/package_status.py
+-rw-r--r--  2.0 unx    57199 b- defN 23-May-17 09:26 cloudsmith_api/models/package_tag.py
+-rw-r--r--  2.0 unx     5352 b- defN 23-May-17 09:26 cloudsmith_api/models/package_tag_request.py
+-rw-r--r--  2.0 unx     3547 b- defN 23-May-17 09:26 cloudsmith_api/models/package_usage_metrics.py
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-17 09:26 cloudsmith_api/models/package_version_badge.py
+-rw-r--r--  2.0 unx     5707 b- defN 23-May-17 09:26 cloudsmith_api/models/package_vulnerability.py
+-rw-r--r--  2.0 unx     7491 b- defN 23-May-17 09:26 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     5318 b- defN 23-May-17 09:26 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-17 09:26 cloudsmith_api/models/python_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-May-17 09:26 cloudsmith_api/models/python_package_upload_request.py
+-rw-r--r--  2.0 unx     3358 b- defN 23-May-17 09:26 cloudsmith_api/models/quota.py
+-rw-r--r--  2.0 unx     3463 b- defN 23-May-17 09:26 cloudsmith_api/models/quota_history.py
+-rw-r--r--  2.0 unx     7675 b- defN 23-May-17 09:26 cloudsmith_api/models/rate_check.py
+-rw-r--r--  2.0 unx    58899 b- defN 23-May-17 09:26 cloudsmith_api/models/raw_package_upload.py
+-rw-r--r--  2.0 unx    11674 b- defN 23-May-17 09:26 cloudsmith_api/models/raw_package_upload_request.py
+-rw-r--r--  2.0 unx    66229 b- defN 23-May-17 09:26 cloudsmith_api/models/repository.py
+-rw-r--r--  2.0 unx    14861 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_audit_log.py
+-rw-r--r--  2.0 unx    67555 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_create.py
+-rw-r--r--  2.0 unx    52996 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_create_request.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     4488 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx     4424 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     4312 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     3906 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     7359 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx     8734 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_gpg_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_gpg_key_create.py
+-rw-r--r--  2.0 unx     7702 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_dict.py
+-rw-r--r--  2.0 unx     3818 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_input.py
+-rw-r--r--  2.0 unx     3881 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     3790 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx    51807 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_request_patch.py
+-rw-r--r--  2.0 unx     7753 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_rsa_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_rsa_key_create.py
+-rw-r--r--  2.0 unx    40544 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_action.py
+-rw-r--r--  2.0 unx    41541 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_refresh.py
+-rw-r--r--  2.0 unx    21868 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_refresh_request.py
+-rw-r--r--  2.0 unx    22374 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_request.py
+-rw-r--r--  2.0 unx    22569 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_request_patch.py
+-rw-r--r--  2.0 unx     3505 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_sync.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_sync_request.py
+-rw-r--r--  2.0 unx    30728 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_webhook.py
+-rw-r--r--  2.0 unx    18912 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_webhook_request.py
+-rw-r--r--  2.0 unx    18774 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-May-17 09:26 cloudsmith_api/models/resources_rate_check.py
+-rw-r--r--  2.0 unx     2790 b- defN 23-May-17 09:26 cloudsmith_api/models/respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     2825 b- defN 23-May-17 09:26 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/rpm_package_upload.py
+-rw-r--r--  2.0 unx     7374 b- defN 23-May-17 09:26 cloudsmith_api/models/rpm_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/ruby_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/ruby_package_upload_request.py
+-rw-r--r--  2.0 unx     8234 b- defN 23-May-17 09:26 cloudsmith_api/models/service.py
+-rw-r--r--  2.0 unx     6726 b- defN 23-May-17 09:26 cloudsmith_api/models/service_request.py
+-rw-r--r--  2.0 unx     6701 b- defN 23-May-17 09:26 cloudsmith_api/models/service_request_patch.py
+-rw-r--r--  2.0 unx     4951 b- defN 23-May-17 09:26 cloudsmith_api/models/service_teams.py
+-rw-r--r--  2.0 unx     4584 b- defN 23-May-17 09:26 cloudsmith_api/models/status_basic.py
+-rw-r--r--  2.0 unx     8478 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_allocated_limit.py
+-rw-r--r--  2.0 unx     6140 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx     4670 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_region.py
+-rw-r--r--  2.0 unx     6847 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_usage.py
+-rw-r--r--  2.0 unx     5048 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_usage_raw.py
+-rw-r--r--  2.0 unx     2665 b- defN 23-May-17 09:26 cloudsmith_api/models/tags.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-May-17 09:26 cloudsmith_api/models/terraform_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-May-17 09:26 cloudsmith_api/models/terraform_package_upload_request.py
+-rw-r--r--  2.0 unx     5738 b- defN 23-May-17 09:26 cloudsmith_api/models/usage.py
+-rw-r--r--  2.0 unx     4147 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_fieldset.py
+-rw-r--r--  2.0 unx     4277 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_limits.py
+-rw-r--r--  2.0 unx     4334 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_limits_raw.py
+-rw-r--r--  2.0 unx     4382 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_raw.py
+-rw-r--r--  2.0 unx     3590 b- defN 23-May-17 09:26 cloudsmith_api/models/user_auth_token.py
+-rw-r--r--  2.0 unx     4612 b- defN 23-May-17 09:26 cloudsmith_api/models/user_auth_token_request.py
+-rw-r--r--  2.0 unx     8019 b- defN 23-May-17 09:26 cloudsmith_api/models/user_brief.py
+-rw-r--r--  2.0 unx    11110 b- defN 23-May-17 09:26 cloudsmith_api/models/user_profile.py
+-rw-r--r--  2.0 unx    60899 b- defN 23-May-17 09:26 cloudsmith_api/models/vagrant_package_upload.py
+-rw-r--r--  2.0 unx     9492 b- defN 23-May-17 09:26 cloudsmith_api/models/vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx    13112 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability.py
+-rw-r--r--  2.0 unx     5400 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan.py
+-rw-r--r--  2.0 unx    10348 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     9725 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx     8443 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan_version.py
+-rw-r--r--  2.0 unx     4751 b- defN 23-May-17 09:26 cloudsmith_api/models/webhook_template.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 09:26 test/__init__.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-17 09:26 test/test_allocated_limit.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_alpine_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_alpine_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-17 09:26 test/test_architecture.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-17 09:26 test/test_audit_log_api.py
+-rw-r--r--  2.0 unx      883 b- defN 23-May-17 09:26 test/test_badges_api.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_cargo_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_cargo_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_common_downloads_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_common_metrics.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_composer_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_composer_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_conan_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_conan_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_conda_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_conda_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_cran_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_cran_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_dart_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_dart_package_upload_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_deb_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_deb_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-17 09:26 test/test_distribution.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-17 09:26 test/test_distribution_full.py
+-rw-r--r--  2.0 unx      940 b- defN 23-May-17 09:26 test/test_distribution_version.py
+-rw-r--r--  2.0 unx     1019 b- defN 23-May-17 09:26 test/test_distros_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_docker_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_docker_package_upload_request.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-May-17 09:26 test/test_entitlements_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_error_detail.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-17 09:26 test/test_eula.py
+-rw-r--r--  2.0 unx     1503 b- defN 23-May-17 09:26 test/test_files_api.py
+-rw-r--r--  2.0 unx      834 b- defN 23-May-17 09:26 test/test_format.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_format_support.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-May-17 09:26 test/test_formats_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-17 09:26 test/test_geo_ip_location.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-17 09:26 test/test_go_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_go_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_helm_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_helm_package_upload_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_hex_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_hex_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-17 09:26 test/test_history.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-17 09:26 test/test_history_fieldset.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_history_fieldset_raw.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_luarocks_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_maven_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_maven_package_upload_request.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-May-17 09:26 test/test_metrics_api.py
+-rw-r--r--  2.0 unx      858 b- defN 23-May-17 09:26 test/test_namespace.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_namespace_audit_log.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-May-17 09:26 test/test_namespaces_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_nested_license_policy.py
+-rw-r--r--  2.0 unx      990 b- defN 23-May-17 09:26 test/test_nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1032 b- defN 23-May-17 09:26 test/test_nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_npm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_npm_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_nuget_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_nuget_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-17 09:26 test/test_organization.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_organization_group_sync.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_organization_group_sync_request.py
+-rw-r--r--  2.0 unx      932 b- defN 23-May-17 09:26 test/test_organization_invite.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_organization_invite_extend.py
+-rw-r--r--  2.0 unx      990 b- defN 23-May-17 09:26 test/test_organization_invite_request.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_organization_invite_update.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-May-17 09:26 test/test_organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx      964 b- defN 23-May-17 09:26 test/test_organization_membership.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-May-17 09:26 test/test_organization_package_license_policy.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-May-17 09:26 test/test_organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-May-17 09:26 test/test_organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-May-17 09:26 test/test_organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1154 b- defN 23-May-17 09:26 test/test_organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-May-17 09:26 test/test_organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-17 09:26 test/test_organization_team.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_organization_team_members.py
+-rw-r--r--  2.0 unx      998 b- defN 23-May-17 09:26 test/test_organization_team_membership.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_organization_team_request.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_organization_team_request_patch.py
+-rw-r--r--  2.0 unx     8724 b- defN 23-May-17 09:26 test/test_orgs_api.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-17 09:26 test/test_p2_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_p2_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-17 09:26 test/test_package.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_package_copy.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_package_copy_request.py
+-rw-r--r--  2.0 unx      940 b- defN 23-May-17 09:26 test/test_package_dependencies.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_package_dependency.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_package_file.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_package_file_parts_upload.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_package_file_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_package_file_upload_request.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-17 09:26 test/test_package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-17 09:26 test/test_package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_package_move.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_package_move_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_package_quarantine.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_package_quarantine_request.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_package_resync.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_package_status.py
+-rw-r--r--  2.0 unx      868 b- defN 23-May-17 09:26 test/test_package_tag.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_package_tag_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_package_usage_metrics.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_package_version_badge.py
+-rw-r--r--  2.0 unx      948 b- defN 23-May-17 09:26 test/test_package_vulnerability.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-May-17 09:26 test/test_package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     1182 b- defN 23-May-17 09:26 test/test_package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    11377 b- defN 23-May-17 09:26 test/test_packages_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_python_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_python_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-17 09:26 test/test_quota.py
+-rw-r--r--  2.0 unx     1364 b- defN 23-May-17 09:26 test/test_quota_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-17 09:26 test/test_quota_history.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-17 09:26 test/test_rate_check.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-17 09:26 test/test_rates_api.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_raw_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_raw_package_upload_request.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-17 09:26 test/test_repos_api.py
+-rw-r--r--  2.0 unx      866 b- defN 23-May-17 09:26 test/test_repository.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_repository_audit_log.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-17 09:26 test/test_repository_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_repository_create_request.py
+-rw-r--r--  2.0 unx      944 b- defN 23-May-17 09:26 test/test_repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-17 09:26 test/test_repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-17 09:26 test/test_repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-17 09:26 test/test_repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-May-17 09:26 test/test_repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-17 09:26 test/test_repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-17 09:26 test/test_repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-May-17 09:26 test/test_repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_repository_gpg_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_repository_gpg_key_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_repository_privilege_dict.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_repository_privilege_input.py
+-rw-r--r--  2.0 unx     1040 b- defN 23-May-17 09:26 test/test_repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-May-17 09:26 test/test_repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_repository_request_patch.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_repository_rsa_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_repository_rsa_key_create.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-17 09:26 test/test_repository_token.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_repository_token_action.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_repository_token_refresh.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_repository_token_refresh_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_repository_token_request.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_repository_token_request_patch.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_repository_token_sync.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_repository_token_sync_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_repository_webhook.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_repository_webhook_request.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_resources_rate_check.py
+-rw-r--r--  2.0 unx     1026 b- defN 23-May-17 09:26 test/test_respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     1084 b- defN 23-May-17 09:26 test/test_respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_rpm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_rpm_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_ruby_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_ruby_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-17 09:26 test/test_service.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-17 09:26 test/test_service_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_service_request_patch.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-17 09:26 test/test_service_teams.py
+-rw-r--r--  2.0 unx      864 b- defN 23-May-17 09:26 test/test_status_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_status_basic.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_storage_allocated_limit.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_storage_region.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-17 09:26 test/test_storage_regions_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-17 09:26 test/test_storage_usage.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-17 09:26 test/test_storage_usage_raw.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-17 09:26 test/test_tags.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_terraform_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_terraform_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-17 09:26 test/test_usage.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_usage_fieldset.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_usage_limits.py
+-rw-r--r--  2.0 unx      902 b- defN 23-May-17 09:26 test/test_usage_limits_raw.py
+-rw-r--r--  2.0 unx      852 b- defN 23-May-17 09:26 test/test_usage_raw.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_user_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-17 09:26 test/test_user_auth_token.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-17 09:26 test/test_user_auth_token_request.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-17 09:26 test/test_user_brief.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_user_profile.py
+-rw-r--r--  2.0 unx      865 b- defN 23-May-17 09:26 test/test_users_api.py
+-rw-r--r--  2.0 unx      950 b- defN 23-May-17 09:26 test/test_vagrant_package_upload.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx     1487 b- defN 23-May-17 09:26 test/test_vulnerabilities_api.py
+-rw-r--r--  2.0 unx      890 b- defN 23-May-17 09:26 test/test_vulnerability.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_vulnerability_scan.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_vulnerability_scan_version.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-17 09:26 test/test_webhook_template.py
+-rw-r--r--  2.0 unx     1557 b- defN 23-May-17 09:26 test/test_webhooks_api.py
+-rw-r--r--  2.0 unx      457 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    39881 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/RECORD
+411 files, 4309307 bytes uncompressed, 658862 bytes compressed:  84.7%
```

## zipnote {}

```diff
@@ -192,14 +192,20 @@
 
 Filename: cloudsmith_api/models/helm_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/helm_package_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/hex_package_upload.py
+Comment: 
+
+Filename: cloudsmith_api/models/hex_package_upload_request.py
+Comment: 
+
 Filename: cloudsmith_api/models/history.py
 Comment: 
 
 Filename: cloudsmith_api/models/history_fieldset.py
 Comment: 
 
 Filename: cloudsmith_api/models/history_fieldset_raw.py
@@ -750,14 +756,20 @@
 
 Filename: test/test_helm_package_upload.py
 Comment: 
 
 Filename: test/test_helm_package_upload_request.py
 Comment: 
 
+Filename: test/test_hex_package_upload.py
+Comment: 
+
+Filename: test/test_hex_package_upload_request.py
+Comment: 
+
 Filename: test/test_history.py
 Comment: 
 
 Filename: test/test_history_fieldset.py
 Comment: 
 
 Filename: test/test_history_fieldset_raw.py
@@ -1203,20 +1215,20 @@
 
 Filename: test/test_webhook_template.py
 Comment: 
 
 Filename: test/test_webhooks_api.py
 Comment: 
 
-Filename: cloudsmith_api-2.0.2.dist-info/METADATA
+Filename: cloudsmith_api-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cloudsmith_api-2.0.2.dist-info/WHEEL
+Filename: cloudsmith_api-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cloudsmith_api-2.0.2.dist-info/top_level.txt
+Filename: cloudsmith_api-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudsmith_api-2.0.2.dist-info/RECORD
+Filename: cloudsmith_api-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudsmith_api/__init__.py

```diff
@@ -77,14 +77,16 @@
 from cloudsmith_api.models.format import Format
 from cloudsmith_api.models.format_support import FormatSupport
 from cloudsmith_api.models.geo_ip_location import GeoIpLocation
 from cloudsmith_api.models.go_package_upload import GoPackageUpload
 from cloudsmith_api.models.go_package_upload_request import GoPackageUploadRequest
 from cloudsmith_api.models.helm_package_upload import HelmPackageUpload
 from cloudsmith_api.models.helm_package_upload_request import HelmPackageUploadRequest
+from cloudsmith_api.models.hex_package_upload import HexPackageUpload
+from cloudsmith_api.models.hex_package_upload_request import HexPackageUploadRequest
 from cloudsmith_api.models.history import History
 from cloudsmith_api.models.history_fieldset import HistoryFieldset
 from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw
 from cloudsmith_api.models.luarocks_package_upload import LuarocksPackageUpload
 from cloudsmith_api.models.luarocks_package_upload_request import LuarocksPackageUploadRequest
 from cloudsmith_api.models.maven_package_upload import MavenPackageUpload
 from cloudsmith_api.models.maven_package_upload_request import MavenPackageUploadRequest
```

## cloudsmith_api/api_client.py

```diff
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.0.2/python'
+        self.user_agent = 'Swagger-Codegen/2.0.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

## cloudsmith_api/configuration.py

```diff
@@ -254,9 +254,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 2.0.2".\
+               "SDK Package Version: 2.0.3".\
                format(env=sys.platform, pyversion=sys.version)
```

## cloudsmith_api/api/packages_api.py

```diff
@@ -2650,14 +2650,125 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def packages_upload_hex(self, owner, repo, **kwargs):  # noqa: E501
+        """Create a new Hex package  # noqa: E501
+
+        Create a new Hex package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_upload_hex(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param HexPackageUploadRequest data:
+        :return: HexPackageUpload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.packages_upload_hex_with_http_info(owner, repo, **kwargs)  # noqa: E501
+        else:
+            (data) = self.packages_upload_hex_with_http_info(owner, repo, **kwargs)  # noqa: E501
+            return data
+
+    def packages_upload_hex_with_http_info(self, owner, repo, **kwargs):  # noqa: E501
+        """Create a new Hex package  # noqa: E501
+
+        Create a new Hex package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_upload_hex_with_http_info(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param HexPackageUploadRequest data:
+        :return: HexPackageUpload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'repo', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method packages_upload_hex" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `packages_upload_hex`")  # noqa: E501
+        # verify the required parameter 'repo' is set
+        if self.api_client.client_side_validation and ('repo' not in params or
+                                                       params['repo'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `repo` when calling `packages_upload_hex`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'repo' in params:
+            path_params['repo'] = params['repo']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/packages/{owner}/{repo}/upload/hex/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='HexPackageUpload',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def packages_upload_luarocks(self, owner, repo, **kwargs):  # noqa: E501
         """Create a new LuaRocks package  # noqa: E501
 
         Create a new LuaRocks package  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.packages_upload_luarocks(owner, repo, async_req=True)
@@ -5196,14 +5307,125 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def packages_validate_upload_hex(self, owner, repo, **kwargs):  # noqa: E501
+        """Validate parameters for create Hex package  # noqa: E501
+
+        Validate parameters for create Hex package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_validate_upload_hex(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param HexPackageUploadRequest data:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.packages_validate_upload_hex_with_http_info(owner, repo, **kwargs)  # noqa: E501
+        else:
+            (data) = self.packages_validate_upload_hex_with_http_info(owner, repo, **kwargs)  # noqa: E501
+            return data
+
+    def packages_validate_upload_hex_with_http_info(self, owner, repo, **kwargs):  # noqa: E501
+        """Validate parameters for create Hex package  # noqa: E501
+
+        Validate parameters for create Hex package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_validate_upload_hex_with_http_info(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param HexPackageUploadRequest data:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'repo', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method packages_validate_upload_hex" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `packages_validate_upload_hex`")  # noqa: E501
+        # verify the required parameter 'repo' is set
+        if self.api_client.client_side_validation and ('repo' not in params or
+                                                       params['repo'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `repo` when calling `packages_validate_upload_hex`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'repo' in params:
+            path_params['repo'] = params['repo']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/packages/{owner}/{repo}/validate-upload/hex/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

## cloudsmith_api/api/vulnerabilities_api.py

```diff
@@ -259,59 +259,59 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def vulnerabilities_read(self, owner, repo, package, scan_id, **kwargs):  # noqa: E501
-        """Returns a Scan Result.  # noqa: E501
+    def vulnerabilities_read(self, owner, repo, package, identifier, **kwargs):  # noqa: E501
+        """Get a scan result.  # noqa: E501
 
-        Returns a Scan Result.  # noqa: E501
+        Get a scan result.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.vulnerabilities_read(owner, repo, package, scan_id, async_req=True)
+        >>> thread = api.vulnerabilities_read(owner, repo, package, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str repo: (required)
         :param str package: (required)
-        :param str scan_id: (required)
+        :param str identifier: (required)
         :return: VulnerabilityScanResults
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.vulnerabilities_read_with_http_info(owner, repo, package, scan_id, **kwargs)  # noqa: E501
+            return self.vulnerabilities_read_with_http_info(owner, repo, package, identifier, **kwargs)  # noqa: E501
         else:
-            (data) = self.vulnerabilities_read_with_http_info(owner, repo, package, scan_id, **kwargs)  # noqa: E501
+            (data) = self.vulnerabilities_read_with_http_info(owner, repo, package, identifier, **kwargs)  # noqa: E501
             return data
 
-    def vulnerabilities_read_with_http_info(self, owner, repo, package, scan_id, **kwargs):  # noqa: E501
-        """Returns a Scan Result.  # noqa: E501
+    def vulnerabilities_read_with_http_info(self, owner, repo, package, identifier, **kwargs):  # noqa: E501
+        """Get a scan result.  # noqa: E501
 
-        Returns a Scan Result.  # noqa: E501
+        Get a scan result.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.vulnerabilities_read_with_http_info(owner, repo, package, scan_id, async_req=True)
+        >>> thread = api.vulnerabilities_read_with_http_info(owner, repo, package, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str repo: (required)
         :param str package: (required)
-        :param str scan_id: (required)
+        :param str identifier: (required)
         :return: VulnerabilityScanResults
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['owner', 'repo', 'package', 'scan_id']  # noqa: E501
+        all_params = ['owner', 'repo', 'package', 'identifier']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -330,30 +330,30 @@
         if self.api_client.client_side_validation and ('repo' not in params or
                                                        params['repo'] is None):  # noqa: E501
             raise ValueError("Missing the required parameter `repo` when calling `vulnerabilities_read`")  # noqa: E501
         # verify the required parameter 'package' is set
         if self.api_client.client_side_validation and ('package' not in params or
                                                        params['package'] is None):  # noqa: E501
             raise ValueError("Missing the required parameter `package` when calling `vulnerabilities_read`")  # noqa: E501
-        # verify the required parameter 'scan_id' is set
-        if self.api_client.client_side_validation and ('scan_id' not in params or
-                                                       params['scan_id'] is None):  # noqa: E501
-            raise ValueError("Missing the required parameter `scan_id` when calling `vulnerabilities_read`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `vulnerabilities_read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'owner' in params:
             path_params['owner'] = params['owner']  # noqa: E501
         if 'repo' in params:
             path_params['repo'] = params['repo']  # noqa: E501
         if 'package' in params:
             path_params['package'] = params['package']  # noqa: E501
-        if 'scan_id' in params:
-            path_params['scan_id'] = params['scan_id']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -367,15 +367,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['apikey']  # noqa: E501
 
         return self.api_client.call_api(
-            '/vulnerabilities/{owner}/{repo}/{package}/{scan_id}/', 'GET',
+            '/vulnerabilities/{owner}/{repo}/{package}/{identifier}/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='VulnerabilityScanResults',  # noqa: E501
```

## cloudsmith_api/models/__init__.py

```diff
@@ -52,14 +52,16 @@
 from cloudsmith_api.models.format import Format
 from cloudsmith_api.models.format_support import FormatSupport
 from cloudsmith_api.models.geo_ip_location import GeoIpLocation
 from cloudsmith_api.models.go_package_upload import GoPackageUpload
 from cloudsmith_api.models.go_package_upload_request import GoPackageUploadRequest
 from cloudsmith_api.models.helm_package_upload import HelmPackageUpload
 from cloudsmith_api.models.helm_package_upload_request import HelmPackageUploadRequest
+from cloudsmith_api.models.hex_package_upload import HexPackageUpload
+from cloudsmith_api.models.hex_package_upload_request import HexPackageUploadRequest
 from cloudsmith_api.models.history import History
 from cloudsmith_api.models.history_fieldset import HistoryFieldset
 from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw
 from cloudsmith_api.models.luarocks_package_upload import LuarocksPackageUpload
 from cloudsmith_api.models.luarocks_package_upload_request import LuarocksPackageUploadRequest
 from cloudsmith_api.models.maven_package_upload import MavenPackageUpload
 from cloudsmith_api.models.maven_package_upload_request import MavenPackageUploadRequest
```

## cloudsmith_api/models/eula.py

```diff
@@ -50,15 +50,16 @@
 
         self._identifier = None
         self._number = None
         self.discriminator = None
 
         if identifier is not None:
             self.identifier = identifier
-        self.number = number
+        if number is not None:
+            self.number = number
 
     @property
     def identifier(self):
         """Gets the identifier of this Eula.
 
         A unique identifier that you can use for your own EULA tracking purposes. This might be a date, or a semantic version, etc. The only requirement is that it is unique across multiple EULAs.
 
@@ -101,16 +102,14 @@
         """Sets the number of this Eula.
 
         A sequential identifier that increments by one for each new commit in a repository.
 
         :param number: The number of this Eula.
         :type: int
         """
-        if self._configuration.client_side_validation and number is None:
-            raise ValueError("Invalid value for `number`, must not be `None`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 number is not None and number > 2147483647):  # noqa: E501
             raise ValueError("Invalid value for `number`, must be a value less than or equal to `2147483647`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 number is not None and number < 0):  # noqa: E501
             raise ValueError("Invalid value for `number`, must be a value greater than or equal to `0`")  # noqa: E501
```

## cloudsmith_api/models/nested_license_policy.py

```diff
@@ -34,43 +34,46 @@
     """
     swagger_types = {
         'allow_unknown_licenses': 'bool',
         'created_at': 'datetime',
         'description': 'str',
         'name': 'str',
         'on_violation_quarantine': 'bool',
+        'package_query_string': 'str',
         'slug_perm': 'str',
         'spdx_identifiers': 'list[str]',
         'updated_at': 'datetime',
         'url': 'str'
     }
 
     attribute_map = {
         'allow_unknown_licenses': 'allow_unknown_licenses',
         'created_at': 'created_at',
         'description': 'description',
         'name': 'name',
         'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string',
         'slug_perm': 'slug_perm',
         'spdx_identifiers': 'spdx_identifiers',
         'updated_at': 'updated_at',
         'url': 'url'
     }
 
-    def __init__(self, allow_unknown_licenses=None, created_at=None, description=None, name=None, on_violation_quarantine=None, slug_perm=None, spdx_identifiers=None, updated_at=None, url=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_licenses=None, created_at=None, description=None, name=None, on_violation_quarantine=None, package_query_string=None, slug_perm=None, spdx_identifiers=None, updated_at=None, url=None, _configuration=None):  # noqa: E501
         """NestedLicensePolicy - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_licenses = None
         self._created_at = None
         self._description = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self._slug_perm = None
         self._spdx_identifiers = None
         self._updated_at = None
         self._url = None
         self.discriminator = None
 
         if allow_unknown_licenses is not None:
@@ -79,14 +82,16 @@
             self.created_at = created_at
         if description is not None:
             self.description = description
         if name is not None:
             self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
         if slug_perm is not None:
             self.slug_perm = slug_perm
         self.spdx_identifiers = spdx_identifiers
         if updated_at is not None:
             self.updated_at = updated_at
         if url is not None:
             self.url = url
@@ -199,14 +204,38 @@
         :param on_violation_quarantine: The on_violation_quarantine of this NestedLicensePolicy.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
     @property
+    def package_query_string(self):
+        """Gets the package_query_string of this NestedLicensePolicy.
+
+
+        :return: The package_query_string of this NestedLicensePolicy.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this NestedLicensePolicy.
+
+
+        :param package_query_string: The package_query_string of this NestedLicensePolicy.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
+    @property
     def slug_perm(self):
         """Gets the slug_perm of this NestedLicensePolicy.
 
 
         :return: The slug_perm of this NestedLicensePolicy.
         :rtype: str
         """
```

## cloudsmith_api/models/nested_vulnerability_policy.py

```diff
@@ -35,43 +35,46 @@
     swagger_types = {
         'allow_unknown_severity': 'bool',
         'created_at': 'datetime',
         'description': 'str',
         'min_severity': 'str',
         'name': 'str',
         'on_violation_quarantine': 'bool',
+        'package_query_string': 'str',
         'slug_perm': 'str',
         'updated_at': 'datetime',
         'url': 'str'
     }
 
     attribute_map = {
         'allow_unknown_severity': 'allow_unknown_severity',
         'created_at': 'created_at',
         'description': 'description',
         'min_severity': 'min_severity',
         'name': 'name',
         'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string',
         'slug_perm': 'slug_perm',
         'updated_at': 'updated_at',
         'url': 'url'
     }
 
-    def __init__(self, allow_unknown_severity=None, created_at=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, slug_perm=None, updated_at=None, url=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_severity=None, created_at=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, package_query_string=None, slug_perm=None, updated_at=None, url=None, _configuration=None):  # noqa: E501
         """NestedVulnerabilityPolicy - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_severity = None
         self._created_at = None
         self._description = None
         self._min_severity = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self._slug_perm = None
         self._updated_at = None
         self._url = None
         self.discriminator = None
 
         if allow_unknown_severity is not None:
             self.allow_unknown_severity = allow_unknown_severity
@@ -81,14 +84,16 @@
             self.description = description
         if min_severity is not None:
             self.min_severity = min_severity
         if name is not None:
             self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
         if slug_perm is not None:
             self.slug_perm = slug_perm
         if updated_at is not None:
             self.updated_at = updated_at
         if url is not None:
             self.url = url
 
@@ -230,14 +235,38 @@
         :param on_violation_quarantine: The on_violation_quarantine of this NestedVulnerabilityPolicy.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
     @property
+    def package_query_string(self):
+        """Gets the package_query_string of this NestedVulnerabilityPolicy.
+
+
+        :return: The package_query_string of this NestedVulnerabilityPolicy.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this NestedVulnerabilityPolicy.
+
+
+        :param package_query_string: The package_query_string of this NestedVulnerabilityPolicy.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
+    @property
     def slug_perm(self):
         """Gets the slug_perm of this NestedVulnerabilityPolicy.
 
 
         :return: The slug_perm of this NestedVulnerabilityPolicy.
         :rtype: str
         """
```

## cloudsmith_api/models/nested_vulnerability_scan_results.py

```diff
@@ -201,24 +201,26 @@
 
         self._num_vulnerabilities = num_vulnerabilities
 
     @property
     def scan_id(self):
         """Gets the scan_id of this NestedVulnerabilityScanResults.
 
+        Deprecated (23-05-15): Please use 'identifier' instead. Previously: A monotonically increasing number that identified a scan within a repository.
 
         :return: The scan_id of this NestedVulnerabilityScanResults.
         :rtype: int
         """
         return self._scan_id
 
     @scan_id.setter
     def scan_id(self, scan_id):
         """Sets the scan_id of this NestedVulnerabilityScanResults.
 
+        Deprecated (23-05-15): Please use 'identifier' instead. Previously: A monotonically increasing number that identified a scan within a repository.
 
         :param scan_id: The scan_id of this NestedVulnerabilityScanResults.
         :type: int
         """
         if self._configuration.client_side_validation and scan_id is None:
             raise ValueError("Invalid value for `scan_id`, must not be `None`")  # noqa: E501
```

## cloudsmith_api/models/organization_package_license_policy.py

```diff
@@ -34,55 +34,60 @@
     """
     swagger_types = {
         'allow_unknown_licenses': 'bool',
         'created_at': 'datetime',
         'description': 'str',
         'name': 'str',
         'on_violation_quarantine': 'bool',
+        'package_query_string': 'str',
         'slug_perm': 'str',
         'spdx_identifiers': 'list[str]',
         'updated_at': 'datetime'
     }
 
     attribute_map = {
         'allow_unknown_licenses': 'allow_unknown_licenses',
         'created_at': 'created_at',
         'description': 'description',
         'name': 'name',
         'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string',
         'slug_perm': 'slug_perm',
         'spdx_identifiers': 'spdx_identifiers',
         'updated_at': 'updated_at'
     }
 
-    def __init__(self, allow_unknown_licenses=None, created_at=None, description=None, name=None, on_violation_quarantine=None, slug_perm=None, spdx_identifiers=None, updated_at=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_licenses=None, created_at=None, description=None, name=None, on_violation_quarantine=None, package_query_string=None, slug_perm=None, spdx_identifiers=None, updated_at=None, _configuration=None):  # noqa: E501
         """OrganizationPackageLicensePolicy - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_licenses = None
         self._created_at = None
         self._description = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self._slug_perm = None
         self._spdx_identifiers = None
         self._updated_at = None
         self.discriminator = None
 
         if allow_unknown_licenses is not None:
             self.allow_unknown_licenses = allow_unknown_licenses
         if created_at is not None:
             self.created_at = created_at
         if description is not None:
             self.description = description
         self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
         if slug_perm is not None:
             self.slug_perm = slug_perm
         self.spdx_identifiers = spdx_identifiers
         if updated_at is not None:
             self.updated_at = updated_at
 
     @property
@@ -201,14 +206,38 @@
         :param on_violation_quarantine: The on_violation_quarantine of this OrganizationPackageLicensePolicy.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
     @property
+    def package_query_string(self):
+        """Gets the package_query_string of this OrganizationPackageLicensePolicy.
+
+
+        :return: The package_query_string of this OrganizationPackageLicensePolicy.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this OrganizationPackageLicensePolicy.
+
+
+        :param package_query_string: The package_query_string of this OrganizationPackageLicensePolicy.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
+    @property
     def slug_perm(self):
         """Gets the slug_perm of this OrganizationPackageLicensePolicy.
 
 
         :return: The slug_perm of this OrganizationPackageLicensePolicy.
         :rtype: str
         """
```

## cloudsmith_api/models/organization_package_license_policy_request.py

```diff
@@ -33,45 +33,50 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'allow_unknown_licenses': 'bool',
         'description': 'str',
         'name': 'str',
         'on_violation_quarantine': 'bool',
+        'package_query_string': 'str',
         'spdx_identifiers': 'list[str]'
     }
 
     attribute_map = {
         'allow_unknown_licenses': 'allow_unknown_licenses',
         'description': 'description',
         'name': 'name',
         'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string',
         'spdx_identifiers': 'spdx_identifiers'
     }
 
-    def __init__(self, allow_unknown_licenses=None, description=None, name=None, on_violation_quarantine=None, spdx_identifiers=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_licenses=None, description=None, name=None, on_violation_quarantine=None, package_query_string=None, spdx_identifiers=None, _configuration=None):  # noqa: E501
         """OrganizationPackageLicensePolicyRequest - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_licenses = None
         self._description = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self._spdx_identifiers = None
         self.discriminator = None
 
         if allow_unknown_licenses is not None:
             self.allow_unknown_licenses = allow_unknown_licenses
         if description is not None:
             self.description = description
         self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
         self.spdx_identifiers = spdx_identifiers
 
     @property
     def allow_unknown_licenses(self):
         """Gets the allow_unknown_licenses of this OrganizationPackageLicensePolicyRequest.
 
 
@@ -165,14 +170,38 @@
         :param on_violation_quarantine: The on_violation_quarantine of this OrganizationPackageLicensePolicyRequest.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
     @property
+    def package_query_string(self):
+        """Gets the package_query_string of this OrganizationPackageLicensePolicyRequest.
+
+
+        :return: The package_query_string of this OrganizationPackageLicensePolicyRequest.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this OrganizationPackageLicensePolicyRequest.
+
+
+        :param package_query_string: The package_query_string of this OrganizationPackageLicensePolicyRequest.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
+    @property
     def spdx_identifiers(self):
         """Gets the spdx_identifiers of this OrganizationPackageLicensePolicyRequest.
 
 
         :return: The spdx_identifiers of this OrganizationPackageLicensePolicyRequest.
         :rtype: list[str]
         """
```

## cloudsmith_api/models/organization_package_license_policy_request_patch.py

```diff
@@ -33,46 +33,51 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'allow_unknown_licenses': 'bool',
         'description': 'str',
         'name': 'str',
         'on_violation_quarantine': 'bool',
+        'package_query_string': 'str',
         'spdx_identifiers': 'list[str]'
     }
 
     attribute_map = {
         'allow_unknown_licenses': 'allow_unknown_licenses',
         'description': 'description',
         'name': 'name',
         'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string',
         'spdx_identifiers': 'spdx_identifiers'
     }
 
-    def __init__(self, allow_unknown_licenses=None, description=None, name=None, on_violation_quarantine=None, spdx_identifiers=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_licenses=None, description=None, name=None, on_violation_quarantine=None, package_query_string=None, spdx_identifiers=None, _configuration=None):  # noqa: E501
         """OrganizationPackageLicensePolicyRequestPatch - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_licenses = None
         self._description = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self._spdx_identifiers = None
         self.discriminator = None
 
         if allow_unknown_licenses is not None:
             self.allow_unknown_licenses = allow_unknown_licenses
         if description is not None:
             self.description = description
         if name is not None:
             self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
         if spdx_identifiers is not None:
             self.spdx_identifiers = spdx_identifiers
 
     @property
     def allow_unknown_licenses(self):
         """Gets the allow_unknown_licenses of this OrganizationPackageLicensePolicyRequestPatch.
 
@@ -165,14 +170,38 @@
         :param on_violation_quarantine: The on_violation_quarantine of this OrganizationPackageLicensePolicyRequestPatch.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
     @property
+    def package_query_string(self):
+        """Gets the package_query_string of this OrganizationPackageLicensePolicyRequestPatch.
+
+
+        :return: The package_query_string of this OrganizationPackageLicensePolicyRequestPatch.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this OrganizationPackageLicensePolicyRequestPatch.
+
+
+        :param package_query_string: The package_query_string of this OrganizationPackageLicensePolicyRequestPatch.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
+    @property
     def spdx_identifiers(self):
         """Gets the spdx_identifiers of this OrganizationPackageLicensePolicyRequestPatch.
 
 
         :return: The spdx_identifiers of this OrganizationPackageLicensePolicyRequestPatch.
         :rtype: list[str]
         """
```

## cloudsmith_api/models/organization_package_vulnerability_policy.py

```diff
@@ -35,41 +35,44 @@
     swagger_types = {
         'allow_unknown_severity': 'bool',
         'created_at': 'datetime',
         'description': 'str',
         'min_severity': 'str',
         'name': 'str',
         'on_violation_quarantine': 'bool',
+        'package_query_string': 'str',
         'slug_perm': 'str',
         'updated_at': 'datetime'
     }
 
     attribute_map = {
         'allow_unknown_severity': 'allow_unknown_severity',
         'created_at': 'created_at',
         'description': 'description',
         'min_severity': 'min_severity',
         'name': 'name',
         'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string',
         'slug_perm': 'slug_perm',
         'updated_at': 'updated_at'
     }
 
-    def __init__(self, allow_unknown_severity=None, created_at=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, slug_perm=None, updated_at=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_severity=None, created_at=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, package_query_string=None, slug_perm=None, updated_at=None, _configuration=None):  # noqa: E501
         """OrganizationPackageVulnerabilityPolicy - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_severity = None
         self._created_at = None
         self._description = None
         self._min_severity = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self._slug_perm = None
         self._updated_at = None
         self.discriminator = None
 
         if allow_unknown_severity is not None:
             self.allow_unknown_severity = allow_unknown_severity
         if created_at is not None:
@@ -77,14 +80,16 @@
         if description is not None:
             self.description = description
         if min_severity is not None:
             self.min_severity = min_severity
         self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
         if slug_perm is not None:
             self.slug_perm = slug_perm
         if updated_at is not None:
             self.updated_at = updated_at
 
     @property
     def allow_unknown_severity(self):
@@ -232,14 +237,38 @@
         :param on_violation_quarantine: The on_violation_quarantine of this OrganizationPackageVulnerabilityPolicy.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
     @property
+    def package_query_string(self):
+        """Gets the package_query_string of this OrganizationPackageVulnerabilityPolicy.
+
+
+        :return: The package_query_string of this OrganizationPackageVulnerabilityPolicy.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this OrganizationPackageVulnerabilityPolicy.
+
+
+        :param package_query_string: The package_query_string of this OrganizationPackageVulnerabilityPolicy.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
+    @property
     def slug_perm(self):
         """Gets the slug_perm of this OrganizationPackageVulnerabilityPolicy.
 
 
         :return: The slug_perm of this OrganizationPackageVulnerabilityPolicy.
         :rtype: str
         """
```

## cloudsmith_api/models/organization_package_vulnerability_policy_request.py

```diff
@@ -33,47 +33,52 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'allow_unknown_severity': 'bool',
         'description': 'str',
         'min_severity': 'str',
         'name': 'str',
-        'on_violation_quarantine': 'bool'
+        'on_violation_quarantine': 'bool',
+        'package_query_string': 'str'
     }
 
     attribute_map = {
         'allow_unknown_severity': 'allow_unknown_severity',
         'description': 'description',
         'min_severity': 'min_severity',
         'name': 'name',
-        'on_violation_quarantine': 'on_violation_quarantine'
+        'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string'
     }
 
-    def __init__(self, allow_unknown_severity=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_severity=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, package_query_string=None, _configuration=None):  # noqa: E501
         """OrganizationPackageVulnerabilityPolicyRequest - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_severity = None
         self._description = None
         self._min_severity = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self.discriminator = None
 
         if allow_unknown_severity is not None:
             self.allow_unknown_severity = allow_unknown_severity
         if description is not None:
             self.description = description
         if min_severity is not None:
             self.min_severity = min_severity
         self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
 
     @property
     def allow_unknown_severity(self):
         """Gets the allow_unknown_severity of this OrganizationPackageVulnerabilityPolicyRequest.
 
         Denotes whether vulnerabilities detected by a security scan with an unknown severity are permitted by this policy.
 
@@ -195,14 +200,38 @@
 
         :param on_violation_quarantine: The on_violation_quarantine of this OrganizationPackageVulnerabilityPolicyRequest.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
+    @property
+    def package_query_string(self):
+        """Gets the package_query_string of this OrganizationPackageVulnerabilityPolicyRequest.
+
+
+        :return: The package_query_string of this OrganizationPackageVulnerabilityPolicyRequest.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this OrganizationPackageVulnerabilityPolicyRequest.
+
+
+        :param package_query_string: The package_query_string of this OrganizationPackageVulnerabilityPolicyRequest.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

## cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py

```diff
@@ -33,48 +33,53 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'allow_unknown_severity': 'bool',
         'description': 'str',
         'min_severity': 'str',
         'name': 'str',
-        'on_violation_quarantine': 'bool'
+        'on_violation_quarantine': 'bool',
+        'package_query_string': 'str'
     }
 
     attribute_map = {
         'allow_unknown_severity': 'allow_unknown_severity',
         'description': 'description',
         'min_severity': 'min_severity',
         'name': 'name',
-        'on_violation_quarantine': 'on_violation_quarantine'
+        'on_violation_quarantine': 'on_violation_quarantine',
+        'package_query_string': 'package_query_string'
     }
 
-    def __init__(self, allow_unknown_severity=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, _configuration=None):  # noqa: E501
+    def __init__(self, allow_unknown_severity=None, description=None, min_severity='Critical', name=None, on_violation_quarantine=None, package_query_string=None, _configuration=None):  # noqa: E501
         """OrganizationPackageVulnerabilityPolicyRequestPatch - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow_unknown_severity = None
         self._description = None
         self._min_severity = None
         self._name = None
         self._on_violation_quarantine = None
+        self._package_query_string = None
         self.discriminator = None
 
         if allow_unknown_severity is not None:
             self.allow_unknown_severity = allow_unknown_severity
         if description is not None:
             self.description = description
         if min_severity is not None:
             self.min_severity = min_severity
         if name is not None:
             self.name = name
         if on_violation_quarantine is not None:
             self.on_violation_quarantine = on_violation_quarantine
+        if package_query_string is not None:
+            self.package_query_string = package_query_string
 
     @property
     def allow_unknown_severity(self):
         """Gets the allow_unknown_severity of this OrganizationPackageVulnerabilityPolicyRequestPatch.
 
         Denotes whether vulnerabilities detected by a security scan with an unknown severity are permitted by this policy.
 
@@ -194,14 +199,38 @@
 
         :param on_violation_quarantine: The on_violation_quarantine of this OrganizationPackageVulnerabilityPolicyRequestPatch.
         :type: bool
         """
 
         self._on_violation_quarantine = on_violation_quarantine
 
+    @property
+    def package_query_string(self):
+        """Gets the package_query_string of this OrganizationPackageVulnerabilityPolicyRequestPatch.
+
+
+        :return: The package_query_string of this OrganizationPackageVulnerabilityPolicyRequestPatch.
+        :rtype: str
+        """
+        return self._package_query_string
+
+    @package_query_string.setter
+    def package_query_string(self, package_query_string):
+        """Sets the package_query_string of this OrganizationPackageVulnerabilityPolicyRequestPatch.
+
+
+        :param package_query_string: The package_query_string of this OrganizationPackageVulnerabilityPolicyRequestPatch.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                package_query_string is not None and len(package_query_string) < 1):
+            raise ValueError("Invalid value for `package_query_string`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._package_query_string = package_query_string
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

## cloudsmith_api/models/repository_token.py

```diff
@@ -528,24 +528,26 @@
 
         self._has_limits = has_limits
 
     @property
     def identifier(self):
         """Gets the identifier of this RepositoryToken.
 
+        Deprecated (23-05-15): Please use 'slug_perm' instead. Previously: A monotonically increasing number that identified an entitlement within a repository.
 
         :return: The identifier of this RepositoryToken.
         :rtype: int
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier):
         """Sets the identifier of this RepositoryToken.
 
+        Deprecated (23-05-15): Please use 'slug_perm' instead. Previously: A monotonically increasing number that identified an entitlement within a repository.
 
         :param identifier: The identifier of this RepositoryToken.
         :type: int
         """
 
         self._identifier = identifier
```

## cloudsmith_api/models/repository_token_refresh.py

```diff
@@ -529,24 +529,26 @@
 
         self._has_limits = has_limits
 
     @property
     def identifier(self):
         """Gets the identifier of this RepositoryTokenRefresh.
 
+        Deprecated (23-05-15): Please use 'slug_perm' instead. Previously: A monotonically increasing number that identified an entitlement within a repository.
 
         :return: The identifier of this RepositoryTokenRefresh.
         :rtype: int
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier):
         """Sets the identifier of this RepositoryTokenRefresh.
 
+        Deprecated (23-05-15): Please use 'slug_perm' instead. Previously: A monotonically increasing number that identified an entitlement within a repository.
 
         :param identifier: The identifier of this RepositoryTokenRefresh.
         :type: int
         """
 
         self._identifier = identifier
```

## cloudsmith_api/models/repository_webhook.py

```diff
@@ -321,24 +321,26 @@
 
         self._events = events
 
     @property
     def identifier(self):
         """Gets the identifier of this RepositoryWebhook.
 
+        Deprecated (23-05-15): Please use 'slug_perm' instead. Previously: A monotonically increasing number that identified a webhook request within a repository.
 
         :return: The identifier of this RepositoryWebhook.
         :rtype: int
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier):
         """Sets the identifier of this RepositoryWebhook.
 
+        Deprecated (23-05-15): Please use 'slug_perm' instead. Previously: A monotonically increasing number that identified a webhook request within a repository.
 
         :param identifier: The identifier of this RepositoryWebhook.
         :type: int
         """
 
         self._identifier = identifier
```

## cloudsmith_api/models/status_basic.py

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'detail': 'detail',
         'version': 'version'
     }
 
-    def __init__(self, detail='Cloudsmith API is operational.', version='1.249.4', _configuration=None):  # noqa: E501
+    def __init__(self, detail='Cloudsmith API is operational.', version='1.263.0', _configuration=None):  # noqa: E501
         """StatusBasic - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._detail = None
         self._version = None
```

## cloudsmith_api/models/vulnerability_scan_results.py

```diff
@@ -250,24 +250,26 @@
 
         self._scan = scan
 
     @property
     def scan_id(self):
         """Gets the scan_id of this VulnerabilityScanResults.
 
+        Deprecated (23-05-15): Please use 'identifier' instead. Previously: A monotonically increasing number that identified a scan within a repository.
 
         :return: The scan_id of this VulnerabilityScanResults.
         :rtype: int
         """
         return self._scan_id
 
     @scan_id.setter
     def scan_id(self, scan_id):
         """Sets the scan_id of this VulnerabilityScanResults.
 
+        Deprecated (23-05-15): Please use 'identifier' instead. Previously: A monotonically increasing number that identified a scan within a repository.
 
         :param scan_id: The scan_id of this VulnerabilityScanResults.
         :type: int
         """
         if self._configuration.client_side_validation and scan_id is None:
             raise ValueError("Invalid value for `scan_id`, must not be `None`")  # noqa: E501
```

## cloudsmith_api/models/vulnerability_scan_results_list.py

```diff
@@ -223,24 +223,26 @@
 
         self._package = package
 
     @property
     def scan_id(self):
         """Gets the scan_id of this VulnerabilityScanResultsList.
 
+        Deprecated (23-05-15): Please use 'identifier' instead. Previously: A monotonically increasing number that identified a scan within a repository.
 
         :return: The scan_id of this VulnerabilityScanResultsList.
         :rtype: int
         """
         return self._scan_id
 
     @scan_id.setter
     def scan_id(self, scan_id):
         """Sets the scan_id of this VulnerabilityScanResultsList.
 
+        Deprecated (23-05-15): Please use 'identifier' instead. Previously: A monotonically increasing number that identified a scan within a repository.
 
         :param scan_id: The scan_id of this VulnerabilityScanResultsList.
         :type: int
         """
         if self._configuration.client_side_validation and scan_id is None:
             raise ValueError("Invalid value for `scan_id`, must not be `None`")  # noqa: E501
```

## test/test_packages_api.py

```diff
@@ -186,14 +186,21 @@
     def test_packages_upload_helm(self):
         """Test case for packages_upload_helm
 
         Create a new Helm package  # noqa: E501
         """
         pass
 
+    def test_packages_upload_hex(self):
+        """Test case for packages_upload_hex
+
+        Create a new Hex package  # noqa: E501
+        """
+        pass
+
     def test_packages_upload_luarocks(self):
         """Test case for packages_upload_luarocks
 
         Create a new LuaRocks package  # noqa: E501
         """
         pass
 
@@ -347,14 +354,21 @@
     def test_packages_validate_upload_helm(self):
         """Test case for packages_validate_upload_helm
 
         Validate parameters for create Helm package  # noqa: E501
         """
         pass
 
+    def test_packages_validate_upload_hex(self):
+        """Test case for packages_validate_upload_hex
+
+        Validate parameters for create Hex package  # noqa: E501
+        """
+        pass
+
     def test_packages_validate_upload_luarocks(self):
         """Test case for packages_validate_upload_luarocks
 
         Validate parameters for create LuaRocks package  # noqa: E501
         """
         pass
```

## test/test_vulnerabilities_api.py

```diff
@@ -42,15 +42,15 @@
         Lists scan results for a specific package.  # noqa: E501
         """
         pass
 
     def test_vulnerabilities_read(self):
         """Test case for vulnerabilities_read
 
-        Returns a Scan Result.  # noqa: E501
+        Get a scan result.  # noqa: E501
         """
         pass
 
     def test_vulnerabilities_repo_list(self):
         """Test case for vulnerabilities_repo_list
 
         Lists scan results for a specific repository.  # noqa: E501
```

## Comparing `cloudsmith_api-2.0.2.dist-info/RECORD` & `cloudsmith_api-2.0.3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-cloudsmith_api/__init__.py,sha256=NxNLPzjHYTWxaurn7a1Nfg_JJyveMWwEhOIExubwtGk,15755
-cloudsmith_api/api_client.py,sha256=db62D6KBLLKVV2yJOrvjoUgs3WiiLzAcaLDH7j9mkls,25067
-cloudsmith_api/configuration.py,sha256=rhBZacb4NPqOHLKnZN0uQeZmQriesFXzTSlRSHOiym4,8390
+cloudsmith_api/__init__.py,sha256=7OHUHU3rrnJgK02ZONaolRJvdd6QvNxqZF7MtpZm2Gw,15910
+cloudsmith_api/api_client.py,sha256=HASptj_Sexdb0XKrFAjSEWIqLXd7q9bv3vNsMDB0d3Q,25067
+cloudsmith_api/configuration.py,sha256=ZSn2tDaIx7vAhxU3JHaF_G8vs7JnQWQj3933WYcoNdc,8390
 cloudsmith_api/rest.py,sha256=IVGz52ALLAOqfC3YGAkqFfFjiLz5mAB_R0mIs51372Y,13166
 cloudsmith_api/api/__init__.py,sha256=oHMaETBtdkm77g6ZMGgBaWJb1Q3a8jlD8Nh02VKZd2U,1131
 cloudsmith_api/api/audit_log_api.py,sha256=cDN0Rsgck9w4qB19hpWzsTETl41Zsm-pk8Wrr14EDGs,11039
 cloudsmith_api/api/badges_api.py,sha256=PF8u5FZiEm1BFP8e52ZEDjzMo9skZVM9Qc7arsPk4vc,11425
 cloudsmith_api/api/distros_api.py,sha256=44C2sU3C43GkhRNPLK-jxlB8KrS8-KFe7Bj7KxAc-cU,7978
 cloudsmith_api/api/entitlements_api.py,sha256=Ao8Zk99xiIDEf-5GTz9YbgyaVig05QDGN0Pc2TpZmmo,54786
 cloudsmith_api/api/files_api.py,sha256=lsuhZ5M3ugbdQoqeci23QCYe15g2zVmJ3nF_nRsljZM,26620
 cloudsmith_api/api/formats_api.py,sha256=7Bv_EKqHBEnSHJIbtQ_oh-5laVu5EmofmZwBJo9h4og,7930
 cloudsmith_api/api/metrics_api.py,sha256=cTqkKtutQn2u-zNS7FHVTkxX-LSc3xRpjgbLDIqsWWc,19214
 cloudsmith_api/api/namespaces_api.py,sha256=2qCN92-asz_tZyASYgXE7gpAPBfL6W13khfmuOYV8CA,8514
 cloudsmith_api/api/orgs_api.py,sha256=mPEe7pszQCmE63DPPsc6HUXj3Z_5Awgh8gPRqTacNKQ,195413
-cloudsmith_api/api/packages_api.py,sha256=KbZCkscS-6aoPYiEIiexa_zTKRN0l_62iNsjOkLn3QQ,275618
+cloudsmith_api/api/packages_api.py,sha256=YV6Bq61JHgMEavSzrD9k86JN7YSUVTqL6djPQqtmzHY,284986
 cloudsmith_api/api/quota_api.py,sha256=cLljkIY1w8-urDPf5Zi31YdaoWsyVrzKKz1t3Qasm_w,16386
 cloudsmith_api/api/rates_api.py,sha256=iVavoIQtWfbFE6C_jPnTQP8uG8wk0YS-ejHztrajZdY,4157
 cloudsmith_api/api/repos_api.py,sha256=9IYStNbWWFqBnTEQfDnB14Dfp4-jrVfMG7Ea0FBnKUo,98642
 cloudsmith_api/api/status_api.py,sha256=Y7fJjz1UeBzgC2y7F8EcnBuJIFUh553zQDdk1oLGOIQ,4118
 cloudsmith_api/api/storage_regions_api.py,sha256=27lr9PVQ8G84depb-1M7z1dJ5srWscFsU776W7SRVpc,8075
 cloudsmith_api/api/user_api.py,sha256=B2_HoP2ZNBYI-2GfmmSEmucylTZV_VhU7GnnP4aYPpE,7631
 cloudsmith_api/api/users_api.py,sha256=fjOMJWnFJ8qx5i5WkiR4cdpsKR2RzdoUT_V0w-TIZVM,4706
-cloudsmith_api/api/vulnerabilities_api.py,sha256=jW4-4p0G9a31UiJZZ0Bm6Iz0gQxNLSjGSS3oNVbAQjw,22056
+cloudsmith_api/api/vulnerabilities_api.py,sha256=gF5GPsUNONLhHE7bf_MIvqlyNU967AZVm0wHNWmYIoY,22091
 cloudsmith_api/api/webhooks_api.py,sha256=RsnHyob8BKBLbqKHq3U7TizhcFJF-VCkgzJllmTZliw,26050
-cloudsmith_api/models/__init__.py,sha256=WxCGgbJ71FAPYLFkhb2Olerq1BEGcLrhhy-yAJUS8cc,14558
+cloudsmith_api/models/__init__.py,sha256=BozmJco6SwxgXq7a9r1qzkdNYDPQqOijgygLONWx2kU,14713
 cloudsmith_api/models/allocated_limit.py,sha256=1SlEiDZ2Ozouu8Gg6CrYf47I7pJjyxUOCFtJd7Q0yzA,7305
 cloudsmith_api/models/allocated_limit_raw.py,sha256=p6vlL-y9gGwoER9aLnDeexcM0Ci6W5as9765n74SfRE,5410
 cloudsmith_api/models/alpine_package_upload.py,sha256=IUVVXR1YrQt0d52V93rFkdkHGg5YkymjC4pjUKpcxrQ,58771
 cloudsmith_api/models/alpine_package_upload_request.py,sha256=jrzolgP1mvgRKgLiDfWe6J2VS9hywOudnbpg-8zM3lk,7437
 cloudsmith_api/models/architecture.py,sha256=bzGmeP8O7tYFZfdkboF5_E34LlX-NyN2HU4W9T1Bkds,4748
 cloudsmith_api/models/cargo_package_upload.py,sha256=y6a8rNJxe9H4GWMv72MJkqnCPP-7L3YfGALtFbn8RvI,58494
 cloudsmith_api/models/cargo_package_upload_request.py,sha256=RmfIq722CsU9jPUpsofwJRXdTzjwZ0OG8js66XFUPpQ,6177
@@ -52,53 +52,55 @@
 cloudsmith_api/models/distribution.py,sha256=5mh3fWHu2vQU55xO00F4cEoaq76Dtl9sFAqx_WU8y6U,6159
 cloudsmith_api/models/distribution_full.py,sha256=xtxjZk2KOtB__JUCFv--RslyfXI8Pj_g1VaxhTpMdxU,8542
 cloudsmith_api/models/distribution_version.py,sha256=9EFxXMgzUVHKjvELtjUQThMkfpKiwsGA6ctJ8nVKGAY,4497
 cloudsmith_api/models/docker_package_upload.py,sha256=0wb3UWMXsq4W9heBrBUG9FiKHENK3gUShys80ozqjaI,58771
 cloudsmith_api/models/docker_package_upload_request.py,sha256=ZS0lzh-aryr88n5-tVxU3dFrF4wSHe-xsq8Zn4cTbcg,6194
 cloudsmith_api/models/entitlement_usage_metrics.py,sha256=fC2EAybHNP8Fp5Au-VPsEqvA9UQaB-5I1-zLiq-URVc,3541
 cloudsmith_api/models/error_detail.py,sha256=nUsm2ghwLE3GFYyz48jSjqqCbakBefdXR1PTGKaAelw,3729
-cloudsmith_api/models/eula.py,sha256=98LLu29GqR4Fa4T_shHXgQ6_eJMNQ4lYYPWULeaeEqk,5590
+cloudsmith_api/models/eula.py,sha256=_dafCxq6v5Cz8HxaCyjTr0T-ka9oMqsc36vy_QLuAwk,5458
 cloudsmith_api/models/format.py,sha256=w9JIldZS2mRBRKo-4tYyPP9ve-4wdF-xTf9gEBvJMuI,11287
 cloudsmith_api/models/format_support.py,sha256=-TbnGczxma_ziAuD4ss-jwdHSPhE6cAI_za52K_Gbpg,7319
 cloudsmith_api/models/geo_ip_location.py,sha256=w5oOjWMH_GcOQtcUwVo0gWk_dDkPVGwmHJ2IC0RxURY,8615
 cloudsmith_api/models/go_package_upload.py,sha256=Slt7_6-PvfajmCK0wHQOKjbdwBA9qs4EgZf__MtSvFE,57663
 cloudsmith_api/models/go_package_upload_request.py,sha256=UgLfJ7yrqfuch7bEjriI8c151CWwStC21nsgOl3Hw4g,6126
 cloudsmith_api/models/helm_package_upload.py,sha256=1AwH6eg9iLHxOf-VK1lzNuWqof7zGa3D1YXjhx7YnrA,58217
 cloudsmith_api/models/helm_package_upload_request.py,sha256=QNb20d7lYd1U1y7gJ_Q5Htm5NMphVtry4U12Mcmfbas,6160
+cloudsmith_api/models/hex_package_upload.py,sha256=cPGtS3VlNKXbKRbuwuDOvM8FTzNOebDym4xM6u9oQ7Y,57940
+cloudsmith_api/models/hex_package_upload_request.py,sha256=q-4Uh4f2OJmPY4CDL-P6YhlMGpOogbakNnMcYUPBNhs,6143
 cloudsmith_api/models/history.py,sha256=17AfMvcTcXVi0L8gkqSdytdMeVbNRrLVSToP9SnWsxE,7028
 cloudsmith_api/models/history_fieldset.py,sha256=Cng-daGoLVr2Hc2tlZ7_lktiEllkIGUcKjcTKG0pU-Q,5168
 cloudsmith_api/models/history_fieldset_raw.py,sha256=EV7mi9q3pTap9fsh1cVuSpTUrHrQxcmUreT-EFoUcq0,5246
 cloudsmith_api/models/luarocks_package_upload.py,sha256=D8VMxUWsIKi-evMg-AJW0r89t3hVfhrlSfa6jDNYMjM,59325
 cloudsmith_api/models/luarocks_package_upload_request.py,sha256=FQc8EpOCyRHBRBOmLC9xAl0TlZihGUnLhCE-hUlnIjk,6228
 cloudsmith_api/models/maven_package_upload.py,sha256=I68w-cFKGv_d_7h2GU_lVbq28iQbyNJiuaPezLTG9JY,61667
 cloudsmith_api/models/maven_package_upload_request.py,sha256=tEVqdFfD9sdGz6R2radMCadKIh6ReRxFktJ2ZOEjBv8,14513
 cloudsmith_api/models/namespace.py,sha256=pPo1q6hL3GaOyfeMuz85jZtPvZ7NZ5pM7GKt4VQPFfw,5806
 cloudsmith_api/models/namespace_audit_log.py,sha256=WRKsSuHhPThpTFC9aQLbWMIjxXpimne5yzQkxK-VtkU,18223
-cloudsmith_api/models/nested_license_policy.py,sha256=FDeCtx5VoWOI73YslB3z6eQa_Bloc093a6WYc94YRBc,10461
-cloudsmith_api/models/nested_vulnerability_policy.py,sha256=QfFboFfy2trv7bZe9-6I1u4eE88lQHaCmfi-6g-RUKo,11097
-cloudsmith_api/models/nested_vulnerability_scan_results.py,sha256=skZp2mjRwEh9khje1YHLN7njmZZNEiiZlQhzL_3ByJA,9219
+cloudsmith_api/models/nested_license_policy.py,sha256=YbHzNrWlplzoXh67Oc_sWEsILyvD8Cui3S1n1dulX-E,11620
+cloudsmith_api/models/nested_vulnerability_policy.py,sha256=fzPV_bEEBmwvbzfQuVJHUe651yw8J3Q9tJlNRVCWJlY,12280
+cloudsmith_api/models/nested_vulnerability_scan_results.py,sha256=qvEo7UgdZvUIvphxs78C6M9ev30XpAGuDwIESAI7AWA,9527
 cloudsmith_api/models/npm_package_upload.py,sha256=IEPmH7bgimdDPVNzVZDpKI03DNtqQYnJW5qFXI1SUHw,57940
 cloudsmith_api/models/npm_package_upload_request.py,sha256=xpqvQTM7dP6S81Ztl89g0PoQoVCTg8QJr1hlZ5wZmR4,7663
 cloudsmith_api/models/nuget_package_upload.py,sha256=eExC3CDlMs3F_LvmunNevVqw3H6pTrpz-Bfoc17uW5c,58494
 cloudsmith_api/models/nuget_package_upload_request.py,sha256=_V5hSUOnLmqhcbTKRgYQIaAINNMxtcx2oYRSOXQP4No,7272
 cloudsmith_api/models/organization.py,sha256=BzOVB7ziaUvwmW8387INoJtf90stbPfxkBZ-XYqhKvQ,7918
 cloudsmith_api/models/organization_group_sync.py,sha256=Z-_Ia7wrql-e4T2lJBQVP1KZs0-9XbXQyEMXOqJV8ZM,8391
 cloudsmith_api/models/organization_group_sync_request.py,sha256=KBOHy5g1JAfcqBqvZRPupOF9huDSiJ2e_p3ZS9M0nfc,8223
 cloudsmith_api/models/organization_invite.py,sha256=Az2o6U-T9A-J39v5rDu-IIVHXkMxypHl79A0llK3_CM,10169
 cloudsmith_api/models/organization_invite_extend.py,sha256=cnrSWvGjyFgoOCYxQls0Zv0ExztcXez-XCT8aJ6mhWY,10519
 cloudsmith_api/models/organization_invite_request.py,sha256=xJLQdrXDXsAeTOKsgenEY5HGpqi18xsAAjRXbv2KA8w,5661
 cloudsmith_api/models/organization_invite_update.py,sha256=xnY-FGOU6_nI4ZRJQoYINB9OlTx8pSc07SxnwzaEVHQ,3821
 cloudsmith_api/models/organization_invite_update_request_patch.py,sha256=LzGXkpzloxzgfKYHWoO8nMYzX6yLs785T3LASWmMG1M,3929
 cloudsmith_api/models/organization_membership.py,sha256=5Y9s4HF4xVgK1CINFIpfUd7mLS9ZpmfdD8eAKpM5bXU,12300
-cloudsmith_api/models/organization_package_license_policy.py,sha256=5jempFC6tp8UaT4xJ-v35YIFAK_uBRvjz5TWiV6x3PE,11008
-cloudsmith_api/models/organization_package_license_policy_request.py,sha256=R3oBRZjcac_ebmLaKqo9iZzc9iF6SB1fpNWaIhmW6TI,8427
-cloudsmith_api/models/organization_package_license_policy_request_patch.py,sha256=Ca5Ozz45VIxKamxUJmayH3NBcD6EzRrLxmpnUAJWKhw,8280
-cloudsmith_api/models/organization_package_vulnerability_policy.py,sha256=9P8wK_nBFdib9GvgHyquELcR4k4N0Z-YGeYUbnx3c90,11620
-cloudsmith_api/models/organization_package_vulnerability_policy_request.py,sha256=2TFyV4TBreOH7DSGH62t57GCjVO_iRCrow0ayPzaf_0,8967
-cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py,sha256=DirhztKtbU7ZfyDFhmAZ8G01h-3bA3suinUW_3ElOsw,8962
+cloudsmith_api/models/organization_package_license_policy.py,sha256=-HQNPHYw4iP82GpzvQugoiJjZmu29SnUb2Z6IiGCZTQ,12219
+cloudsmith_api/models/organization_package_license_policy_request.py,sha256=xf4Mj27AamztWi1XtZIFqh3PQBzKSanK9O3-2C3FMUM,9666
+cloudsmith_api/models/organization_package_license_policy_request_patch.py,sha256=vg6vU8KV8wqKWpeeMzih0-7oO28KrP9PAcAlIyLqN1M,9539
+cloudsmith_api/models/organization_package_vulnerability_policy.py,sha256=yruKPpCyA2qqeWpkPhfs5IXI3XzFsO4r-HiHoYhajVc,12855
+cloudsmith_api/models/organization_package_vulnerability_policy_request.py,sha256=1e9rbhiTVI4DJDn6Ipu6AOF9OqKMAhjzc0dgEapHS1g,10230
+cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py,sha256=XUo9Dg-MrwgxY0oxn3VxQ8P0gILy5jWqIqAFEgafkCc,10245
 cloudsmith_api/models/organization_team.py,sha256=SJl-c2DybDkjhh99Z6I5HhAmUqoRsTISKn74VqG2pKs,8110
 cloudsmith_api/models/organization_team_members.py,sha256=erGYU0Ld15obQdUSnPRUEuqHuZiKdbM_sJIZ8cxfZu0,3669
 cloudsmith_api/models/organization_team_membership.py,sha256=yKw8jnDGeZnGe5gHOn4qOELSE54Vy4rE8CvHLKUIjTI,4783
 cloudsmith_api/models/organization_team_request.py,sha256=acFbvl-oZo00j8PszeTWbJef-gmHQi4t6t2uR3d0D1w,7065
 cloudsmith_api/models/organization_team_request_patch.py,sha256=Bh6jE5bFOQ9DH_ZFCXlvFxp_g7mMlxNFLOl_W2Z6OGs,7040
 cloudsmith_api/models/p2_package_upload.py,sha256=3YHZTGVGfMkvsY679eDd2WrekadM_KaVI2YyYe7BPmg,57663
 cloudsmith_api/models/p2_package_upload_request.py,sha256=VOEHo4ToZzZAt5m_XCSv7RcJLB7moanktYqidGoXPdw,6126
@@ -150,37 +152,37 @@
 cloudsmith_api/models/repository_privilege_dict.py,sha256=ZzruAgyQiiIBB5qBFag4El1tWR4-QHqDe66-r57LiA0,7702
 cloudsmith_api/models/repository_privilege_input.py,sha256=H1uipl0JCqgrB-Ea-F2WOV0U-YOZenD_wgViKq-c5yc,3818
 cloudsmith_api/models/repository_privilege_input_request.py,sha256=SbVMKEhvmAAapeV3o1yK-hE9L8yiErCuda8dgMnQ83w,3881
 cloudsmith_api/models/repository_privilege_input_request_patch.py,sha256=gRV-R-eAcfYqAKbE6bAR1hlIsfe99hJwQMps5gN2e-A,3790
 cloudsmith_api/models/repository_request_patch.py,sha256=EQwQuihT-MvPt83hsuoT-25Q4Gs6kg8cPa26uahzYz0,51807
 cloudsmith_api/models/repository_rsa_key.py,sha256=m5HzgFF21eCDsik255LryTsadctALhkq3LqD2SaskZc,7753
 cloudsmith_api/models/repository_rsa_key_create.py,sha256=4QsWN17vYUeiCVIDr548BPRJPEOCR3a8UTP2vlMVoKo,5133
-cloudsmith_api/models/repository_token.py,sha256=DIiQ5ZIwzMHLwKo-fPQ7ZkovCZov5RPjgo6anj2-evU,40222
+cloudsmith_api/models/repository_token.py,sha256=frV2-K-4kK6TPSo-oS4X2AY0M5dLSi2RDM1-MzqmTAg,40544
 cloudsmith_api/models/repository_token_action.py,sha256=M6nBZsDLWOtqs2nGoiOsTtEpcDVLb_24REhGQDeZoPk,2750
-cloudsmith_api/models/repository_token_refresh.py,sha256=l_XUV2lnvb9JOwh4xeN9tTD25TIfpkWXPFx0IIw2cXw,41219
+cloudsmith_api/models/repository_token_refresh.py,sha256=SYYqA-IlDvePLUyBnS042xW873Fw_JjyKRWgiZnMJ_I,41541
 cloudsmith_api/models/repository_token_refresh_request.py,sha256=hX1_e-Q1jtVb-QTr_AkgESElIX_tNcHnf68qL5w2tFE,21868
 cloudsmith_api/models/repository_token_request.py,sha256=WIV-TiYm7Qq625QDyc1Kvs0d5Rh-_I6PhdVhIUllQwE,22374
 cloudsmith_api/models/repository_token_request_patch.py,sha256=8A3H75DvnqyU1-fVmE54O1hyAOtijUjNz7SYv0MeGA8,22569
 cloudsmith_api/models/repository_token_sync.py,sha256=heyuf6pEUaCNhTyZHhBb5ktOXKZ_nTuJ9zMY9BzW3ME,3505
 cloudsmith_api/models/repository_token_sync_request.py,sha256=AhwroLUUylZJlQvCxYFaOdLI0vt9m3GIep9781xu9Sg,3904
-cloudsmith_api/models/repository_webhook.py,sha256=bGH-t5dC3wTnAqV60GTX3gGfaQhTEFqMb4H--RtyXpk,30400
+cloudsmith_api/models/repository_webhook.py,sha256=D4GRg4sUnfqxFUI-CXP3SnDX9uLxTtKJpm0Mp457nHc,30728
 cloudsmith_api/models/repository_webhook_request.py,sha256=FbkfdGvrZn7yS2PVFpgxgWDnqpfbknuJZfXluVxu9jk,18912
 cloudsmith_api/models/repository_webhook_request_patch.py,sha256=TbujXUmPBjgatch193r4wqhdoofPhWVrkfZh01GvPj8,18774
 cloudsmith_api/models/resources_rate_check.py,sha256=7LlUfH6WkOYY9J1O26LYHbK0jXnXCPyL206-G19VtWs,3523
 cloudsmith_api/models/respository_geo_ip_enable_disable.py,sha256=oSzM7HSHfh7875ZOr9wbap9ciy2zFeooAVd4ceT1-7w,2790
 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py,sha256=h5cWc3qwFHoh5ckaXmbIdDVAyxBu1xWTtC6hr3LxxZ4,2825
 cloudsmith_api/models/rpm_package_upload.py,sha256=EzTFVTqVaif9B17_0HZMz9sB1n-oQcxT0ng23Mbsl4U,57940
 cloudsmith_api/models/rpm_package_upload_request.py,sha256=dI7_B02n2f4DhzcTl_dClukOTFHbuL2ITWwnTEyZrOM,7374
 cloudsmith_api/models/ruby_package_upload.py,sha256=cLi1WS4JxzNIRkDjUAMtIM_Fx12s_-Th51ysO_t08Bk,58217
 cloudsmith_api/models/ruby_package_upload_request.py,sha256=pA2MIcN9TvnQBQdh-W3VsQRgkB2VkQg4lWuFalrmHmw,6160
 cloudsmith_api/models/service.py,sha256=lhEXDlJBEf2h_uhqlb0gLo9fPePbEi9Ayo4aC6Zyo6w,8234
 cloudsmith_api/models/service_request.py,sha256=JOv9I8cUiQqTFOBomiwC3KVnewi8x2Rc6NUpp4wg42g,6726
 cloudsmith_api/models/service_request_patch.py,sha256=G3Kyh4R5MA_qsdxaqygbWco5zFqdRmklQGaW0MfAKGQ,6701
 cloudsmith_api/models/service_teams.py,sha256=JVUDlli2nc2oVtCGZQo29lHNQRuRuEsGKei-ShRyYlA,4951
-cloudsmith_api/models/status_basic.py,sha256=cjAe5Y4FhS9avgP5LGAQwTHTjv41S29jVpkuO4aeC-c,4584
+cloudsmith_api/models/status_basic.py,sha256=uZwbfEza4MD1w7Jci-mvQ39HvpfGN95KogngviBJrXI,4584
 cloudsmith_api/models/storage_allocated_limit.py,sha256=NkE1HLffx1kwuA0GamS5COBvOE3I0CyNa44Ox2vkTcQ,8478
 cloudsmith_api/models/storage_allocated_limit_raw.py,sha256=EZ2PZeIOBGfue8u0HVjurLNClceuFc5wH2UKoBqdtyQ,6140
 cloudsmith_api/models/storage_region.py,sha256=dx_5FJDAJmHrcNI4cBWiZJ6Jr06fFCA5TWYxGob9BTc,4670
 cloudsmith_api/models/storage_usage.py,sha256=EfRE_skvZ85zdc57ZKXwpacL85QGDSrMiYKf2sBQxMQ,6847
 cloudsmith_api/models/storage_usage_raw.py,sha256=fFnveEKU771hbXtZXfCV262Tm3B3RNJH6-4JPC4QFqA,5048
 cloudsmith_api/models/tags.py,sha256=p-1Zwln_mYSv2tQ3naimZtoRiFgntVOAOd9phO2zuDw,2665
 cloudsmith_api/models/terraform_package_upload.py,sha256=hXd--8XCuyh1gj9XMwmAytVoKt9zIE3qsKTYhG5H-Ws,59602
@@ -194,16 +196,16 @@
 cloudsmith_api/models/user_auth_token_request.py,sha256=_mi1GgiNsLkMMFONOpRemg1SD8DPbJxQvmNIEWDg214,4612
 cloudsmith_api/models/user_brief.py,sha256=FjY-e7q8d3O3pE43TuR0Oi3SzihNVkmLvjMCluJH-RE,8019
 cloudsmith_api/models/user_profile.py,sha256=R7MrOiT5xeTjkw9W2oo0S0Jr15FoyoWts6ACWJHUNrE,11110
 cloudsmith_api/models/vagrant_package_upload.py,sha256=YHZRrw8Fx5owKP2IxNKjyTgGW7G3iziRUrTkQ0xsExc,60899
 cloudsmith_api/models/vagrant_package_upload_request.py,sha256=QCeUkKr6NXB6wAEbFS5prYiv_2BCHyOpHOd0QNM3gTQ,9492
 cloudsmith_api/models/vulnerability.py,sha256=EhiEvjqjau_YWOJQvHUx8ez_iNK0L62OsooXqlYOe6s,13112
 cloudsmith_api/models/vulnerability_scan.py,sha256=l_c1Fi1f5yWuFpkZJ8b9fnoUT24mR-GymVyOXhyStr4,5400
-cloudsmith_api/models/vulnerability_scan_results.py,sha256=kIfT6aN_ptfQP7yCPym3o8Ep9PdvYYgELikIQojP1Es,10040
-cloudsmith_api/models/vulnerability_scan_results_list.py,sha256=TQ3ed-Bwh6Y9GSbs8wXqWZwN9m9YSAiYlB0IvRk6o7E,9417
+cloudsmith_api/models/vulnerability_scan_results.py,sha256=ahAY0NoI56ZhZE7a6a5zC81VuwfKXGObU0KVGNo0b74,10348
+cloudsmith_api/models/vulnerability_scan_results_list.py,sha256=pw3m5ew-YNHR26IhiF8xaoaKZskjaySO53zNH_FbvkY,9725
 cloudsmith_api/models/vulnerability_scan_version.py,sha256=iEIDkLWfEL7Xh6wKKm7-DGY2vzbrrJNiMDzSHOKpKwM,8443
 cloudsmith_api/models/webhook_template.py,sha256=7gckCqIgyXL1qtzgJ_ShilhjC4OAj0E5dmfS6bt0MEM,4751
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_allocated_limit.py,sha256=Z9YkpJvxvcybMcK7lhy2w5WWUnB3sqf4g2YiZOZe11g,900
 test/test_allocated_limit_raw.py,sha256=do3JYGvEItmUtaw3jvSXDqtZZPFq4d8aA-FuB6e6jvE,926
 test/test_alpine_package_upload.py,sha256=WsaGcAtKxDgIqI52TuiTekpdFxTKZPUHXg-AgFcoi7A,942
 test/test_alpine_package_upload_request.py,sha256=uHCsktTOkhnw99LhXnMYfqSIapL_CZk5Bue7JBtPUW0,1000
@@ -246,14 +248,16 @@
 test/test_format_support.py,sha256=9Pg-T22EECmGmsSxSoLueanDlajn8gk4ZTTkNU58daM,892
 test/test_formats_api.py,sha256=yIEx4POX4lFZ1bUrXWwKzIUuicJhogOLFbzXwPXrbCM,1022
 test/test_geo_ip_location.py,sha256=emR0Gn9O08c3hIq3Z0AHl1I3lrGFDQtD5xEjbEuI5GM,894
 test/test_go_package_upload.py,sha256=-JNWeb4MtT6zYxdaJ4hSnx3_YnSeF1zLUx-Z1rUCSC4,910
 test/test_go_package_upload_request.py,sha256=NkySpOxmeCFPIQaf6mSFxuE6u1-jSAuGc2do4S46I08,968
 test/test_helm_package_upload.py,sha256=10o8yyxk6c5dgU7c-XUAqtFhyB1xjZaAYxmFgXF6g2U,926
 test/test_helm_package_upload_request.py,sha256=nnG38-2Bl3noBV6PGpbmtF5FagtEUasLwd01B8oO9DM,984
+test/test_hex_package_upload.py,sha256=CSrRr2OYKpSoHiJ07iIr_ihsBjljZzY6QoG4nyexyY8,918
+test/test_hex_package_upload_request.py,sha256=5nHxbziLWQR3Iwy34yoboVTjqJsPrrbXWJ-7FmTGMDQ,976
 test/test_history.py,sha256=KcfXovwetcML_pfkqu-mXgjfORWPwk1RaK8YwkdQWsA,842
 test/test_history_fieldset.py,sha256=Bm7FOpV8w9-Whk32HtjzdUtzYZv4DJARQ6DhczdDmn4,908
 test/test_history_fieldset_raw.py,sha256=47wxdjeecweq3QtbNu6SBptW_MLpYI7q1KM2YLjwMks,934
 test/test_luarocks_package_upload.py,sha256=GYj_FvW7CbegzPRB19VjteBuCeLK5S-TVhN5cSnTkFg,958
 test/test_luarocks_package_upload_request.py,sha256=6xLeA8NDCWrRdfLFtOS3ohBNh0xzJ58CUoJvSB-XusU,1016
 test/test_maven_package_upload.py,sha256=5jSiC-GuZ3BSqByMsDRoi9iGbuOdOlkpycLiY_WFITQ,934
 test/test_maven_package_upload_request.py,sha256=2SF-gjJYFmlNinfiCRDCj0AASmwzr2AsbxluOJTpMkA,992
@@ -311,15 +315,15 @@
 test/test_package_tag.py,sha256=BkcYyKWhYR0zx_a940tYo5Pm4bguJW6fnpnIboBQBi4,868
 test/test_package_tag_request.py,sha256=HXsOuuK6Tfv6fqZw8r5-PihQTJekhC5_L8kfmyh2F0w,926
 test/test_package_usage_metrics.py,sha256=SA2_RAqLdmvnXrhKq4rFEMb6jJ0uj1sIZO-WjwU9NrE,942
 test/test_package_version_badge.py,sha256=FceEfshIzpn-tZWImTMJWnhpiHObWejQv2syqoOFJ4s,942
 test/test_package_vulnerability.py,sha256=mTIkCXM1qjoanj2t0zdhGxV6TUzo9mhNmUqI1hzMlTs,948
 test/test_package_vulnerability_policy_violation_log.py,sha256=iIrZ6ABnEq_AmAr3jUd9vR_FQh66W1xB7ztdstyFMY4,1098
 test/test_package_vulnerability_policy_violation_log_cursor_page.py,sha256=W5uSYYF6ZzUruutsT4Jj78KOEnNqzN-HZaIzB2IEn2Y,1182
-test/test_packages_api.py,sha256=2PIK8EGrIouF2dUQoIodbgOmw0mrRx69qCQLSvJIX_E,11023
+test/test_packages_api.py,sha256=rFq5IloMIrPnB7yynnQgB5pIyXQGQDn7AZPDIiXY42k,11377
 test/test_python_package_upload.py,sha256=9TqfbGmuNwLq5E3K2DW3jSTsj3NIUlgmQwPLQWcH3YY,942
 test/test_python_package_upload_request.py,sha256=I2Si5Gxo2QZcYiqnG9rJoKD3_uwa58Kj5XUDVS-IUpw,1000
 test/test_quota.py,sha256=MBDyrqP8f-c-sfrwseJSKhJr8n-CHk_RdVWKnzXQVeY,826
 test/test_quota_api.py,sha256=9s116ymseG0AEs5GjlYvA6sZQt3TA8314jiigYyHQ8I,1364
 test/test_quota_history.py,sha256=He4i2YAkLW9vikiNV6RkUOQvs5gUqjRUxgHihqriPAw,884
 test/test_rate_check.py,sha256=3chA15laHCwLu0QXKOyTCdiJKJbOzAQOeUTftcsaGCg,860
 test/test_rates_api.py,sha256=eEs-UjEVTAr5b40hueduthNROAGZfwy6pEx2VQaRaHM,862
@@ -389,19 +393,19 @@
 test/test_user_auth_token.py,sha256=D19JwH469XeJEaLc9DicTHHIeM0BQySBP8crk4IpSMA,894
 test/test_user_auth_token_request.py,sha256=IsMDmx2fIeyniPMtzj5ZRwGalAbJmHB9mqQnWQfVz0Q,952
 test/test_user_brief.py,sha256=i4HR1YTMkN_un1wqpCxJVffgDkK_An3kChIUexVNklg,860
 test/test_user_profile.py,sha256=xhUpzGSJMXEfH36iBJYMfNnK6Q0eg4-Xc_7gPSIZMkI,876
 test/test_users_api.py,sha256=LQ-S4lEkFqRvv97Dz9y8AZfbSGVIr8PMV4g8Omw1vwI,865
 test/test_vagrant_package_upload.py,sha256=epUVY08Iq5IbuL7Ww5WqGUYrncdM6SIK79xA78B5BgQ,950
 test/test_vagrant_package_upload_request.py,sha256=d2_neFB4EeiQC5vV075bUeFz9x1kL71fDSnhBTP_7Es,1008
-test/test_vulnerabilities_api.py,sha256=YSnCGbbjTdfKx_p0-r06LItn8i9Lv3Uj33c0FwLbr24,1491
+test/test_vulnerabilities_api.py,sha256=WNudYFcWhd5gqMybuJ4QG6Pqi87ntDsFyzwtsspP9kA,1487
 test/test_vulnerability.py,sha256=4QDPIFWXKuHg_oy9PTRqFhO8yvsur5VyUFhDVkQ-Dnc,890
 test/test_vulnerability_scan.py,sha256=mGc0AETJ-UP30jb32rN5LvHeP8KFteXB8afWUED2mfI,924
 test/test_vulnerability_scan_results.py,sha256=8-nfCw6UiVWIOsTyge5XETxWxfCkB4hQf4km2lQ3pVI,982
 test/test_vulnerability_scan_results_list.py,sha256=dtcBvhUgGr6LluGnjA6x7dqQ7bkeSbCuPJpKSdHm1kQ,1016
 test/test_vulnerability_scan_version.py,sha256=hgxu72nwZ8rfEgverNQQ9_DF1A-cxa0kIBXPkEEknuk,982
 test/test_webhook_template.py,sha256=kCtiNGZ65WVUpB0an-VxzQ6-F1k-w7kTmHqdgQLSKDU,908
 test/test_webhooks_api.py,sha256=ujU1QfkYPe4MwlMR0M-p2rEfSVTzPO1Q3uB8VLiDbOg,1557
-cloudsmith_api-2.0.2.dist-info/METADATA,sha256=la8ps_jKiBQ1_cDuF0kpYVCiZF7Ndt9b7xNZ68xVFhk,457
-cloudsmith_api-2.0.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-cloudsmith_api-2.0.2.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
-cloudsmith_api-2.0.2.dist-info/RECORD,,
+cloudsmith_api-2.0.3.dist-info/METADATA,sha256=tl3RDn7PkU9J2DysX0BXwFSQ7RT5WOif9sfrjcqNb5o,457
+cloudsmith_api-2.0.3.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+cloudsmith_api-2.0.3.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
+cloudsmith_api-2.0.3.dist-info/RECORD,,
```

