# Comparing `tmp/atproto-0.0.4.tar.gz` & `tmp/atproto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.4.tar", max compression
+gzip compressed data, was "atproto-0.0.5.tar", max compression
```

## Comparing `atproto-0.0.4.tar` & `atproto-0.0.5.tar`

### file list

```diff
@@ -1,152 +1,167 @@
--rw-r--r--   0        0        0     1061 2023-05-12 18:48:38.738671 atproto-0.0.4/LICENSE
--rw-r--r--   0        0        0     9588 2023-05-12 18:48:38.738671 atproto-0.0.4/README.md
--rw-r--r--   0        0        0      300 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/__init__.py
--rw-r--r--   0        0        0      619 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/cid/__init__.py
--rw-r--r--   0        0        0       23 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/cli/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0     2317 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    18860 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0     2562 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11855 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      944 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0     4658 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3871 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5298 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/uri/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0     5994 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0     3719 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     5555 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0      469 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    10098 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     3278 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      836 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      890 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0     1014 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      927 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0     1061 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      970 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1778 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1564 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2457 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1248 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4321 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1041 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1497 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0     1076 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      855 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1181 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0     1066 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      734 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2441 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      738 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      665 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0      667 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0     1004 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1133 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1123 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      999 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      574 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      576 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      830 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1932 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      586 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1735 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      553 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0     9928 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      712 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0     1071 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      839 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0     1097 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      839 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1161 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      890 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      824 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      953 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      911 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1129 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1370 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      651 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      621 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      887 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      586 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0     1077 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0     1499 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      825 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     2140 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1236 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      969 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1038 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1171 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1817 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1319 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      644 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      742 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0     1052 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      880 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1352 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0     1117 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1296 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      659 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1271 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0     1028 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      704 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0     1024 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      729 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      589 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      628 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      583 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      752 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      744 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      822 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      986 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      764 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      872 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      916 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      969 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1253 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      637 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      640 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2782 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      425 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/type_conversion.py
--rw-r--r--   0        0        0     3285 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0    65433 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      361 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    64495 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4353 2023-05-12 18:48:38.746671 atproto-0.0.4/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-12 18:48:38.746671 atproto-0.0.4/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0     2083 2023-05-12 18:48:38.754671 atproto-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    11408 1970-01-01 00:00:00.000000 atproto-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-17 07:30:57.252256 atproto-0.0.5/LICENSE
+-rw-r--r--   0        0        0     9596 2023-05-17 07:30:57.252256 atproto-0.0.5/README.md
+-rw-r--r--   0        0        0      332 2023-05-17 07:30:57.252256 atproto-0.0.5/atproto/__init__.py
+-rw-r--r--   0        0        0     1764 2023-05-17 07:30:57.252256 atproto-0.0.5/atproto/car/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2353 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    19303 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11855 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      944 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/exceptions.py
+-rw-r--r--   0        0        0     2569 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/leb128/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4658 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3871 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5298 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     5994 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0     3719 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     5555 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0      469 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    11424 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     4054 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      820 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      836 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      890 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0     1014 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      927 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      670 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0     1061 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      970 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1778 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1564 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2457 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1248 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4321 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1041 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1497 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0     1076 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      855 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1181 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0     1066 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      734 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2441 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      738 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2446 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      667 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0     1004 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1133 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1123 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0     1097 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0     1004 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0     1033 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      999 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0     1121 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      705 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      574 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      575 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      576 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      577 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      830 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1932 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      586 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1735 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    10100 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      595 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      712 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      594 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0     1071 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      839 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0     1097 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      839 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1231 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      890 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      824 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      953 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      911 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1129 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1370 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      651 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      621 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      586 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1077 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1499 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      825 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     2140 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1236 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      969 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1038 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1171 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1817 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1319 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      734 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      644 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      742 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0     1052 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      880 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1352 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0     1117 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1296 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      659 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1271 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0     1028 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      704 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0     1024 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      729 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      589 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      628 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      583 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      744 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      822 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      986 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      764 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      872 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      916 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      969 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1253 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      637 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      640 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2782 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      547 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3285 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    73381 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      361 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    72323 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4353 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2321 2023-05-17 07:31:29.892268 atproto-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11450 1970-01-01 00:00:00.000000 atproto-0.0.5/PKG-INFO
```

### Comparing `atproto-0.0.4/LICENSE` & `atproto-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/README.md` & `atproto-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -199,37 +199,37 @@
 The instances of data and params models should be passed as arguments to the methods that were described above.
 
 Dict-based:
 ```python
 from atproto import Client
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 # The params model will be created automatically internally for you!
 print(client.com.atproto.identity.resolve_handle({'handle': 'marshal.dev'}))
 ```
 
 Class-based:
 ```python
 from atproto import Client, models
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 params = models.ComAtprotoIdentityResolveHandle.Params('marshal.dev')
 print(client.com.atproto.identity.resolve_handle(params))
 ```
 
 Class-based with keywords:
 ```python
 from atproto import Client, models
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 params = models.ComAtprotoIdentityResolveHandle.Params(handle='marshal.dev')
 print(client.com.atproto.identity.resolve_handle(params))
 ```
 
 Tip: look at typehint of the method to figure out the name and the path to the input/data model!
 
@@ -240,15 +240,15 @@
 This is how we can send a post with the image using low-level XRPC Client:
 ```python
 from datetime import datetime
 
 from atproto import Client, models
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 
 with open('cat.jpg', 'rb') as f:
     img_data = f.read()
 
     upload = client.com.atproto.repo.upload_blob(img_data)
     images = [models.AppBskyEmbedImages.Image(alt='Img alt', image=upload.blob)]
```

