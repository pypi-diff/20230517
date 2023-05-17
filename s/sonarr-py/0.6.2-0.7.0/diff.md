# Comparing `tmp/sonarr-py-0.6.2.tar.gz` & `tmp/sonarr-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonarr-py-0.6.2.tar", last modified: Mon Mar 27 14:23:44 2023, max compression
+gzip compressed data, was "sonarr-py-0.7.0.tar", last modified: Wed May 17 06:52:10 2023, max compression
```

## Comparing `sonarr-py-0.6.2.tar` & `sonarr-py-0.7.0.tar`

### file list

```diff
@@ -1,209 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:44.657568 sonarr-py-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-03-27 14:23:44.657568 sonarr-py-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37911 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:23:44.657568 sonarr-py-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:44.605566 sonarr-py-0.6.2/sonarr/
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:44.621566 sonarr-py-0.6.2/sonarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/auto_tagging_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23355 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30322 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53633 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/episode_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43090 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/episode_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52961 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31059 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52336 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/language_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/language_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52504 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32136 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53176 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25201 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26584 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30902 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/rename_episode_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/season_pass_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/series_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/series_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/series_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29393 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29525 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:44.657568 sonarr-py-0.6.2/sonarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/add_series_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/alternate_title_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/authentication_required_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/auto_tagging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/auto_tagging_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episode_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episode_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episode_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episode_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episode_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episode_title_required_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/episodes_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/language_profile_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/language_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/localization_language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/localization_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/manual_import_reprocess_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/parsed_episode_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/privacy_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/quality_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/rename_episode_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/season_pass_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/season_pass_series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/season_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/season_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/series_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/series_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/series_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/series_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/series_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/unmapped_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-03-27 14:23:31.000000 sonarr-py-0.6.2/sonarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:23:44.657568 sonarr-py-0.6.2/sonarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-03-27 14:23:44.000000 sonarr-py-0.6.2/sonarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-03-27 14:23:44.000000 sonarr-py-0.6.2/sonarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:23:44.000000 sonarr-py-0.6.2/sonarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 14:23:44.000000 sonarr-py-0.6.2/sonarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 14:23:44.000000 sonarr-py-0.6.2/sonarr_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    38463 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38013 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.256320 sonarr-py-0.7.0/sonarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.264320 sonarr-py-0.7.0/sonarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/auto_tagging_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23355 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30322 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53633 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/episode_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43090 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/episode_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52961 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31059 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52336 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/language_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/language_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52504 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32710 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53176 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25201 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26584 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30902 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/rename_episode_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/season_pass_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31995 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29393 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/sonarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/add_series_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/alternate_title_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/authentication_required_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/auto_tagging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/auto_tagging_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_title_required_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episodes_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language_profile_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/localization_language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/localization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/manual_import_reprocess_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/parsed_episode_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/privacy_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/release_episode_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rename_episode_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_pass_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_pass_series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/unmapped_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/sonarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38463 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/top_level.txt
```

### Comparing `sonarr-py-0.6.2/PKG-INFO` & `sonarr-py-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonarr-py
-Version: 0.6.2
+Version: 0.7.0
 Summary: Sonarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/sonarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/sonarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,15 +12,15 @@
 
 # sonarr-py
 Sonarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.6.2
+- Package version: 0.7.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -352,14 +352,15 @@
  - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
  - [BlocklistResource](docs/BlocklistResource.md)
  - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
@@ -424,14 +425,15 @@
  - [QueueBulkResource](docs/QueueBulkResource.md)
  - [QueueResource](docs/QueueResource.md)
  - [QueueResourcePagingResource](docs/QueueResourcePagingResource.md)
  - [QueueStatusResource](docs/QueueStatusResource.md)
  - [Ratings](docs/Ratings.md)
  - [Rejection](docs/Rejection.md)
  - [RejectionType](docs/RejectionType.md)
+ - [ReleaseEpisodeResource](docs/ReleaseEpisodeResource.md)
  - [ReleaseProfileResource](docs/ReleaseProfileResource.md)
  - [ReleaseResource](docs/ReleaseResource.md)
  - [RemotePathMappingResource](docs/RemotePathMappingResource.md)
  - [RenameEpisodeResource](docs/RenameEpisodeResource.md)
  - [RescanAfterRefreshType](docs/RescanAfterRefreshType.md)
  - [Revision](docs/Revision.md)
  - [RootFolderResource](docs/RootFolderResource.md)
```

### Comparing `sonarr-py-0.6.2/README.md` & `sonarr-py-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # sonarr-py
 Sonarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.6.2
+- Package version: 0.7.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -340,14 +340,15 @@
  - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
  - [BlocklistResource](docs/BlocklistResource.md)
  - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
@@ -412,14 +413,15 @@
  - [QueueBulkResource](docs/QueueBulkResource.md)
  - [QueueResource](docs/QueueResource.md)
  - [QueueResourcePagingResource](docs/QueueResourcePagingResource.md)
  - [QueueStatusResource](docs/QueueStatusResource.md)
  - [Ratings](docs/Ratings.md)
  - [Rejection](docs/Rejection.md)
  - [RejectionType](docs/RejectionType.md)
+ - [ReleaseEpisodeResource](docs/ReleaseEpisodeResource.md)
  - [ReleaseProfileResource](docs/ReleaseProfileResource.md)
  - [ReleaseResource](docs/ReleaseResource.md)
  - [RemotePathMappingResource](docs/RemotePathMappingResource.md)
  - [RenameEpisodeResource](docs/RenameEpisodeResource.md)
  - [RescanAfterRefreshType](docs/RescanAfterRefreshType.md)
  - [Revision](docs/Revision.md)
  - [RootFolderResource](docs/RootFolderResource.md)
```

### Comparing `sonarr-py-0.6.2/pyproject.toml` & `sonarr-py-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 [project]
 name = "sonarr-py"
-version = "0.6.2"
+version = "0.7.0"
 dependencies = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
     "pydantic>=1.10.2",
     "aenum"
 ]
```

### Comparing `sonarr-py-0.6.2/sonarr/__init__.py` & `sonarr-py-0.7.0/sonarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 # x-release-please-end
 
 # import apis into sdk package
 from sonarr.api.api_info_api import ApiInfoApi
 from sonarr.api.authentication_api import AuthenticationApi
 from sonarr.api.auto_tagging_api import AutoTaggingApi
 from sonarr.api.backup_api import BackupApi
@@ -109,14 +109,15 @@
 from sonarr.models.blocklist_bulk_resource import BlocklistBulkResource
 from sonarr.models.blocklist_resource import BlocklistResource
 from sonarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 from sonarr.models.certificate_validation_type import CertificateValidationType
 from sonarr.models.command import Command
 from sonarr.models.command_priority import CommandPriority
 from sonarr.models.command_resource import CommandResource
+from sonarr.models.command_result import CommandResult
 from sonarr.models.command_status import CommandStatus
 from sonarr.models.command_trigger import CommandTrigger
 from sonarr.models.custom_filter_resource import CustomFilterResource
 from sonarr.models.custom_format_resource import CustomFormatResource
 from sonarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from sonarr.models.delay_profile_resource import DelayProfileResource
 from sonarr.models.disk_space_resource import DiskSpaceResource
@@ -181,14 +182,15 @@
 from sonarr.models.queue_bulk_resource import QueueBulkResource
 from sonarr.models.queue_resource import QueueResource
 from sonarr.models.queue_resource_paging_resource import QueueResourcePagingResource
 from sonarr.models.queue_status_resource import QueueStatusResource
 from sonarr.models.ratings import Ratings
 from sonarr.models.rejection import Rejection
 from sonarr.models.rejection_type import RejectionType
+from sonarr.models.release_episode_resource import ReleaseEpisodeResource
 from sonarr.models.release_profile_resource import ReleaseProfileResource
 from sonarr.models.release_resource import ReleaseResource
 from sonarr.models.remote_path_mapping_resource import RemotePathMappingResource
 from sonarr.models.rename_episode_resource import RenameEpisodeResource
 from sonarr.models.rescan_after_refresh_type import RescanAfterRefreshType
 from sonarr.models.revision import Revision
 from sonarr.models.root_folder_resource import RootFolderResource
```

### Comparing `sonarr-py-0.6.2/sonarr/api/__init__.py` & `sonarr-py-0.7.0/sonarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/api_info_api.py` & `sonarr-py-0.7.0/sonarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/authentication_api.py` & `sonarr-py-0.7.0/sonarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/auto_tagging_api.py` & `sonarr-py-0.7.0/sonarr/api/auto_tagging_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/backup_api.py` & `sonarr-py-0.7.0/sonarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/blocklist_api.py` & `sonarr-py-0.7.0/sonarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/calendar_api.py` & `sonarr-py-0.7.0/sonarr/api/calendar_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from datetime import datetime
 
