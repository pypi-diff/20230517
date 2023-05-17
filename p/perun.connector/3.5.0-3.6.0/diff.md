# Comparing `tmp/perun.connector-3.5.0.tar.gz` & `tmp/perun.connector-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.connector-3.5.0.tar", last modified: Wed Apr  5 21:31:55 2023, max compression
+gzip compressed data, was "perun.connector-3.6.0.tar", last modified: Wed May 17 09:18:03 2023, max compression
```

## Comparing `perun.connector-3.5.0.tar` & `perun.connector-3.6.0.tar`

### file list

```diff
@@ -1,351 +1,351 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:55.564860 perun.connector-3.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-04-04 22:24:27.000000 perun.connector-3.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      275 2023-04-05 21:31:55.564860 perun.connector-3.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-04 22:24:27.000000 perun.connector-3.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.640815 perun.connector-3.5.0/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.660816 perun.connector-3.5.0/perun/connector/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.660816 perun.connector-3.5.0/perun/connector/adapters/
--rw-rw-rw-   0 root         (0) root         (0)    17238 2023-04-05 12:39:00.000000 perun.connector-3.5.0/perun/connector/adapters/AdapterInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    14966 2023-04-05 12:39:00.000000 perun.connector-3.5.0/perun/connector/adapters/AdaptersManager.py
--rw-rw-rw-   0 root         (0) root         (0)    28065 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/adapters/LdapAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    42235 2023-04-05 13:05:29.000000 perun.connector-3.5.0/perun/connector/adapters/PerunRpcAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/adapters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.660816 perun.connector-3.5.0/perun/connector/config_templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/config_templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.660816 perun.connector-3.5.0/perun/connector/connectors/
--rw-rw-rw-   0 root         (0) root         (0)     4189 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/connectors/LdapConnector.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.664816 perun.connector-3.5.0/perun/connector/models/
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/Facility.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/Group.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/HasIdAbstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/Member.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/MemberStatusEnum.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/Resource.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/User.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/UserExtSource.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/VO.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.740817 perun.connector-3.5.0/perun/connector/perun_openapi/
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.996823 perun.connector-3.5.0/perun/connector/perun_openapi/api/
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   843770 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/attributes_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    56442 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/audit_messages_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   175597 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/authz_resolver_api.py
--rw-rw-rw-   0 root         (0) root         (0)   130963 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/cabinet_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    81270 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/consents_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/database_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    81685 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/ext_sources_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   544064 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/facilities_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   255356 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/groups_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5328 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/integration_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   271253 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/members_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    28296 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/owners_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   271089 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/registrar_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   452385 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/resources_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    22249 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/rt_messages_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    25572 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/searcher_api.py
--rw-rw-rw-   0 root         (0) root         (0)   367216 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/services_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   107772 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/tasks_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)   306683 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/users_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    31350 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/utils_api.py
--rw-rw-rw-   0 root         (0) root         (0)   198688 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api/vos_manager_api.py
--rw-rw-rw-   0 root         (0) root         (0)    38897 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:54.000824 perun.connector-3.5.0/perun/connector/perun_openapi/apis/
--rw-rw-rw-   0 root         (0) root         (0)     2287 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18147 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:55.560860 perun.connector-3.5.0/perun/connector/perun_openapi/model/
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12548 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12265 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/add_user_ext_source_input.py
--rw-rw-rw-   0 root         (0) root         (0)    12230 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/app_state.py
--rw-rw-rw-   0 root         (0) root         (0)    12173 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/app_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14842 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/application.py
--rw-rw-rw-   0 root         (0) root         (0)    13343 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/application_form.py
--rw-rw-rw-   0 root         (0) root         (0)    16033 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/application_form_item.py
--rw-rw-rw-   0 root         (0) root         (0)    13021 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/application_form_item_data.py
--rw-rw-rw-   0 root         (0) root         (0)    13346 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/application_mail.py
--rw-rw-rw-   0 root         (0) root         (0)    12539 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/applications_order_column.py
--rw-rw-rw-   0 root         (0) root         (0)    14787 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/applications_page_query.py
--rw-rw-rw-   0 root         (0) root         (0)    13061 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/assigned_group.py
--rw-rw-rw-   0 root         (0) root         (0)    12311 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/assigned_member.py
--rw-rw-rw-   0 root         (0) root         (0)    13798 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/assigned_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    15808 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12347 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_action.py
--rw-rw-rw-   0 root         (0) root         (0)    16505 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    12688 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_policy.py
--rw-rw-rw-   0 root         (0) root         (0)    12888 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_policy_collection.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_rights.py
--rw-rw-rw-   0 root         (0) root         (0)    12563 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_rules.py
--rw-rw-rw-   0 root         (0) root         (0)    15539 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/audit_event.py
--rw-rw-rw-   0 root         (0) root         (0)    12654 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/audit_message.py
--rw-rw-rw-   0 root         (0) root         (0)    12762 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/audit_messages_page_query.py
--rw-rw-rw-   0 root         (0) root         (0)    20415 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/auditable.py
--rw-rw-rw-   0 root         (0) root         (0)    15698 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/author.py
--rw-rw-rw-   0 root         (0) root         (0)    15034 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/authorship.py
--rw-rw-rw-   0 root         (0) root         (0)    11301 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/authz_roles.py
--rw-rw-rw-   0 root         (0) root         (0)    14879 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/ban.py
--rw-rw-rw-   0 root         (0) root         (0)    14344 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/ban_on_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    14354 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/ban_on_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    14306 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/ban_on_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    12646 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/brand.py
--rw-rw-rw-   0 root         (0) root         (0)    14887 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/candidate.py
--rw-rw-rw-   0 root         (0) root         (0)    14318 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/category.py
--rw-rw-rw-   0 root         (0) root         (0)    15270 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/consent.py
--rw-rw-rw-   0 root         (0) root         (0)    14644 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/consent_hub.py
--rw-rw-rw-   0 root         (0) root         (0)    12267 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/consent_status.py
--rw-rw-rw-   0 root         (0) root         (0)    15246 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/destination.py
--rw-rw-rw-   0 root         (0) root         (0)    12432 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/destination_propagation_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13073 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/destination_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12530 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ban_on_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    12554 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ban_on_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ban_on_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    12140 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)    12827 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    12180 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_group.py
--rw-rw-rw-   0 root         (0) root         (0)    12189 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_host.py
--rw-rw-rw-   0 root         (0) root         (0)    12727 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_identity.py
--rw-rw-rw-   0 root         (0) root         (0)    12225 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12212 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/entityless_attributes_by_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    14314 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)    11974 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/ext_source_object.py
--rw-rw-rw-   0 root         (0) root         (0)    14622 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/facility.py
--rw-rw-rw-   0 root         (0) root         (0)    12302 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/facility_propagation_state.py
--rw-rw-rw-   0 root         (0) root         (0)    12595 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/facility_state.py
--rw-rw-rw-   0 root         (0) root         (0)    12357 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/facility_with_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12418 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/gen_data_node.py
--rw-rw-rw-   0 root         (0) root         (0)    11668 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/gen_member_data_node.py
--rw-rw-rw-   0 root         (0) root         (0)    12082 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/graph_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12233 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/graph_file_format.py
--rw-rw-rw-   0 root         (0) root         (0)    15471 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/group.py
--rw-rw-rw-   0 root         (0) root         (0)    12452 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/group_member_data.py
--rw-rw-rw-   0 root         (0) root         (0)    13052 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/group_member_relation.py
--rw-rw-rw-   0 root         (0) root         (0)    12445 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/group_resource_status.py
--rw-rw-rw-   0 root         (0) root         (0)    12161 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/groups_order_column.py
--rw-rw-rw-   0 root         (0) root         (0)    13319 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/groups_page_query.py
--rw-rw-rw-   0 root         (0) root         (0)    12274 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/hashed_gen_data.py
--rw-rw-rw-   0 root         (0) root         (0)    14141 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/host.py
--rw-rw-rw-   0 root         (0) root         (0)    12629 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/identity.py
--rw-rw-rw-   0 root         (0) root         (0)    12200 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_application_mail_for_group.py
--rw-rw-rw-   0 root         (0) root         (0)    12158 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_application_mail_for_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    13405 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_destination_to_multiple_services.py
--rw-rw-rw-   0 root         (0) root         (0)    12265 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_destinations_defined_by_hosts_on_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    12401 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_member_candidates.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_assign_resource_tag_to_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12339 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_assign_resource_tags_to_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12198 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_attribute_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    12246 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_attribute_policy_collections.py
--rw-rw-rw-   0 root         (0) root         (0)    11994 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_attribute_rights.py
--rw-rw-rw-   0 root         (0) root         (0)    12150 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_block_services_on_destinations.py
--rw-rw-rw-   0 root         (0) root         (0)    12357 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_change_non_authz_password_by_token.py
--rw-rw-rw-   0 root         (0) root         (0)    12920 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_change_password_for_login.py
--rw-rw-rw-   0 root         (0) root         (0)    12906 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_change_password_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)    12218 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_check_password_strength.py
--rw-rw-rw-   0 root         (0) root         (0)    11843 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_consolidate.py
--rw-rw-rw-   0 root         (0) root         (0)    12790 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_copy_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12597 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_alternative_password.py
--rw-rw-rw-   0 root         (0) root         (0)    12096 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_attribute_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    11999 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_authorship.py
--rw-rw-rw-   0 root         (0) root         (0)    11957 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_category.py
--rw-rw-rw-   0 root         (0) root         (0)    12019 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_category_nr.py
--rw-rw-rw-   0 root         (0) root         (0)    12468 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_member_for_candidate.py
--rw-rw-rw-   0 root         (0) root         (0)    12269 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_member_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)    13318 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_member_from_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)    12463 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_owner.py
--rw-rw-rw-   0 root         (0) root         (0)    12020 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_publication.py
--rw-rw-rw-   0 root         (0) root         (0)    12026 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_publication_system.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_resource_tag_with_resource_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11936 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)    12462 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_service_user.py
--rw-rw-rw-   0 root         (0) root         (0)    12115 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_services_package.py
--rw-rw-rw-   0 root         (0) root         (0)    13130 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_sponsored_member.py
--rw-rw-rw-   0 root         (0) root         (0)    13829 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_sponsored_member_from_csv.py
--rw-rw-rw-   0 root         (0) root         (0)    13555 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_sponsored_members.py
--rw-rw-rw-   0 root         (0) root         (0)    11861 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_thanks.py
--rw-rw-rw-   0 root         (0) root         (0)    11849 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_vo_with_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    12077 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_delete_groups.py
--rw-rw-rw-   0 root         (0) root         (0)    12031 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_delete_resource_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    12227 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_entityless_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12273 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_form_item_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12282 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_form_items_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12288 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_all_resources_by_resource_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    12197 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_facilities.py
--rw-rw-rw-   0 root         (0) root         (0)    12830 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_match_resources.py
--rw-rw-rw-   0 root         (0) root         (0)    12532 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_members_by_user_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12045 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_messages_page.py
--rw-rw-rw-   0 root         (0) root         (0)    12232 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_applications.py
--rw-rw-rw-   0 root         (0) root         (0)    12416 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_groups.py
--rw-rw-rw-   0 root         (0) root         (0)    12426 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_members.py
--rw-rw-rw-   0 root         (0) root         (0)    12472 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_subgroups.py
--rw-rw-rw-   0 root         (0) root         (0)    12238 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_users.py
--rw-rw-rw-   0 root         (0) root         (0)    12194 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_resources.py
--rw-rw-rw-   0 root         (0) root         (0)    12182 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)    12676 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_invitations_from_csv.py
--rw-rw-rw-   0 root         (0) root         (0)    12600 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_invite_member_candidates.py
--rw-rw-rw-   0 root         (0) root         (0)    12227 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_lock_publications.py
--rw-rw-rw-   0 root         (0) root         (0)    12325 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_remove_resource_tag_from_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12345 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_remove_resource_tags_from_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12135 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_remove_rich_destinations.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_reserve_password_for_login.py
--rw-rw-rw-   0 root         (0) root         (0)    12242 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_reserve_password_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)    12516 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_send_message.py
--rw-rw-rw-   0 root         (0) root         (0)    12045 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_ban.py
--rw-rw-rw-   0 root         (0) root         (0)    12096 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_ban_for_user_on_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    12251 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12159 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13283 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_resource_group_user_member_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12843 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_resource_user_member_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12367 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_user_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12203 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12223 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12499 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_resource_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12519 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_resource_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12187 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_host_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_host_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12239 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12467 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_group_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12487 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_group_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12946 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_group_with_user_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12991 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_resource_and_user_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12515 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_resource_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12535 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_resource_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12712 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_with_user_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12251 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12271 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12519 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_group_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12992 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_group_with_group_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12215 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_sending_enabled.py
--rw-rw-rw-   0 root         (0) root         (0)    12990 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_sponsored_member.py
--rw-rw-rw-   0 root         (0) root         (0)    12187 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12365 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12385 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12483 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_facility_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12503 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_facility_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    12155 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_vo_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_vo_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11943 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_vo_ban.py
--rw-rw-rw-   0 root         (0) root         (0)    12977 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_specific_member.py
--rw-rw-rw-   0 root         (0) root         (0)    12375 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_submit_application.py
--rw-rw-rw-   0 root         (0) root         (0)    12153 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_unlock_services_on_destinations.py
--rw-rw-rw-   0 root         (0) root         (0)    11984 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_application_mail.py
--rw-rw-rw-   0 root         (0) root         (0)    12054 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_ban.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_ban1.py
--rw-rw-rw-   0 root         (0) root         (0)    12087 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_ban_for_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    11957 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_category.py
--rw-rw-rw-   0 root         (0) root         (0)    12010 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_consent_hub.py
--rw-rw-rw-   0 root         (0) root         (0)    11957 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    11909 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_form.py
--rw-rw-rw-   0 root         (0) root         (0)    12208 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_form_items_for_group.py
--rw-rw-rw-   0 root         (0) root         (0)    12178 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_form_items_for_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    11894 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_group.py
--rw-rw-rw-   0 root         (0) root         (0)    12020 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_publication.py
--rw-rw-rw-   0 root         (0) root         (0)    12026 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_publication_system.py
--rw-rw-rw-   0 root         (0) root         (0)    11957 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12031 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_resource_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11936 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)    12115 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_services_package.py
--rw-rw-rw-   0 root         (0) root         (0)    11873 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_user.py
--rw-rw-rw-   0 root         (0) root         (0)    11831 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_vo.py
--rw-rw-rw-   0 root         (0) root         (0)    12439 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/item_texts.py
--rw-rw-rw-   0 root         (0) root         (0)    12246 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/mail_text.py
--rw-rw-rw-   0 root         (0) root         (0)    13046 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/mail_type.py
--rw-rw-rw-   0 root         (0) root         (0)    15918 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/member.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/member_candidate.py
--rw-rw-rw-   0 root         (0) root         (0)    12227 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/member_group_status.py
--rw-rw-rw-   0 root         (0) root         (0)    12212 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/member_with_sponsors.py
--rw-rw-rw-   0 root         (0) root         (0)    12416 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/members_order_column.py
--rw-rw-rw-   0 root         (0) root         (0)    14145 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/members_page_query.py
--rw-rw-rw-   0 root         (0) root         (0)    13319 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/namespace_rules.py
--rw-rw-rw-   0 root         (0) root         (0)    12844 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/new_apps.py
--rw-rw-rw-   0 root         (0) root         (0)    14625 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/owner.py
--rw-rw-rw-   0 root         (0) root         (0)    12265 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/owner_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12707 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_audit_messages.py
--rw-rw-rw-   0 root         (0) root         (0)    12737 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_applications.py
--rw-rw-rw-   0 root         (0) root         (0)    12677 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_groups.py
--rw-rw-rw-   0 root         (0) root         (0)    12687 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_members.py
--rw-rw-rw-   0 root         (0) root         (0)    12667 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_users.py
--rw-rw-rw-   0 root         (0) root         (0)    11854 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_apps_config.py
--rw-rw-rw-   0 root         (0) root         (0)    18334 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_bean.py
--rw-rw-rw-   0 root         (0) root         (0)    12058 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_exception.py
--rw-rw-rw-   0 root         (0) root         (0)    12434 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_policy.py
--rw-rw-rw-   0 root         (0) root         (0)    13759 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_principal.py
--rw-rw-rw-   0 root         (0) root         (0)    17120 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/publication.py
--rw-rw-rw-   0 root         (0) root         (0)    14791 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/publication_for_gui.py
--rw-rw-rw-   0 root         (0) root         (0)    15184 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/publication_system.py
--rw-rw-rw-   0 root         (0) root         (0)    15115 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/resource.py
--rw-rw-rw-   0 root         (0) root         (0)    12175 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/resource_state.py
--rw-rw-rw-   0 root         (0) root         (0)    14343 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/resource_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    17416 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_application.py
--rw-rw-rw-   0 root         (0) root         (0)    14810 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_destination.py
--rw-rw-rw-   0 root         (0) root         (0)    14251 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_facility.py
--rw-rw-rw-   0 root         (0) root         (0)    14281 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_group.py
--rw-rw-rw-   0 root         (0) root         (0)    15389 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_member.py
--rw-rw-rw-   0 root         (0) root         (0)    14902 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    14756 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_user.py
--rw-rw-rw-   0 root         (0) root         (0)    12543 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)    14726 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/role_management_rules.py
--rw-rw-rw-   0 root         (0) root         (0)    13072 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/role_object.py
--rw-rw-rw-   0 root         (0) root         (0)    11963 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/rt_message.py
--rw-rw-rw-   0 root         (0) root         (0)    14358 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/security_team.py
--rw-rw-rw-   0 root         (0) root         (0)    15576 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/service.py
--rw-rw-rw-   0 root         (0) root         (0)    12183 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/service_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14214 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/service_for_gui.py
--rw-rw-rw-   0 root         (0) root         (0)    13419 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/service_state.py
--rw-rw-rw-   0 root         (0) root         (0)    14367 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/services_package.py
--rw-rw-rw-   0 root         (0) root         (0)    12034 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_for_group.py
--rw-rw-rw-   0 root         (0) root         (0)    11900 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)    12622 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_object.py
--rw-rw-rw-   0 root         (0) root         (0)    12539 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_objects.py
--rw-rw-rw-   0 root         (0) root         (0)    12464 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_object.py
--rw-rw-rw-   0 root         (0) root         (0)    12495 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_objects.py
--rw-rw-rw-   0 root         (0) root         (0)    12520 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/simple_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    12122 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/sorting_order.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/sponsor.py
--rw-rw-rw-   0 root         (0) root         (0)    13311 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/sponsored_user_data.py
--rw-rw-rw-   0 root         (0) root         (0)    15607 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task.py
--rw-rw-rw-   0 root         (0) root         (0)    12123 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_and_destination_id_object.py
--rw-rw-rw-   0 root         (0) root         (0)    12538 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_and_destination_name_object.py
--rw-rw-rw-   0 root         (0) root         (0)    11720 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_id_object.py
--rw-rw-rw-   0 root         (0) root         (0)    16287 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_result.py
--rw-rw-rw-   0 root         (0) root         (0)    11860 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_result_id_object.py
--rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_result_status.py
--rw-rw-rw-   0 root         (0) root         (0)    12728 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/task_status.py
--rw-rw-rw-   0 root         (0) root         (0)    15225 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/thanks.py
--rw-rw-rw-   0 root         (0) root         (0)    14159 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/thanks_for_gui.py
--rw-rw-rw-   0 root         (0) root         (0)    13804 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/type.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_for_group.py
--rw-rw-rw-   0 root         (0) root         (0)    11906 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)    12628 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_object.py
--rw-rw-rw-   0 root         (0) root         (0)    12545 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_objects.py
--rw-rw-rw-   0 root         (0) root         (0)    12470 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_object.py
--rw-rw-rw-   0 root         (0) root         (0)    12501 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_objects.py
--rw-rw-rw-   0 root         (0) root         (0)    16812 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    15208 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)    12056 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/users_order_column.py
--rw-rw-rw-   0 root         (0) root         (0)    14734 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/users_page_query.py
--rw-rw-rw-   0 root         (0) root         (0)    14322 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/vo.py
--rw-rw-rw-   0 root         (0) root         (0)    12324 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/vo_admin_roles.py
--rw-rw-rw-   0 root         (0) root         (0)    12374 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model/vo_member_statuses.py
--rw-rw-rw-   0 root         (0) root         (0)    81986 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:55.560860 perun.connector-3.5.0/perun/connector/perun_openapi/models/
--rw-rw-rw-   0 root         (0) root         (0)    26439 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14528 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/perun_openapi/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:55.564860 perun.connector-3.5.0/perun/connector/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/utils/AttributeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/utils/Logger.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 22:24:27.000000 perun.connector-3.5.0/perun/connector/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 21:31:53.660816 perun.connector-3.5.0/perun.connector.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2023-04-05 21:31:53.000000 perun.connector-3.5.0/perun.connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19600 2023-04-05 21:31:53.000000 perun.connector-3.5.0/perun.connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 21:31:53.000000 perun.connector-3.5.0/perun.connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-05 21:31:53.000000 perun.connector-3.5.0/perun.connector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-05 21:31:53.000000 perun.connector-3.5.0/perun.connector.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-05 21:31:55.564860 perun.connector-3.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-04-04 22:24:27.000000 perun.connector-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.807700 perun.connector-3.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-17 09:11:05.000000 perun.connector-3.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-17 09:18:03.807700 perun.connector-3.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-17 09:11:05.000000 perun.connector-3.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.627695 perun.connector-3.6.0/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.635695 perun.connector-3.6.0/perun/connector/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.671696 perun.connector-3.6.0/perun/connector/adapters/
+-rw-rw-rw-   0 root         (0) root         (0)    17238 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/adapters/AdapterInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)    14966 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/adapters/AdaptersManager.py
+-rw-rw-rw-   0 root         (0) root         (0)    28065 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/adapters/LdapAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    46720 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/adapters/PerunRpcAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/adapters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.671696 perun.connector-3.6.0/perun/connector/config_templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/config_templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.687697 perun.connector-3.6.0/perun/connector/connectors/
+-rw-rw-rw-   0 root         (0) root         (0)     4189 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/connectors/LdapConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.723698 perun.connector-3.6.0/perun/connector/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/Facility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/Group.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/HasIdAbstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/Member.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/MemberStatusEnum.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/Resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/User.py
+-rw-rw-rw-   0 root         (0) root         (0)      851 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/UserExtSource.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/VO.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.727697 perun.connector-3.6.0/perun/connector/perun_openapi/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.771699 perun.connector-3.6.0/perun/connector/perun_openapi/api/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   843770 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/attributes_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    56442 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/audit_messages_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   175597 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/authz_resolver_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   130963 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/cabinet_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    81270 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/consents_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/database_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    81685 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/ext_sources_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   544064 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/facilities_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   255356 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/groups_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5328 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/integration_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   271253 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/members_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    28296 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/owners_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   271089 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/registrar_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   452385 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/resources_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    22249 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/rt_messages_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    25572 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/searcher_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   367216 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/services_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   107772 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/tasks_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   306683 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/users_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    31350 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/utils_api.py
+-rw-rw-rw-   0 root         (0) root         (0)   198688 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api/vos_manager_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    38897 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.771699 perun.connector-3.6.0/perun/connector/perun_openapi/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18147 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.807700 perun.connector-3.6.0/perun/connector/perun_openapi/model/
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12548 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12265 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/add_user_ext_source_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    12230 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/app_state.py
+-rw-rw-rw-   0 root         (0) root         (0)    12173 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/app_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14842 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/application.py
+-rw-rw-rw-   0 root         (0) root         (0)    13343 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/application_form.py
+-rw-rw-rw-   0 root         (0) root         (0)    16033 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/application_form_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    13021 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/application_form_item_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13346 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/application_mail.py
+-rw-rw-rw-   0 root         (0) root         (0)    12539 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/applications_order_column.py
+-rw-rw-rw-   0 root         (0) root         (0)    14787 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/applications_page_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    13061 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/assigned_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    12311 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/assigned_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    13798 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/assigned_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    15808 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12347 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    16505 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12688 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)    12888 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_policy_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)    12425 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_rights.py
+-rw-rw-rw-   0 root         (0) root         (0)    12563 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    15539 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/audit_event.py
+-rw-rw-rw-   0 root         (0) root         (0)    12654 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/audit_message.py
+-rw-rw-rw-   0 root         (0) root         (0)    12762 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/audit_messages_page_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    20415 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/auditable.py
+-rw-rw-rw-   0 root         (0) root         (0)    15698 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/author.py
+-rw-rw-rw-   0 root         (0) root         (0)    15034 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/authorship.py
+-rw-rw-rw-   0 root         (0) root         (0)    11301 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/authz_roles.py
+-rw-rw-rw-   0 root         (0) root         (0)    14879 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/ban.py
+-rw-rw-rw-   0 root         (0) root         (0)    14344 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/ban_on_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    14354 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/ban_on_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    14306 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/ban_on_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    12646 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/brand.py
+-rw-rw-rw-   0 root         (0) root         (0)    14887 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/candidate.py
+-rw-rw-rw-   0 root         (0) root         (0)    14318 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/category.py
+-rw-rw-rw-   0 root         (0) root         (0)    15270 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/consent.py
+-rw-rw-rw-   0 root         (0) root         (0)    14644 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/consent_hub.py
+-rw-rw-rw-   0 root         (0) root         (0)    12267 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/consent_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    15246 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/destination.py
+-rw-rw-rw-   0 root         (0) root         (0)    12432 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/destination_propagation_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13073 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/destination_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12530 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ban_on_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12554 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ban_on_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ban_on_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    12140 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    12827 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12180 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    12189 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_host.py
+-rw-rw-rw-   0 root         (0) root         (0)    12727 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_identity.py
+-rw-rw-rw-   0 root         (0) root         (0)    12225 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12212 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/entityless_attributes_by_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    14314 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    11974 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/ext_source_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    14622 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12302 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/facility_propagation_state.py
+-rw-rw-rw-   0 root         (0) root         (0)    12595 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/facility_state.py
+-rw-rw-rw-   0 root         (0) root         (0)    12357 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/facility_with_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12418 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/gen_data_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    11668 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/gen_member_data_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    12082 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/graph_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12233 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/graph_file_format.py
+-rw-rw-rw-   0 root         (0) root         (0)    15471 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/group.py
+-rw-rw-rw-   0 root         (0) root         (0)    12452 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/group_member_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13052 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/group_member_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12445 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/group_resource_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    12161 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/groups_order_column.py
+-rw-rw-rw-   0 root         (0) root         (0)    13319 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/groups_page_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    12274 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/hashed_gen_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    14141 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/host.py
+-rw-rw-rw-   0 root         (0) root         (0)    12629 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/identity.py
+-rw-rw-rw-   0 root         (0) root         (0)    12200 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_application_mail_for_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    12158 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_application_mail_for_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    13405 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_destination_to_multiple_services.py
+-rw-rw-rw-   0 root         (0) root         (0)    12265 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_destinations_defined_by_hosts_on_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12401 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_member_candidates.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_assign_resource_tag_to_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12339 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_assign_resource_tags_to_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12198 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_attribute_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    12246 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_attribute_policy_collections.py
+-rw-rw-rw-   0 root         (0) root         (0)    11994 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_attribute_rights.py
+-rw-rw-rw-   0 root         (0) root         (0)    12150 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_block_services_on_destinations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12357 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_change_non_authz_password_by_token.py
+-rw-rw-rw-   0 root         (0) root         (0)    12920 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_change_password_for_login.py
+-rw-rw-rw-   0 root         (0) root         (0)    12906 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_change_password_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    12218 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_check_password_strength.py
+-rw-rw-rw-   0 root         (0) root         (0)    11843 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_consolidate.py
+-rw-rw-rw-   0 root         (0) root         (0)    12790 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_copy_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12597 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_alternative_password.py
+-rw-rw-rw-   0 root         (0) root         (0)    12096 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_attribute_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    11999 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_authorship.py
+-rw-rw-rw-   0 root         (0) root         (0)    11957 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_category.py
+-rw-rw-rw-   0 root         (0) root         (0)    12019 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_category_nr.py
+-rw-rw-rw-   0 root         (0) root         (0)    12468 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_member_for_candidate.py
+-rw-rw-rw-   0 root         (0) root         (0)    12269 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_member_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13318 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_member_from_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    12463 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_owner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12020 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_publication.py
+-rw-rw-rw-   0 root         (0) root         (0)    12026 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_publication_system.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_resource_tag_with_resource_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11936 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    12462 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_service_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    12115 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_services_package.py
+-rw-rw-rw-   0 root         (0) root         (0)    13130 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_sponsored_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    13829 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_sponsored_member_from_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    13555 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_sponsored_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    11861 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_thanks.py
+-rw-rw-rw-   0 root         (0) root         (0)    11849 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_vo_with_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    12077 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_delete_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    12031 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_delete_resource_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    12227 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_entityless_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12273 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_form_item_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12282 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_form_items_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12288 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_all_resources_by_resource_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    12197 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_facilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    12830 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_match_resources.py
+-rw-rw-rw-   0 root         (0) root         (0)    12532 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_members_by_user_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12045 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_messages_page.py
+-rw-rw-rw-   0 root         (0) root         (0)    12232 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_applications.py
+-rw-rw-rw-   0 root         (0) root         (0)    12416 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    12426 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    12472 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_subgroups.py
+-rw-rw-rw-   0 root         (0) root         (0)    12238 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_users.py
+-rw-rw-rw-   0 root         (0) root         (0)    12194 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_resources.py
+-rw-rw-rw-   0 root         (0) root         (0)    12182 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)    12676 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_invitations_from_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    12600 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_invite_member_candidates.py
+-rw-rw-rw-   0 root         (0) root         (0)    12227 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_lock_publications.py
+-rw-rw-rw-   0 root         (0) root         (0)    12325 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_remove_resource_tag_from_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12345 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_remove_resource_tags_from_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12135 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_remove_rich_destinations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_reserve_password_for_login.py
+-rw-rw-rw-   0 root         (0) root         (0)    12242 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_reserve_password_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    12516 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_send_message.py
+-rw-rw-rw-   0 root         (0) root         (0)    12045 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_ban.py
+-rw-rw-rw-   0 root         (0) root         (0)    12096 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_ban_for_user_on_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12251 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12159 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13283 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_resource_group_user_member_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12843 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_resource_user_member_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12367 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_user_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12203 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12223 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12499 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_resource_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12519 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_resource_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12187 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_host_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_host_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12219 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12239 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12467 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_group_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12487 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_group_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12946 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_group_with_user_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12991 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_resource_and_user_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12515 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_resource_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12535 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_resource_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12712 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_with_user_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12251 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12271 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12519 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_group_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12992 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_group_with_group_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12215 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_sending_enabled.py
+-rw-rw-rw-   0 root         (0) root         (0)    12990 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_sponsored_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    12187 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12365 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12385 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12483 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_facility_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12503 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_facility_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12155 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_vo_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_vo_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11943 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_vo_ban.py
+-rw-rw-rw-   0 root         (0) root         (0)    12977 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_specific_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    12375 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_submit_application.py
+-rw-rw-rw-   0 root         (0) root         (0)    12153 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_unlock_services_on_destinations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11984 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_application_mail.py
+-rw-rw-rw-   0 root         (0) root         (0)    12054 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_ban.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_ban1.py
+-rw-rw-rw-   0 root         (0) root         (0)    12087 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_ban_for_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    11957 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_category.py
+-rw-rw-rw-   0 root         (0) root         (0)    12010 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_consent_hub.py
+-rw-rw-rw-   0 root         (0) root         (0)    11957 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    11909 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_form.py
+-rw-rw-rw-   0 root         (0) root         (0)    12208 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_form_items_for_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    12178 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_form_items_for_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    11894 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    12020 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_publication.py
+-rw-rw-rw-   0 root         (0) root         (0)    12026 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_publication_system.py
+-rw-rw-rw-   0 root         (0) root         (0)    11957 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12031 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_resource_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11936 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    12115 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_services_package.py
+-rw-rw-rw-   0 root         (0) root         (0)    11873 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    11831 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    12439 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/item_texts.py
+-rw-rw-rw-   0 root         (0) root         (0)    12246 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/mail_text.py
+-rw-rw-rw-   0 root         (0) root         (0)    13046 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/mail_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    15918 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/member.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/member_candidate.py
+-rw-rw-rw-   0 root         (0) root         (0)    12227 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/member_group_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    12212 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/member_with_sponsors.py
+-rw-rw-rw-   0 root         (0) root         (0)    12416 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/members_order_column.py
+-rw-rw-rw-   0 root         (0) root         (0)    14145 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/members_page_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    13319 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/namespace_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    12844 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/new_apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/owner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12265 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/owner_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12707 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_audit_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)    12737 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_applications.py
+-rw-rw-rw-   0 root         (0) root         (0)    12677 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    12687 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    12667 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_users.py
+-rw-rw-rw-   0 root         (0) root         (0)    11854 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_apps_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    18334 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_bean.py
+-rw-rw-rw-   0 root         (0) root         (0)    12058 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)    12434 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)    13759 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_principal.py
+-rw-rw-rw-   0 root         (0) root         (0)    17120 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/publication.py
+-rw-rw-rw-   0 root         (0) root         (0)    14791 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/publication_for_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)    15184 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/publication_system.py
+-rw-rw-rw-   0 root         (0) root         (0)    15115 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    12175 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/resource_state.py
+-rw-rw-rw-   0 root         (0) root         (0)    14343 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/resource_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    17416 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_application.py
+-rw-rw-rw-   0 root         (0) root         (0)    14810 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_destination.py
+-rw-rw-rw-   0 root         (0) root         (0)    14251 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_facility.py
+-rw-rw-rw-   0 root         (0) root         (0)    14281 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    15389 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    14902 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    14756 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    12543 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    14726 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/role_management_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    13072 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/role_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    11963 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/rt_message.py
+-rw-rw-rw-   0 root         (0) root         (0)    14358 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/security_team.py
+-rw-rw-rw-   0 root         (0) root         (0)    15576 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/service.py
+-rw-rw-rw-   0 root         (0) root         (0)    12183 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/service_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14214 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/service_for_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)    13419 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/service_state.py
+-rw-rw-rw-   0 root         (0) root         (0)    14367 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/services_package.py
+-rw-rw-rw-   0 root         (0) root         (0)    12034 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_for_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    11900 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    12622 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    12539 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    12464 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    12495 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    12520 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/simple_attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)    12122 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/sorting_order.py
+-rw-rw-rw-   0 root         (0) root         (0)    13456 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/sponsor.py
+-rw-rw-rw-   0 root         (0) root         (0)    13311 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/sponsored_user_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    15607 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    12123 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_and_destination_id_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    12538 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_and_destination_name_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    11720 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_id_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    16287 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_result_id_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_result_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    12728 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/task_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    15225 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/thanks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14159 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/thanks_for_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)    13804 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_for_group.py
+-rw-rw-rw-   0 root         (0) root         (0)    11906 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_for_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    12628 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    12545 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    12470 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    12501 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    16812 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    15208 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    12056 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/users_order_column.py
+-rw-rw-rw-   0 root         (0) root         (0)    14734 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/users_page_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    14322 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/vo.py
+-rw-rw-rw-   0 root         (0) root         (0)    12324 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/vo_admin_roles.py
+-rw-rw-rw-   0 root         (0) root         (0)    12374 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model/vo_member_statuses.py
+-rw-rw-rw-   0 root         (0) root         (0)    81986 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.807700 perun.connector-3.6.0/perun/connector/perun_openapi/models/
+-rw-rw-rw-   0 root         (0) root         (0)    26439 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14528 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/perun_openapi/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.807700 perun.connector-3.6.0/perun/connector/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/utils/AttributeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/utils/Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:11:05.000000 perun.connector-3.6.0/perun/connector/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:18:03.635695 perun.connector-3.6.0/perun.connector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-17 09:18:03.000000 perun.connector-3.6.0/perun.connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19600 2023-05-17 09:18:03.000000 perun.connector-3.6.0/perun.connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:18:03.000000 perun.connector-3.6.0/perun.connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-17 09:18:03.000000 perun.connector-3.6.0/perun.connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-17 09:18:03.000000 perun.connector-3.6.0/perun.connector.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-17 09:18:03.807700 perun.connector-3.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-17 09:11:05.000000 perun.connector-3.6.0/setup.py
```

### Comparing `perun.connector-3.5.0/LICENSE` & `perun.connector-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/__init__.py` & `perun.connector-3.6.0/perun/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/adapters/AdapterInterface.py` & `perun.connector-3.6.0/perun/connector/adapters/AdapterInterface.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/adapters/AdaptersManager.py` & `perun.connector-3.6.0/perun/connector/adapters/AdaptersManager.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/adapters/LdapAdapter.py` & `perun.connector-3.6.0/perun/connector/adapters/LdapAdapter.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/adapters/PerunRpcAdapter.py` & `perun.connector-3.6.0/perun/connector/adapters/PerunRpcAdapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import List, Union, Optional
 
 from perun.connector.perun_openapi.model.input_get_facilities import InputGetFacilities
 
 from perun.connector.perun_openapi.api.searcher_api import SearcherApi
 
 from perun.connector import perun_openapi