### Comparing `atproto-0.0.4/atproto/codegen/__init__.py` & `atproto-0.0.5/atproto/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.5/atproto/codegen/clients/generate_async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/codegen/models/builder.py` & `atproto-0.0.5/atproto/codegen/models/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 _LEX_DEF_TYPES_FOR_REFS = {models.LexDefinitionType.QUERY, models.LexDefinitionType.PROCEDURE}
 _LEX_DEF_TYPES_FOR_DATA = {models.LexDefinitionType.PROCEDURE}
 _LEX_DEF_TYPES_FOR_RECORDS = {models.LexDefinitionType.RECORD}
 _LEX_DEF_TYPES_FOR_DEF = {
     models.LexDefinitionType.OBJECT,
     models.LexPrimitiveType.STRING,
     models.LexDefinitionType.TOKEN,
+    models.LexDefinitionType.ARRAY,
 }
 
 LexDefs = Dict[
     str,
     Union[
         models.LexXrpcProcedure,
         models.LexXrpcQuery,
```

### Comparing `atproto-0.0.4/atproto/codegen/models/generator.py` & `atproto-0.0.5/atproto/codegen/models/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,14 +335,18 @@
         f"{get_def_model_name(def_name)}: Literal['{def_name}'] = '{def_name}'",
         '',
         '',
     ]
     return join_code(lines)
 
 
+def _generate_def_array(nsid: NSID, def_name: str, def_model: models.LexArray) -> str:
+    return f'{get_def_model_name(def_name)} = {_get_model_field_typehint(nsid, def_name, def_model, optional=False)}\n'
+
+
 def _generate_def_string(def_name: str, def_model: models.LexString) -> str:
     # FIXME(MarshalX): Doesn't support all fields
 
     if not def_model.knownValues:
         return ''
 
     # FIXME(MarshalX): Use ref resolver
@@ -390,18 +394,22 @@
 def _generate_def_models(lex_db: builder.LexDB) -> None:
     for nsid, defs in lex_db.items():
         _save_code_import_if_not_exist(nsid)
 
         for def_name, def_model in defs.items():
             if isinstance(def_model, models.LexToken):
                 save_code_part(nsid, _generate_def_token(def_name))
-            if isinstance(def_model, models.LexString):
+            elif isinstance(def_model, models.LexString):
                 save_code_part(nsid, _generate_def_string(def_name, def_model))
-            if isinstance(def_model, models.LexObject):
+            elif isinstance(def_model, models.LexObject):
                 save_code_part(nsid, _generate_def_model(nsid, def_name, def_model, ModelType.DEF))
+            elif isinstance(def_model, models.LexArray):
+                save_code_part(nsid, _generate_def_array(nsid, def_name, def_model))
+            else:
+                raise ValueError(f'Unhandled type {type(def_model)}')
 
 
 def _generate_record_models(lex_db: builder.LexDB) -> None:
     for nsid, defs in lex_db.items():
         _save_code_import_if_not_exist(nsid)
 
         for def_name, def_record in defs.items():
```

### Comparing `atproto-0.0.4/atproto/codegen/namespaces/builder.py` & `atproto-0.0.5/atproto/codegen/namespaces/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/codegen/namespaces/generator.py` & `atproto-0.0.5/atproto/codegen/namespaces/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/exceptions.py` & `atproto-0.0.5/atproto/exceptions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/lexicon/models.py` & `atproto-0.0.5/atproto/lexicon/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/lexicon/parser.py` & `atproto-0.0.5/atproto/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/nsid/__init__.py` & `atproto-0.0.5/atproto/nsid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/uri/__init__.py` & `atproto-0.0.5/atproto/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.5/atproto/xrpc_client/client/async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/client/base.py` & `atproto-0.0.5/atproto/xrpc_client/client/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/client/client.py` & `atproto-0.0.5/atproto/xrpc_client/client/client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.5/atproto/xrpc_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from atproto.xrpc_client.models.app.bsky.actor import defs as AppBskyActorDefs
 from atproto.xrpc_client.models.app.bsky.actor import (
+    get_preferences as AppBskyActorGetPreferences,
+)
+from atproto.xrpc_client.models.app.bsky.actor import (
     get_profile as AppBskyActorGetProfile,
 )
 from atproto.xrpc_client.models.app.bsky.actor import (
     get_profiles as AppBskyActorGetProfiles,
 )
 from atproto.xrpc_client.models.app.bsky.actor import (
     get_suggestions as AppBskyActorGetSuggestions,
 )
 from atproto.xrpc_client.models.app.bsky.actor import profile as AppBskyActorProfile
 from atproto.xrpc_client.models.app.bsky.actor import (
+    put_preferences as AppBskyActorPutPreferences,
+)
+from atproto.xrpc_client.models.app.bsky.actor import (
     search_actors as AppBskyActorSearchActors,
 )
 from atproto.xrpc_client.models.app.bsky.actor import (
     search_actors_typeahead as AppBskyActorSearchActorsTypeahead,
 )
 from atproto.xrpc_client.models.app.bsky.embed import external as AppBskyEmbedExternal
 from atproto.xrpc_client.models.app.bsky.embed import images as AppBskyEmbedImages
@@ -36,31 +42,45 @@
 from atproto.xrpc_client.models.app.bsky.feed import (
     get_timeline as AppBskyFeedGetTimeline,
 )
 from atproto.xrpc_client.models.app.bsky.feed import like as AppBskyFeedLike
 from atproto.xrpc_client.models.app.bsky.feed import post as AppBskyFeedPost
 from atproto.xrpc_client.models.app.bsky.feed import repost as AppBskyFeedRepost
 from atproto.xrpc_client.models.app.bsky.graph import block as AppBskyGraphBlock
+from atproto.xrpc_client.models.app.bsky.graph import defs as AppBskyGraphDefs
 from atproto.xrpc_client.models.app.bsky.graph import follow as AppBskyGraphFollow
 from atproto.xrpc_client.models.app.bsky.graph import (
     get_blocks as AppBskyGraphGetBlocks,
 )
 from atproto.xrpc_client.models.app.bsky.graph import (
     get_followers as AppBskyGraphGetFollowers,
 )
 from atproto.xrpc_client.models.app.bsky.graph import (
     get_follows as AppBskyGraphGetFollows,
 )
+from atproto.xrpc_client.models.app.bsky.graph import get_list as AppBskyGraphGetList
+from atproto.xrpc_client.models.app.bsky.graph import (
+    get_list_mutes as AppBskyGraphGetListMutes,
+)
+from atproto.xrpc_client.models.app.bsky.graph import get_lists as AppBskyGraphGetLists
 from atproto.xrpc_client.models.app.bsky.graph import get_mutes as AppBskyGraphGetMutes
+from atproto.xrpc_client.models.app.bsky.graph import list as AppBskyGraphList
+from atproto.xrpc_client.models.app.bsky.graph import listitem as AppBskyGraphListitem
 from atproto.xrpc_client.models.app.bsky.graph import (
     mute_actor as AppBskyGraphMuteActor,
 )
 from atproto.xrpc_client.models.app.bsky.graph import (
+    mute_actor_list as AppBskyGraphMuteActorList,
+)
+from atproto.xrpc_client.models.app.bsky.graph import (
     unmute_actor as AppBskyGraphUnmuteActor,
 )
+from atproto.xrpc_client.models.app.bsky.graph import (
+    unmute_actor_list as AppBskyGraphUnmuteActorList,
+)
 from atproto.xrpc_client.models.app.bsky.notification import (
     get_unread_count as AppBskyNotificationGetUnreadCount,
 )
 from atproto.xrpc_client.models.app.bsky.notification import (
     list_notifications as AppBskyNotificationListNotifications,
 )
 from atproto.xrpc_client.models.app.bsky.notification import (
@@ -68,17 +88,23 @@
 )
 from atproto.xrpc_client.models.app.bsky.richtext import facet as AppBskyRichtextFacet
 from atproto.xrpc_client.models.app.bsky.unspecced import (
     get_popular as AppBskyUnspeccedGetPopular,
 )
 from atproto.xrpc_client.models.com.atproto.admin import defs as ComAtprotoAdminDefs
 from atproto.xrpc_client.models.com.atproto.admin import (
+    disable_account_invites as ComAtprotoAdminDisableAccountInvites,
+)
+from atproto.xrpc_client.models.com.atproto.admin import (
     disable_invite_codes as ComAtprotoAdminDisableInviteCodes,
 )
 from atproto.xrpc_client.models.com.atproto.admin import (
+    enable_account_invites as ComAtprotoAdminEnableAccountInvites,
+)
+from atproto.xrpc_client.models.com.atproto.admin import (
     get_invite_codes as ComAtprotoAdminGetInviteCodes,
 )
 from atproto.xrpc_client.models.com.atproto.admin import (
     get_moderation_action as ComAtprotoAdminGetModerationAction,
 )
 from atproto.xrpc_client.models.com.atproto.admin import (
     get_moderation_actions as ComAtprotoAdminGetModerationActions,
@@ -150,14 +176,17 @@
 from atproto.xrpc_client.models.com.atproto.repo import (
     list_records as ComAtprotoRepoListRecords,
 )
 from atproto.xrpc_client.models.com.atproto.repo import (
     put_record as ComAtprotoRepoPutRecord,
 )
 from atproto.xrpc_client.models.com.atproto.repo import (
+    rebase_repo as ComAtprotoRepoRebaseRepo,
+)
+from atproto.xrpc_client.models.com.atproto.repo import (
     strong_ref as ComAtprotoRepoStrongRef,
 )
 from atproto.xrpc_client.models.com.atproto.repo import (
     upload_blob as ComAtprotoRepoUploadBlob,
 )
 from atproto.xrpc_client.models.com.atproto.server import (
     create_account as ComAtprotoServerCreateAccount,
```

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/external.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/images.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_followers.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_follows.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/base.py` & `atproto-0.0.5/atproto/xrpc_client/models/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.5/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/defs.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,23 +188,25 @@
         did: Did.
         handle: Handle.
         email: Email.
         relatedRecords: Related records.
         indexedAt: Indexed at.
         moderation: Moderation.
         invitedBy: Invited by.
+        invitesDisabled: Invites disabled.
     """
 
     did: str
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
     relatedRecords: List['base.RecordModelBase']
     email: Optional[str] = None
     invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
+    invitesDisabled: Optional[bool] = None
 
     _type: str = 'com.atproto.admin.defs#repoView'
 
 
 @dataclass
 class RepoViewDetail(base.ModelBase):
 
@@ -216,24 +218,26 @@
         email: Email.
         relatedRecords: Related records.
         indexedAt: Indexed at.
         moderation: Moderation.
         labels: Labels.
         invitedBy: Invited by.
         invites: Invites.
+        invitesDisabled: Invites disabled.
     """
 
     did: str
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
     relatedRecords: List['base.RecordModelBase']
     email: Optional[str] = None
     invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
     invites: Optional[List['models.ComAtprotoServerDefs.InviteCode']] = None
+    invitesDisabled: Optional[bool] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
     _type: str = 'com.atproto.admin.defs#repoViewDetail'
 
 
 @dataclass
 class RepoRef(base.ModelBase):
```

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 class Params(base.ParamsModelBase):
 
     """Parameters model for :obj:`com.atproto.admin.getModerationReports`.
 
     Attributes:
         subject: Subject.
         resolved: Resolved.
+        actionType: Action type.
         limit: Limit.
         cursor: Cursor.
     """
 
+    actionType: Optional[str] = None
     cursor: Optional[str] = None
     limit: Optional[int] = None
     resolved: Optional[bool] = None
     subject: Optional[str] = None
 
 
 @dataclass
```

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_repo.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/update_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 class Data(base.DataModelBase):
 
     """Input data model for :obj:`com.atproto.server.createAccount`.
 
     Attributes:
         email: Email.
         handle: Handle.
+        did: Did.
         inviteCode: Invite code.
         password: Password.
         recoveryKey: Recovery key.
     """
 
     email: str
     handle: str
     password: str
+    did: Optional[str] = None
     inviteCode: Optional[str] = None
     recoveryKey: Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
```

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_session.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/defs.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/describe_server.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_session.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_head.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_record.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/models/utils.py` & `atproto-0.0.5/atproto/xrpc_client/models/utils.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.5/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,657 @@
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models.utils import get_or_create_model, get_response_model
 from atproto.xrpc_client.namespaces.base import DefaultNamespace, NamespaceBase
 
 
 @dataclass
+class AppNamespace(NamespaceBase):
+    bsky: 'BskyNamespace' = field(default_factory=DefaultNamespace)
+
+    def __post_init__(self):
+        self.bsky = BskyNamespace(self._client)
+
+
+@dataclass
+class BskyNamespace(NamespaceBase):
+    actor: 'ActorNamespace' = field(default_factory=DefaultNamespace)
+    feed: 'FeedNamespace' = field(default_factory=DefaultNamespace)
+    graph: 'GraphNamespace' = field(default_factory=DefaultNamespace)
+    notification: 'NotificationNamespace' = field(default_factory=DefaultNamespace)
+    unspecced: 'UnspeccedNamespace' = field(default_factory=DefaultNamespace)
+
+    def __post_init__(self):
+        self.actor = ActorNamespace(self._client)
+        self.feed = FeedNamespace(self._client)
+        self.graph = GraphNamespace(self._client)
+        self.notification = NotificationNamespace(self._client)
+        self.unspecced = UnspeccedNamespace(self._client)
+
+
+@dataclass
+class ActorNamespace(NamespaceBase):
+    async def get_preferences(
+        self, params: Optional[Union[dict, 'models.AppBskyActorGetPreferences.Params']] = None, **kwargs
+    ) -> models.AppBskyActorGetPreferences.Response:
+        """Get private preferences attached to the account.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetPreferences.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetPreferences.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.actor.getPreferences', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetPreferences.Response)
+
+    async def get_profile(
+        self, params: Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
+    ) -> models.AppBskyActorGetProfile.ResponseRef:
+        """Get profile.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetProfile.ResponseRef`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetProfile.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.actor.getProfile', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetProfile.ResponseRef)
+
+    async def get_profiles(
+        self, params: Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
+    ) -> models.AppBskyActorGetProfiles.Response:
+        """Get profiles.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetProfiles.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetProfiles.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.actor.getProfiles', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetProfiles.Response)
+
+    async def get_suggestions(
+        self, params: Optional[Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
+    ) -> models.AppBskyActorGetSuggestions.Response:
+        """Get a list of actors suggested for following. Used in discovery UIs.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetSuggestions.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetSuggestions.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.actor.getSuggestions', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetSuggestions.Response)
+
+    async def put_preferences(self, data: Union[dict, 'models.AppBskyActorPutPreferences.Data'], **kwargs) -> bool:
+        """Sets the private preferences attached to the account.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyActorPutPreferences.Data)
+        response = await self._client.invoke_procedure(
+            'app.bsky.actor.putPreferences', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    async def search_actors(
+        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
+    ) -> models.AppBskyActorSearchActors.Response:
+        """Find actors matching search criteria.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorSearchActors.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorSearchActors.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.actor.searchActors', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorSearchActors.Response)
+
+    async def search_actors_typeahead(
+        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
+    ) -> models.AppBskyActorSearchActorsTypeahead.Response:
+        """Find actor suggestions for a search term.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorSearchActorsTypeahead.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorSearchActorsTypeahead.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.actor.searchActorsTypeahead', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
+
+
+@dataclass
+class GraphNamespace(NamespaceBase):
+    async def get_blocks(
+        self, params: Optional[Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
+    ) -> models.AppBskyGraphGetBlocks.Response:
+        """Who is the requester's account blocking?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetBlocks.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetBlocks.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getBlocks', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetBlocks.Response)
+
+    async def get_followers(
+        self, params: Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
+    ) -> models.AppBskyGraphGetFollowers.Response:
+        """Who is following an actor?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetFollowers.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetFollowers.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getFollowers', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetFollowers.Response)
+
+    async def get_follows(
+        self, params: Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
+    ) -> models.AppBskyGraphGetFollows.Response:
+        """Who is an actor following?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetFollows.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetFollows.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getFollows', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetFollows.Response)
+
+    async def get_list(
+        self, params: Union[dict, 'models.AppBskyGraphGetList.Params'], **kwargs
+    ) -> models.AppBskyGraphGetList.Response:
+        """Fetch a list of actors.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetList.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetList.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getList', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetList.Response)
+
+    async def get_list_mutes(
+        self, params: Optional[Union[dict, 'models.AppBskyGraphGetListMutes.Params']] = None, **kwargs
+    ) -> models.AppBskyGraphGetListMutes.Response:
+        """Which lists is the requester's account muting?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetListMutes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetListMutes.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getListMutes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetListMutes.Response)
+
+    async def get_lists(
+        self, params: Union[dict, 'models.AppBskyGraphGetLists.Params'], **kwargs
+    ) -> models.AppBskyGraphGetLists.Response:
+        """Fetch a list of lists that belong to an actor.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetLists.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetLists.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getLists', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetLists.Response)
+
+    async def get_mutes(
+        self, params: Optional[Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
+    ) -> models.AppBskyGraphGetMutes.Response:
+        """Who does the viewer mute?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetMutes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetMutes.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.graph.getMutes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetMutes.Response)
+
+    async def mute_actor(self, data: Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
+        """Mute an actor by did or handle.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphMuteActor.Data)
+        response = await self._client.invoke_procedure(
+            'app.bsky.graph.muteActor', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    async def mute_actor_list(self, data: Union[dict, 'models.AppBskyGraphMuteActorList.Data'], **kwargs) -> bool:
+        """Mute a list of actors.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphMuteActorList.Data)
+        response = await self._client.invoke_procedure(
+            'app.bsky.graph.muteActorList', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    async def unmute_actor(self, data: Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
+        """Unmute an actor by did or handle.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphUnmuteActor.Data)
+        response = await self._client.invoke_procedure(
+            'app.bsky.graph.unmuteActor', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    async def unmute_actor_list(self, data: Union[dict, 'models.AppBskyGraphUnmuteActorList.Data'], **kwargs) -> bool:
+        """Unmute a list of actors.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphUnmuteActorList.Data)
+        response = await self._client.invoke_procedure(
+            'app.bsky.graph.unmuteActorList', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+
+@dataclass
+class FeedNamespace(NamespaceBase):
+    async def get_author_feed(
+        self, params: Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
+    ) -> models.AppBskyFeedGetAuthorFeed.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
+
+    async def get_likes(
+        self, params: Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
+    ) -> models.AppBskyFeedGetLikes.Response:
+        """Get likes.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
+
+    async def get_post_thread(
+        self, params: Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPostThread.Response:
+        """Get post thread.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
+
+    async def get_posts(
+        self, params: Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPosts.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
+
+    async def get_reposted_by(
+        self, params: Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
+    ) -> models.AppBskyFeedGetRepostedBy.Response:
+        """Get reposted by.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
+
+    async def get_timeline(
+        self, params: Optional[Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
+    ) -> models.AppBskyFeedGetTimeline.Response:
+        """A view of the user's home timeline.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
+
+
+@dataclass
+class UnspeccedNamespace(NamespaceBase):
+    async def get_popular(
+        self, params: Optional[Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
+    ) -> models.AppBskyUnspeccedGetPopular.Response:
+        """An unspecced view of globally popular items.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyUnspeccedGetPopular.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyUnspeccedGetPopular.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.unspecced.getPopular', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyUnspeccedGetPopular.Response)
+
+
+@dataclass
+class NotificationNamespace(NamespaceBase):
+    async def get_unread_count(
+        self, params: Optional[Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
+    ) -> models.AppBskyNotificationGetUnreadCount.Response:
+        """Get unread count.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyNotificationGetUnreadCount.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyNotificationGetUnreadCount.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.notification.getUnreadCount', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyNotificationGetUnreadCount.Response)
+
+    async def list_notifications(
+        self, params: Optional[Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
+    ) -> models.AppBskyNotificationListNotifications.Response:
+        """List notifications.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyNotificationListNotifications.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyNotificationListNotifications.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.notification.listNotifications', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyNotificationListNotifications.Response)
+
+    async def update_seen(self, data: Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
+        """Notify server that the user has seen notifications.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyNotificationUpdateSeen.Data)
+        response = await self._client.invoke_procedure(
+            'app.bsky.notification.updateSeen', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+
+@dataclass
 class ComNamespace(NamespaceBase):
     atproto: 'AtprotoNamespace' = field(default_factory=DefaultNamespace)
 
     def __post_init__(self):
         self.atproto = AtprotoNamespace(self._client)
 
 
@@ -779,14 +1422,34 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoRepoPutRecord.Response)
 
+    async def rebase_repo(self, data: Union[dict, 'models.ComAtprotoRepoRebaseRepo.Data'], **kwargs) -> bool:
+        """Simple rebase of repo that deletes history.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.ComAtprotoRepoRebaseRepo.Data)
+        response = await self._client.invoke_procedure(
+            'com.atproto.repo.rebaseRepo', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
     async def upload_blob(
         self, data: 'models.ComAtprotoRepoUploadBlob.Data', **kwargs
     ) -> models.ComAtprotoRepoUploadBlob.Response:
         """Upload a new blob to be added to repo in a later request.
 
         Args:
             data: Input data alias.
@@ -803,14 +1466,36 @@
             'com.atproto.repo.uploadBlob', data=data, input_encoding='*/*', output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoUploadBlob.Response)
 
 
 @dataclass
 class AdminNamespace(NamespaceBase):
+    async def disable_account_invites(
+        self, data: Union[dict, 'models.ComAtprotoAdminDisableAccountInvites.Data'], **kwargs
+    ) -> bool:
+        """Disable an account from receiving new invite codes, but does not invalidate existing codes.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.ComAtprotoAdminDisableAccountInvites.Data)
+        response = await self._client.invoke_procedure(
+            'com.atproto.admin.disableAccountInvites', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
     async def disable_invite_codes(
         self, data: Optional[Union[dict, 'models.ComAtprotoAdminDisableInviteCodes.Data']] = None, **kwargs
     ) -> bool:
         """Disable some set of codes and/or all codes associated with a set of users.
 
         Args:
             data: Input data.
@@ -825,14 +1510,36 @@
 
         data = get_or_create_model(data, models.ComAtprotoAdminDisableInviteCodes.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.admin.disableInviteCodes', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
+    async def enable_account_invites(
+        self, data: Union[dict, 'models.ComAtprotoAdminEnableAccountInvites.Data'], **kwargs
+    ) -> bool:
+        """Re-enable an accounts ability to receive invite codes.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.ComAtprotoAdminEnableAccountInvites.Data)
+        response = await self._client.invoke_procedure(
+            'com.atproto.admin.enableAccountInvites', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
     async def get_invite_codes(
         self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetInviteCodes.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetInviteCodes.Response:
         """Admin view of invite codes.
 
         Args:
             params: Parameters.
@@ -1221,502 +1928,7 @@
         """
 
         params = get_or_create_model(params, models.ComAtprotoLabelQueryLabels.Params)
         response = await self._client.invoke_query(
             'com.atproto.label.queryLabels', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoLabelQueryLabels.Response)
-
-
-@dataclass
-class AppNamespace(NamespaceBase):
-    bsky: 'BskyNamespace' = field(default_factory=DefaultNamespace)
-
-    def __post_init__(self):
-        self.bsky = BskyNamespace(self._client)
-
-
-@dataclass
-class BskyNamespace(NamespaceBase):
-    actor: 'ActorNamespace' = field(default_factory=DefaultNamespace)
-    feed: 'FeedNamespace' = field(default_factory=DefaultNamespace)
-    graph: 'GraphNamespace' = field(default_factory=DefaultNamespace)
-    notification: 'NotificationNamespace' = field(default_factory=DefaultNamespace)
-    unspecced: 'UnspeccedNamespace' = field(default_factory=DefaultNamespace)
-
-    def __post_init__(self):
-        self.actor = ActorNamespace(self._client)
-        self.feed = FeedNamespace(self._client)
-        self.graph = GraphNamespace(self._client)
-        self.notification = NotificationNamespace(self._client)
-        self.unspecced = UnspeccedNamespace(self._client)
-
-
-@dataclass
-class FeedNamespace(NamespaceBase):
-    async def get_author_feed(
-        self, params: Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
-    ) -> models.AppBskyFeedGetAuthorFeed.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
-
-    async def get_likes(
-        self, params: Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
-    ) -> models.AppBskyFeedGetLikes.Response:
-        """Get likes.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
-
-    async def get_post_thread(
-        self, params: Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPostThread.Response:
-        """Get post thread.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
-
-    async def get_posts(
-        self, params: Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPosts.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
-
-    async def get_reposted_by(
-        self, params: Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
-    ) -> models.AppBskyFeedGetRepostedBy.Response:
-        """Get reposted by.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
-
-    async def get_timeline(
-        self, params: Optional[Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
-    ) -> models.AppBskyFeedGetTimeline.Response:
-        """A view of the user's home timeline.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
-
-
-@dataclass
-class ActorNamespace(NamespaceBase):
-    async def get_profile(
-        self, params: Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
-    ) -> models.AppBskyActorGetProfile.ResponseRef:
-        """Get profile.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorGetProfile.ResponseRef`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorGetProfile.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.actor.getProfile', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorGetProfile.ResponseRef)
-
-    async def get_profiles(
-        self, params: Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
-    ) -> models.AppBskyActorGetProfiles.Response:
-        """Get profiles.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorGetProfiles.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorGetProfiles.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.actor.getProfiles', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorGetProfiles.Response)
-
-    async def get_suggestions(
-        self, params: Optional[Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
-    ) -> models.AppBskyActorGetSuggestions.Response:
-        """Get a list of actors suggested for following. Used in discovery UIs.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorGetSuggestions.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorGetSuggestions.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.actor.getSuggestions', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorGetSuggestions.Response)
-
-    async def search_actors(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
-    ) -> models.AppBskyActorSearchActors.Response:
-        """Find actors matching search criteria.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorSearchActors.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorSearchActors.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.actor.searchActors', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorSearchActors.Response)
-
-    async def search_actors_typeahead(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
-    ) -> models.AppBskyActorSearchActorsTypeahead.Response:
-        """Find actor suggestions for a search term.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorSearchActorsTypeahead.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorSearchActorsTypeahead.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.actor.searchActorsTypeahead', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
-
-
-@dataclass
-class GraphNamespace(NamespaceBase):
-    async def get_blocks(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
-    ) -> models.AppBskyGraphGetBlocks.Response:
-        """Who is the requester's account blocking?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetBlocks.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetBlocks.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.graph.getBlocks', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetBlocks.Response)
-
-    async def get_followers(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
-    ) -> models.AppBskyGraphGetFollowers.Response:
-        """Who is following an actor?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetFollowers.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetFollowers.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.graph.getFollowers', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetFollowers.Response)
-
-    async def get_follows(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
-    ) -> models.AppBskyGraphGetFollows.Response:
-        """Who is an actor following?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetFollows.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetFollows.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.graph.getFollows', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetFollows.Response)
-
-    async def get_mutes(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
-    ) -> models.AppBskyGraphGetMutes.Response:
-        """Who does the viewer mute?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetMutes.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetMutes.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.graph.getMutes', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetMutes.Response)
-
-    async def mute_actor(self, data: Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
-        """Mute an actor by did or handle.
-
-        Args:
-            data: Input data.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`bool`: Success status.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        data = get_or_create_model(data, models.AppBskyGraphMuteActor.Data)
-        response = await self._client.invoke_procedure(
-            'app.bsky.graph.muteActor', data=data, input_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, bool)
-
-    async def unmute_actor(self, data: Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
-        """Unmute an actor by did or handle.
-
-        Args:
-            data: Input data.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`bool`: Success status.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        data = get_or_create_model(data, models.AppBskyGraphUnmuteActor.Data)
-        response = await self._client.invoke_procedure(
-            'app.bsky.graph.unmuteActor', data=data, input_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, bool)
-
-
-@dataclass
-class UnspeccedNamespace(NamespaceBase):
-    async def get_popular(
-        self, params: Optional[Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
-    ) -> models.AppBskyUnspeccedGetPopular.Response:
-        """An unspecced view of globally popular items.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyUnspeccedGetPopular.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyUnspeccedGetPopular.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.unspecced.getPopular', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyUnspeccedGetPopular.Response)
-
-
-@dataclass
-class NotificationNamespace(NamespaceBase):
-    async def get_unread_count(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
-    ) -> models.AppBskyNotificationGetUnreadCount.Response:
-        """Get unread count.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyNotificationGetUnreadCount.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyNotificationGetUnreadCount.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.notification.getUnreadCount', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyNotificationGetUnreadCount.Response)
-
-    async def list_notifications(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
-    ) -> models.AppBskyNotificationListNotifications.Response:
-        """List notifications.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyNotificationListNotifications.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyNotificationListNotifications.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.notification.listNotifications', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyNotificationListNotifications.Response)
-
-    async def update_seen(self, data: Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
-        """Notify server that the user has seen notifications.
-
-        Args:
-            data: Input data.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`bool`: Success status.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        data = get_or_create_model(data, models.AppBskyNotificationUpdateSeen.Data)
-        response = await self._client.invoke_procedure(
-            'app.bsky.notification.updateSeen', data=data, input_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, bool)
```

### Comparing `atproto-0.0.4/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.5/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,657 @@
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models.utils import get_or_create_model, get_response_model
 from atproto.xrpc_client.namespaces.base import DefaultNamespace, NamespaceBase
 
 
 @dataclass
+class AppNamespace(NamespaceBase):
+    bsky: 'BskyNamespace' = field(default_factory=DefaultNamespace)
+
+    def __post_init__(self):
+        self.bsky = BskyNamespace(self._client)
+
+
+@dataclass
+class BskyNamespace(NamespaceBase):
+    actor: 'ActorNamespace' = field(default_factory=DefaultNamespace)
+    feed: 'FeedNamespace' = field(default_factory=DefaultNamespace)
+    graph: 'GraphNamespace' = field(default_factory=DefaultNamespace)
+    notification: 'NotificationNamespace' = field(default_factory=DefaultNamespace)
+    unspecced: 'UnspeccedNamespace' = field(default_factory=DefaultNamespace)
+
+    def __post_init__(self):
+        self.actor = ActorNamespace(self._client)
+        self.feed = FeedNamespace(self._client)
+        self.graph = GraphNamespace(self._client)
+        self.notification = NotificationNamespace(self._client)
+        self.unspecced = UnspeccedNamespace(self._client)
+
+
+@dataclass
+class ActorNamespace(NamespaceBase):
+    def get_preferences(
+        self, params: Optional[Union[dict, 'models.AppBskyActorGetPreferences.Params']] = None, **kwargs
+    ) -> models.AppBskyActorGetPreferences.Response:
+        """Get private preferences attached to the account.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetPreferences.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetPreferences.Params)
+        response = self._client.invoke_query(
+            'app.bsky.actor.getPreferences', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetPreferences.Response)
+
+    def get_profile(
+        self, params: Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
+    ) -> models.AppBskyActorGetProfile.ResponseRef:
+        """Get profile.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetProfile.ResponseRef`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetProfile.Params)
+        response = self._client.invoke_query(
+            'app.bsky.actor.getProfile', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetProfile.ResponseRef)
+
+    def get_profiles(
+        self, params: Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
+    ) -> models.AppBskyActorGetProfiles.Response:
+        """Get profiles.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetProfiles.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetProfiles.Params)
+        response = self._client.invoke_query(
+            'app.bsky.actor.getProfiles', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetProfiles.Response)
+
+    def get_suggestions(
+        self, params: Optional[Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
+    ) -> models.AppBskyActorGetSuggestions.Response:
+        """Get a list of actors suggested for following. Used in discovery UIs.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorGetSuggestions.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorGetSuggestions.Params)
+        response = self._client.invoke_query(
+            'app.bsky.actor.getSuggestions', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorGetSuggestions.Response)
+
+    def put_preferences(self, data: Union[dict, 'models.AppBskyActorPutPreferences.Data'], **kwargs) -> bool:
+        """Sets the private preferences attached to the account.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyActorPutPreferences.Data)
+        response = self._client.invoke_procedure(
+            'app.bsky.actor.putPreferences', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    def search_actors(
+        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
+    ) -> models.AppBskyActorSearchActors.Response:
+        """Find actors matching search criteria.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorSearchActors.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorSearchActors.Params)
+        response = self._client.invoke_query(
+            'app.bsky.actor.searchActors', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorSearchActors.Response)
+
+    def search_actors_typeahead(
+        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
+    ) -> models.AppBskyActorSearchActorsTypeahead.Response:
+        """Find actor suggestions for a search term.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyActorSearchActorsTypeahead.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyActorSearchActorsTypeahead.Params)
+        response = self._client.invoke_query(
+            'app.bsky.actor.searchActorsTypeahead', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
+
+
+@dataclass
+class GraphNamespace(NamespaceBase):
+    def get_blocks(
+        self, params: Optional[Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
+    ) -> models.AppBskyGraphGetBlocks.Response:
+        """Who is the requester's account blocking?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetBlocks.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetBlocks.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getBlocks', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetBlocks.Response)
+
+    def get_followers(
+        self, params: Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
+    ) -> models.AppBskyGraphGetFollowers.Response:
+        """Who is following an actor?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetFollowers.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetFollowers.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getFollowers', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetFollowers.Response)
+
+    def get_follows(
+        self, params: Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
+    ) -> models.AppBskyGraphGetFollows.Response:
+        """Who is an actor following?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetFollows.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetFollows.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getFollows', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetFollows.Response)
+
+    def get_list(
+        self, params: Union[dict, 'models.AppBskyGraphGetList.Params'], **kwargs
+    ) -> models.AppBskyGraphGetList.Response:
+        """Fetch a list of actors.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetList.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetList.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getList', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetList.Response)
+
+    def get_list_mutes(
+        self, params: Optional[Union[dict, 'models.AppBskyGraphGetListMutes.Params']] = None, **kwargs
+    ) -> models.AppBskyGraphGetListMutes.Response:
+        """Which lists is the requester's account muting?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetListMutes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetListMutes.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getListMutes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetListMutes.Response)
+
+    def get_lists(
+        self, params: Union[dict, 'models.AppBskyGraphGetLists.Params'], **kwargs
+    ) -> models.AppBskyGraphGetLists.Response:
+        """Fetch a list of lists that belong to an actor.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetLists.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetLists.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getLists', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetLists.Response)
+
+    def get_mutes(
+        self, params: Optional[Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
+    ) -> models.AppBskyGraphGetMutes.Response:
+        """Who does the viewer mute?
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyGraphGetMutes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyGraphGetMutes.Params)
+        response = self._client.invoke_query(
+            'app.bsky.graph.getMutes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyGraphGetMutes.Response)
+
+    def mute_actor(self, data: Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
+        """Mute an actor by did or handle.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphMuteActor.Data)
+        response = self._client.invoke_procedure(
+            'app.bsky.graph.muteActor', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    def mute_actor_list(self, data: Union[dict, 'models.AppBskyGraphMuteActorList.Data'], **kwargs) -> bool:
+        """Mute a list of actors.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphMuteActorList.Data)
+        response = self._client.invoke_procedure(
+            'app.bsky.graph.muteActorList', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    def unmute_actor(self, data: Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
+        """Unmute an actor by did or handle.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphUnmuteActor.Data)
+        response = self._client.invoke_procedure(
+            'app.bsky.graph.unmuteActor', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+    def unmute_actor_list(self, data: Union[dict, 'models.AppBskyGraphUnmuteActorList.Data'], **kwargs) -> bool:
+        """Unmute a list of actors.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyGraphUnmuteActorList.Data)
+        response = self._client.invoke_procedure(
+            'app.bsky.graph.unmuteActorList', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+
+@dataclass
+class FeedNamespace(NamespaceBase):
+    def get_author_feed(
+        self, params: Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
+    ) -> models.AppBskyFeedGetAuthorFeed.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
+
+    def get_likes(
+        self, params: Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
+    ) -> models.AppBskyFeedGetLikes.Response:
+        """Get likes.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
+
+    def get_post_thread(
+        self, params: Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPostThread.Response:
+        """Get post thread.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
+
+    def get_posts(
+        self, params: Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPosts.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
+
+    def get_reposted_by(
+        self, params: Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
+    ) -> models.AppBskyFeedGetRepostedBy.Response:
+        """Get reposted by.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
+
+    def get_timeline(
+        self, params: Optional[Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
+    ) -> models.AppBskyFeedGetTimeline.Response:
+        """A view of the user's home timeline.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
+
+
+@dataclass
+class UnspeccedNamespace(NamespaceBase):
+    def get_popular(
+        self, params: Optional[Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
+    ) -> models.AppBskyUnspeccedGetPopular.Response:
+        """An unspecced view of globally popular items.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyUnspeccedGetPopular.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyUnspeccedGetPopular.Params)
+        response = self._client.invoke_query(
+            'app.bsky.unspecced.getPopular', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyUnspeccedGetPopular.Response)
+
+
+@dataclass
+class NotificationNamespace(NamespaceBase):
+    def get_unread_count(
+        self, params: Optional[Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
+    ) -> models.AppBskyNotificationGetUnreadCount.Response:
+        """Get unread count.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyNotificationGetUnreadCount.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyNotificationGetUnreadCount.Params)
+        response = self._client.invoke_query(
+            'app.bsky.notification.getUnreadCount', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyNotificationGetUnreadCount.Response)
+
+    def list_notifications(
+        self, params: Optional[Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
+    ) -> models.AppBskyNotificationListNotifications.Response:
+        """List notifications.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyNotificationListNotifications.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyNotificationListNotifications.Params)
+        response = self._client.invoke_query(
+            'app.bsky.notification.listNotifications', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyNotificationListNotifications.Response)
+
+    def update_seen(self, data: Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
+        """Notify server that the user has seen notifications.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.AppBskyNotificationUpdateSeen.Data)
+        response = self._client.invoke_procedure(
+            'app.bsky.notification.updateSeen', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
+
+@dataclass
 class ComNamespace(NamespaceBase):
     atproto: 'AtprotoNamespace' = field(default_factory=DefaultNamespace)
 
     def __post_init__(self):
         self.atproto = AtprotoNamespace(self._client)
 
 
@@ -773,14 +1416,34 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoRepoPutRecord.Response)
 
+    def rebase_repo(self, data: Union[dict, 'models.ComAtprotoRepoRebaseRepo.Data'], **kwargs) -> bool:
+        """Simple rebase of repo that deletes history.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.ComAtprotoRepoRebaseRepo.Data)
+        response = self._client.invoke_procedure(
+            'com.atproto.repo.rebaseRepo', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
     def upload_blob(
         self, data: 'models.ComAtprotoRepoUploadBlob.Data', **kwargs
     ) -> models.ComAtprotoRepoUploadBlob.Response:
         """Upload a new blob to be added to repo in a later request.
 
         Args:
             data: Input data alias.
@@ -797,14 +1460,36 @@
             'com.atproto.repo.uploadBlob', data=data, input_encoding='*/*', output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoUploadBlob.Response)
 
 
 @dataclass
 class AdminNamespace(NamespaceBase):
+    def disable_account_invites(
+        self, data: Union[dict, 'models.ComAtprotoAdminDisableAccountInvites.Data'], **kwargs
+    ) -> bool:
+        """Disable an account from receiving new invite codes, but does not invalidate existing codes.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.ComAtprotoAdminDisableAccountInvites.Data)
+        response = self._client.invoke_procedure(
+            'com.atproto.admin.disableAccountInvites', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
     def disable_invite_codes(
         self, data: Optional[Union[dict, 'models.ComAtprotoAdminDisableInviteCodes.Data']] = None, **kwargs
     ) -> bool:
         """Disable some set of codes and/or all codes associated with a set of users.
 
         Args:
             data: Input data.
@@ -819,14 +1504,36 @@
 
         data = get_or_create_model(data, models.ComAtprotoAdminDisableInviteCodes.Data)
         response = self._client.invoke_procedure(
             'com.atproto.admin.disableInviteCodes', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
+    def enable_account_invites(
+        self, data: Union[dict, 'models.ComAtprotoAdminEnableAccountInvites.Data'], **kwargs
+    ) -> bool:
+        """Re-enable an accounts ability to receive invite codes.
+
+        Args:
+            data: Input data.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        data = get_or_create_model(data, models.ComAtprotoAdminEnableAccountInvites.Data)
+        response = self._client.invoke_procedure(
+            'com.atproto.admin.enableAccountInvites', data=data, input_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, bool)
+
     def get_invite_codes(
         self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetInviteCodes.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetInviteCodes.Response:
         """Admin view of invite codes.
 
         Args:
             params: Parameters.
@@ -1215,502 +1922,7 @@
         """
 
         params = get_or_create_model(params, models.ComAtprotoLabelQueryLabels.Params)
         response = self._client.invoke_query(
             'com.atproto.label.queryLabels', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoLabelQueryLabels.Response)
-
-
-@dataclass
-class AppNamespace(NamespaceBase):
-    bsky: 'BskyNamespace' = field(default_factory=DefaultNamespace)
-
-    def __post_init__(self):
-        self.bsky = BskyNamespace(self._client)
-
-
-@dataclass
-class BskyNamespace(NamespaceBase):
-    actor: 'ActorNamespace' = field(default_factory=DefaultNamespace)
-    feed: 'FeedNamespace' = field(default_factory=DefaultNamespace)
-    graph: 'GraphNamespace' = field(default_factory=DefaultNamespace)
-    notification: 'NotificationNamespace' = field(default_factory=DefaultNamespace)
-    unspecced: 'UnspeccedNamespace' = field(default_factory=DefaultNamespace)
-
-    def __post_init__(self):
-        self.actor = ActorNamespace(self._client)
-        self.feed = FeedNamespace(self._client)
-        self.graph = GraphNamespace(self._client)
-        self.notification = NotificationNamespace(self._client)
-        self.unspecced = UnspeccedNamespace(self._client)
-
-
-@dataclass
-class FeedNamespace(NamespaceBase):
-    def get_author_feed(
-        self, params: Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
-    ) -> models.AppBskyFeedGetAuthorFeed.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
-
-    def get_likes(
-        self, params: Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
-    ) -> models.AppBskyFeedGetLikes.Response:
-        """Get likes.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
-
-    def get_post_thread(
-        self, params: Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPostThread.Response:
-        """Get post thread.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
-
-    def get_posts(
-        self, params: Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPosts.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
-
-    def get_reposted_by(
-        self, params: Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
-    ) -> models.AppBskyFeedGetRepostedBy.Response:
-        """Get reposted by.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
-
-    def get_timeline(
-        self, params: Optional[Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
-    ) -> models.AppBskyFeedGetTimeline.Response:
-        """A view of the user's home timeline.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
-
-
-@dataclass
-class ActorNamespace(NamespaceBase):
-    def get_profile(
-        self, params: Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
-    ) -> models.AppBskyActorGetProfile.ResponseRef:
-        """Get profile.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorGetProfile.ResponseRef`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorGetProfile.Params)
-        response = self._client.invoke_query(
-            'app.bsky.actor.getProfile', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorGetProfile.ResponseRef)
-
-    def get_profiles(
-        self, params: Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
-    ) -> models.AppBskyActorGetProfiles.Response:
-        """Get profiles.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorGetProfiles.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorGetProfiles.Params)
-        response = self._client.invoke_query(
-            'app.bsky.actor.getProfiles', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorGetProfiles.Response)
-
-    def get_suggestions(
-        self, params: Optional[Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
-    ) -> models.AppBskyActorGetSuggestions.Response:
-        """Get a list of actors suggested for following. Used in discovery UIs.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorGetSuggestions.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorGetSuggestions.Params)
-        response = self._client.invoke_query(
-            'app.bsky.actor.getSuggestions', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorGetSuggestions.Response)
-
-    def search_actors(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
-    ) -> models.AppBskyActorSearchActors.Response:
-        """Find actors matching search criteria.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorSearchActors.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorSearchActors.Params)
-        response = self._client.invoke_query(
-            'app.bsky.actor.searchActors', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorSearchActors.Response)
-
-    def search_actors_typeahead(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
-    ) -> models.AppBskyActorSearchActorsTypeahead.Response:
-        """Find actor suggestions for a search term.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyActorSearchActorsTypeahead.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyActorSearchActorsTypeahead.Params)
-        response = self._client.invoke_query(
-            'app.bsky.actor.searchActorsTypeahead', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
-
-
-@dataclass
-class GraphNamespace(NamespaceBase):
-    def get_blocks(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
-    ) -> models.AppBskyGraphGetBlocks.Response:
-        """Who is the requester's account blocking?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetBlocks.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetBlocks.Params)
-        response = self._client.invoke_query(
-            'app.bsky.graph.getBlocks', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetBlocks.Response)
-
-    def get_followers(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
-    ) -> models.AppBskyGraphGetFollowers.Response:
-        """Who is following an actor?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetFollowers.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetFollowers.Params)
-        response = self._client.invoke_query(
-            'app.bsky.graph.getFollowers', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetFollowers.Response)
-
-    def get_follows(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
-    ) -> models.AppBskyGraphGetFollows.Response:
-        """Who is an actor following?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetFollows.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetFollows.Params)
-        response = self._client.invoke_query(
-            'app.bsky.graph.getFollows', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetFollows.Response)
-
-    def get_mutes(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
-    ) -> models.AppBskyGraphGetMutes.Response:
-        """Who does the viewer mute?
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyGraphGetMutes.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyGraphGetMutes.Params)
-        response = self._client.invoke_query(
-            'app.bsky.graph.getMutes', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyGraphGetMutes.Response)
-
-    def mute_actor(self, data: Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
-        """Mute an actor by did or handle.
-
-        Args:
-            data: Input data.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`bool`: Success status.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        data = get_or_create_model(data, models.AppBskyGraphMuteActor.Data)
-        response = self._client.invoke_procedure(
-            'app.bsky.graph.muteActor', data=data, input_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, bool)
-
-    def unmute_actor(self, data: Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
-        """Unmute an actor by did or handle.
-
-        Args:
-            data: Input data.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`bool`: Success status.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        data = get_or_create_model(data, models.AppBskyGraphUnmuteActor.Data)
-        response = self._client.invoke_procedure(
-            'app.bsky.graph.unmuteActor', data=data, input_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, bool)
-
-
-@dataclass
-class UnspeccedNamespace(NamespaceBase):
-    def get_popular(
-        self, params: Optional[Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
-    ) -> models.AppBskyUnspeccedGetPopular.Response:
-        """An unspecced view of globally popular items.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyUnspeccedGetPopular.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyUnspeccedGetPopular.Params)
-        response = self._client.invoke_query(
-            'app.bsky.unspecced.getPopular', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyUnspeccedGetPopular.Response)
-
-
-@dataclass
-class NotificationNamespace(NamespaceBase):
-    def get_unread_count(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
-    ) -> models.AppBskyNotificationGetUnreadCount.Response:
-        """Get unread count.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyNotificationGetUnreadCount.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyNotificationGetUnreadCount.Params)
-        response = self._client.invoke_query(
-            'app.bsky.notification.getUnreadCount', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyNotificationGetUnreadCount.Response)
-
-    def list_notifications(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
-    ) -> models.AppBskyNotificationListNotifications.Response:
-        """List notifications.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyNotificationListNotifications.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyNotificationListNotifications.Params)
-        response = self._client.invoke_query(
-            'app.bsky.notification.listNotifications', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyNotificationListNotifications.Response)
-
-    def update_seen(self, data: Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
-        """Notify server that the user has seen notifications.
-
-        Args:
-            data: Input data.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`bool`: Success status.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        data = get_or_create_model(data, models.AppBskyNotificationUpdateSeen.Data)
-        response = self._client.invoke_procedure(
-            'app.bsky.notification.updateSeen', data=data, input_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, bool)
```

### Comparing `atproto-0.0.4/atproto/xrpc_client/request.py` & `atproto-0.0.5/atproto/xrpc_client/request.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.4/pyproject.toml` & `atproto-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.4"
+version = "0.0.5" # placeholder. Dynamic version from Git Tag
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
@@ -33,27 +33,37 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = "0.24.0"
 dacite = "1.8.0"
 multiformats = "0.2.1"
 typing-extensions = "4.5.0"
+dag-cbor = "0.3.2"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 isort = "5.11.5"
 sphinx = "5.3.0"
 myst-parser = "1.0.0"
 sphinx-copybutton = "0.5.2"
 sphinx-favicon = "1.0.1"
 furo = "2023.3.27"
 sphinxext-opengraph = "0.8.2"
 
+# poetry self add "poetry-dynamic-versioning[plugin]"
+[tool.poetry-dynamic-versioning]
+enable = false
+strict = true
+bump = true
+metadata = false
+vcs = "git"
+style = "pep440"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `atproto-0.0.4/PKG-INFO` & `atproto-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.4
+Version: 0.0.5
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 Requires-Python: >=3.7,<4.0
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
 Requires-Dist: dacite (==1.8.0)
+Requires-Dist: dag-cbor (==0.3.2)
 Requires-Dist: httpx (==0.24.0)
 Requires-Dist: multiformats (==0.2.1)
 Requires-Dist: typing-extensions (==4.5.0)
 Project-URL: Author, https://github.com/MarshalX
 Project-URL: Documentation, https://atproto.rtfd.io
 Project-URL: Repository, https://github.com/MarshalX/atproto
 Project-URL: Tracker, https://github.com/MarshalX/atproto/issues
@@ -240,37 +241,37 @@
 The instances of data and params models should be passed as arguments to the methods that were described above.
 
 Dict-based:
 ```python
 from atproto import Client
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 # The params model will be created automatically internally for you!
 print(client.com.atproto.identity.resolve_handle({'handle': 'marshal.dev'}))
 ```
 
 Class-based:
 ```python
 from atproto import Client, models
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 params = models.ComAtprotoIdentityResolveHandle.Params('marshal.dev')
 print(client.com.atproto.identity.resolve_handle(params))
 ```
 
 Class-based with keywords:
 ```python
 from atproto import Client, models
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 params = models.ComAtprotoIdentityResolveHandle.Params(handle='marshal.dev')
 print(client.com.atproto.identity.resolve_handle(params))
 ```
 
 Tip: look at typehint of the method to figure out the name and the path to the input/data model!
 
@@ -281,15 +282,15 @@
 This is how we can send a post with the image using low-level XRPC Client:
 ```python
 from datetime import datetime
 
 from atproto import Client, models
 
 
-client=Client()
+client = Client()
 client.login('my-username', 'my-password')
 
 with open('cat.jpg', 'rb') as f:
     img_data = f.read()
 
     upload = client.com.atproto.repo.upload_blob(img_data)
     images = [models.AppBskyEmbedImages.Image(alt='Img alt', image=upload.blob)]
```