-from pydantic import StrictBool, StrictInt
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from sonarr.models.episode_resource import EpisodeResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
@@ -182,35 +182,37 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_calendar(self, start : Optional[datetime] = None, end : Optional[datetime] = None, unmonitored : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode_file : Optional[StrictBool] = None, include_episode_images : Optional[StrictBool] = None, **kwargs) -> List[EpisodeResource]:  # noqa: E501
+    def list_calendar(self, start : Optional[datetime] = None, end : Optional[datetime] = None, unmonitored : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode_file : Optional[StrictBool] = None, include_episode_images : Optional[StrictBool] = None, tags : Optional[StrictStr] = None, **kwargs) -> List[EpisodeResource]:  # noqa: E501
         """list_calendar  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_calendar(start, end, unmonitored, include_series, include_episode_file, include_episode_images, async_req=True)
+        >>> thread = api.list_calendar(start, end, unmonitored, include_series, include_episode_file, include_episode_images, tags, async_req=True)
         >>> result = thread.get()
 
         :param start:
         :type start: datetime
         :param end:
         :type end: datetime
         :param unmonitored:
         :type unmonitored: bool
         :param include_series:
         :type include_series: bool
         :param include_episode_file:
         :type include_episode_file: bool
         :param include_episode_images:
         :type include_episode_images: bool
+        :param tags:
+        :type tags: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -219,38 +221,40 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[EpisodeResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_calendar_with_http_info(start, end, unmonitored, include_series, include_episode_file, include_episode_images, **kwargs)  # noqa: E501
+        return self.list_calendar_with_http_info(start, end, unmonitored, include_series, include_episode_file, include_episode_images, tags, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_calendar_with_http_info(self, start : Optional[datetime] = None, end : Optional[datetime] = None, unmonitored : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode_file : Optional[StrictBool] = None, include_episode_images : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def list_calendar_with_http_info(self, start : Optional[datetime] = None, end : Optional[datetime] = None, unmonitored : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode_file : Optional[StrictBool] = None, include_episode_images : Optional[StrictBool] = None, tags : Optional[StrictStr] = None, **kwargs):  # noqa: E501
         """list_calendar  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_calendar_with_http_info(start, end, unmonitored, include_series, include_episode_file, include_episode_images, async_req=True)
+        >>> thread = api.list_calendar_with_http_info(start, end, unmonitored, include_series, include_episode_file, include_episode_images, tags, async_req=True)
         >>> result = thread.get()
 
         :param start:
         :type start: datetime
         :param end:
         :type end: datetime
         :param unmonitored:
         :type unmonitored: bool
         :param include_series:
         :type include_series: bool
         :param include_episode_file:
         :type include_episode_file: bool
         :param include_episode_images:
         :type include_episode_images: bool