@@ -58,14 +59,18 @@
 
         if "rp_id_attribute" not in config_data:
             self._RP_ID_ATTR = "urn:perun:facility:attribute-def:def:rpIdentifier"
         else:
             self._RP_ID_ATTR = config_data["rp_id_attribute"]
 
         self._ATTRIBUTE_UTILS = AttributeUtils(attrs_map)
+        self._COOKIE_FILEPATH = config_data.get(
+            "cookie_filepath", "/tmp/perun-cookie.txt"
+        )
+        self.cookie = self._load_cookie_from_file(self._COOKIE_FILEPATH)
 
     def _set_up_openapi_config(self, config_data: dict[str, str]) -> None:
         auth_type = config_data["auth_type"]
         self._CONFIG = Configuration(host=config_data["host"])
 
         if auth_type == self._BASIC_AUTH:
             self._CONFIG.username = config_data["username"]
@@ -80,21 +85,34 @@
                 f"supported way of authentication, please "
                 f'set "auth_type" to one of "'
                 f'{self._BASIC_AUTH}", "{self._BEARER_AUTH}" '
                 f'or "{self._API_KEY_AUTH}"'
             )
             raise ValueError(exception_message)
 
+    def _call_api(self, callable_method, params: dict):
+        params["_return_http_data_only"] = False
+        data, status, headers = callable_method(**params)
+        cookie = headers.get("Set-Cookie", "")
+        cookie = re.match(r"PERUNSESSION=\w+;", cookie)
+        if cookie:
+            cookie = cookie.group()
+            if cookie != self.cookie:
+                self.cookie = cookie
+                self._save_cookie_to_file(self._COOKIE_FILEPATH, self.cookie)
+        return data
+
     def get_perun_user(self, idp_id: str, uids: List[str]) -> Optional[User]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             api_instance = UsersManagerApi(api_client)
             for uid in uids:
                 try:
