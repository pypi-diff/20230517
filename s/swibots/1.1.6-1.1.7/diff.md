# Comparing `tmp/swibots-1.1.6.tar.gz` & `tmp/swibots-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.1.6.tar", last modified: Tue May 16 11:53:25 2023, max compression
+gzip compressed data, was "swibots-1.1.7.tar", last modified: Wed May 17 11:23:34 2023, max compression
```

## Comparing `swibots-1.1.6.tar` & `swibots-1.1.7.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.600408 swibots-1.1.6/
--rw-rw-rw-   0        0        0     1892 2023-05-16 11:53:25.597411 swibots-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2023-02-13 07:44:30.000000 swibots-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 11:53:25.601411 swibots-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-05-16 11:46:42.000000 swibots-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:24.981410 swibots-1.1.6/swibots/
--rw-rw-rw-   0        0        0      236 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.064413 swibots-1.1.6/swibots/api/
--rw-rw-rw-   0        0        0      140 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/__init__.py
--rw-rw-rw-   0        0        0     2236 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.070413 swibots-1.1.6/swibots/api/auth/
--rw-rw-rw-   0        0        0       85 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/auth_client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.076408 swibots-1.1.6/swibots/api/auth/controllers/
--rw-rw-rw-   0        0        0       73 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/controllers/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/controllers/user_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.085426 swibots-1.1.6/swibots/api/auth/methods/
--rw-rw-rw-   0        0        0       94 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/methods/__init__.py
--rw-rw-rw-   0        0        0      650 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/methods/get_me.py
--rw-rw-rw-   0        0        0      837 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/methods/login.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.091409 swibots-1.1.6/swibots/api/auth/models/
--rw-rw-rw-   0        0        0       56 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/models/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/auth/models/auth_user.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.097411 swibots-1.1.6/swibots/api/bot/
--rw-rw-rw-   0        0        0       83 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/bot_client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.103409 swibots-1.1.6/swibots/api/bot/controllers/
--rw-rw-rw-   0        0        0       71 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/controllers/__init__.py
--rw-rw-rw-   0        0        0     1790 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/controllers/bot_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.114411 swibots-1.1.6/swibots/api/bot/methods/
--rw-rw-rw-   0        0        0      209 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/methods/__init__.py
--rw-rw-rw-   0        0        0      540 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/methods/delete_bot_info.py
--rw-rw-rw-   0        0        0      582 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/methods/get_bot_info.py
--rw-rw-rw-   0        0        0      615 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/methods/update_bot_info.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.124412 swibots-1.1.6/swibots/api/bot/models/
--rw-rw-rw-   0        0        0      116 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/models/__init__.py
--rw-rw-rw-   0        0        0      955 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/models/bot_command_info.py
--rw-rw-rw-   0        0        0     1585 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/bot/models/bot_info.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.130410 swibots-1.1.6/swibots/api/chat/
--rw-rw-rw-   0        0        0      107 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/__init__.py
--rw-rw-rw-   0        0        0     5372 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/chat_client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.135439 swibots-1.1.6/swibots/api/chat/controllers/
--rw-rw-rw-   0        0        0       83 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/controllers/__init__.py
--rw-rw-rw-   0        0        0    21518 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/controllers/message_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.160414 swibots-1.1.6/swibots/api/chat/events/
--rw-rw-rw-   0        0        0      326 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/events/__init__.py
--rw-rw-rw-   0        0        0     2073 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/events/callback_query_event.py
--rw-rw-rw-   0        0        0     2731 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/events/chat_event.py
--rw-rw-rw-   0        0        0     2095 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/events/command_event.py
--rw-rw-rw-   0        0        0     2103 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/events/inline_query_event.py
--rw-rw-rw-   0        0        0     2434 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/events/message_event.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.249411 swibots-1.1.6/swibots/api/chat/methods/
--rw-rw-rw-   0        0        0     1709 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/__init__.py
--rw-rw-rw-   0        0        0      654 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/answer_inline_query.py
--rw-rw-rw-   0        0        0      693 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/clear_conversation.py
--rw-rw-rw-   0        0        0      705 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/delete_message.py
--rw-rw-rw-   0        0        0      707 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/delete_messages_from_user.py
--rw-rw-rw-   0        0        0     1358 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/download_media.py
--rw-rw-rw-   0        0        0      750 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/edit_message.py
--rw-rw-rw-   0        0        0      853 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/edit_message_text.py
--rw-rw-rw-   0        0        0      693 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/flag_message.py
--rw-rw-rw-   0        0        0     1192 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/forward_message.py
--rw-rw-rw-   0        0        0     1139 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_channel_chat_history.py
--rw-rw-rw-   0        0        0      725 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_community_media_files.py
--rw-rw-rw-   0        0        0      883 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_community_media_files_by_status.py
--rw-rw-rw-   0        0        0      636 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_flag_messages.py
--rw-rw-rw-   0        0        0     1090 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_group_chat_history.py
--rw-rw-rw-   0        0        0      649 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_message.py
--rw-rw-rw-   0        0        0      707 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_messages.py
--rw-rw-rw-   0        0        0     1102 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_messages_between_users.py
--rw-rw-rw-   0        0        0      560 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_unread_messages_count.py
--rw-rw-rw-   0        0        0      785 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/get_user_media_files.py
--rw-rw-rw-   0        0        0      881 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/reply_message.py
--rw-rw-rw-   0        0        0     1032 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/reply_message_text.py
--rw-rw-rw-   0        0        0      849 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/send_message.py
--rw-rw-rw-   0        0        0     1136 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/methods/send_text.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.274410 swibots-1.1.6/swibots/api/chat/models/
--rw-rw-rw-   0        0        0      305 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/__init__.py
--rw-rw-rw-   0        0        0      920 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/group_chat_history.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.306410 swibots-1.1.6/swibots/api/chat/models/inline/
--rw-rw-rw-   0        0        0      565 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query.py
--rw-rw-rw-   0        0        0     1871 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query_answer.py
--rw-rw-rw-   0        0        0      991 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result.py
--rw-rw-rw-   0        0        0     1158 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-rw-   0        0        0     1273 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-rw-   0        0        0     1620 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     1760 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_video.py
--rw-rw-rw-   0        0        0      581 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/input_message_content.py
--rw-rw-rw-   0        0        0      201 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline/types.py
--rw-rw-rw-   0        0        0      886 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline_keyboard_button.py
--rw-rw-rw-   0        0        0      170 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline_keyboard_color.py
--rw-rw-rw-   0        0        0      146 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline_keyboard_size.py
--rw-rw-rw-   0        0        0     2065 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/inline_markup.py
--rw-rw-rw-   0        0        0    10769 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/chat/models/message.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.309411 swibots-1.1.6/swibots/api/common/
--rw-rw-rw-   0        0        0       44 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.316412 swibots-1.1.6/swibots/api/common/events/
--rw-rw-rw-   0        0        0       46 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/events/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/events/event.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.327408 swibots-1.1.6/swibots/api/common/models/
--rw-rw-rw-   0        0        0      101 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/models/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/models/media.py
--rw-rw-rw-   0        0        0     1565 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/models/media_upload_request.py
--rw-rw-rw-   0        0        0     1706 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/common/models/user.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.333414 swibots-1.1.6/swibots/api/community/
--rw-rw-rw-   0        0        0       90 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/__init__.py
--rw-rw-rw-   0        0        0     5180 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/community_client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.345411 swibots-1.1.6/swibots/api/community/controllers/
--rw-rw-rw-   0        0        0      102 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/controllers/__init__.py
--rw-rw-rw-   0        0        0      595 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/controllers/channel_controller.py
--rw-rw-rw-   0        0        0      616 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/controllers/community_controller.py
--rw-rw-rw-   0        0        0      576 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/controllers/group_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.382411 swibots-1.1.6/swibots/api/community/events/
--rw-rw-rw-   0        0        0      566 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/events/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/channel_created_event.py
--rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/channel_deleted_event.py
--rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/channel_updated_event.py
--rw-rw-rw-   0        0        0     2303 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/events/community_event.py
--rw-rw-rw-   0        0        0     1383 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/events/community_updated_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/group_created_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/group_deleted_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/group_updated_event.py
--rw-rw-rw-   0        0        0     1421 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/member_joined_event.py
--rw-rw-rw-   0        0        0     1418 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/member_left_event.py
--rw-rw-rw-   0        0        0     1414 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/api/community/events/user_banned_event.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.395410 swibots-1.1.6/swibots/api/community/methods/
--rw-rw-rw-   0        0        0      194 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/methods/__init__.py
--rw-rw-rw-   0        0        0      643 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/methods/get_channel.py
--rw-rw-rw-   0        0        0      668 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/methods/get_community.py
--rw-rw-rw-   0        0        0      619 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/methods/get_group.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.411414 swibots-1.1.6/swibots/api/community/models/
--rw-rw-rw-   0        0        0      132 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/models/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/models/channel.py
--rw-rw-rw-   0        0        0     2954 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/models/community.py
--rw-rw-rw-   0        0        0     2720 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/api/community/models/group.py
--rw-rw-rw-   0        0        0     9347 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/app.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.435412 swibots-1.1.6/swibots/base/
--rw-rw-rw-   0        0        0      262 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/__init__.py
--rw-rw-rw-   0        0        0       69 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/rest_controller.py
--rw-rw-rw-   0        0        0      370 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/rest_request.py
--rw-rw-rw-   0        0        0      644 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/rest_response.py
--rw-rw-rw-   0        0        0     4261 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/switch_client.py
--rw-rw-rw-   0        0        0     1180 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/switch_object.py
--rw-rw-rw-   0        0        0      543 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/base/switch_ws_async_client.py
--rw-rw-rw-   0        0        0     4329 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bot_app.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.457410 swibots-1.1.6/swibots/bots/
--rw-rw-rw-   0        0        0      201 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/__init__.py
--rw-rw-rw-   0        0        0     4646 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/bot.py
--rw-rw-rw-   0        0        0     1646 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/bot_context.py
--rw-rw-rw-   0        0        0      109 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.506410 swibots-1.1.6/swibots/bots/decorators/
--rw-rw-rw-   0        0        0      999 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/__init__.py
--rw-rw-rw-   0        0        0      540 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0      510 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_channel_created.py
--rw-rw-rw-   0        0        0      544 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_channel_deleted.py
--rw-rw-rw-   0        0        0      541 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_channel_updated.py
--rw-rw-rw-   0        0        0      574 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_command.py
--rw-rw-rw-   0        0        0      544 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_community_updated.py
--rw-rw-rw-   0        0        0      536 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_group_created.py
--rw-rw-rw-   0        0        0      536 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_group_deleted.py
--rw-rw-rw-   0        0        0      534 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_group_updated.py
--rw-rw-rw-   0        0        0      537 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0      534 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_member_joined.py
--rw-rw-rw-   0        0        0      529 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_member_left.py
--rw-rw-rw-   0        0        0      503 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_message.py
--rw-rw-rw-   0        0        0      543 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_unknown_command.py
--rw-rw-rw-   0        0        0      509 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/decorators/on_user_banned.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.511412 swibots-1.1.6/swibots/bots/filters/
--rw-rw-rw-   0        0        0       22 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/filters/__init__.py
--rw-rw-rw-   0        0        0     8057 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/filters/filter.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.565413 swibots-1.1.6/swibots/bots/handlers/
--rw-rw-rw-   0        0        0     1300 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/base_handler.py
--rw-rw-rw-   0        0        0      985 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0      704 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/channel_created_handler.py
--rw-rw-rw-   0        0        0      711 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/channel_deleted_handler.py
--rw-rw-rw-   0        0        0      758 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/channel_updated_handler.py
--rw-rw-rw-   0        0        0     1514 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/command_handler.py
--rw-rw-rw-   0        0        0      686 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/community_updated_handler.py
--rw-rw-rw-   0        0        0     1325 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/event_handler.py
--rw-rw-rw-   0        0        0      703 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/group_created_handler.py
--rw-rw-rw-   0        0        0      800 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/group_deleted_handler.py
--rw-rw-rw-   0        0        0      800 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/group_updated_handler.py
--rw-rw-rw-   0        0        0      867 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0      702 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/member_joined_handler.py
--rw-rw-rw-   0        0        0      697 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/member_left_handler.py
--rw-rw-rw-   0        0        0      960 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/message_handler.py
--rw-rw-rw-   0        0        0      885 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/handlers/unknown_command_handler.py
--rw-rw-rw-   0        0        0      693 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/bots/handlers/user_banned_handler.py
--rw-rw-rw-   0        0        0      285 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/bots/register_command.py
--rw-rw-rw-   0        0        0     1645 2023-05-16 11:45:38.000000 swibots-1.1.6/swibots/config.py
--rw-rw-rw-   0        0        0     1333 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/error.py
--rw-rw-rw-   0        0        0      878 2023-05-16 11:13:47.000000 swibots-1.1.6/swibots/types.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.575409 swibots-1.1.6/swibots/utils/
--rw-rw-rw-   0        0        0       75 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/__init__.py
--rw-rw-rw-   0        0        0     5880 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/rest_client.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.578409 swibots-1.1.6/swibots/utils/ws/
--rw-rw-rw-   0        0        0       48 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.588409 swibots-1.1.6/swibots/utils/ws/asyncstomp/
--rw-rw-rw-   0        0        0      150 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-rw-   0        0        0     9743 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-rw-   0        0        0      980 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.595409 swibots-1.1.6/swibots/utils/ws/common/
--rw-rw-rw-   0        0        0      100 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/common/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/common/ws_frame.py
--rw-rw-rw-   0        0        0      430 2023-02-13 07:44:31.000000 swibots-1.1.6/swibots/utils/ws/common/ws_message.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:53:25.058408 swibots-1.1.6/swibots.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-05-16 11:53:24.000000 swibots-1.1.6/swibots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7283 2023-05-16 11:53:24.000000 swibots-1.1.6/swibots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:53:24.000000 swibots-1.1.6/swibots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-16 11:53:24.000000 swibots-1.1.6/swibots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 11:53:24.000000 swibots-1.1.6/swibots.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:34.413421 swibots-1.1.7/
+-rw-rw-rw-   0        0        0     1892 2023-05-17 11:23:34.412420 swibots-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1538 2023-02-13 07:44:30.000000 swibots-1.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:23:34.414424 swibots-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-05-17 11:22:26.000000 swibots-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:30.900147 swibots-1.1.7/swibots/
+-rw-rw-rw-   0        0        0      236 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.000149 swibots-1.1.7/swibots/api/
+-rw-rw-rw-   0        0        0      140 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/__init__.py
+-rw-rw-rw-   0        0        0     2236 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.036147 swibots-1.1.7/swibots/api/auth/
+-rw-rw-rw-   0        0        0       85 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/__init__.py
+-rw-rw-rw-   0        0        0     1220 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/auth_client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.078149 swibots-1.1.7/swibots/api/auth/controllers/
+-rw-rw-rw-   0        0        0       73 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/controllers/user_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.155147 swibots-1.1.7/swibots/api/auth/methods/
+-rw-rw-rw-   0        0        0       94 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/methods/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/methods/get_me.py
+-rw-rw-rw-   0        0        0      837 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/methods/login.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.198146 swibots-1.1.7/swibots/api/auth/models/
+-rw-rw-rw-   0        0        0       56 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/models/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/auth/models/auth_user.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.245147 swibots-1.1.7/swibots/api/bot/
+-rw-rw-rw-   0        0        0       83 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/bot_client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.286146 swibots-1.1.7/swibots/api/bot/controllers/
+-rw-rw-rw-   0        0        0       71 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1790 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/controllers/bot_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.371691 swibots-1.1.7/swibots/api/bot/methods/
+-rw-rw-rw-   0        0        0      209 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/methods/__init__.py
+-rw-rw-rw-   0        0        0      540 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/methods/delete_bot_info.py
+-rw-rw-rw-   0        0        0      582 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/methods/get_bot_info.py
+-rw-rw-rw-   0        0        0      615 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/methods/update_bot_info.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.433691 swibots-1.1.7/swibots/api/bot/models/
+-rw-rw-rw-   0        0        0      116 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/models/__init__.py
+-rw-rw-rw-   0        0        0      955 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/models/bot_command_info.py
+-rw-rw-rw-   0        0        0     1585 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/bot/models/bot_info.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.475696 swibots-1.1.7/swibots/api/chat/
+-rw-rw-rw-   0        0        0      107 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/__init__.py
+-rw-rw-rw-   0        0        0     5372 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/chat_client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.521691 swibots-1.1.7/swibots/api/chat/controllers/
+-rw-rw-rw-   0        0        0       83 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/controllers/__init__.py
+-rw-rw-rw-   0        0        0    21518 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/controllers/message_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:31.663691 swibots-1.1.7/swibots/api/chat/events/
+-rw-rw-rw-   0        0        0      326 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/events/__init__.py
+-rw-rw-rw-   0        0        0     2073 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/events/callback_query_event.py
+-rw-rw-rw-   0        0        0     2731 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/events/chat_event.py
+-rw-rw-rw-   0        0        0     2095 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/events/command_event.py
+-rw-rw-rw-   0        0        0     2103 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/events/inline_query_event.py
+-rw-rw-rw-   0        0        0     2434 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/events/message_event.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.247690 swibots-1.1.7/swibots/api/chat/methods/
+-rw-rw-rw-   0        0        0     1709 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/__init__.py
+-rw-rw-rw-   0        0        0      654 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/answer_inline_query.py
+-rw-rw-rw-   0        0        0      693 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/clear_conversation.py
+-rw-rw-rw-   0        0        0      705 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/delete_message.py
+-rw-rw-rw-   0        0        0      707 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/delete_messages_from_user.py
+-rw-rw-rw-   0        0        0     1358 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/download_media.py
+-rw-rw-rw-   0        0        0      750 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/edit_message.py
+-rw-rw-rw-   0        0        0      853 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/edit_message_text.py
+-rw-rw-rw-   0        0        0      693 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/flag_message.py
+-rw-rw-rw-   0        0        0     1192 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/forward_message.py
+-rw-rw-rw-   0        0        0     1139 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_channel_chat_history.py
+-rw-rw-rw-   0        0        0      725 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_community_media_files.py
+-rw-rw-rw-   0        0        0      883 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rw-rw-rw-   0        0        0      636 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_flag_messages.py
+-rw-rw-rw-   0        0        0     1090 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_group_chat_history.py
+-rw-rw-rw-   0        0        0      649 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_message.py
+-rw-rw-rw-   0        0        0      707 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_messages.py
+-rw-rw-rw-   0        0        0     1102 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_messages_between_users.py
+-rw-rw-rw-   0        0        0      560 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_unread_messages_count.py
+-rw-rw-rw-   0        0        0      785 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/get_user_media_files.py
+-rw-rw-rw-   0        0        0      881 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/reply_message.py
+-rw-rw-rw-   0        0        0     1032 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/reply_message_text.py
+-rw-rw-rw-   0        0        0      849 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/send_message.py
+-rw-rw-rw-   0        0        0     1136 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/methods/send_text.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.428254 swibots-1.1.7/swibots/api/chat/models/
+-rw-rw-rw-   0        0        0      305 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/__init__.py
+-rw-rw-rw-   0        0        0      920 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/group_chat_history.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.680756 swibots-1.1.7/swibots/api/chat/models/inline/
+-rw-rw-rw-   0        0        0      565 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query.py
+-rw-rw-rw-   0        0        0     1871 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query_answer.py
+-rw-rw-rw-   0        0        0      991 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result.py
+-rw-rw-rw-   0        0        0     1158 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     1273 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     1620 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     1760 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_video.py
+-rw-rw-rw-   0        0        0      581 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/input_message_content.py
+-rw-rw-rw-   0        0        0      201 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline/types.py
+-rw-rw-rw-   0        0        0      886 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0      170 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline_keyboard_color.py
+-rw-rw-rw-   0        0        0      146 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline_keyboard_size.py
+-rw-rw-rw-   0        0        0     2065 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/inline_markup.py
+-rw-rw-rw-   0        0        0    10769 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/chat/models/message.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.698755 swibots-1.1.7/swibots/api/common/
+-rw-rw-rw-   0        0        0       44 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.736757 swibots-1.1.7/swibots/api/common/events/
+-rw-rw-rw-   0        0        0       46 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/events/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/events/event.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.818759 swibots-1.1.7/swibots/api/common/models/
+-rw-rw-rw-   0        0        0      101 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/models/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/models/media.py
+-rw-rw-rw-   0        0        0     1565 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/models/media_upload_request.py
+-rw-rw-rw-   0        0        0     1706 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/common/models/user.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.861756 swibots-1.1.7/swibots/api/community/
+-rw-rw-rw-   0        0        0       90 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/__init__.py
+-rw-rw-rw-   0        0        0     5180 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/community_client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:32.950755 swibots-1.1.7/swibots/api/community/controllers/
+-rw-rw-rw-   0        0        0      102 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/controllers/__init__.py
+-rw-rw-rw-   0        0        0      595 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/controllers/channel_controller.py
+-rw-rw-rw-   0        0        0      616 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/controllers/community_controller.py
+-rw-rw-rw-   0        0        0      576 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/controllers/group_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.189756 swibots-1.1.7/swibots/api/community/events/
+-rw-rw-rw-   0        0        0      566 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/events/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/channel_created_event.py
+-rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/channel_deleted_event.py
+-rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/channel_updated_event.py
+-rw-rw-rw-   0        0        0     2303 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/events/community_event.py
+-rw-rw-rw-   0        0        0     1383 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/events/community_updated_event.py
+-rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/group_created_event.py
+-rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/group_deleted_event.py
+-rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/group_updated_event.py
+-rw-rw-rw-   0        0        0     1421 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/member_joined_event.py
+-rw-rw-rw-   0        0        0     1418 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/member_left_event.py
+-rw-rw-rw-   0        0        0     1414 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/api/community/events/user_banned_event.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.263756 swibots-1.1.7/swibots/api/community/methods/
+-rw-rw-rw-   0        0        0      194 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/methods/__init__.py
+-rw-rw-rw-   0        0        0      643 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/methods/get_channel.py
+-rw-rw-rw-   0        0        0      668 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/methods/get_community.py
+-rw-rw-rw-   0        0        0      619 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/methods/get_group.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.339759 swibots-1.1.7/swibots/api/community/models/
+-rw-rw-rw-   0        0        0      132 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/models/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/models/channel.py
+-rw-rw-rw-   0        0        0     2954 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/models/community.py
+-rw-rw-rw-   0        0        0     2720 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/api/community/models/group.py
+-rw-rw-rw-   0        0        0     9347 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/app.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.467419 swibots-1.1.7/swibots/base/
+-rw-rw-rw-   0        0        0      262 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/rest_controller.py
+-rw-rw-rw-   0        0        0      370 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/rest_request.py
+-rw-rw-rw-   0        0        0      644 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/rest_response.py
+-rw-rw-rw-   0        0        0     4261 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/switch_client.py
+-rw-rw-rw-   0        0        0     1180 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/switch_object.py
+-rw-rw-rw-   0        0        0      543 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/base/switch_ws_async_client.py
+-rw-rw-rw-   0        0        0     4329 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bot_app.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.559422 swibots-1.1.7/swibots/bots/
+-rw-rw-rw-   0        0        0      201 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/__init__.py
+-rw-rw-rw-   0        0        0     4646 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/bot.py
+-rw-rw-rw-   0        0        0     1646 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/bot_context.py
+-rw-rw-rw-   0        0        0      109 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.826424 swibots-1.1.7/swibots/bots/decorators/
+-rw-rw-rw-   0        0        0      999 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/__init__.py
+-rw-rw-rw-   0        0        0      540 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0      510 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_channel_created.py
+-rw-rw-rw-   0        0        0      544 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_channel_deleted.py
+-rw-rw-rw-   0        0        0      541 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_channel_updated.py
+-rw-rw-rw-   0        0        0      574 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_command.py
+-rw-rw-rw-   0        0        0      544 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_community_updated.py
+-rw-rw-rw-   0        0        0      536 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_group_created.py
+-rw-rw-rw-   0        0        0      536 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_group_deleted.py
+-rw-rw-rw-   0        0        0      534 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_group_updated.py
+-rw-rw-rw-   0        0        0      537 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0      534 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_member_joined.py
+-rw-rw-rw-   0        0        0      529 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_member_left.py
+-rw-rw-rw-   0        0        0      503 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_message.py
+-rw-rw-rw-   0        0        0      543 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_unknown_command.py
+-rw-rw-rw-   0        0        0      509 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/decorators/on_user_banned.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:33.864419 swibots-1.1.7/swibots/bots/filters/
+-rw-rw-rw-   0        0        0       22 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/filters/__init__.py
+-rw-rw-rw-   0        0        0     8057 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/filters/filter.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:34.204422 swibots-1.1.7/swibots/bots/handlers/
+-rw-rw-rw-   0        0        0     1300 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/base_handler.py
+-rw-rw-rw-   0        0        0      985 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0      704 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/channel_created_handler.py
+-rw-rw-rw-   0        0        0      711 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/channel_deleted_handler.py
+-rw-rw-rw-   0        0        0      758 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/channel_updated_handler.py
+-rw-rw-rw-   0        0        0     1514 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/command_handler.py
+-rw-rw-rw-   0        0        0      686 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/community_updated_handler.py
+-rw-rw-rw-   0        0        0     1325 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/event_handler.py
+-rw-rw-rw-   0        0        0      703 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/group_created_handler.py
+-rw-rw-rw-   0        0        0      800 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/group_deleted_handler.py
+-rw-rw-rw-   0        0        0      800 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/group_updated_handler.py
+-rw-rw-rw-   0        0        0      867 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0      702 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/member_joined_handler.py
+-rw-rw-rw-   0        0        0      697 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/member_left_handler.py
+-rw-rw-rw-   0        0        0      960 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/message_handler.py
+-rw-rw-rw-   0        0        0      885 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/handlers/unknown_command_handler.py
+-rw-rw-rw-   0        0        0      693 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/bots/handlers/user_banned_handler.py
+-rw-rw-rw-   0        0        0      285 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/bots/register_command.py
+-rw-rw-rw-   0        0        0     1647 2023-05-17 11:22:56.000000 swibots-1.1.7/swibots/config.py
+-rw-rw-rw-   0        0        0     1333 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/error.py
+-rw-rw-rw-   0        0        0      878 2023-05-16 11:13:47.000000 swibots-1.1.7/swibots/types.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:34.262422 swibots-1.1.7/swibots/utils/
+-rw-rw-rw-   0        0        0       75 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/__init__.py
+-rw-rw-rw-   0        0        0     5880 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/rest_client.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:34.276422 swibots-1.1.7/swibots/utils/ws/
+-rw-rw-rw-   0        0        0       48 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:34.344424 swibots-1.1.7/swibots/utils/ws/asyncstomp/
+-rw-rw-rw-   0        0        0      150 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/asyncstomp/__init__.py
+-rw-rw-rw-   0        0        0     9743 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-rw-rw-   0        0        0      980 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:34.410430 swibots-1.1.7/swibots/utils/ws/common/
+-rw-rw-rw-   0        0        0      100 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/common/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/common/ws_frame.py
+-rw-rw-rw-   0        0        0      430 2023-02-13 07:44:31.000000 swibots-1.1.7/swibots/utils/ws/common/ws_message.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:23:30.961146 swibots-1.1.7/swibots.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-05-17 11:23:29.000000 swibots-1.1.7/swibots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7283 2023-05-17 11:23:29.000000 swibots-1.1.7/swibots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:23:29.000000 swibots-1.1.7/swibots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-17 11:23:29.000000 swibots-1.1.7/swibots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 11:23:29.000000 swibots-1.1.7/swibots.egg-info/top_level.txt
```

### Comparing `swibots-1.1.6/PKG-INFO` & `swibots-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.1.6
+Version: 1.1.7
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.1.6/README.md` & `swibots-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/setup.py` & `swibots-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.1.6",
+    version="1.1.7",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.1.6/swibots/api/api_client.py` & `swibots-1.1.7/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/auth/auth_client.py` & `swibots-1.1.7/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/auth/controllers/user_controller.py` & `swibots-1.1.7/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/auth/methods/get_me.py` & `swibots-1.1.7/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/auth/methods/login.py` & `swibots-1.1.7/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/auth/models/auth_user.py` & `swibots-1.1.7/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/bot_client.py` & `swibots-1.1.7/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.1.7/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.1.7/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.1.7/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.1.7/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/models/bot_command_info.py` & `swibots-1.1.7/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/bot/models/bot_info.py` & `swibots-1.1.7/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/chat_client.py` & `swibots-1.1.7/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/controllers/message_controller.py` & `swibots-1.1.7/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/events/callback_query_event.py` & `swibots-1.1.7/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/events/chat_event.py` & `swibots-1.1.7/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/events/command_event.py` & `swibots-1.1.7/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/events/inline_query_event.py` & `swibots-1.1.7/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/events/message_event.py` & `swibots-1.1.7/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/__init__.py` & `swibots-1.1.7/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.1.7/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.1.7/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/delete_message.py` & `swibots-1.1.7/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.1.7/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/download_media.py` & `swibots-1.1.7/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/edit_message.py` & `swibots-1.1.7/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.1.7/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/flag_message.py` & `swibots-1.1.7/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/forward_message.py` & `swibots-1.1.7/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.1.7/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.1.7/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.1.7/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.1.7/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.1.7/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_message.py` & `swibots-1.1.7/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_messages.py` & `swibots-1.1.7/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.1.7/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.1.7/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.1.7/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/reply_message.py` & `swibots-1.1.7/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.1.7/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/send_message.py` & `swibots-1.1.7/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/methods/send_text.py` & `swibots-1.1.7/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/group_chat_history.py` & `swibots-1.1.7/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/__init__.py` & `swibots-1.1.7/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.1.7/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.1.7/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.1.7/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.1.7/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/inline_markup.py` & `swibots-1.1.7/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/chat/models/message.py` & `swibots-1.1.7/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/common/events/event.py` & `swibots-1.1.7/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/common/models/media.py` & `swibots-1.1.7/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/common/models/media_upload_request.py` & `swibots-1.1.7/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/common/models/user.py` & `swibots-1.1.7/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/community_client.py` & `swibots-1.1.7/swibots/api/community/community_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/controllers/channel_controller.py` & `swibots-1.1.7/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/controllers/community_controller.py` & `swibots-1.1.7/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/controllers/group_controller.py` & `swibots-1.1.7/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/__init__.py` & `swibots-1.1.7/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/channel_created_event.py` & `swibots-1.1.7/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.1.7/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/channel_updated_event.py` & `swibots-1.1.7/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/community_event.py` & `swibots-1.1.7/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/community_updated_event.py` & `swibots-1.1.7/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/group_created_event.py` & `swibots-1.1.7/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/group_deleted_event.py` & `swibots-1.1.7/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/group_updated_event.py` & `swibots-1.1.7/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/member_joined_event.py` & `swibots-1.1.7/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/member_left_event.py` & `swibots-1.1.7/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/events/user_banned_event.py` & `swibots-1.1.7/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/methods/get_channel.py` & `swibots-1.1.7/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/methods/get_community.py` & `swibots-1.1.7/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/methods/get_group.py` & `swibots-1.1.7/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/models/channel.py` & `swibots-1.1.7/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/models/community.py` & `swibots-1.1.7/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/api/community/models/group.py` & `swibots-1.1.7/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/app.py` & `swibots-1.1.7/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/base/rest_response.py` & `swibots-1.1.7/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/base/switch_client.py` & `swibots-1.1.7/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/base/switch_object.py` & `swibots-1.1.7/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/base/switch_ws_async_client.py` & `swibots-1.1.7/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bot_app.py` & `swibots-1.1.7/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/bot.py` & `swibots-1.1.7/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/bot_context.py` & `swibots-1.1.7/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/__init__.py` & `swibots-1.1.7/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_callback_query.py` & `swibots-1.1.7/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.1.7/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.1.7/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_command.py` & `swibots-1.1.7/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_community_updated.py` & `swibots-1.1.7/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_group_created.py` & `swibots-1.1.7/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.1.7/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_group_updated.py` & `swibots-1.1.7/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_inline_query.py` & `swibots-1.1.7/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_member_joined.py` & `swibots-1.1.7/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_member_left.py` & `swibots-1.1.7/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.1.7/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/filters/filter.py` & `swibots-1.1.7/swibots/bots/filters/filter.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/__init__.py` & `swibots-1.1.7/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/base_handler.py` & `swibots-1.1.7/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.1.7/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.1.7/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.1.7/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.1.7/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/command_handler.py` & `swibots-1.1.7/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.1.7/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/event_handler.py` & `swibots-1.1.7/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/group_created_handler.py` & `swibots-1.1.7/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.1.7/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.1.7/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.1.7/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.1.7/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/member_left_handler.py` & `swibots-1.1.7/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/message_handler.py` & `swibots-1.1.7/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.1.7/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.1.7/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/config.py` & `swibots-1.1.7/swibots/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 
 APP_CONFIG = {
     "CHAT_SERVICE": {
         "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
         "WS_URL": os.getenv("CHAT_SERVICE_WS_URL")
-        or "ws://api-gateway.switch.pe/v1/websocket/message/ws",
+        or "wss://api-gateway.switch.pe/v1/websocket/message/ws",
     },
     "BOT_SERVICE": {
         "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
     },
     "AUTH_SERVICE": {
         "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api",
     },
@@ -25,15 +25,15 @@
     return APP_CONFIG
 
 
 def reload_config():
     APP_CONFIG["CHAT_SERVICE"]['BASE_URL'] = os.getenv(
         "CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
     APP_CONFIG["CHAT_SERVICE"]['WS_URL'] = os.getenv(
-        "CHAT_SERVICE_WS_URL") or "ws://api-gateway.switch.pe/v1/websocket/message/ws"
+        "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/message/ws"
     APP_CONFIG["BOT_SERVICE"]['BASE_URL'] = os.getenv(
         "BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
     APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
         "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api"
     APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
         "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
     APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
```

### Comparing `swibots-1.1.6/swibots/error.py` & `swibots-1.1.7/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/types.py` & `swibots-1.1.7/swibots/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/utils/rest_client.py` & `swibots-1.1.7/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/utils/types.py` & `swibots-1.1.7/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.1.7/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.1.7/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots/utils/ws/common/ws_frame.py` & `swibots-1.1.7/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.6/swibots.egg-info/PKG-INFO` & `swibots-1.1.7/swibots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.1.6
+Version: 1.1.7
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.1.6/swibots.egg-info/SOURCES.txt` & `swibots-1.1.7/swibots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