+        :param tags:
+        :type tags: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -275,15 +279,16 @@
 
         _all_params = [
             'start',
             'end',
             'unmonitored',
             'include_series',
             'include_episode_file',
-            'include_episode_images'
+            'include_episode_images',
+            'tags'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -318,14 +323,16 @@
             _query_params.append(('unmonitored', _params['unmonitored']))
         if _params.get('include_series') is not None:  # noqa: E501
             _query_params.append(('includeSeries', _params['include_series']))
         if _params.get('include_episode_file') is not None:  # noqa: E501
             _query_params.append(('includeEpisodeFile', _params['include_episode_file']))
         if _params.get('include_episode_images') is not None:  # noqa: E501
             _query_params.append(('includeEpisodeImages', _params['include_episode_images']))
+        if _params.get('tags') is not None:  # noqa: E501
+            _query_params.append(('tags', _params['tags']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `sonarr-py-0.6.2/sonarr/api/calendar_feed_api.py` & `sonarr-py-0.7.0/sonarr/api/calendar_feed_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,29 +38,29 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_feed_v3_calendar_sonarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, premieres_only : Optional[StrictBool] = None, as_all_day : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+    def get_feed_v3_calendar_sonarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tags : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, premieres_only : Optional[StrictBool] = None, as_all_day : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """get_feed_v3_calendar_sonarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_feed_v3_calendar_sonarr_ics(past_days, future_days, tag_list, unmonitored, premieres_only, as_all_day, async_req=True)
+        >>> thread = api.get_feed_v3_calendar_sonarr_ics(past_days, future_days, tags, unmonitored, premieres_only, as_all_day, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
-        :param tag_list:
-        :type tag_list: str
+        :param tags:
+        :type tags: str
         :param unmonitored:
         :type unmonitored: bool
         :param premieres_only:
         :type premieres_only: bool
         :param as_all_day:
         :type as_all_day: bool
         :param async_req: Whether to execute the request asynchronously.
@@ -75,32 +75,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_feed_v3_calendar_sonarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, premieres_only, as_all_day, **kwargs)  # noqa: E501
+        return self.get_feed_v3_calendar_sonarr_ics_with_http_info(past_days, future_days, tags, unmonitored, premieres_only, as_all_day, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_feed_v3_calendar_sonarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, premieres_only : Optional[StrictBool] = None, as_all_day : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def get_feed_v3_calendar_sonarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tags : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, premieres_only : Optional[StrictBool] = None, as_all_day : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """get_feed_v3_calendar_sonarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_feed_v3_calendar_sonarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, premieres_only, as_all_day, async_req=True)
+        >>> thread = api.get_feed_v3_calendar_sonarr_ics_with_http_info(past_days, future_days, tags, unmonitored, premieres_only, as_all_day, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
-        :param tag_list:
-        :type tag_list: str
+        :param tags:
+        :type tags: str
         :param unmonitored:
         :type unmonitored: bool
         :param premieres_only:
         :type premieres_only: bool
         :param as_all_day:
         :type as_all_day: bool
         :param async_req: Whether to execute the request asynchronously.
@@ -128,15 +128,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'past_days',
             'future_days',
-            'tag_list',
+            'tags',
             'unmonitored',
             'premieres_only',
             'as_all_day'
         ]
         _all_params.extend(
             [
                 'async_req',
@@ -166,16 +166,16 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('past_days') is not None:  # noqa: E501
             _query_params.append(('pastDays', _params['past_days']))
         if _params.get('future_days') is not None:  # noqa: E501
             _query_params.append(('futureDays', _params['future_days']))
-        if _params.get('tag_list') is not None:  # noqa: E501
-            _query_params.append(('tagList', _params['tag_list']))
+        if _params.get('tags') is not None:  # noqa: E501
+            _query_params.append(('tags', _params['tags']))
         if _params.get('unmonitored') is not None:  # noqa: E501
             _query_params.append(('unmonitored', _params['unmonitored']))
         if _params.get('premieres_only') is not None:  # noqa: E501
             _query_params.append(('premieresOnly', _params['premieres_only']))
         if _params.get('as_all_day') is not None:  # noqa: E501
             _query_params.append(('asAllDay', _params['as_all_day']))
```

### Comparing `sonarr-py-0.6.2/sonarr/api/command_api.py` & `sonarr-py-0.7.0/sonarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/custom_filter_api.py` & `sonarr-py-0.7.0/sonarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/custom_format_api.py` & `sonarr-py-0.7.0/sonarr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/cutoff_api.py` & `sonarr-py-0.7.0/sonarr/api/cutoff_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/delay_profile_api.py` & `sonarr-py-0.7.0/sonarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/disk_space_api.py` & `sonarr-py-0.7.0/sonarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/download_client_api.py` & `sonarr-py-0.7.0/sonarr/api/download_client_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/download_client_config_api.py` & `sonarr-py-0.7.0/sonarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/episode_api.py` & `sonarr-py-0.7.0/sonarr/api/episode_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -351,23 +351,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def put_episode_monitor(self, episodes_monitored_resource : Optional[EpisodesMonitoredResource] = None, **kwargs) -> None:  # noqa: E501
+    def put_episode_monitor(self, include_images : Optional[StrictBool] = None, episodes_monitored_resource : Optional[EpisodesMonitoredResource] = None, **kwargs) -> None:  # noqa: E501
         """put_episode_monitor  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_episode_monitor(episodes_monitored_resource, async_req=True)
+        >>> thread = api.put_episode_monitor(include_images, episodes_monitored_resource, async_req=True)
         >>> result = thread.get()
 
+        :param include_images:
+        :type include_images: bool
         :param episodes_monitored_resource:
         :type episodes_monitored_resource: EpisodesMonitoredResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -378,26 +380,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.put_episode_monitor_with_http_info(episodes_monitored_resource, **kwargs)  # noqa: E501
+        return self.put_episode_monitor_with_http_info(include_images, episodes_monitored_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def put_episode_monitor_with_http_info(self, episodes_monitored_resource : Optional[EpisodesMonitoredResource] = None, **kwargs):  # noqa: E501
+    def put_episode_monitor_with_http_info(self, include_images : Optional[StrictBool] = None, episodes_monitored_resource : Optional[EpisodesMonitoredResource] = None, **kwargs):  # noqa: E501
         """put_episode_monitor  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_episode_monitor_with_http_info(episodes_monitored_resource, async_req=True)
+        >>> thread = api.put_episode_monitor_with_http_info(include_images, episodes_monitored_resource, async_req=True)
         >>> result = thread.get()
 
+        :param include_images:
+        :type include_images: bool
         :param episodes_monitored_resource:
         :type episodes_monitored_resource: EpisodesMonitoredResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -419,14 +423,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
+            'include_images',
             'episodes_monitored_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -450,14 +455,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('include_images') is not None:  # noqa: E501
+            _query_params.append(('includeImages', _params['include_images']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `sonarr-py-0.6.2/sonarr/api/episode_file_api.py` & `sonarr-py-0.7.0/sonarr/api/episode_file_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/file_system_api.py` & `sonarr-py-0.7.0/sonarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/health_api.py` & `sonarr-py-0.7.0/sonarr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/history_api.py` & `sonarr-py-0.7.0/sonarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/host_config_api.py` & `sonarr-py-0.7.0/sonarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/import_list_api.py` & `sonarr-py-0.7.0/sonarr/api/import_list_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/import_list_exclusion_api.py` & `sonarr-py-0.7.0/sonarr/api/import_list_exclusion_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/indexer_api.py` & `sonarr-py-0.7.0/sonarr/api/indexer_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/indexer_config_api.py` & `sonarr-py-0.7.0/sonarr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/initialize_js_api.py` & `sonarr-py-0.7.0/sonarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/language_api.py` & `sonarr-py-0.7.0/sonarr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/language_profile_api.py` & `sonarr-py-0.7.0/sonarr/api/language_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/language_profile_schema_api.py` & `sonarr-py-0.7.0/sonarr/api/language_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/localization_api.py` & `sonarr-py-0.7.0/sonarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/log_api.py` & `sonarr-py-0.7.0/sonarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/log_file_api.py` & `sonarr-py-0.7.0/sonarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/manual_import_api.py` & `sonarr-py-0.7.0/sonarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/media_cover_api.py` & `sonarr-py-0.7.0/sonarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/media_management_config_api.py` & `sonarr-py-0.7.0/sonarr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/metadata_api.py` & `sonarr-py-0.7.0/sonarr/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/missing_api.py` & `sonarr-py-0.7.0/sonarr/api/missing_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/naming_config_api.py` & `sonarr-py-0.7.0/sonarr/api/naming_config_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -314,27 +314,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_naming_config_examples(self, rename_episodes : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, multi_episode_style : Optional[StrictInt] = None, standard_episode_format : Optional[StrictStr] = None, daily_episode_format : Optional[StrictStr] = None, anime_episode_format : Optional[StrictStr] = None, series_folder_format : Optional[StrictStr] = None, season_folder_format : Optional[StrictStr] = None, specials_folder_format : Optional[StrictStr] = None, include_series_title : Optional[StrictBool] = None, include_episode_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs) -> None:  # noqa: E501
+    def get_naming_config_examples(self, rename_episodes : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, colon_replacement_format : Optional[StrictInt] = None, multi_episode_style : Optional[StrictInt] = None, standard_episode_format : Optional[StrictStr] = None, daily_episode_format : Optional[StrictStr] = None, anime_episode_format : Optional[StrictStr] = None, series_folder_format : Optional[StrictStr] = None, season_folder_format : Optional[StrictStr] = None, specials_folder_format : Optional[StrictStr] = None, include_series_title : Optional[StrictBool] = None, include_episode_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs) -> None:  # noqa: E501
         """get_naming_config_examples  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_naming_config_examples(rename_episodes, replace_illegal_characters, multi_episode_style, standard_episode_format, daily_episode_format, anime_episode_format, series_folder_format, season_folder_format, specials_folder_format, include_series_title, include_episode_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
+        >>> thread = api.get_naming_config_examples(rename_episodes, replace_illegal_characters, colon_replacement_format, multi_episode_style, standard_episode_format, daily_episode_format, anime_episode_format, series_folder_format, season_folder_format, specials_folder_format, include_series_title, include_episode_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
         >>> result = thread.get()
 
         :param rename_episodes:
         :type rename_episodes: bool
         :param replace_illegal_characters:
         :type replace_illegal_characters: bool
+        :param colon_replacement_format:
+        :type colon_replacement_format: int
         :param multi_episode_style:
         :type multi_episode_style: int
         :param standard_episode_format:
         :type standard_episode_format: str
         :param daily_episode_format:
         :type daily_episode_format: str
         :param anime_episode_format:
@@ -373,30 +375,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_naming_config_examples_with_http_info(rename_episodes, replace_illegal_characters, multi_episode_style, standard_episode_format, daily_episode_format, anime_episode_format, series_folder_format, season_folder_format, specials_folder_format, include_series_title, include_episode_title, include_quality, replace_spaces, separator, number_style, id, resource_name, **kwargs)  # noqa: E501
+        return self.get_naming_config_examples_with_http_info(rename_episodes, replace_illegal_characters, colon_replacement_format, multi_episode_style, standard_episode_format, daily_episode_format, anime_episode_format, series_folder_format, season_folder_format, specials_folder_format, include_series_title, include_episode_title, include_quality, replace_spaces, separator, number_style, id, resource_name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_naming_config_examples_with_http_info(self, rename_episodes : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, multi_episode_style : Optional[StrictInt] = None, standard_episode_format : Optional[StrictStr] = None, daily_episode_format : Optional[StrictStr] = None, anime_episode_format : Optional[StrictStr] = None, series_folder_format : Optional[StrictStr] = None, season_folder_format : Optional[StrictStr] = None, specials_folder_format : Optional[StrictStr] = None, include_series_title : Optional[StrictBool] = None, include_episode_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def get_naming_config_examples_with_http_info(self, rename_episodes : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, colon_replacement_format : Optional[StrictInt] = None, multi_episode_style : Optional[StrictInt] = None, standard_episode_format : Optional[StrictStr] = None, daily_episode_format : Optional[StrictStr] = None, anime_episode_format : Optional[StrictStr] = None, series_folder_format : Optional[StrictStr] = None, season_folder_format : Optional[StrictStr] = None, specials_folder_format : Optional[StrictStr] = None, include_series_title : Optional[StrictBool] = None, include_episode_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs):  # noqa: E501
         """get_naming_config_examples  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_naming_config_examples_with_http_info(rename_episodes, replace_illegal_characters, multi_episode_style, standard_episode_format, daily_episode_format, anime_episode_format, series_folder_format, season_folder_format, specials_folder_format, include_series_title, include_episode_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
+        >>> thread = api.get_naming_config_examples_with_http_info(rename_episodes, replace_illegal_characters, colon_replacement_format, multi_episode_style, standard_episode_format, daily_episode_format, anime_episode_format, series_folder_format, season_folder_format, specials_folder_format, include_series_title, include_episode_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
         >>> result = thread.get()
 
         :param rename_episodes:
         :type rename_episodes: bool
         :param replace_illegal_characters:
         :type replace_illegal_characters: bool
+        :param colon_replacement_format:
+        :type colon_replacement_format: int
         :param multi_episode_style:
         :type multi_episode_style: int
         :param standard_episode_format:
         :type standard_episode_format: str
         :param daily_episode_format:
         :type daily_episode_format: str
         :param anime_episode_format:
@@ -448,14 +452,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'rename_episodes',
             'replace_illegal_characters',
+            'colon_replacement_format',
             'multi_episode_style',
             'standard_episode_format',
             'daily_episode_format',
             'anime_episode_format',
             'series_folder_format',
             'season_folder_format',
             'specials_folder_format',
@@ -497,14 +502,16 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('rename_episodes') is not None:  # noqa: E501
             _query_params.append(('RenameEpisodes', _params['rename_episodes']))
         if _params.get('replace_illegal_characters') is not None:  # noqa: E501
             _query_params.append(('ReplaceIllegalCharacters', _params['replace_illegal_characters']))
+        if _params.get('colon_replacement_format') is not None:  # noqa: E501
+            _query_params.append(('ColonReplacementFormat', _params['colon_replacement_format']))
         if _params.get('multi_episode_style') is not None:  # noqa: E501
             _query_params.append(('MultiEpisodeStyle', _params['multi_episode_style']))
         if _params.get('standard_episode_format') is not None:  # noqa: E501
             _query_params.append(('StandardEpisodeFormat', _params['standard_episode_format']))
         if _params.get('daily_episode_format') is not None:  # noqa: E501
             _query_params.append(('DailyEpisodeFormat', _params['daily_episode_format']))
         if _params.get('anime_episode_format') is not None:  # noqa: E501
```

### Comparing `sonarr-py-0.6.2/sonarr/api/notification_api.py` & `sonarr-py-0.7.0/sonarr/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/parse_api.py` & `sonarr-py-0.7.0/sonarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/ping_api.py` & `sonarr-py-0.7.0/sonarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/quality_definition_api.py` & `sonarr-py-0.7.0/sonarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/quality_profile_api.py` & `sonarr-py-0.7.0/sonarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/quality_profile_schema_api.py` & `sonarr-py-0.7.0/sonarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/queue_action_api.py` & `sonarr-py-0.7.0/sonarr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/queue_api.py` & `sonarr-py-0.7.0/sonarr/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/queue_details_api.py` & `sonarr-py-0.7.0/sonarr/api/queue_details_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/queue_status_api.py` & `sonarr-py-0.7.0/sonarr/api/queue_status_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/release_api.py` & `sonarr-py-0.7.0/sonarr/api/release_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/release_profile_api.py` & `sonarr-py-0.7.0/sonarr/api/release_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/release_push_api.py` & `sonarr-py-0.7.0/sonarr/api/release_push_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/remote_path_mapping_api.py` & `sonarr-py-0.7.0/sonarr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/rename_episode_api.py` & `sonarr-py-0.7.0/sonarr/api/rename_episode_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/root_folder_api.py` & `sonarr-py-0.7.0/sonarr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/season_pass_api.py` & `sonarr-py-0.7.0/sonarr/api/season_pass_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/series_api.py` & `sonarr-py-0.7.0/sonarr/api/series_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,25 +187,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_series(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_series(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_series  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_series(id, async_req=True)
+        >>> thread = api.delete_series(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -214,28 +218,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_series_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_series_with_http_info(id, delete_files, add_import_list_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_series_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_series_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_series  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_series_with_http_info(id, async_req=True)
+        >>> thread = api.delete_series_with_http_info(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -255,15 +263,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'delete_files',
+            'add_import_list_exclusion'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -288,14 +298,18 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('delete_files') is not None:  # noqa: E501
+            _query_params.append(('deleteFiles', _params['delete_files']))
+        if _params.get('add_import_list_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportListExclusion', _params['add_import_list_exclusion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -611,25 +625,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_series(self, id : StrictStr, series_resource : Optional[SeriesResource] = None, **kwargs) -> SeriesResource:  # noqa: E501
+    def update_series(self, id : StrictStr, move_files : Optional[StrictBool] = None, series_resource : Optional[SeriesResource] = None, **kwargs) -> SeriesResource:  # noqa: E501
         """update_series  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_series(id, series_resource, async_req=True)
+        >>> thread = api.update_series(id, move_files, series_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param series_resource:
         :type series_resource: SeriesResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -640,28 +656,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SeriesResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_series_with_http_info(id, series_resource, **kwargs)  # noqa: E501
+        return self.update_series_with_http_info(id, move_files, series_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_series_with_http_info(self, id : StrictStr, series_resource : Optional[SeriesResource] = None, **kwargs):  # noqa: E501
+    def update_series_with_http_info(self, id : StrictStr, move_files : Optional[StrictBool] = None, series_resource : Optional[SeriesResource] = None, **kwargs):  # noqa: E501
         """update_series  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_series_with_http_info(id, series_resource, async_req=True)
+        >>> thread = api.update_series_with_http_info(id, move_files, series_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param series_resource:
         :type series_resource: SeriesResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -684,14 +702,15 @@
         :rtype: tuple(SeriesResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'move_files',
             'series_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -717,14 +736,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('move_files') is not None:  # noqa: E501
+            _query_params.append(('moveFiles', _params['move_files']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `sonarr-py-0.6.2/sonarr/api/series_editor_api.py` & `sonarr-py-0.7.0/sonarr/api/series_editor_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/series_import_api.py` & `sonarr-py-0.7.0/sonarr/api/series_import_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/series_lookup_api.py` & `sonarr-py-0.7.0/sonarr/api/series_lookup_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/static_resource_api.py` & `sonarr-py-0.7.0/sonarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/system_api.py` & `sonarr-py-0.7.0/sonarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/tag_api.py` & `sonarr-py-0.7.0/sonarr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/tag_details_api.py` & `sonarr-py-0.7.0/sonarr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/task_api.py` & `sonarr-py-0.7.0/sonarr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/ui_config_api.py` & `sonarr-py-0.7.0/sonarr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/update_api.py` & `sonarr-py-0.7.0/sonarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api/update_log_file_api.py` & `sonarr-py-0.7.0/sonarr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/api_client.py` & `sonarr-py-0.7.0/sonarr/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'sonarr-py/v0.6.2'
+        self.user_agent = 'sonarr-py/v0.7.0'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -187,14 +187,18 @@
 
         # auth setting
         self.update_params_for_auth(
             header_params, query_params, auth_settings,
             resource_path, method, body,
             request_auth=_request_auth)
 
+        # request timeout
+        if not _request_timeout:
+            _request_timeout = config.request_timeout
+
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
```

### Comparing `sonarr-py-0.6.2/sonarr/configuration.py` & `sonarr-py-0.7.0/sonarr/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
       and data received from the server, independent of any validation performed by
       the server side. If the input data does not satisfy the JSON schema validation
       rules specified in the OpenAPI document, an exception is raised.
       If disabled_client_side_validations is set, structural validation is
       disabled. This can be useful to troubleshoot data validation problem, such as
       when the OpenAPI document validation rules do not match the actual API data
       received by the server.
+    :param request_timeout: Default request timeout.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
@@ -105,14 +106,15 @@
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
                  disabled_client_side_validations="",
+                 request_timeout=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
         self._base_path = "http://localhost:8989" if host is None else host
@@ -147,14 +149,17 @@
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
+        self.request_timeout = request_timeout
+        """Request Timeout
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("sonarr")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -421,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.6.2'
+        sdkversion = '0.7.0'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `sonarr-py-0.6.2/sonarr/exceptions.py` & `sonarr-py-0.7.0/sonarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/__init__.py` & `sonarr-py-0.7.0/sonarr/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from sonarr.models.blocklist_bulk_resource import BlocklistBulkResource
 from sonarr.models.blocklist_resource import BlocklistResource
 from sonarr.models.blocklist_resource_paging_resource import BlocklistResourcePagingResource
 from sonarr.models.certificate_validation_type import CertificateValidationType
 from sonarr.models.command import Command
 from sonarr.models.command_priority import CommandPriority
 from sonarr.models.command_resource import CommandResource
+from sonarr.models.command_result import CommandResult
 from sonarr.models.command_status import CommandStatus
 from sonarr.models.command_trigger import CommandTrigger
 from sonarr.models.custom_filter_resource import CustomFilterResource
 from sonarr.models.custom_format_resource import CustomFormatResource
 from sonarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from sonarr.models.delay_profile_resource import DelayProfileResource
 from sonarr.models.disk_space_resource import DiskSpaceResource
@@ -99,14 +100,15 @@
 from sonarr.models.queue_bulk_resource import QueueBulkResource
 from sonarr.models.queue_resource import QueueResource
 from sonarr.models.queue_resource_paging_resource import QueueResourcePagingResource
 from sonarr.models.queue_status_resource import QueueStatusResource
 from sonarr.models.ratings import Ratings
 from sonarr.models.rejection import Rejection
 from sonarr.models.rejection_type import RejectionType
+from sonarr.models.release_episode_resource import ReleaseEpisodeResource
 from sonarr.models.release_profile_resource import ReleaseProfileResource
 from sonarr.models.release_resource import ReleaseResource
 from sonarr.models.remote_path_mapping_resource import RemotePathMappingResource
 from sonarr.models.rename_episode_resource import RenameEpisodeResource
 from sonarr.models.rescan_after_refresh_type import RescanAfterRefreshType
 from sonarr.models.revision import Revision
 from sonarr.models.root_folder_resource import RootFolderResource
```

### Comparing `sonarr-py-0.6.2/sonarr/models/add_series_options.py` & `sonarr-py-0.7.0/sonarr/models/add_series_options.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/alternate_title_resource.py` & `sonarr-py-0.7.0/sonarr/models/alternate_title_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/apply_tags.py` & `sonarr-py-0.7.0/sonarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/authentication_required_type.py` & `sonarr-py-0.7.0/sonarr/models/authentication_required_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/authentication_type.py` & `sonarr-py-0.7.0/sonarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/auto_tagging_resource.py` & `sonarr-py-0.7.0/sonarr/models/auto_tagging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/auto_tagging_specification_schema.py` & `sonarr-py-0.7.0/sonarr/models/auto_tagging_specification_schema.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/backup_resource.py` & `sonarr-py-0.7.0/sonarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/backup_type.py` & `sonarr-py-0.7.0/sonarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/blocklist_bulk_resource.py` & `sonarr-py-0.7.0/sonarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/blocklist_resource.py` & `sonarr-py-0.7.0/sonarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/blocklist_resource_paging_resource.py` & `sonarr-py-0.7.0/sonarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/certificate_validation_type.py` & `sonarr-py-0.7.0/sonarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/command.py` & `sonarr-py-0.7.0/sonarr/models/command.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/command_priority.py` & `sonarr-py-0.7.0/sonarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/command_resource.py` & `sonarr-py-0.7.0/sonarr/models/command_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 from sonarr.models.command import Command
 from sonarr.models.command_priority import CommandPriority
+from sonarr.models.command_result import CommandResult
 from sonarr.models.command_status import CommandStatus
 from sonarr.models.command_trigger import CommandTrigger
 
 class CommandResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -33,26 +34,27 @@
     id: Optional[int]
     name: Optional[str]
     command_name: Optional[str]
     message: Optional[str]
     body: Optional[Command]
     priority: Optional[CommandPriority]
     status: Optional[CommandStatus]
+    result: Optional[CommandResult]
     queued: Optional[datetime]
     started: Optional[datetime]
     ended: Optional[datetime]
     duration: Optional[str]
     exception: Optional[str]
     trigger: Optional[CommandTrigger]
     client_user_agent: Optional[str]
     state_change_time: Optional[datetime]
     send_updates_to_client: Optional[bool]
     update_scheduled_task: Optional[bool]
     last_execution_time: Optional[datetime]
-    __properties = ["id", "name", "commandName", "message", "body", "priority", "status", "queued", "started", "ended", "duration", "exception", "trigger", "clientUserAgent", "stateChangeTime", "sendUpdatesToClient", "updateScheduledTask", "lastExecutionTime"]
+    __properties = ["id", "name", "commandName", "message", "body", "priority", "status", "result", "queued", "started", "ended", "duration", "exception", "trigger", "clientUserAgent", "stateChangeTime", "sendUpdatesToClient", "updateScheduledTask", "lastExecutionTime"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -131,14 +133,15 @@
             "id": obj.get("id"),
             "name": obj.get("name"),
             "command_name": obj.get("commandName"),
             "message": obj.get("message"),
             "body": Command.from_dict(obj.get("body")) if obj.get("body") is not None else None,
             "priority": obj.get("priority"),
             "status": obj.get("status"),
+            "result": obj.get("result"),
             "queued": obj.get("queued"),
             "started": obj.get("started"),
             "ended": obj.get("ended"),
             "duration": obj.get("duration"),
             "exception": obj.get("exception"),
             "trigger": obj.get("trigger"),
             "client_user_agent": obj.get("clientUserAgent"),
```

### Comparing `sonarr-py-0.6.2/sonarr/models/command_status.py` & `sonarr-py-0.7.0/sonarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/command_trigger.py` & `sonarr-py-0.7.0/sonarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/custom_filter_resource.py` & `sonarr-py-0.7.0/sonarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/custom_format_resource.py` & `sonarr-py-0.7.0/sonarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/custom_format_specification_schema.py` & `sonarr-py-0.7.0/sonarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/delay_profile_resource.py` & `sonarr-py-0.7.0/sonarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/disk_space_resource.py` & `sonarr-py-0.7.0/sonarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/download_client_config_resource.py` & `sonarr-py-0.7.0/sonarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/download_client_resource.py` & `sonarr-py-0.7.0/sonarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/download_protocol.py` & `sonarr-py-0.7.0/sonarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/episode_file_list_resource.py` & `sonarr-py-0.7.0/sonarr/models/episode_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/episode_file_resource.py` & `sonarr-py-0.7.0/sonarr/models/episode_file_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/episode_history_event_type.py` & `sonarr-py-0.7.0/sonarr/models/episode_history_event_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/episode_resource.py` & `sonarr-py-0.7.0/sonarr/models/episode_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     tvdb_id: Optional[int]
     episode_file_id: Optional[int]
     season_number: Optional[int]
     episode_number: Optional[int]
     title: Optional[str]
     air_date: Optional[str]
     air_date_utc: Optional[datetime]
+    runtime: Optional[int]
     overview: Optional[str]
     episode_file: Optional[EpisodeFileResource]
     has_file: Optional[bool]
     monitored: Optional[bool]
     absolute_episode_number: Optional[int]
     scene_absolute_episode_number: Optional[int]
     scene_episode_number: Optional[int]
@@ -49,15 +50,15 @@
     unverified_scene_numbering: Optional[bool]
     end_time: Optional[datetime]
     grab_date: Optional[datetime]
     series_title: Optional[str]
     series: Optional[SeriesResource]
     images: Optional[List]
     grabbed: Optional[bool]
-    __properties = ["id", "seriesId", "tvdbId", "episodeFileId", "seasonNumber", "episodeNumber", "title", "airDate", "airDateUtc", "overview", "episodeFile", "hasFile", "monitored", "absoluteEpisodeNumber", "sceneAbsoluteEpisodeNumber", "sceneEpisodeNumber", "sceneSeasonNumber", "unverifiedSceneNumbering", "endTime", "grabDate", "seriesTitle", "series", "images", "grabbed"]
+    __properties = ["id", "seriesId", "tvdbId", "episodeFileId", "seasonNumber", "episodeNumber", "title", "airDate", "airDateUtc", "runtime", "overview", "episodeFile", "hasFile", "monitored", "absoluteEpisodeNumber", "sceneAbsoluteEpisodeNumber", "sceneEpisodeNumber", "sceneSeasonNumber", "unverifiedSceneNumbering", "endTime", "grabDate", "seriesTitle", "series", "images", "grabbed"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -160,14 +161,15 @@
             "tvdb_id": obj.get("tvdbId"),
             "episode_file_id": obj.get("episodeFileId"),
             "season_number": obj.get("seasonNumber"),
             "episode_number": obj.get("episodeNumber"),
             "title": obj.get("title"),
             "air_date": obj.get("airDate"),
             "air_date_utc": obj.get("airDateUtc"),
+            "runtime": obj.get("runtime"),
             "overview": obj.get("overview"),
             "episode_file": EpisodeFileResource.from_dict(obj.get("episodeFile")) if obj.get("episodeFile") is not None else None,
             "has_file": obj.get("hasFile"),
             "monitored": obj.get("monitored"),
             "absolute_episode_number": obj.get("absoluteEpisodeNumber"),
             "scene_absolute_episode_number": obj.get("sceneAbsoluteEpisodeNumber"),
             "scene_episode_number": obj.get("sceneEpisodeNumber"),
```

### Comparing `sonarr-py-0.6.2/sonarr/models/episode_resource_paging_resource.py` & `sonarr-py-0.7.0/sonarr/models/episode_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/episode_title_required_type.py` & `sonarr-py-0.7.0/sonarr/models/episode_title_required_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/episodes_monitored_resource.py` & `sonarr-py-0.7.0/sonarr/models/episodes_monitored_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/field.py` & `sonarr-py-0.7.0/sonarr/models/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     type: Optional[str]
     advanced: Optional[bool]
     select_options: Optional[List]
     select_options_provider_action: Optional[str]
     section: Optional[str]
     hidden: Optional[str]
     privacy: Optional[PrivacyLevel]
-    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "privacy"]
+    placeholder: Optional[str]
+    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "privacy", "placeholder"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -118,14 +119,18 @@
         if self.section is None:
             _dict['section'] = None
 
         # set to None if hidden (nullable) is None
         if self.hidden is None:
             _dict['hidden'] = None
 
+        # set to None if placeholder (nullable) is None
+        if self.placeholder is None:
+            _dict['placeholder'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Field:
         """Create an instance of Field from a dict"""
         if obj is None:
             return None
@@ -143,11 +148,12 @@
             "value": obj.get("value"),
             "type": obj.get("type"),
             "advanced": obj.get("advanced"),
             "select_options": [SelectOption.from_dict(_item) for _item in obj.get("selectOptions")] if obj.get("selectOptions") is not None else None,
             "select_options_provider_action": obj.get("selectOptionsProviderAction"),
             "section": obj.get("section"),
             "hidden": obj.get("hidden"),
-            "privacy": obj.get("privacy")
+            "privacy": obj.get("privacy"),
+            "placeholder": obj.get("placeholder")
         })
         return _obj
```

### Comparing `sonarr-py-0.6.2/sonarr/models/file_date_type.py` & `sonarr-py-0.7.0/sonarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/health_check_result.py` & `sonarr-py-0.7.0/sonarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/health_resource.py` & `sonarr-py-0.7.0/sonarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/history_resource.py` & `sonarr-py-0.7.0/sonarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/history_resource_paging_resource.py` & `sonarr-py-0.7.0/sonarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/host_config_resource.py` & `sonarr-py-0.7.0/sonarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/import_list_exclusion_resource.py` & `sonarr-py-0.7.0/sonarr/models/import_list_exclusion_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/import_list_resource.py` & `sonarr-py-0.7.0/sonarr/models/import_list_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/import_list_type.py` & `sonarr-py-0.7.0/sonarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/indexer_config_resource.py` & `sonarr-py-0.7.0/sonarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/indexer_resource.py` & `sonarr-py-0.7.0/sonarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/language.py` & `sonarr-py-0.7.0/sonarr/models/language.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/language_profile_item_resource.py` & `sonarr-py-0.7.0/sonarr/models/language_profile_item_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/language_profile_resource.py` & `sonarr-py-0.7.0/sonarr/models/language_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/language_resource.py` & `sonarr-py-0.7.0/sonarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/localization_language_resource.py` & `sonarr-py-0.7.0/sonarr/models/localization_language_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/localization_resource.py` & `sonarr-py-0.7.0/sonarr/models/localization_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/log_file_resource.py` & `sonarr-py-0.7.0/sonarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/log_resource.py` & `sonarr-py-0.7.0/sonarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/log_resource_paging_resource.py` & `sonarr-py-0.7.0/sonarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/manual_import_reprocess_resource.py` & `sonarr-py-0.7.0/sonarr/models/manual_import_reprocess_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/manual_import_resource.py` & `sonarr-py-0.7.0/sonarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/media_cover.py` & `sonarr-py-0.7.0/sonarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/media_cover_types.py` & `sonarr-py-0.7.0/sonarr/models/media_cover_types.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/media_info_resource.py` & `sonarr-py-0.7.0/sonarr/models/media_info_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class MediaInfoResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `sonarr-py-0.6.2/sonarr/models/media_management_config_resource.py` & `sonarr-py-0.7.0/sonarr/models/media_management_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/metadata_resource.py` & `sonarr-py-0.7.0/sonarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/monitor_types.py` & `sonarr-py-0.7.0/sonarr/models/series_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MonitorTypes(str, Enum):
+class SeriesTypes(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    UNKNOWN = 'unknown'
-    ALL = 'all'
-    FUTURE = 'future'
-    MISSING = 'missing'
-    EXISTING = 'existing'
-    FIRSTSEASON = 'firstSeason'
-    LATESTSEASON = 'latestSeason'
-    PILOT = 'pilot'
-    NONE = 'none'
+    STANDARD = 'standard'
+    DAILY = 'daily'
+    ANIME = 'anime'
```

### Comparing `sonarr-py-0.6.2/sonarr/models/monitoring_options.py` & `sonarr-py-0.7.0/sonarr/models/monitoring_options.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/naming_config_resource.py` & `sonarr-py-0.7.0/sonarr/models/naming_config_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,29 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     rename_episodes: Optional[bool]
     replace_illegal_characters: Optional[bool]
+    colon_replacement_format: Optional[int]
     multi_episode_style: Optional[int]
     standard_episode_format: Optional[str]
     daily_episode_format: Optional[str]
     anime_episode_format: Optional[str]
     series_folder_format: Optional[str]
     season_folder_format: Optional[str]
     specials_folder_format: Optional[str]
     include_series_title: Optional[bool]
     include_episode_title: Optional[bool]
     include_quality: Optional[bool]
     replace_spaces: Optional[bool]
     separator: Optional[str]
     number_style: Optional[str]
-    __properties = ["id", "renameEpisodes", "replaceIllegalCharacters", "multiEpisodeStyle", "standardEpisodeFormat", "dailyEpisodeFormat", "animeEpisodeFormat", "seriesFolderFormat", "seasonFolderFormat", "specialsFolderFormat", "includeSeriesTitle", "includeEpisodeTitle", "includeQuality", "replaceSpaces", "separator", "numberStyle"]
+    __properties = ["id", "renameEpisodes", "replaceIllegalCharacters", "colonReplacementFormat", "multiEpisodeStyle", "standardEpisodeFormat", "dailyEpisodeFormat", "animeEpisodeFormat", "seriesFolderFormat", "seasonFolderFormat", "specialsFolderFormat", "includeSeriesTitle", "includeEpisodeTitle", "includeQuality", "replaceSpaces", "separator", "numberStyle"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -114,14 +115,15 @@
         if type(obj) is not dict:
             return NamingConfigResource.parse_obj(obj)
 
         _obj = NamingConfigResource.parse_obj({
             "id": obj.get("id"),
             "rename_episodes": obj.get("renameEpisodes"),
             "replace_illegal_characters": obj.get("replaceIllegalCharacters"),
+            "colon_replacement_format": obj.get("colonReplacementFormat"),
             "multi_episode_style": obj.get("multiEpisodeStyle"),
             "standard_episode_format": obj.get("standardEpisodeFormat"),
             "daily_episode_format": obj.get("dailyEpisodeFormat"),
             "anime_episode_format": obj.get("animeEpisodeFormat"),
             "series_folder_format": obj.get("seriesFolderFormat"),
             "season_folder_format": obj.get("seasonFolderFormat"),
             "specials_folder_format": obj.get("specialsFolderFormat"),
```

### Comparing `sonarr-py-0.6.2/sonarr/models/notification_resource.py` & `sonarr-py-0.7.0/sonarr/models/notification_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,31 +39,37 @@
     tags: Optional[List]
     presets: Optional[List]
     link: Optional[str]
     on_grab: Optional[bool]
     on_download: Optional[bool]
     on_upgrade: Optional[bool]
     on_rename: Optional[bool]
+    on_series_add: Optional[bool]
     on_series_delete: Optional[bool]
     on_episode_file_delete: Optional[bool]
     on_episode_file_delete_for_upgrade: Optional[bool]
     on_health_issue: Optional[bool]
+    on_health_restored: Optional[bool]
     on_application_update: Optional[bool]
+    on_manual_interaction_required: Optional[bool]
     supports_on_grab: Optional[bool]
     supports_on_download: Optional[bool]
     supports_on_upgrade: Optional[bool]
     supports_on_rename: Optional[bool]
+    supports_on_series_add: Optional[bool]
     supports_on_series_delete: Optional[bool]
     supports_on_episode_file_delete: Optional[bool]
     supports_on_episode_file_delete_for_upgrade: Optional[bool]
     supports_on_health_issue: Optional[bool]
+    supports_on_health_restored: Optional[bool]
     supports_on_application_update: Optional[bool]
+    supports_on_manual_interaction_required: Optional[bool]
     include_health_warnings: Optional[bool]
     test_command: Optional[str]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onDownload", "onUpgrade", "onRename", "onSeriesDelete", "onEpisodeFileDelete", "onEpisodeFileDeleteForUpgrade", "onHealthIssue", "onApplicationUpdate", "supportsOnGrab", "supportsOnDownload", "supportsOnUpgrade", "supportsOnRename", "supportsOnSeriesDelete", "supportsOnEpisodeFileDelete", "supportsOnEpisodeFileDeleteForUpgrade", "supportsOnHealthIssue", "supportsOnApplicationUpdate", "includeHealthWarnings", "testCommand"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onDownload", "onUpgrade", "onRename", "onSeriesAdd", "onSeriesDelete", "onEpisodeFileDelete", "onEpisodeFileDeleteForUpgrade", "onHealthIssue", "onHealthRestored", "onApplicationUpdate", "onManualInteractionRequired", "supportsOnGrab", "supportsOnDownload", "supportsOnUpgrade", "supportsOnRename", "supportsOnSeriesAdd", "supportsOnSeriesDelete", "supportsOnEpisodeFileDelete", "supportsOnEpisodeFileDeleteForUpgrade", "supportsOnHealthIssue", "supportsOnHealthRestored", "supportsOnApplicationUpdate", "supportsOnManualInteractionRequired", "includeHealthWarnings", "testCommand"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -168,26 +174,32 @@
             "tags": obj.get("tags"),
             "presets": [NotificationResource.from_dict(_item) for _item in obj.get("presets")] if obj.get("presets") is not None else None,
             "link": obj.get("link"),
             "on_grab": obj.get("onGrab"),
             "on_download": obj.get("onDownload"),
             "on_upgrade": obj.get("onUpgrade"),
             "on_rename": obj.get("onRename"),
+            "on_series_add": obj.get("onSeriesAdd"),
             "on_series_delete": obj.get("onSeriesDelete"),
             "on_episode_file_delete": obj.get("onEpisodeFileDelete"),
             "on_episode_file_delete_for_upgrade": obj.get("onEpisodeFileDeleteForUpgrade"),
             "on_health_issue": obj.get("onHealthIssue"),
+            "on_health_restored": obj.get("onHealthRestored"),
             "on_application_update": obj.get("onApplicationUpdate"),
+            "on_manual_interaction_required": obj.get("onManualInteractionRequired"),
             "supports_on_grab": obj.get("supportsOnGrab"),
             "supports_on_download": obj.get("supportsOnDownload"),
             "supports_on_upgrade": obj.get("supportsOnUpgrade"),
             "supports_on_rename": obj.get("supportsOnRename"),
+            "supports_on_series_add": obj.get("supportsOnSeriesAdd"),
             "supports_on_series_delete": obj.get("supportsOnSeriesDelete"),
             "supports_on_episode_file_delete": obj.get("supportsOnEpisodeFileDelete"),
             "supports_on_episode_file_delete_for_upgrade": obj.get("supportsOnEpisodeFileDeleteForUpgrade"),
             "supports_on_health_issue": obj.get("supportsOnHealthIssue"),
+            "supports_on_health_restored": obj.get("supportsOnHealthRestored"),
             "supports_on_application_update": obj.get("supportsOnApplicationUpdate"),
+            "supports_on_manual_interaction_required": obj.get("supportsOnManualInteractionRequired"),
             "include_health_warnings": obj.get("includeHealthWarnings"),
             "test_command": obj.get("testCommand")
         })
         return _obj
```

### Comparing `sonarr-py-0.6.2/sonarr/models/paging_resource_filter.py` & `sonarr-py-0.7.0/sonarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/parse_resource.py` & `sonarr-py-0.7.0/sonarr/models/parse_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/parsed_episode_info.py` & `sonarr-py-0.7.0/sonarr/models/parsed_episode_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from sonarr.models.language import Language
 from sonarr.models.quality_model import QualityModel
 from sonarr.models.series_title_info import SeriesTitleInfo
 
 class ParsedEpisodeInfo(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `sonarr-py-0.6.2/sonarr/models/ping_resource.py` & `sonarr-py-0.7.0/sonarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/privacy_level.py` & `sonarr-py-0.7.0/sonarr/models/privacy_level.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/profile_format_item_resource.py` & `sonarr-py-0.7.0/sonarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/proper_download_types.py` & `sonarr-py-0.7.0/sonarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/provider_message.py` & `sonarr-py-0.7.0/sonarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/provider_message_type.py` & `sonarr-py-0.7.0/sonarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/proxy_type.py` & `sonarr-py-0.7.0/sonarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/quality.py` & `sonarr-py-0.7.0/sonarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/quality_definition_resource.py` & `sonarr-py-0.7.0/sonarr/models/quality_definition_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 from sonarr.models.quality import Quality
 
 class QualityDefinitionResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sonarr-py-0.6.2/sonarr/models/quality_model.py` & `sonarr-py-0.7.0/sonarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/quality_profile_quality_item_resource.py` & `sonarr-py-0.7.0/sonarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/quality_profile_resource.py` & `sonarr-py-0.7.0/sonarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/quality_source.py` & `sonarr-py-0.7.0/sonarr/models/quality_source.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/queue_bulk_resource.py` & `sonarr-py-0.7.0/sonarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/queue_resource.py` & `sonarr-py-0.7.0/sonarr/models/queue_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from sonarr.models.custom_format_resource import CustomFormatResource
 from sonarr.models.download_protocol import DownloadProtocol
 from sonarr.models.episode_resource import EpisodeResource
 from sonarr.models.language import Language
 from sonarr.models.quality_model import QualityModel
 from sonarr.models.series_resource import SeriesResource
@@ -34,14 +34,15 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     series_id: Optional[int]
     episode_id: Optional[int]
+    season_number: Optional[int]
     series: Optional[SeriesResource]
     episode: Optional[EpisodeResource]
     languages: Optional[List]
     quality: Optional[QualityModel]
     custom_formats: Optional[List]
     size: Optional[float]
     title: Optional[str]
@@ -54,15 +55,16 @@
     status_messages: Optional[List]
     error_message: Optional[str]
     download_id: Optional[str]
     protocol: Optional[DownloadProtocol]
     download_client: Optional[str]
     indexer: Optional[str]
     output_path: Optional[str]
-    __properties = ["id", "seriesId", "episodeId", "series", "episode", "languages", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath"]
+    episode_has_file: Optional[bool]
+    __properties = ["id", "seriesId", "episodeId", "seasonNumber", "series", "episode", "languages", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "episodeHasFile"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -121,14 +123,18 @@
         if self.series_id is None:
             _dict['seriesId'] = None
 
         # set to None if episode_id (nullable) is None
         if self.episode_id is None:
             _dict['episodeId'] = None
 
+        # set to None if season_number (nullable) is None
+        if self.season_number is None:
+            _dict['seasonNumber'] = None
+
         # set to None if languages (nullable) is None
         if self.languages is None:
             _dict['languages'] = None
 
         # set to None if custom_formats (nullable) is None
         if self.custom_formats is None:
             _dict['customFormats'] = None
@@ -180,14 +186,15 @@
         if type(obj) is not dict:
             return QueueResource.parse_obj(obj)
 
         _obj = QueueResource.parse_obj({
             "id": obj.get("id"),
             "series_id": obj.get("seriesId"),
             "episode_id": obj.get("episodeId"),
+            "season_number": obj.get("seasonNumber"),
             "series": SeriesResource.from_dict(obj.get("series")) if obj.get("series") is not None else None,
             "episode": EpisodeResource.from_dict(obj.get("episode")) if obj.get("episode") is not None else None,
             "languages": [Language.from_dict(_item) for _item in obj.get("languages")] if obj.get("languages") is not None else None,
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
             "size": obj.get("size"),
             "title": obj.get("title"),
@@ -199,11 +206,12 @@
             "tracked_download_state": obj.get("trackedDownloadState"),
             "status_messages": [TrackedDownloadStatusMessage.from_dict(_item) for _item in obj.get("statusMessages")] if obj.get("statusMessages") is not None else None,
             "error_message": obj.get("errorMessage"),
             "download_id": obj.get("downloadId"),
             "protocol": obj.get("protocol"),
             "download_client": obj.get("downloadClient"),
             "indexer": obj.get("indexer"),
-            "output_path": obj.get("outputPath")
+            "output_path": obj.get("outputPath"),
+            "episode_has_file": obj.get("episodeHasFile")
         })
         return _obj
```

### Comparing `sonarr-py-0.6.2/sonarr/models/queue_resource_paging_resource.py` & `sonarr-py-0.7.0/sonarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/queue_status_resource.py` & `sonarr-py-0.7.0/sonarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/ratings.py` & `sonarr-py-0.7.0/sonarr/models/ratings.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class Ratings(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `sonarr-py-0.6.2/sonarr/models/rejection.py` & `sonarr-py-0.7.0/sonarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/rejection_type.py` & `sonarr-py-0.7.0/sonarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/release_profile_resource.py` & `sonarr-py-0.7.0/sonarr/models/release_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/release_resource.py` & `sonarr-py-0.7.0/sonarr/models/release_resource.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from sonarr.models.alternate_title_resource import AlternateTitleResource
 from sonarr.models.custom_format_resource import CustomFormatResource
 from sonarr.models.download_protocol import DownloadProtocol
 from sonarr.models.language import Language
 from sonarr.models.quality_model import QualityModel
+from sonarr.models.release_episode_resource import ReleaseEpisodeResource
 
 class ReleaseResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -53,14 +54,16 @@
     air_date: Optional[str]
     series_title: Optional[str]
     episode_numbers: Optional[List]
     absolute_episode_numbers: Optional[List]
     mapped_season_number: Optional[int]
     mapped_episode_numbers: Optional[List]
     mapped_absolute_episode_numbers: Optional[List]
+    mapped_series_id: Optional[int]
+    mapped_episode_info: Optional[List]
     approved: Optional[bool]
     temporarily_rejected: Optional[bool]
     rejected: Optional[bool]
     tvdb_id: Optional[int]
     tv_rage_id: Optional[int]
     rejections: Optional[List]
     publish_date: Optional[datetime]
@@ -80,15 +83,18 @@
     protocol: Optional[DownloadProtocol]
     is_daily: Optional[bool]
     is_absolute_numbering: Optional[bool]
     is_possible_special_episode: Optional[bool]
     special: Optional[bool]
     series_id: Optional[int]
     episode_id: Optional[int]
-    __properties = ["id", "guid", "quality", "qualityWeight", "age", "ageHours", "ageMinutes", "size", "indexerId", "indexer", "releaseGroup", "subGroup", "releaseHash", "title", "fullSeason", "sceneSource", "seasonNumber", "languages", "languageWeight", "airDate", "seriesTitle", "episodeNumbers", "absoluteEpisodeNumbers", "mappedSeasonNumber", "mappedEpisodeNumbers", "mappedAbsoluteEpisodeNumbers", "approved", "temporarilyRejected", "rejected", "tvdbId", "tvRageId", "rejections", "publishDate", "commentUrl", "downloadUrl", "infoUrl", "episodeRequested", "downloadAllowed", "releaseWeight", "customFormats", "customFormatScore", "sceneMapping", "magnetUrl", "infoHash", "seeders", "leechers", "protocol", "isDaily", "isAbsoluteNumbering", "isPossibleSpecialEpisode", "special", "seriesId", "episodeId"]
+    episode_ids: Optional[List]
+    download_client_id: Optional[int]
+    should_override: Optional[bool]
+    __properties = ["id", "guid", "quality", "qualityWeight", "age", "ageHours", "ageMinutes", "size", "indexerId", "indexer", "releaseGroup", "subGroup", "releaseHash", "title", "fullSeason", "sceneSource", "seasonNumber", "languages", "languageWeight", "airDate", "seriesTitle", "episodeNumbers", "absoluteEpisodeNumbers", "mappedSeasonNumber", "mappedEpisodeNumbers", "mappedAbsoluteEpisodeNumbers", "mappedSeriesId", "mappedEpisodeInfo", "approved", "temporarilyRejected", "rejected", "tvdbId", "tvRageId", "rejections", "publishDate", "commentUrl", "downloadUrl", "infoUrl", "episodeRequested", "downloadAllowed", "releaseWeight", "customFormats", "customFormatScore", "sceneMapping", "magnetUrl", "infoHash", "seeders", "leechers", "protocol", "isDaily", "isAbsoluteNumbering", "isPossibleSpecialEpisode", "special", "seriesId", "episodeId", "episodeIds", "downloadClientId", "shouldOverride"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -119,14 +125,21 @@
         # override the default output from pydantic by calling `to_dict()` of each item in languages (list)
         _items = []
         if self.languages:
             for _item in self.languages:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['languages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in mapped_episode_info (list)
+        _items = []
+        if self.mapped_episode_info:
+            for _item in self.mapped_episode_info:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['mappedEpisodeInfo'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in custom_formats (list)
         _items = []
         if self.custom_formats:
             for _item in self.custom_formats:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['customFormats'] = _items
@@ -185,14 +198,22 @@
         if self.mapped_episode_numbers is None:
             _dict['mappedEpisodeNumbers'] = None
 
         # set to None if mapped_absolute_episode_numbers (nullable) is None
         if self.mapped_absolute_episode_numbers is None:
             _dict['mappedAbsoluteEpisodeNumbers'] = None
 
+        # set to None if mapped_series_id (nullable) is None
+        if self.mapped_series_id is None:
+            _dict['mappedSeriesId'] = None
+
+        # set to None if mapped_episode_info (nullable) is None
+        if self.mapped_episode_info is None:
+            _dict['mappedEpisodeInfo'] = None
+
         # set to None if rejections (nullable) is None
         if self.rejections is None:
             _dict['rejections'] = None
 
         # set to None if comment_url (nullable) is None
         if self.comment_url is None:
             _dict['commentUrl'] = None
@@ -229,14 +250,26 @@
         if self.series_id is None:
             _dict['seriesId'] = None
 
         # set to None if episode_id (nullable) is None
         if self.episode_id is None:
             _dict['episodeId'] = None
 
+        # set to None if episode_ids (nullable) is None
+        if self.episode_ids is None:
+            _dict['episodeIds'] = None
+
+        # set to None if download_client_id (nullable) is None
+        if self.download_client_id is None:
+            _dict['downloadClientId'] = None
+
+        # set to None if should_override (nullable) is None
+        if self.should_override is None:
+            _dict['shouldOverride'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ReleaseResource:
         """Create an instance of ReleaseResource from a dict"""
         if obj is None:
             return None
@@ -267,14 +300,16 @@
             "air_date": obj.get("airDate"),
             "series_title": obj.get("seriesTitle"),
             "episode_numbers": obj.get("episodeNumbers"),
             "absolute_episode_numbers": obj.get("absoluteEpisodeNumbers"),
             "mapped_season_number": obj.get("mappedSeasonNumber"),
             "mapped_episode_numbers": obj.get("mappedEpisodeNumbers"),
             "mapped_absolute_episode_numbers": obj.get("mappedAbsoluteEpisodeNumbers"),
+            "mapped_series_id": obj.get("mappedSeriesId"),
+            "mapped_episode_info": [ReleaseEpisodeResource.from_dict(_item) for _item in obj.get("mappedEpisodeInfo")] if obj.get("mappedEpisodeInfo") is not None else None,
             "approved": obj.get("approved"),
             "temporarily_rejected": obj.get("temporarilyRejected"),
             "rejected": obj.get("rejected"),
             "tvdb_id": obj.get("tvdbId"),
             "tv_rage_id": obj.get("tvRageId"),
             "rejections": obj.get("rejections"),
             "publish_date": obj.get("publishDate"),
@@ -293,11 +328,14 @@
             "leechers": obj.get("leechers"),
             "protocol": obj.get("protocol"),
             "is_daily": obj.get("isDaily"),
             "is_absolute_numbering": obj.get("isAbsoluteNumbering"),
             "is_possible_special_episode": obj.get("isPossibleSpecialEpisode"),
             "special": obj.get("special"),
             "series_id": obj.get("seriesId"),
-            "episode_id": obj.get("episodeId")
+            "episode_id": obj.get("episodeId"),
+            "episode_ids": obj.get("episodeIds"),
+            "download_client_id": obj.get("downloadClientId"),
+            "should_override": obj.get("shouldOverride")
         })
         return _obj
```

### Comparing `sonarr-py-0.6.2/sonarr/models/remote_path_mapping_resource.py` & `sonarr-py-0.7.0/sonarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/rename_episode_resource.py` & `sonarr-py-0.7.0/sonarr/models/rename_episode_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/rescan_after_refresh_type.py` & `sonarr-py-0.7.0/sonarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/revision.py` & `sonarr-py-0.7.0/sonarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/root_folder_resource.py` & `sonarr-py-0.7.0/sonarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/runtime_mode.py` & `sonarr-py-0.7.0/sonarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/season_pass_resource.py` & `sonarr-py-0.7.0/sonarr/models/season_pass_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/season_pass_series_resource.py` & `sonarr-py-0.7.0/sonarr/models/season_pass_series_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/season_resource.py` & `sonarr-py-0.7.0/sonarr/models/season_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/season_statistics_resource.py` & `sonarr-py-0.7.0/sonarr/models/season_statistics_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 
 class SeasonStatisticsResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `sonarr-py-0.6.2/sonarr/models/select_option.py` & `sonarr-py-0.7.0/sonarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/series_editor_resource.py` & `sonarr-py-0.7.0/sonarr/models/series_editor_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/series_resource.py` & `sonarr-py-0.7.0/sonarr/models/series_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/series_statistics_resource.py` & `sonarr-py-0.7.0/sonarr/models/series_statistics_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 
 class SeriesStatisticsResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `sonarr-py-0.6.2/sonarr/models/series_status_type.py` & `sonarr-py-0.7.0/sonarr/models/series_status_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/series_title_info.py` & `sonarr-py-0.7.0/sonarr/models/series_title_info.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/series_types.py` & `sonarr-py-0.7.0/sonarr/models/sort_direction.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class SeriesTypes(str, Enum):
+class SortDirection(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    STANDARD = 'standard'
-    DAILY = 'daily'
-    ANIME = 'anime'
+    DEFAULT = 'default'
+    ASCENDING = 'ascending'
+    DESCENDING = 'descending'
```

### Comparing `sonarr-py-0.6.2/sonarr/models/sort_direction.py` & `sonarr-py-0.7.0/sonarr/models/tracked_download_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class SortDirection(str, Enum):
+class TrackedDownloadStatus(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    DEFAULT = 'default'
-    ASCENDING = 'ascending'
-    DESCENDING = 'descending'
+    OK = 'ok'
+    WARNING = 'warning'
+    ERROR = 'error'
```

### Comparing `sonarr-py-0.6.2/sonarr/models/system_resource.py` & `sonarr-py-0.7.0/sonarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/tag_details_resource.py` & `sonarr-py-0.7.0/sonarr/models/tag_details_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/tag_resource.py` & `sonarr-py-0.7.0/sonarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/task_resource.py` & `sonarr-py-0.7.0/sonarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/tracked_download_state.py` & `sonarr-py-0.7.0/sonarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/tracked_download_status.py` & `sonarr-py-0.7.0/sonarr/models/update_mechanism.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackedDownloadStatus(str, Enum):
+class UpdateMechanism(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    OK = 'ok'
-    WARNING = 'warning'
-    ERROR = 'error'
+    BUILTIN = 'builtIn'
+    SCRIPT = 'script'
+    EXTERNAL = 'external'
+    APT = 'apt'
+    DOCKER = 'docker'
```

### Comparing `sonarr-py-0.6.2/sonarr/models/tracked_download_status_message.py` & `sonarr-py-0.7.0/sonarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/ui_config_resource.py` & `sonarr-py-0.7.0/sonarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/unmapped_folder.py` & `sonarr-py-0.7.0/sonarr/models/unmapped_folder.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/update_changes.py` & `sonarr-py-0.7.0/sonarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/models/update_mechanism.py` & `sonarr-py-0.7.0/sonarr/models/command_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class UpdateMechanism(str, Enum):
+class CommandResult(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    BUILTIN = 'builtIn'
-    SCRIPT = 'script'
-    EXTERNAL = 'external'
-    APT = 'apt'
-    DOCKER = 'docker'
+    UNKNOWN = 'unknown'
+    SUCCESSFUL = 'successful'
+    UNSUCCESSFUL = 'unsuccessful'
```

### Comparing `sonarr-py-0.6.2/sonarr/models/update_resource.py` & `sonarr-py-0.7.0/sonarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr/rest.py` & `sonarr-py-0.7.0/sonarr/rest.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.6.2/sonarr_py.egg-info/PKG-INFO` & `sonarr-py-0.7.0/sonarr_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonarr-py
-Version: 0.6.2
+Version: 0.7.0
 Summary: Sonarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/sonarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/sonarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,15 +12,15 @@
 
 # sonarr-py
 Sonarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.6.2
+- Package version: 0.7.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -352,14 +352,15 @@
  - [BlocklistBulkResource](docs/BlocklistBulkResource.md)
  - [BlocklistResource](docs/BlocklistResource.md)
  - [BlocklistResourcePagingResource](docs/BlocklistResourcePagingResource.md)
  - [CertificateValidationType](docs/CertificateValidationType.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
@@ -424,14 +425,15 @@
  - [QueueBulkResource](docs/QueueBulkResource.md)
  - [QueueResource](docs/QueueResource.md)
  - [QueueResourcePagingResource](docs/QueueResourcePagingResource.md)
  - [QueueStatusResource](docs/QueueStatusResource.md)
  - [Ratings](docs/Ratings.md)
  - [Rejection](docs/Rejection.md)
  - [RejectionType](docs/RejectionType.md)
+ - [ReleaseEpisodeResource](docs/ReleaseEpisodeResource.md)
  - [ReleaseProfileResource](docs/ReleaseProfileResource.md)
  - [ReleaseResource](docs/ReleaseResource.md)
  - [RemotePathMappingResource](docs/RemotePathMappingResource.md)
  - [RenameEpisodeResource](docs/RenameEpisodeResource.md)
  - [RescanAfterRefreshType](docs/RescanAfterRefreshType.md)
  - [Revision](docs/Revision.md)
  - [RootFolderResource](docs/RootFolderResource.md)
```

### Comparing `sonarr-py-0.6.2/sonarr_py.egg-info/SOURCES.txt` & `sonarr-py-0.7.0/sonarr_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 pyproject.toml
 setup.py
 sonarr/__init__.py
 sonarr/api_client.py
+sonarr/api_response.py
 sonarr/configuration.py
 sonarr/exceptions.py
 sonarr/rest.py
 sonarr/api/__init__.py
 sonarr/api/api_info_api.py
 sonarr/api/authentication_api.py
 sonarr/api/auto_tagging_api.py
@@ -87,14 +88,15 @@
 sonarr/models/blocklist_bulk_resource.py
 sonarr/models/blocklist_resource.py
 sonarr/models/blocklist_resource_paging_resource.py
 sonarr/models/certificate_validation_type.py
 sonarr/models/command.py
 sonarr/models/command_priority.py
 sonarr/models/command_resource.py
+sonarr/models/command_result.py
 sonarr/models/command_status.py
 sonarr/models/command_trigger.py
 sonarr/models/custom_filter_resource.py
 sonarr/models/custom_format_resource.py
 sonarr/models/custom_format_specification_schema.py
 sonarr/models/delay_profile_resource.py
 sonarr/models/disk_space_resource.py
@@ -159,14 +161,15 @@
 sonarr/models/queue_bulk_resource.py
 sonarr/models/queue_resource.py
 sonarr/models/queue_resource_paging_resource.py
 sonarr/models/queue_status_resource.py
 sonarr/models/ratings.py
 sonarr/models/rejection.py
 sonarr/models/rejection_type.py
+sonarr/models/release_episode_resource.py
 sonarr/models/release_profile_resource.py
 sonarr/models/release_resource.py
 sonarr/models/remote_path_mapping_resource.py
 sonarr/models/rename_episode_resource.py
 sonarr/models/rescan_after_refresh_type.py
 sonarr/models/revision.py
 sonarr/models/root_folder_resource.py
```