-                    user = api_instance.get_user_by_ext_source_name_and_ext_login(
-                        ext_login=uid, ext_source_name=idp_id
+                    user = self._call_api(
+                        api_instance.get_user_by_ext_source_name_and_ext_login,
+                        {"ext_login": uid, "ext_source_name": idp_id},
                     )
                     name = ""
                     for user_attr in [
                         "title_before",
                         "first_name",
                         "middle_name",
                         "last_name",
@@ -114,17 +132,20 @@
 
     def _get_group_unique_name(
         self,
         attributes_api_instance: AttributesManagerApi,
         group_name: str,
         group_id: int,
     ) -> str:
-        attr = attributes_api_instance.get_attribute(
-            group=group_id,
-            attribute_name="urn:perun:group:attribute-def:virt:voShortName",
+        attr = self._call_api(
+            attributes_api_instance.get_attribute,
+            {
+                "group": group_id,
+                "attribute_name": "urn:perun:group:attribute-def:virt:voShortName",
+            },
         )
         return f'{attr["value"]}:{group_name}'
 
     def _create_internal_representation_groups(
         self,
         input_groups: List[perun_openapi.model.group.Group],
         converted_groups: List[Group],
@@ -152,107 +173,118 @@
                     )
                 )
                 unique_ids.append(group["id"])
 
     def get_member_groups(
         self, user: Union[User, int], vo: Union[VO, int]
     ) -> List[Group]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             members_api_instance = MembersManagerApi(api_client)
             groups_api_instance = GroupsManagerApi(api_client)
             attributes_api_instance = AttributesManagerApi(api_client)
 
             converted_groups = []
             if not isinstance(vo, VO):
                 vo = self.get_vo(vo_id=vo)
             user_id = AdapterInterface.get_object_id(user)
-            member = members_api_instance.get_member_by_user(vo.id, user_id)
+            member = self._call_api(
+                members_api_instance.get_member_by_user, {"vo": vo.id, "user": user_id}
+            )
             member_groups = []
             if member:
-                member_groups = groups_api_instance.get_all_member_groups(member["id"])
+                member_groups = self._call_api(
+                    groups_api_instance.get_all_member_groups, {"member": member["id"]}
+                )
             self._create_internal_representation_groups(
                 member_groups, converted_groups, attributes_api_instance, vo
             )
             return converted_groups
 
     def get_sp_groups_by_facility(self, facility: Union[Facility, int]) -> List[Group]:
         if facility is None:
             return []
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
             facilities_api_instance = FacilitiesManagerApi(api_client)
             resources_api_instance = ResourcesManagerApi(api_client)
 
             facility_id = AdapterInterface.get_object_id(facility)
-            resources = facilities_api_instance.get_assigned_resources_for_facility(
-                facility_id
+            resources = self._call_api(
+                facilities_api_instance.get_assigned_resources_for_facility,
+                {"facility": facility_id},
             )
 
             resources_ids = [resource.id for resource in resources]
 
             sp_groups = []
             for resource_id in resources_ids:
-                groups = resources_api_instance.get_assigned_groups(resource_id)
+                groups = self._call_api(
+                    resources_api_instance.get_assigned_groups,
+                    {"resource": resource_id},
+                )
                 if groups:
                     vo = self.get_vo(vo_id=groups[0]["vo_id"])
 
                 self._create_internal_representation_groups(
                     groups, sp_groups, attributes_api_instance, vo
                 )
             return sp_groups
 
     def get_sp_groups_by_rp_id(self, rp_id: str) -> List[Group]:
         facility = self.get_facility_by_rp_identifier(rp_id)
         return self.get_sp_groups_by_facility(facility)
 
     def get_group_by_name(self, vo: Union[VO, int], name: str) -> Group:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
             groups_api_instance = GroupsManagerApi(api_client)
 
             vo_id = AdapterInterface.get_object_id(vo)
-            group = groups_api_instance.get_group_by_name(vo_id, name)
+            group = self._call_api(
+                groups_api_instance.get_group_by_name, {"vo": vo_id, "name": name}
+            )
             group_external_representation = [group]
             converted_group = []
             self._create_internal_representation_groups(
                 group_external_representation, converted_group, attributes_api_instance
             )
             return converted_group[0]
 
     def get_vo(self, short_name="", vo_id=None) -> Optional[VO]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             vos_api_instance = VosManagerApi(api_client)
 
             if short_name and vo_id:
                 raise ValueError(
                     "VO can be obtained either by its short_name or id, "
                     "not both "
                     "at the same time."
                 )
             elif vo_id:
                 vo_lookup_method = vos_api_instance.get_vo_by_id
-                vo_lookup_attribute = vo_id
+                vo_lookup_attribute = {"id": vo_id}
             elif short_name:
                 vo_lookup_method = vos_api_instance.get_vo_by_short_name
-                vo_lookup_attribute = short_name
+                vo_lookup_attribute = {"short_name": short_name}
             else:
                 raise ValueError(
                     "Neither short_name nor id was provided, please specify "
                     "exactly one to find VO by."
                 )
-            vo = vo_lookup_method(vo_lookup_attribute)
+            vo = self._call_api(vo_lookup_method, vo_lookup_attribute)
             return VO(vo.id, vo.name, vo.short_name)
 
     def get_facility_by_rp_identifier(self, rp_identifier: str) -> Optional[Facility]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             facilities_api_instance = FacilitiesManagerApi(api_client)
 
-            facilities = facilities_api_instance.get_facilities_by_attribute(
-                attribute_name=self._RP_ID_ATTR, attribute_value=rp_identifier
+            facilities = self._call_api(
+                facilities_api_instance.get_facilities_by_attribute,
+                {"attribute_name": self._RP_ID_ATTR, "attribute_value": rp_identifier},
             )
 
             if not facilities:
                 raise RPCAdapterNotExistsException(
                     f"No facility with rpID '{rp_identifier}' found."
                 )
 
@@ -270,24 +302,23 @@
 
     def get_users_groups_on_facility(
         self, facility: Union[Facility, int], user: Union[User, int]
     ) -> List[Group]:
         if facility is None:
             return []
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             users_api_instance = UsersManagerApi(api_client)
             attributes_api_instance = AttributesManagerApi(api_client)
 
             facility_id = AdapterInterface.get_object_id(facility)
             user_id = AdapterInterface.get_object_id(user)
-            users_groups_on_facility = (
-                users_api_instance.get_groups_for_facility_where_user_is_active(
-                    user_id, facility_id
-                )
+            users_groups_on_facility = self._call_api(
+                users_api_instance.get_groups_for_facility_where_user_is_active,
+                {"user": user_id, "facility": facility_id},
             )
             converted_groups = []
             self._create_internal_representation_groups(
                 users_groups_on_facility, converted_groups, attributes_api_instance
             )
             return converted_groups
 
@@ -308,20 +339,21 @@
         if len(attribute) != 1:
             self._logger.warning(
                 f"Attribute must contain exactly one name and one value. "
                 f'Given attribute contains: "{attribute}".'
             )
             return []
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             searcher_api = SearcherApi(api_client)
 
             attribute_to_match_in_facilities = InputGetFacilities(attribute)
-            perun_facilities = searcher_api.get_facilities(
-                attribute_to_match_in_facilities
+            perun_facilities = self._call_api(
+                searcher_api.get_facilities,
+                {"input_get_facilities": attribute_to_match_in_facilities},
             )
 
             facilities = []
             for perun_facility in perun_facilities:
                 facility = Facility(
                     perun_facility["id"],
                     perun_facility["name"],
@@ -333,33 +365,36 @@
                 facilities.append(facility)
 
         return facilities
 
     def get_facility_attributes(
         self, facility: Union[Facility, int], attr_names: List[str]
     ) -> dict[str, Union[str, Optional[int], bool, List[str], dict[str, str]]]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
 
             facility_id = AdapterInterface.get_object_id(facility)
-            perun_attrs = attributes_api_instance.get_facility_attributes_by_names(
-                facility_id, attr_names
+            perun_attrs = self._call_api(
+                attributes_api_instance.get_facility_attributes_by_names,
+                {"facility": facility_id, "attr_names": attr_names},
             )
             return self._get_attributes(perun_attrs)
 
     def get_user_ext_source(
         self, ext_source_name: str, ext_source_login: str
     ) -> UserExtSource:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             users_api_instance = UsersManagerApi(api_client)
 
-            user_ext_source_perun = (
-                users_api_instance.get_user_ext_source_by_ext_login_and_ext_source_name(
-                    ext_source_name=ext_source_name, ext_source_login=ext_source_login
-                )
+            user_ext_source_perun = self._call_api(
+                users_api_instance.get_user_ext_source_by_ext_login_and_ext_source_name,
+                {
+                    "ext_source_name": ext_source_name,
+                    "ext_source_login": ext_source_login,
+                },
             )
 
             ext_source_id = user_ext_source_perun["id"]
             login = user_ext_source_perun["login"]
 
             ext_source_details = user_ext_source_perun["ext_source"]
             name = ext_source_details["name"]
@@ -369,24 +404,23 @@
             return UserExtSource(ext_source_id, name, login, user)
 
     def get_user_ext_source_by_unique_attribute_value(
         self,
         attr_name: str,
         attr_value: Union[str, int, bool, List[str], dict[str, str]],
     ) -> UserExtSource:
-        with ApiClient(self._CONFIG) as api_client:
-            users_api_instance = UsersManagerApi(api_client)
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
+            api_function = UsersManagerApi(
+                api_client
+            ).get_user_ext_source_by_unique_attribute_value_and_attribute_name
 
             try:
-                # function name is too long (would never fit formatting requirements)
-                fun_name = (
-                    "get_user_ext_source_by_unique_attribute_value_and_attribute_name"
-                )
-                user_ext_source_perun = getattr(users_api_instance, fun_name)(
-                    attr_name, attr_value
+                user_ext_source_perun = self._call_api(
+                    api_function,
+                    {"attribute_name": attr_name, "attribute_value": attr_value},
                 )
             except ApiException as ex:
                 if '"name":"UserExtSourceNotExistsException"' in ex.body:
                     raise RPCAdapterNotExistsException(
                         f"No user ext source for attr name: '{attr_value}' value: "
                         f"{str(attr_value)} found."
                     )
@@ -402,46 +436,52 @@
             return UserExtSource(ext_source_id, name, login, user)
 
     def update_user_ext_source_last_access(
         self, user_ext_source: Union[UserExtSource, int]
     ) -> None:
         user_ext_source_id = AdapterInterface.get_object_id(user_ext_source)
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             users_api_instance = UsersManagerApi(api_client)
 
-            users_api_instance.update_user_ext_source_last_access(user_ext_source_id)
+            self._call_api(
+                users_api_instance.update_user_ext_source_last_access,
+                {"user_ext_source": user_ext_source_id},
+            )
 
     def get_user_ext_source_attributes(
         self, user_ext_source: Union[UserExtSource, int], attr_names: List[str]
     ) -> dict[str, Union[str, Optional[int], bool, List[str], dict[str, str]]]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
 
             user_ext_source_id = AdapterInterface.get_object_id(user_ext_source)
-            perun_attrs = (
-                attributes_api_instance.get_user_ext_source_attributes_by_names(
-                    user_ext_source=user_ext_source_id, attr_names=attr_names
-                )
+            perun_attrs = self._call_api(
+                attributes_api_instance.get_user_ext_source_attributes_by_names,
+                {"user_ext_source": user_ext_source_id, "attr_names": attr_names},
             )
             return self._get_attributes(perun_attrs)
 
     def set_user_ext_source_attributes(
         self,
         user_ext_source: Union[UserExtSource, int],
         attributes: dict[
             str, Union[str, Optional[int], bool, List[str], dict[str, str]]
         ],
     ) -> None:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
             user_ext_source_id = AdapterInterface.get_object_id(user_ext_source)
             openapi_attributes = self.internal_to_open_api_attrs(attributes)
-            attributes_api_instance.set_user_ext_source_attributes(
-                InputSetUserExtSourceAttributes(user_ext_source_id, openapi_attributes)
+            input_arg = InputSetUserExtSourceAttributes(
+                user_ext_source_id, openapi_attributes
+            )
+            self._call_api(
+                attributes_api_instance.set_user_ext_source_attributes,
+                {"input_set_user_ext_source_attributes": input_arg},
             )
 
     def internal_to_open_api_attrs(
         self,
         attributes: dict[
             str, Union[str, Optional[int], bool, List[str], dict[str, str]]
         ],
@@ -490,51 +530,58 @@
         valid_status = MemberStatusEnum.VALID
 
         return user_status == valid_status
 
     def get_member_by_user(
         self, user: Union[User, int], vo: Union[VO, int]
     ) -> Optional[Member]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             members_api_instance = MembersManagerApi(api_client)
 
             user_id = AdapterInterface.get_object_id(user)
             vo_id = AdapterInterface.get_object_id(vo)
 
-            member = members_api_instance.get_member_by_user(vo_id, user_id)
+            member = self._call_api(
+                members_api_instance.get_member_by_user, {"vo": vo_id, "user": user_id}
+            )
             return Member(member["id"], vo, member["status"])
 
     def get_resource_capabilities_by_facility(
         self, facility: Union[Facility, int], user_groups: List[Union[Group, int]]
     ) -> List[str]:
         capabilities = []
         if facility is None:
             return capabilities
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             facilities_api_instance = FacilitiesManagerApi(api_client)
             resources_api_instance = ResourcesManagerApi(api_client)
             attributes_api_instance = AttributesManagerApi(api_client)
 
             facility_id = AdapterInterface.get_object_id(facility)
-            resources = facilities_api_instance.get_assigned_resources_for_facility(
-                facility_id
+            resources = self._call_api(
+                facilities_api_instance.get_assigned_resources_for_facility,
+                {"facility": facility_id},
             )
             user_groups_ids = [
                 AdapterInterface.get_object_id(user_group) for user_group in user_groups
             ]
             for resource in resources:
-                resource_groups = resources_api_instance.get_assigned_groups(
-                    resource["id"]
+                resource_groups = self._call_api(
+                    resources_api_instance.get_assigned_groups,
+                    {"resource": resource["id"]},
                 )
 
-                resource_capabilities = attributes_api_instance.get_attribute(
-                    resource=resource["id"],
-                    attribute_name="urn:perun:resource:attribute-def:def"
-                    ":capabilities",
+                attr_name = "urn:perun:resource:attribute-def:def:capabilities"
+                resource_capabilities = self._call_api(
+                    attributes_api_instance.get_attribute,
+                    {
+                        "resource": resource["id"],
+                        "attribute_name": attr_name,
+                    },
                 )["value"]
 
                 if resource_capabilities is None:
                     continue
 
                 for resource_group in resource_groups:
                     if resource_group["id"] in user_groups_ids:
@@ -550,22 +597,26 @@
 
     def get_facility_capabilities_by_facility(
         self, facility: Union[Facility, int]
     ) -> List[str]:
         if facility is None:
             return []
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
 
             facility_id = AdapterInterface.get_object_id(facility)
 
-            facility_capabilities = attributes_api_instance.get_attribute(
-                facility=facility_id,
-                attribute_name="urn:perun:facility:attribute-def:def:capabilities",
+            attr_name = "urn:perun:facility:attribute-def:def:capabilities"
+            facility_capabilities = self._call_api(
+                attributes_api_instance.get_attribute,
+                {
+                    "facility": facility_id,
+                    "attribute_name": attr_name,
+                },
             )["value"]
 
             return facility_capabilities
 
     def get_facility_capabilities_by_rp_id(self, rp_identifier: str) -> List[str]:
         facility = self.get_facility_by_rp_identifier(rp_identifier)
         return self.get_facility_capabilities_by_facility(facility)
@@ -573,62 +624,66 @@
     def get_user_attributes(
         self, user: Union[User, int], attr_names: List[str]
     ) -> dict[str, Union[str, Optional[int], bool, List[str], dict[str, str]]]:
         default_attribute_name = "urn:perun:user:attribute-def:virt:loa"
         if not attr_names:
             attr_names.append(default_attribute_name)
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
 
             user_id = AdapterInterface.get_object_id(user)
 
-            perun_attrs = attributes_api_instance.get_user_attributes_by_names(
-                user_id, attr_names
+            perun_attrs = self._call_api(
+                attributes_api_instance.get_user_attributes_by_names,
+                {"user": user_id, "attr_names": attr_names},
             )
 
             return self._get_attributes(perun_attrs)
 
     def get_entityless_attribute(
         self, attr_name: str
     ) -> Union[str, Optional[int], bool, List[str], dict[str, str]]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
 
             attributes = {}
-            perun_attr_values = (
-                attributes_api_instance.get_entityless_attributes_by_name(
-                    attr_name=attr_name
-                )
+            perun_attr_values = self._call_api(
+                attributes_api_instance.get_entityless_attributes_by_name,
+                {"attr_name": attr_name},
             )
 
             attr_id = perun_attr_values[0].get("id")
             if attr_id is None:
                 return attributes
 
-            perun_attr_keys = attributes_api_instance.get_entityless_keys(attr_id)
+            perun_attr_keys = self._call_api(
+                attributes_api_instance.get_entityless_keys,
+                {"attribute_definition": attr_id},
+            )
 
             for i in range(len(perun_attr_values)):
                 attributes[perun_attr_keys[i]] = perun_attr_values[i]["value"]
             return attributes
 
     def get_vo_attributes(
         self, vo: Union[VO, int], attr_names: List[str]
     ) -> dict[str, Union[str, Optional[int], bool, List[str], dict[str, str]]]:
         default_attribute_name = "urn:perun:vo:attribute-def:core:id"
         if not attr_names:
             attr_names.append(default_attribute_name)
 
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
 
             vo_id = AdapterInterface.get_object_id(vo)
 
-            perun_attrs = attributes_api_instance.get_vo_attributes_by_names(
-                vo_id, attr_names
+            perun_attrs = self._call_api(
+                attributes_api_instance.get_vo_attributes_by_names,
+                {"vo": vo_id, "attr_names": attr_names},
             )
 
             return self._get_attributes(perun_attrs)
 
     def _get_attributes(
         self,
         perun_attrs: List[dict[str, Union[str, int, bool, list[str], dict[str, str]]]],
@@ -644,20 +699,21 @@
                 attributes[perun_attr_name] = perun_attr["value"]
 
         return attributes
 
     def get_groups_where_member_is_active(
         self, member: Union[Member, int]
     ) -> List[Group]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             member_id = self.get_object_id(member)
             internal_groups = []
             groups_api_instance = GroupsManagerApi(api_client)
-            perun_groups = groups_api_instance.get_groups_where_member_is_active(
-                member_id
+            perun_groups = self._call_api(
+                groups_api_instance.get_groups_where_member_is_active,
+                {"member": member_id},
             )
             if isinstance(member, Member):
                 vo = member.vo
             elif perun_groups:
                 vo = self.get_vo(vo_id=perun_groups[0]["vo_id"])
             attributes_api_instance = AttributesManagerApi(api_client)
             self._create_internal_representation_groups(
@@ -668,126 +724,138 @@
     def get_groups_where_user_as_member_is_active(
         self, user: Union[User, int], vo: Union[VO, int]
     ) -> List[Group]:
         member = self.get_member_by_user(user, vo)
         return self.get_groups_where_member_is_active(member)
 
     def has_registration_form_group(self, group: Union[Group, int]) -> bool:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             group_id = self.get_object_id(group)
             registrar_api_instance = RegistrarManagerApi(api_client)
-            if not registrar_api_instance.get_group_application_form(group_id):
+            if not self._call_api(
+                registrar_api_instance.get_group_application_form, {"group": group_id}
+            ):
                 return False
             return True
 
     def has_registration_form_vo(self, vo: Union[VO, int]) -> bool:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             vo_id = self.get_object_id(vo)
             registrar_api_instance = RegistrarManagerApi(api_client)
-            if not registrar_api_instance.get_vo_application_form(vo_id):
+            if not self._call_api(
+                registrar_api_instance.get_vo_application_form, {"vo": vo_id}
+            ):
                 return False
             return True
 
     def has_registration_form_by_vo_short_name(self, vo_short_name: str) -> bool:
         vo = self.get_vo(vo_short_name)
         return self.has_registration_form_vo(vo)
 
     def create_facility(self, name: str, description="") -> Facility:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             facilities_api_instance = FacilitiesManagerApi(api_client)
             if description:
-                return facilities_api_instance.create_facility(
-                    name, description=description
+                return self._call_api(
+                    facilities_api_instance.create_facility,
+                    {"name": name, "description": description},
                 )
-            return facilities_api_instance.create_facility(name)
+            return self._call_api(
+                facilities_api_instance.create_facility, {"name": name}
+            )
 
     def set_facility_attributes(
         self,
         facility: Union[Facility, int],
         attributes: dict[
             str, Union[str, Optional[int], bool, List[str], dict[str, str]]
         ],
     ) -> None:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
             facility_id = AdapterInterface.get_object_id(facility)
             openapi_attributes = self.internal_to_open_api_attrs(attributes)
 
-            attributes_api_instance.set_facility_attributes(
-                InputSetFacilityAttributes(
-                    facility=facility_id, attributes=openapi_attributes
-                )
+            self._call_api(
+                attributes_api_instance.set_facility_attributes,
+                {
+                    "input_set_facility_attributes": InputSetFacilityAttributes(
+                        facility=facility_id, attributes=openapi_attributes
+                    )
+                },
             )
 
     def get_attributes_definition(self) -> List[dict[str, Union[str, int, bool]]]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             attributes_api_instance = AttributesManagerApi(api_client)
-            return attributes_api_instance.get_all_attribute_definitions()
-
-    def get_user_role_names(self):
-        with ApiClient(self._CONFIG) as api_client:
-            authz_api_instance = AuthzResolverApi(api_client)
-            return authz_api_instance.get_user_role_names(74017)
+            return self._call_api(
+                attributes_api_instance.get_all_attribute_definitions, {}
+            )
 
     def is_user_perun_admin(self, user: Union[User, int]) -> bool:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             authz_api_instance = AuthzResolverApi(api_client)
-            if "perunadmin" in authz_api_instance.get_user_role_names(
-                AdapterInterface.get_object_id(user)
+            if "perunadmin" in self._call_api(
+                authz_api_instance.get_user_role_names,
+                {"user": AdapterInterface.get_object_id(user)},
             ):
                 return True
             return False
 
     def get_vos_where_user_is_admin(
         self, user: Union[User, int], check_perun_admin=True
     ) -> List[VO]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             if check_perun_admin and self.is_user_perun_admin(user):
                 return self.get_all_vos()
             users_api_instance = UsersManagerApi(api_client)
-            vos = users_api_instance.get_vos_where_user_is_admin(
-                AdapterInterface.get_object_id(user)
+            vos = self._call_api(
+                users_api_instance.get_vos_where_user_is_admin,
+                {"user": AdapterInterface.get_object_id(user)},
             )
             return [VO(vo.id, vo.name, vo.short_name) for vo in vos]
 
     def get_groups_where_user_is_admin(
         self,
         user: Union[User, int],
         check_perun_admin=True,
         fill_group_unique_name=True,
     ) -> List[Group]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             vos = self.get_all_vos()
             attributes_api_instance = AttributesManagerApi(api_client)
             if check_perun_admin and self.is_user_perun_admin(user):
                 groups_api_instance = GroupsManagerApi(api_client)
-                groups = groups_api_instance.get_all_groups_from_all_vos()
+                groups = self._call_api(
+                    groups_api_instance.get_all_groups_from_all_vos, {}
+                )
                 return [
                     Group(
                         group.id,
-                        self.__find_vo_in_list_by_id(vos, group.vo_id),
+                        self._find_vo_in_list_by_id(vos, group.vo_id),
                         group.uuid,
                         group.name,
                         ""
                         if not fill_group_unique_name
                         else self._get_group_unique_name(
                             attributes_api_instance, group.name, group.id
                         ),
                         group.description,
                     )
                     for group in groups
                 ]
             users_api_instance = UsersManagerApi(api_client)
-            groups = users_api_instance.get_groups_where_user_is_admin(
-                AdapterInterface.get_object_id(user)
+            groups = self._call_api(
+                users_api_instance.get_groups_where_user_is_admin,
+                {"user": AdapterInterface.get_object_id(user)},
             )
             return [
                 Group(
                     group.id,
-                    self.__find_vo_in_list_by_id(vos, group.vo_id),
+                    self._find_vo_in_list_by_id(vos, group.vo_id),
                     group.uuid,
                     group.name,
                     ""
                     if not fill_group_unique_name
                     else self._get_group_unique_name(
                         attributes_api_instance, group.name, group.id
                     ),
@@ -795,20 +863,21 @@
                 )
                 for group in groups
             ]
 
     def get_facilities_where_user_is_admin(
         self, user: Union[User, int], check_perun_admin=True, fill_facility_rp_id=True
     ) -> List[Facility]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             if check_perun_admin and self.is_user_perun_admin(user):
                 return self.get_all_facilities(fill_facility_rp_id)
             facilities_api_instance = FacilitiesManagerApi(api_client)
-            facilities = facilities_api_instance.get_facilities_where_user_is_admin(
-                AdapterInterface.get_object_id(user)
+            facilities = self._call_api(
+                facilities_api_instance.get_facilities_where_user_is_admin,
+                {"user": AdapterInterface.get_object_id(user)},
             )
             return [
                 Facility(
                     facility.id,
                     facility.name,
                     facility.description,
                     self._get_rp_id(facility.id) if fill_facility_rp_id else "",
@@ -816,61 +885,62 @@
                 )
                 for facility in facilities
             ]
 
     def get_resources_where_user_is_admin(
         self, user: Union[User, int], check_perun_admin=True, fill_facility_rp_id=True
     ) -> List[Resource]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             resources_api_instance = ResourcesManagerApi(api_client)
             facilities = self.get_all_facilities(fill_facility_rp_id)
             vos = self.get_all_vos()
             if check_perun_admin and self.is_user_perun_admin(user):
                 result = []
                 for vo in vos:
-                    resources = resources_api_instance.get_resources(vo.id)
+                    resources = self._call_api(
+                        resources_api_instance.get_resources, {"vo": vo.id}
+                    )
                     result.extend(
                         [
                             Resource(
                                 resource.id,
                                 vo,
-                                self.__find_facility_in_list_by_id(
+                                self._find_facility_in_list_by_id(
                                     facilities, resource.facility_id
                                 ),
                                 resource.name,
                             )
                             for resource in resources
                         ]
                     )
                 return result
-            resources = resources_api_instance.get_all_resources_where_user_is_admin(
-                AdapterInterface.get_object_id(user)
+            resources = self._call_api(
+                resources_api_instance.get_all_resources_where_user_is_admin,
+                {"user": AdapterInterface.get_object_id(user)},
             )
             return [
                 Resource(
                     resource.id,
-                    self.__find_vo_in_list_by_id(vos, resource.vo_id),
-                    self.__find_facility_in_list_by_id(
-                        facilities, resource.facility_id
-                    ),
+                    self._find_vo_in_list_by_id(vos, resource.vo_id),
+                    self._find_facility_in_list_by_id(facilities, resource.facility_id),
                     resource.name,
                 )
                 for resource in resources
             ]
 
     def get_all_vos(self) -> List[VO]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             vos_api_instance = VosManagerApi(api_client)
-            vos = vos_api_instance.get_all_vos()
+            vos = self._call_api(vos_api_instance.get_all_vos, {})
             return [VO(vo.id, vo.name, vo.short_name) for vo in vos]
 
     def get_all_facilities(self, fill_rp_ids=True) -> List[Facility]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             facilities_api_instance = FacilitiesManagerApi(api_client)
-            facilities = facilities_api_instance.get_all_facilities()
+            facilities = self._call_api(facilities_api_instance.get_all_facilities, {})
             return [
                 Facility(
                     facility.id,
                     facility.name,
                     facility.description,
                     "" if not fill_rp_ids else self._get_rp_id(facility.id),
                     {},
@@ -880,15 +950,15 @@
 
     def get_groups_where_user_is_active_resource(
         self,
         user: Union[User, int],
         resource: Union[Resource, int],
         map_unique_name=True,
     ) -> List[Group]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             if isinstance(resource, Resource):
                 vo = resource.vo
                 resource_id = resource.id
             else:
                 perun_vo = ResourcesManagerApi(api_client).get_vo(resource)
                 vo = VO(perun_vo.id, perun_vo.name, perun_vo.short_name)
                 resource_id = resource
@@ -903,37 +973,40 @@
                 result,
                 AttributesManagerApi(api_client) if map_unique_name else "",
                 vo=vo,
             )
             return result
 
     def get_facility_by_id(self, facility_id: int) -> Facility:
-        with ApiClient(self._CONFIG) as api_client:
-            facility = FacilitiesManagerApi(api_client).get_facility_by_id(facility_id)
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
+            facility = self._call_api(
+                FacilitiesManagerApi(api_client).get_facility_by_id, {"id": facility_id}
+            )
             return Facility(
                 facility_id,
                 facility.name,
                 facility.description,
                 self._get_rp_id(facility_id),
                 {},
             )
 
     def get_resources_for_facility(
         self, facility: Union[Facility, int], map_vo=True
     ) -> List[Resource]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             if isinstance(facility, Facility):
                 facility_id = facility.id
             else:
                 facility_id = facility
                 facility = self.get_facility_by_id(facility)
 
-            resources = FacilitiesManagerApi(
-                api_client
-            ).get_assigned_resources_for_facility(facility_id)
+            resources = self._call_api(
+                FacilitiesManagerApi(api_client).get_assigned_resources_for_facility,
+                {"facility": facility_id},
+            )
             return [
                 Resource(
                     resource.id,
                     self.get_vo(vo_id=resource.vo_id)
                     if map_vo
                     else VO(resource.vo_id, "", ""),
                     facility,
@@ -941,35 +1014,40 @@
                 )
                 for resource in resources
             ]
 
     def get_groups_for_resource(
         self, resource: Union[Resource, int], map_unique_name=True
     ) -> List[Group]:
-        with ApiClient(self._CONFIG) as api_client:
-            if isinstance(resource, Facility):
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
+            if isinstance(resource, Resource):
                 resource_id = resource.id
             else:
                 resource_id = resource
-                resource = self.get_resource_by_id(resource)
-            groups = ResourcesManagerApi(api_client).get_assigned_groups(resource_id)
+                resource = self.get_resource_by_id(resource_id)
+            groups = self._call_api(
+                ResourcesManagerApi(api_client).get_assigned_groups,
+                {"resource": resource_id},
+            )
             result = []
             self._create_internal_representation_groups(
                 groups,
                 result,
                 AttributesManagerApi(api_client) if map_unique_name else "",
                 vo=resource.vo,
             )
             return result
 
     def get_resource_by_id(
         self, resource_id: int, map_vo=True, map_facility=True
     ) -> Resource:
-        with ApiClient(self._CONFIG) as api_client:
-            resource = ResourcesManagerApi(api_client).get_resource_by_id(resource_id)
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
+            resource = self._call_api(
+                ResourcesManagerApi(api_client).get_resource_by_id, {"id": resource_id}
+            )
             facility = (
                 self.get_facility_by_id(resource.facility_id)
                 if map_facility
                 else Facility(resource.facility_id, "", "", "", {})
             )
             vo = (
                 self.get_vo(vo_id=resource.vo_id)
@@ -977,29 +1055,31 @@
                 else VO(resource.vo_id, "", "")
             )
             return Resource(resource.id, vo, facility, resource.name)
 
     def get_all_parent_groups_for_group(
         self, group: Union[Group, int], map_unique_name=True
     ) -> List[Group]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             perun_parent_groups = []
-            perun_group = GroupsManagerApi(api_client).get_group_by_id(
-                self.get_object_id(group)
+            perun_group = self._call_api(
+                GroupsManagerApi(api_client).get_group_by_id,
+                {"id": self.get_object_id(group)},
             )
             if isinstance(group, Group):
                 vo = group.vo
             else:
                 vo = self.get_vo(vo_id=perun_group.vo_id)
             if not perun_group.parent_group_id:
                 return perun_parent_groups
 
             while perun_group.parent_group_id:
-                perun_group = GroupsManagerApi(api_client).get_parent_group(
-                    perun_group.id
+                perun_group = self._call_api(
+                    GroupsManagerApi(api_client).get_parent_group,
+                    {"group": perun_group.id},
                 )
                 perun_parent_groups.append(perun_group)
             result = []
             self._create_internal_representation_groups(
                 perun_parent_groups,
                 result,
                 AttributesManagerApi(api_client) if map_unique_name else "",
@@ -1009,22 +1089,27 @@
 
     def get_facilities_by_attribute_with_attributes(
         self,
         attr_name: str,
         attr_value: Union[str, int, bool, List[str], dict[str, str]],
         attr_names: List[str],
     ) -> List[Facility]:
-        with ApiClient(self._CONFIG) as api_client:
+        with ApiClient(self._CONFIG, cookie=self.cookie) as api_client:
             if self._RP_ID_ATTR not in attr_name:
                 attr_names.append(self._RP_ID_ATTR)
 
-            perun_facilities_attributes = FacilitiesManagerApi(
-                api_client
-            ).get_facilities_by_attribute_with_attributes(
-                attr_name, attr_value, attr_names
+            perun_facilities_attributes = self._call_api(
+                FacilitiesManagerApi(
+                    api_client
+                ).get_facilities_by_attribute_with_attributes,
+                {
+                    "attribute_name": attr_name,
+                    "attribute_value": attr_value,
+                    "attr_names": attr_names,
+                },
             )
 
             facilities = []
             for facility_attrs in perun_facilities_attributes:
                 perun_facility = facility_attrs["facility"]
                 attrs = self._get_attributes(facility_attrs["attributes"])
                 facilities.append(
@@ -1034,18 +1119,35 @@
                         perun_facility.description,
                         attrs[self._RP_ID_ATTR],
                         attrs,
                     )
                 )
             return facilities
 
+    def _save_cookie_to_file(self, filepath, cookie):
+        with open(filepath, "w") as file:
+            try:
+                file.write(cookie)
+            except OSError as e:
+                self._logger(
+                    f"Cannot write cookie to file: {filepath}, error: {e.strerror}"
+                )
+
     @staticmethod
-    def __find_vo_in_list_by_id(vo_list, vo_id):
+    def _find_vo_in_list_by_id(vo_list, vo_id):
         for vo in vo_list:
             if vo.id == vo_id:
                 return vo
 
     @staticmethod
-    def __find_facility_in_list_by_id(facility_list, facility_id):
+    def _find_facility_in_list_by_id(facility_list, facility_id):
         for facility in facility_list:
             if facility.id == facility_id:
                 return facility
+
+    @staticmethod
+    def _load_cookie_from_file(filepath):
+        try:
+            with open(filepath, "r") as f:
+                return f.read()
+        except OSError:
+            return None
```

### Comparing `perun.connector-3.5.0/perun/connector/connectors/LdapConnector.py` & `perun.connector-3.6.0/perun/connector/connectors/LdapConnector.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/models/Facility.py` & `perun.connector-3.6.0/perun/connector/models/Facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/models/Group.py` & `perun.connector-3.6.0/perun/connector/models/Group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/models/Member.py` & `perun.connector-3.6.0/perun/connector/models/Member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/models/Resource.py` & `perun.connector-3.6.0/perun/connector/models/Resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/models/UserExtSource.py` & `perun.connector-3.6.0/perun/connector/models/UserExtSource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/models/VO.py` & `perun.connector-3.6.0/perun/connector/models/VO.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/__init__.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/attributes_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/attributes_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/audit_messages_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/audit_messages_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/authz_resolver_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/authz_resolver_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/cabinet_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/cabinet_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/consents_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/consents_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/database_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/database_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/ext_sources_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/ext_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/facilities_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/facilities_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/groups_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/groups_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/integration_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/integration_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/members_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/members_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/owners_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/owners_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/registrar_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/registrar_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/resources_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/resources_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/rt_messages_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/rt_messages_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/searcher_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/searcher_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/services_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/services_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/tasks_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/tasks_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/users_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/users_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/utils_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api/vos_manager_api.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api/vos_manager_api.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/api_client.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/apis/__init__.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/configuration.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/exceptions.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/action_type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/action_type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/add_user_ext_source_input.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/add_user_ext_source_input.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/app_state.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/app_state.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/app_type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/app_type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/application.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/application.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/application_form.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/application_form.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/application_form_item.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/application_form_item.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/application_form_item_data.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/application_form_item_data.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/application_mail.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/application_mail.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/applications_order_column.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/applications_order_column.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/applications_page_query.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/applications_page_query.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/assigned_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/assigned_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/assigned_member.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/assigned_member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/assigned_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/assigned_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_action.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_action.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_definition.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_definition.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_policy.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_policy.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_policy_collection.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_policy_collection.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_rights.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_rights.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/attribute_rules.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/attribute_rules.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/audit_event.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/audit_event.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/audit_message.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/audit_message.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/audit_messages_page_query.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/audit_messages_page_query.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/auditable.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/auditable.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/author.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/author.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/authorship.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/authorship.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/authz_roles.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/authz_roles.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/ban.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/ban.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/ban_on_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/ban_on_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/ban_on_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/ban_on_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/ban_on_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/ban_on_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/brand.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/brand.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/candidate.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/candidate.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/category.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/category.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/consent.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/consent.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/consent_hub.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/consent_hub.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/consent_status.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/consent_status.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/destination.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/destination.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/destination_propagation_type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/destination_propagation_type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/destination_type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/destination_type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ban_on_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ban_on_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ban_on_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ban_on_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ban_on_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ban_on_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_ext_source.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_ext_source.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_host.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_host.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_identity.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_identity.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/enriched_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/enriched_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/entityless_attributes_by_keys.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/entityless_attributes_by_keys.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/ext_source.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/ext_source.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/ext_source_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/ext_source_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/facility_propagation_state.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/facility_propagation_state.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/facility_state.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/facility_state.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/facility_with_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/facility_with_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/gen_data_node.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/gen_data_node.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/gen_member_data_node.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/gen_member_data_node.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/graph_dto.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/graph_dto.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/graph_file_format.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/graph_file_format.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/group_member_data.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/group_member_data.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/group_member_relation.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/group_member_relation.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/group_resource_status.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/group_resource_status.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/groups_order_column.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/groups_order_column.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/groups_page_query.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/groups_page_query.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/hashed_gen_data.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/hashed_gen_data.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/host.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/host.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/identity.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/identity.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_application_mail_for_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_application_mail_for_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_application_mail_for_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_application_mail_for_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_destination_to_multiple_services.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_destination_to_multiple_services.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_destinations_defined_by_hosts_on_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_destinations_defined_by_hosts_on_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_add_member_candidates.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_add_member_candidates.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_assign_resource_tag_to_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_assign_resource_tag_to_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_assign_resource_tags_to_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_assign_resource_tags_to_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_attribute_definition.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_attribute_policy_collections.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_attribute_policy_collections.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_attribute_rights.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_attribute_rights.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_block_services_on_destinations.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_block_services_on_destinations.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_change_non_authz_password_by_token.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_change_non_authz_password_by_token.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_change_password_for_login.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_change_password_for_login.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_change_password_for_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_change_password_for_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_check_password_strength.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_check_password_strength.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_consolidate.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_consolidate.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_copy_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_copy_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_alternative_password.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_alternative_password.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_attribute_definition.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_authorship.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_authorship.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_category.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_category.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_category_nr.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_category_nr.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_member_for_candidate.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_member_for_candidate.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_member_for_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_member_for_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_member_from_ext_source.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_member_from_ext_source.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_owner.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_owner.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_publication.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_publication.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_publication_system.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_publication_system.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_resource_tag_with_resource_tag.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_resource_tag_with_resource_tag.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_service.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_service.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_service_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_service_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_services_package.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_services_package.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_sponsored_member.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_sponsored_member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_sponsored_member_from_csv.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_sponsored_member_from_csv.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_sponsored_members.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_sponsored_members.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_thanks.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_thanks.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_create_vo_with_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_create_vo_with_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_delete_groups.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_delete_groups.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_delete_resource_tag.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_delete_resource_tag.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_entityless_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_entityless_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_form_item_data.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_form_item_data.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_form_items_data.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_form_items_data.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_all_resources_by_resource_tag.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_all_resources_by_resource_tag.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_facilities.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_facilities.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_match_resources.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_match_resources.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_members_by_user_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_members_by_user_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_messages_page.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_messages_page.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_applications.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_applications.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_groups.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_groups.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_members.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_members.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_subgroups.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_subgroups.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_paginated_users.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_paginated_users.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_resources.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_resources.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_get_users.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_get_users.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_invitations_from_csv.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_invitations_from_csv.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_invite_member_candidates.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_invite_member_candidates.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_lock_publications.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_lock_publications.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_remove_resource_tag_from_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_remove_resource_tag_from_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_remove_resource_tags_from_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_remove_resource_tags_from_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_remove_rich_destinations.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_remove_rich_destinations.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_reserve_password_for_login.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_reserve_password_for_login.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_reserve_password_for_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_reserve_password_for_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_send_message.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_send_message.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_ban.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_ban.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_ban_for_user_on_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_ban_for_user_on_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_resource_group_user_member_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_resource_group_user_member_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_resource_user_member_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_resource_user_member_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_facility_user_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_facility_user_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_resource_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_group_resource_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_group_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_host_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_host_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_host_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_host_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_group_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_group_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_group_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_group_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_group_with_user_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_group_with_user_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_resource_and_user_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_resource_and_user_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_resource_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_resource_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_member_with_user_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_member_with_user_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_group_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_group_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_resource_group_with_group_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_resource_group_with_group_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_sending_enabled.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_sending_enabled.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_sponsored_member.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_sponsored_member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_ext_source_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_facility_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_facility_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_user_facility_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_user_facility_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_vo_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_vo_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_vo_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_vo_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_set_vo_ban.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_set_vo_ban.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_specific_member.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_specific_member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_submit_application.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_submit_application.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_unlock_services_on_destinations.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_unlock_services_on_destinations.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_application_mail.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_application_mail.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_ban.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_ban.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_ban1.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_ban1.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_ban_for_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_ban_for_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_category.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_category.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_consent_hub.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_consent_hub.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_form.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_form.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_form_items_for_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_form_items_for_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_form_items_for_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_form_items_for_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_publication.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_publication.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_publication_system.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_publication_system.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_resource_tag.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_resource_tag.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_service.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_service.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_services_package.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_services_package.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/input_update_vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/input_update_vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/item_texts.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/item_texts.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/mail_text.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/mail_text.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/mail_type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/mail_type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/member.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/member_candidate.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/member_candidate.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/member_group_status.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/member_group_status.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/member_with_sponsors.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/member_with_sponsors.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/members_order_column.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/members_order_column.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/members_page_query.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/members_page_query.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/namespace_rules.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/namespace_rules.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/new_apps.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/new_apps.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/owner.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/owner.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/owner_type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/owner_type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_audit_messages.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_audit_messages.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_applications.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_applications.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_groups.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_groups.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_members.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_members.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/paginated_rich_users.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/paginated_rich_users.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_apps_config.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_apps_config.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_bean.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_bean.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_exception.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_exception.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_policy.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_policy.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/perun_principal.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/perun_principal.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/publication.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/publication.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/publication_for_gui.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/publication_for_gui.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/publication_system.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/publication_system.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/resource_state.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/resource_state.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/resource_tag.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/resource_tag.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_application.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_application.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_destination.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_destination.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_facility.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_facility.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_member.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_member.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_resource.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_resource.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rich_user_ext_source.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rich_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/role_management_rules.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/role_management_rules.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/role_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/role_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/rt_message.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/rt_message.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/security_team.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/security_team.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/service.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/service.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/service_attributes.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/service_attributes.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/service_for_gui.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/service_for_gui.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/service_state.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/service_state.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/services_package.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/services_package.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_for_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_for_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_for_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_for_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_objects.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_group_complementary_objects.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_objects.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/set_role_with_user_complementary_objects.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/simple_attribute.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/simple_attribute.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/sorting_order.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/sorting_order.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/sponsor.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/sponsor.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/sponsored_user_data.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/sponsored_user_data.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_and_destination_id_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_and_destination_id_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_and_destination_name_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_and_destination_name_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_id_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_id_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_result.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_result.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_result_id_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_result_id_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_result_status.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_result_status.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/task_status.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/task_status.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/thanks.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/thanks.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/thanks_for_gui.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/thanks_for_gui.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/type.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/type.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_for_group.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_for_group.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_for_user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_for_user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_objects.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_group_complementary_objects.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_object.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_object.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_objects.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/unset_role_with_user_complementary_objects.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/user.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/user.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/user_ext_source.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/user_ext_source.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/users_order_column.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/users_order_column.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/users_page_query.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/users_page_query.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/vo.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/vo.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/vo_admin_roles.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/vo_admin_roles.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model/vo_member_statuses.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model/vo_member_statuses.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/model_utils.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/models/__init__.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/perun_openapi/rest.py` & `perun.connector-3.6.0/perun/connector/perun_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/utils/AttributeUtils.py` & `perun.connector-3.6.0/perun/connector/utils/AttributeUtils.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun/connector/utils/ConfigStore.py` & `perun.connector-3.6.0/perun/connector/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/perun.connector.egg-info/SOURCES.txt` & `perun.connector-3.6.0/perun.connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.connector-3.5.0/setup.py` & `perun.connector-3.6.0/setup.py`

 * *Files identical despite different names*

