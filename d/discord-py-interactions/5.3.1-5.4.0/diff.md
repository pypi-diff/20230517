# Comparing `tmp/discord-py-interactions-5.3.1.tar.gz` & `tmp/discord-py-interactions-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-5.3.1.tar", last modified: Sat May  6 16:55:29 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.4.0.tar", last modified: Wed May 17 19:04:41 2023, max compression
```

## Comparing `discord-py-interactions-5.3.1.tar` & `discord-py-interactions-5.4.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.991408 discord-py-interactions-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-06 16:55:28.991408 discord-py-interactions-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.947408 discord-py-interactions-5.3.1/discord_py_interactions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-06 16:55:28.000000 discord-py-interactions-5.3.1/discord_py_interactions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-06 16:55:28.000000 discord-py-interactions-5.3.1/discord_py_interactions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:55:28.000000 discord-py-interactions-5.3.1/discord_py_interactions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-06 16:55:28.000000 discord-py-interactions-5.3.1/discord_py_interactions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 16:55:28.000000 discord-py-interactions-5.3.1/discord_py_interactions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.947408 discord-py-interactions-5.3.1/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.947408 discord-py-interactions-5.3.1/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.947408 discord-py-interactions-5.3.1/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.951408 discord-py-interactions-5.3.1/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.955408 discord-py-interactions-5.3.1/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.955408 discord-py-interactions-5.3.1/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.959408 discord-py-interactions-5.3.1/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35371 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.959408 discord-py-interactions-5.3.1/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.963408 discord-py-interactions-5.3.1/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.963408 discord-py-interactions-5.3.1/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88891 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.967408 discord-py-interactions-5.3.1/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.967408 discord-py-interactions-5.3.1/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.971408 discord-py-interactions-5.3.1/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.971408 discord-py-interactions-5.3.1/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/debug_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.971408 discord-py-interactions-5.3.1/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.975408 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.975408 discord-py-interactions-5.3.1/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.983408 discord-py-interactions-5.3.1/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   102931 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    95578 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    38185 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.987408 discord-py-interactions-5.3.1/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.991408 discord-py-interactions-5.3.1/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55485 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    35094 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.991408 discord-py-interactions-5.3.1/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.991408 discord-py-interactions-5.3.1/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/interactions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-06 16:55:28.995408 discord-py-interactions-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-06 16:55:19.000000 discord-py-interactions-5.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:28.991408 discord-py-interactions-5.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-06 16:55:06.000000 discord-py-interactions-5.3.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.406703 discord-py-interactions-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-17 19:04:41.406703 discord-py-interactions-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.370703 discord-py-interactions-5.4.0/discord_py_interactions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-17 19:04:41.000000 discord-py-interactions-5.4.0/discord_py_interactions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-17 19:04:41.000000 discord-py-interactions-5.4.0/discord_py_interactions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:04:41.000000 discord-py-interactions-5.4.0/discord_py_interactions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-17 19:04:41.000000 discord-py-interactions-5.4.0/discord_py_interactions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 19:04:41.000000 discord-py-interactions-5.4.0/discord_py_interactions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.370703 discord-py-interactions-5.4.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.370703 discord-py-interactions-5.4.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.374703 discord-py-interactions-5.4.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.374703 discord-py-interactions-5.4.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.378703 discord-py-interactions-5.4.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.378703 discord-py-interactions-5.4.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.382703 discord-py-interactions-5.4.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35368 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.382703 discord-py-interactions-5.4.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.382703 discord-py-interactions-5.4.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.386703 discord-py-interactions-5.4.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91574 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.386703 discord-py-interactions-5.4.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.386703 discord-py-interactions-5.4.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.390703 discord-py-interactions-5.4.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.390703 discord-py-interactions-5.4.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/debug_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.390703 discord-py-interactions-5.4.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.390703 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.390703 discord-py-interactions-5.4.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.398703 discord-py-interactions-5.4.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103108 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95600 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.402703 discord-py-interactions-5.4.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.402703 discord-py-interactions-5.4.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55763 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.402703 discord-py-interactions-5.4.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.402703 discord-py-interactions-5.4.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/interactions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-17 19:04:41.406703 discord-py-interactions-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-17 19:04:32.000000 discord-py-interactions-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:41.406703 discord-py-interactions-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-17 19:04:21.000000 discord-py-interactions-5.4.0/tests/utils.py
```

### Comparing `discord-py-interactions-5.3.1/LICENSE` & `discord-py-interactions-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/PKG-INFO` & `discord-py-interactions-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.3.1
+Version: 5.4.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.3.1/README.md` & `discord-py-interactions-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/discord_py_interactions.egg-info/PKG-INFO` & `discord-py-interactions-5.4.0/discord_py_interactions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.3.1
+Version: 5.4.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.3.1/discord_py_interactions.egg-info/SOURCES.txt` & `discord-py-interactions-5.4.0/discord_py_interactions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/discord_py_interactions.egg-info/requires.txt` & `discord-py-interactions-5.4.0/discord_py_interactions.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 aiohttp
-attrs
+attrs>=22.1
 discord-typings>=0.5.1
 emoji
 tomli
 
 [all]
 PyNaCl<1.6,>=1.5.0
 aiodns
```

### Comparing `discord-py-interactions-5.3.1/interactions/__init__.py` & `discord-py-interactions-5.4.0/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/__init__.py` & `discord-py-interactions-5.4.0/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/base.py` & `discord-py-interactions-5.4.0/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/discord.py` & `discord-py-interactions-5.4.0/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/internal.py` & `discord-py-interactions-5.4.0/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/__init__.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/_template.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/auto_mod.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/channel_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/guild_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/integrations.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/member_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/message_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/reaction_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/role_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/stage_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/thread_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/user_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/events/processors/voice_events.py` & `discord-py-interactions-5.4.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/gateway/gateway.py` & `discord-py-interactions-5.4.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/gateway/state.py` & `discord-py-interactions-5.4.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/gateway/websocket.py` & `discord-py-interactions-5.4.0/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_client.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from logging import Logger
 from typing import Any, cast, Callable
 from urllib.parse import quote as _uriquote
 from weakref import WeakValueDictionary
 
 import aiohttp
 import discord_typings
-from aiohttp import BaseConnector, ClientSession, ClientWebSocketResponse, FormData
+from aiohttp import BaseConnector, ClientSession, ClientWebSocketResponse, FormData, BasicAuth
 from multidict import CIMultiDictProxy
 
 import interactions.client.const as constants
 from interactions import models
 from interactions.api.http.http_requests import (
     BotRequests,
     ChannelRequests,
@@ -210,29 +210,35 @@
     UserRequests,
     WebhookRequests,
     ScheduledEventsRequests,
 ):
     """A http client for sending requests to the Discord API."""
 
     def __init__(
-        self, connector: BaseConnector | None = None, logger: Logger = MISSING, show_ratelimit_tracebacks: bool = False
+        self,
+        connector: BaseConnector | None = None,
+        logger: Logger = MISSING,
+        show_ratelimit_tracebacks: bool = False,
+        proxy: tuple[str, BasicAuth] | None = None,
     ) -> None:
         self.connector: BaseConnector | None = connector
         self.__session: ClientSession | None = None
         self.token: str | None = None
         self.global_lock: GlobalLock = GlobalLock()
         self._max_attempts: int = 3
 
         self.ratelimit_locks: WeakValueDictionary[str, BucketLock] = WeakValueDictionary()
         self.show_ratelimit_traceback: bool = show_ratelimit_tracebacks
         self._endpoints = {}
 
         self.user_agent: str = (
             f"DiscordBot ({__repo_url__} {__version__} Python/{__py_version__}) aiohttp/{aiohttp.__version__}"
         )
+        self.proxy: tuple[str, BasicAuth] | None = proxy
+        self.__proxy_validated: bool = False
 
         if logger is MISSING:
             logger = constants.get_logger()
         self.logger = logger
 
     def get_ratelimit(self, route: Route) -> BucketLock:
         """
@@ -380,14 +386,18 @@
                     processed_data = self._process_payload(payload, files)
                     if isinstance(processed_data, FormData):
                         kwargs["data"] = processed_data  # pyright: ignore
                     else:
                         kwargs["json"] = processed_data  # pyright: ignore
                     await self.global_lock.wait()
 
+                    if self.proxy:
+                        kwargs["proxy"] = self.proxy[0]
+                        kwargs["proxy_auth"] = self.proxy[1]
+
                     async with self.__session.request(route.method, route.url, **kwargs) as response:
                         result = await response_decode(response)
                         self.ingest_ratelimit(route, response.headers, lock)
 
                         if response.status == 429:
                             # ratelimit exceeded
                             result = cast(dict[str, str], result)
@@ -501,14 +511,27 @@
             The currently logged in bot's data
 
         """
         self.__session = ClientSession(
             connector=self.connector or aiohttp.TCPConnector(limit=self.global_lock.max_requests),
             json_serialize=FastJson.dumps,
         )
+        if not self.__proxy_validated and self.proxy:
+            try:
+                self.logger.info(f"Validating Proxy @ {self.proxy[0]}")
+                async with self.__session.get(
+                    "http://icanhazip.com/", proxy=self.proxy[0], proxy_auth=self.proxy[1]
+                ) as response:
+                    if response.status != 200:
+                        raise RuntimeError("Proxy configuration is invalid")
+                    self.logger.info(f"Proxy Connected @ {(await response.text()).strip()}")
+                    self.__proxy_validated = True
+            except Exception as e:
+                raise RuntimeError("Proxy configuration is invalid") from e
+
         self.token = token
         try:
             result = await self.request(Route("GET", "/users/@me"))
             return cast(dict[str, Any], result)
         except HTTPException as e:
             if e.status == 401:
                 raise LoginError("An improper token was passed") from e
@@ -552,8 +575,10 @@
         return await self.__session.ws_connect(
             url,
             timeout=30,
             max_msg_size=0,
             autoclose=False,
             headers={"User-Agent": self.user_agent},
             compress=0,
+            proxy=self.proxy[0] if self.proxy else None,
+            proxy_auth=self.proxy[1] if self.proxy else None,
         )
```

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/__init__.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/bot.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/channels.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/emojis.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/guild.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         Args:
             guild_id: the id of the guild
             with_counts: when `true`, will return approximate member and presence counts for the guild
         Returns:
             a guild object
 
         """
-        params = {"guild_id": guild_id, "with_counts": int(with_counts)}
-        result = await self.request(Route("GET", "/guilds/{guild_id}"), params=params)
+        params = {"with_counts": int(with_counts)}
+        result = await self.request(Route("GET", "/guilds/{guild_id}", guild_id=guild_id), params=params)
         return cast(discord_typings.GuildData, result)
 
     async def get_guild_preview(self, guild_id: "Snowflake_Type") -> discord_typings.GuildPreviewData:
         """
         Get a guild's preview.
 
         Args:
```

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/interactions.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/members.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/messages.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/reactions.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/scheduled_events.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/stickers.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/threads.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/users.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/http_requests/webhooks.py` & `discord-py-interactions-5.4.0/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/http/route.py` & `discord-py-interactions-5.4.0/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/audio.py` & `discord-py-interactions-5.4.0/interactions/api/voice/audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         self.buffer = AudioBuffer()
 
         self.buffer_seconds = 3
         self.read_ahead_task = threading.Thread(target=self._read_ahead, daemon=True)
 
         self.ffmpeg_before_args = ""
         self.ffmpeg_args = ""
-        self.probe: bool = True
+        self.probe: bool = False
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__}: {self.source}>"
 
     @property
     def _max_buffer_size(self) -> int:
         # 1ms of audio * (buffer seconds * 1000)
```

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/audio_writer.py` & `discord-py-interactions-5.4.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/encryption.py` & `discord-py-interactions-5.4.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/opus.py` & `discord-py-interactions-5.4.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/player.py` & `discord-py-interactions-5.4.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/recorder.py` & `discord-py-interactions-5.4.0/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/api/voice/voice_gateway.py` & `discord-py-interactions-5.4.0/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/bin/opus-x64.dll` & `discord-py-interactions-5.4.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/bin/opus-x86.dll` & `discord-py-interactions-5.4.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/__init__.py` & `discord-py-interactions-5.4.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/auto_shard_client.py` & `discord-py-interactions-5.4.0/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/client.py` & `discord-py-interactions-5.4.0/interactions/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     Sequence,
     Type,
     Union,
     Awaitable,
     Tuple,
 )
 
+from aiohttp import BasicAuth
+
 import interactions.api.events as events
 import interactions.client.const as constants
 from interactions.api.events import BaseEvent, RawGatewayEvent, processors
 from interactions.api.events.internal import CallbackAdded
 from interactions.api.gateway.gateway import GatewayClient
 from interactions.api.gateway.state import ConnectionState
 from interactions.api.http.http_client import HTTPClient
@@ -84,19 +86,25 @@
 from interactions.models.discord.components import get_components_ids, BaseComponent
 from interactions.models.discord.embed import Embed
 from interactions.models.discord.enums import (
     ComponentType,
     Intents,
     InteractionType,
     Status,
+    MessageFlags,
 )
 from interactions.models.discord.file import UPLOADABLE_TYPE
 from interactions.models.discord.snowflake import Snowflake, to_snowflake_list
 from interactions.models.internal.active_voice_state import ActiveVoiceState
-from interactions.models.internal.application_commands import ContextMenu, ModalCommand, GlobalAutoComplete
+from interactions.models.internal.application_commands import (
+    ContextMenu,
+    ModalCommand,
+    GlobalAutoComplete,
+    CallbackType,
+)
 from interactions.models.internal.auto_defer import AutoDefer
 from interactions.models.internal.callback import CallbackObject
 from interactions.models.internal.command import BaseCommand
 from interactions.models.internal.context import (
     BaseContext,
     InteractionContext,
     SlashContext,
@@ -107,18 +115,16 @@
 )
 from interactions.models.internal.listener import Listener
 from interactions.models.internal.tasks import Task
 
 if TYPE_CHECKING:
     from interactions.models import Snowflake_Type, TYPE_ALL_CHANNEL
 
-
 __all__ = ("Client",)
 
-
 # see https://discord.com/developers/docs/topics/gateway#list-of-intents
 _INTENT_EVENTS: dict[BaseEvent, list[Intents]] = {
     # Intents.GUILDS
     events.GuildJoin: [Intents.GUILDS],
     events.GuildLeft: [Intents.GUILDS],
     events.GuildUpdate: [Intents.GUILDS],
     events.RoleCreate: [Intents.GUILDS],
@@ -221,14 +227,15 @@
         activity: The activity the bot should log in "playing"
 
         sync_interactions: Should application commands be synced with discord?
         delete_unused_application_cmds: Delete any commands from discord that aren't implemented in this client
         enforce_interaction_perms: Enforce discord application command permissions, locally
         fetch_members: Should the client fetch members from guilds upon startup (this will delay the client being ready)
         send_command_tracebacks: Automatically send uncaught tracebacks if a command throws an exception
+        send_not_ready_messages: Send a message to the user if they try to use a command before the client is ready
 
         auto_defer: AutoDefer: A system to automatically defer commands after a set duration
         interaction_context: Type[InteractionContext]: InteractionContext: The object to instantiate for Interaction Context
         component_context: Type[ComponentContext]: The object to instantiate for Component Context
         autocomplete_context: Type[AutocompleteContext]: The object to instantiate for Autocomplete Context
         modal_context: Type[ModalContext]: The object to instantiate for Modal Context
 
@@ -237,14 +244,17 @@
 
         debug_scope: Force all application commands to be registered within this scope
         disable_dm_commands: Should interaction commands be disabled in DMs?
         basic_logging: Utilise basic logging to output library data to console. Do not use in combination with `Client.logger`
         logging_level: The level of logging to use for basic_logging. Do not use in combination with `Client.logger`
         logger: The logger interactions.py should use. Do not use in combination with `Client.basic_logging` and `Client.logging_level`. Note: Different loggers with multiple clients are not supported
 
+        proxy: A http/https proxy to use for all requests
+        proxy_auth: The auth to use for the proxy - must be either a tuple of (username, password) or aiohttp.BasicAuth
+
     Optionally, you can configure the caches here, by specifying the name of the cache, followed by a dict-style object to use.
     It is recommended to use `smart_cache.create_cache` to configure the cache here.
     as an example, this is a recommended attribute `message_cache=create_cache(250, 50)`,
 
     ???+ note "Intents Note"
         By default, all non-privileged intents will be enabled
 
@@ -273,20 +283,23 @@
         intents: Union[int, Intents] = Intents.DEFAULT,
         interaction_context: Type[InteractionContext] = InteractionContext,
         logger: logging.Logger = MISSING,
         logging_level: int = logging.INFO,
         modal_context: Type[BaseContext] = ModalContext,
         owner_ids: Iterable["Snowflake_Type"] = (),
         send_command_tracebacks: bool = True,
+        send_not_ready_messages: bool = False,
         shard_id: int = 0,
         show_ratelimit_tracebacks: bool = False,
         slash_context: Type[BaseContext] = SlashContext,
         status: Status = Status.ONLINE,
         sync_ext: bool = True,
         sync_interactions: bool = True,
+        proxy_url: str | None = None,
+        proxy_auth: BasicAuth | tuple[str, str] | None = None,
         token: str | None = None,
         total_shards: int = 1,
         **kwargs,
     ) -> None:
         if logger is MISSING:
             logger = constants.get_logger()
 
@@ -308,25 +321,31 @@
         """Should unused application commands be deleted?"""
         self.sync_ext: bool = sync_ext
         """Should we sync whenever a extension is (un)loaded"""
         self.debug_scope = to_snowflake(debug_scope) if debug_scope is not MISSING else MISSING
         """Sync global commands as guild for quicker command updates during debug"""
         self.send_command_tracebacks: bool = send_command_tracebacks
         """Should the traceback of command errors be sent in reply to the command invocation"""
+        self.send_not_ready_messages: bool = send_not_ready_messages
+        """Should the bot send a message when it is not ready yet in response to a command invocation"""
         if auto_defer is True:
             auto_defer = AutoDefer(enabled=True)
         else:
             auto_defer = auto_defer or AutoDefer()
         self.auto_defer = auto_defer
         """A system to automatically defer commands after a set duration"""
         self.intents = intents if isinstance(intents, Intents) else Intents(intents)
 
         # resources
+        if isinstance(proxy_auth, tuple):
+            proxy_auth = BasicAuth(*proxy_auth)
 
-        self.http: HTTPClient = HTTPClient(logger=self.logger, show_ratelimit_tracebacks=show_ratelimit_tracebacks)
+        self.http: HTTPClient = HTTPClient(
+            logger=self.logger, show_ratelimit_tracebacks=show_ratelimit_tracebacks, proxy=(proxy_url, proxy_auth)
+        )
         """The HTTP client to use when interacting with discord endpoints"""
 
         # context factories
         self.interaction_context: Type[BaseContext] = interaction_context
         """The object to instantiate for Interaction Context"""
         self.component_context: Type[BaseContext] = component_context
         """The object to instantiate for Component Context"""
@@ -382,14 +401,15 @@
         self.interaction_tree: Dict[
             "Snowflake_Type", Dict[str, InteractionCommand | Dict[str, InteractionCommand]]
         ] = {}
         """A dictionary of registered application commands in a tree"""
         self._component_callbacks: Dict[str, Callable[..., Coroutine]] = {}
         self._regex_component_callbacks: Dict[re.Pattern, Callable[..., Coroutine]] = {}
         self._modal_callbacks: Dict[str, Callable[..., Coroutine]] = {}
+        self._regex_modal_callbacks: Dict[re.Pattern, Callable[..., Coroutine]] = {}
         self._global_autocompletes: Dict[str, GlobalAutoComplete] = {}
         self.processors: Dict[str, Callable[..., Coroutine]] = {}
         self.__modules = {}
         self.ext: Dict[str, Extension] = {}
         """A dictionary of mounted ext"""
         self.listeners: Dict[str, list[Listener]] = {}
         self.waits: Dict[str, List] = {}
@@ -680,15 +700,15 @@
                 out = "".join(traceback.format_exception(event.error))
                 if self.http.token is not None:
                     out = out.replace(self.http.token, "[REDACTED TOKEN]")
                 await event.ctx.send(
                     embeds=Embed(
                         title=f"Error: {type(event.error).__name__}",
                         color=BrandColors.RED,
-                        description=f"```\n{out[:EMBED_MAX_DESC_LENGTH-8]}```",
+                        description=f"```\n{out[:EMBED_MAX_DESC_LENGTH - 8]}```",
                     )
                 )
 
     @Listener.create(is_default_listener=True)
     async def on_command_completion(self, event: events.CommandCompletion) -> None:
         """
         Called *after* any command is ran.
@@ -1301,17 +1321,22 @@
         """
         Add a modal callback to the client.
 
         Args:
             command: The command to add
         """
         for listener in command.listeners:
-            if listener in self._modal_callbacks.keys():
-                raise ValueError(f"Duplicate Component! Multiple modal callbacks for `{listener}`")
-            self._modal_callbacks[listener] = command
+            if isinstance(listener, re.Pattern):
+                if listener in self._regex_component_callbacks.keys():
+                    raise ValueError(f"Duplicate Component! Multiple modal callbacks for `{listener}`")
+                self._regex_modal_callbacks[listener] = command
+            else:
+                if listener in self._modal_callbacks.keys():
+                    raise ValueError(f"Duplicate Component! Multiple modal callbacks for `{listener}`")
+                self._modal_callbacks[listener] = command
             continue
 
     def add_global_autocomplete(self, callback: GlobalAutoComplete) -> None:
         """
         Add a global autocomplete to the client.
 
         Args:
@@ -1555,16 +1580,15 @@
             delete_cmds: Whether to delete commands.
         """
         sync_payload = []
         sync_needed_flag = False
 
         for local_cmd in self.interactions_by_scope.get(cmd_scope, {}).values():
             remote_cmd_json = next(
-                (v for v in remote_commands if int(v["id"]) == local_cmd.cmd_id.get(cmd_scope)),
-                None,
+                (c for c in remote_commands if int(c["id"]) == int(local_cmd.cmd_id.get(cmd_scope, 0))), None
             )
             local_cmd_json = next((c for c in local_cmds_json[cmd_scope] if c["name"] == str(local_cmd.name)))
 
             if sync_needed(local_cmd_json, remote_cmd_json):
                 sync_needed_flag = True
                 sync_payload.append(local_cmd_json)
             elif not delete_cmds and remote_cmd_json:
@@ -1692,14 +1716,40 @@
                 else:
                     channel = await self.cache.fetch_dm_channel(cls.author_id)
                 cls.channel_id = channel.id
             except Forbidden:
                 self.logger.debug(f"Failed to fetch channel data for {data['channel_id']}")
         return cls
 
+    async def handle_pre_ready_response(self, data: dict) -> None:
+        """
+        Respond to an interaction that was received before the bot was ready.
+
+        Args:
+            data: The interaction data
+
+        """
+        if data["type"] == InteractionType.AUTOCOMPLETE:
+            # we do not want to respond to autocompletes as discord will cache the response,
+            # so we just ignore them
+            return
+
+        with contextlib.suppress(HTTPException):
+            await self.http.post_initial_response(
+                {
+                    "type": CallbackType.CHANNEL_MESSAGE_WITH_SOURCE,
+                    "data": {
+                        "content": f"{self.user.display_name} is starting up. Please try again in a few seconds",
+                        "flags": MessageFlags.EPHEMERAL,
+                    },
+                },
+                token=data["token"],
+                interaction_id=data["id"],
+            )
+
     async def _run_slash_command(self, command: SlashCommand, ctx: "InteractionContext") -> Any:
         """Overrideable method that executes slash commands, can be used to wrap callback execution"""
         return await command(ctx, **ctx.kwargs)
 
     @processors.Processor.define("raw_interaction_create")
     async def _dispatch_interaction(self, event: RawGatewayEvent) -> None:  # noqa: C901
         """
@@ -1709,14 +1759,16 @@
             raw interaction event
 
         """
         interaction_data = event.data
 
         if not self._startup:
             self.logger.warning("Received interaction before startup completed, ignoring")
+            if self.send_not_ready_messages:
+                await self.handle_pre_ready_response(interaction_data)
             return
 
         if interaction_data["type"] in (
             InteractionType.APPLICATION_COMMAND,
             InteractionType.AUTOCOMPLETE,
         ):
             interaction_id = interaction_data["data"]["id"]
@@ -1788,16 +1840,26 @@
             if component_type == ComponentType.STRING_SELECT:
                 self.dispatch(events.Select(ctx))
 
         elif interaction_data["type"] == InteractionType.MODAL_RESPONSE:
             ctx = await self.get_context(interaction_data)
             self.dispatch(events.ModalCompletion(ctx=ctx))
 
-            if callback := self._modal_callbacks.get(ctx.custom_id):
-                await self.__dispatch_interaction(ctx=ctx, callback=callback(ctx), error_callback=events.ModalError)
+            modal_callback = self._modal_callbacks.get(ctx.custom_id)
+            if not modal_callback:
+                # evaluate regex component callbacks
+                for regex, callback in self._regex_modal_callbacks.items():
+                    if regex.match(ctx.custom_id):
+                        modal_callback = callback
+                        break
+
+            if modal_callback:
+                await self.__dispatch_interaction(
+                    ctx=ctx, callback=modal_callback(ctx), error_callback=events.ModalError
+                )
 
         else:
             raise NotImplementedError(f"Unknown Interaction Received: {interaction_data['type']}")
 
     # todo add typing once context is re-implemented
     async def __dispatch_interaction(
         self,
```

### Comparing `discord-py-interactions-5.3.1/interactions/client/const.py` & `discord-py-interactions-5.4.0/interactions/client/const.py`

 * *Files 25% similar despite different names*

```diff
@@ -216,9 +216,53 @@
 T_co = TypeVar("T_co", covariant=True)
 Absent = Union[T, Missing]
 AsyncCallable = Callable[..., Coroutine]
 
 LIB_PATH = os.sep.join(__file__.split(os.sep)[:-2])
 """The path to the library folder."""
 
-RECOVERABLE_WEBSOCKET_CLOSE_CODES = (4000, 4001, 4002, 4003, 4005, 4007, 4008, 4009)
-NON_RESUMABLE_WEBSOCKET_CLOSE_CODES = (1000, 4007)
+# fmt: off
+RECOVERABLE_WEBSOCKET_CLOSE_CODES = (  # Codes that are recoverable, and the bot will reconnect
+    1000,  # Normal closure
+    1001,  # Server going away
+    1003,  # Unsupported Data
+    1005,  # No status code
+    1006,  # Abnormal closure
+    1008,  # Policy Violation
+    1009,  # Message too big
+    1011,  # Server error
+    1012,  # Server is restarting
+    1014,  # Handshake failed
+    1015,  # TLS error
+    4000,  # Unknown error
+    4001,  # Unknown opcode
+    4002,  # Decode error
+    4003,  # Not authenticated
+    4005,  # Already authenticated
+    4007,  # Invalid seq
+    4008,  # Rate limited
+    4009,  # Session timed out
+)
+NON_RESUMABLE_WEBSOCKET_CLOSE_CODES = (  # Codes that are recoverable, but the bot won't be able to resume the session
+    1000,  # Normal closure
+    1003,  # Unsupported Data
+    1008,  # Policy Violation
+    1009,  # Message too big
+    1011,  # Server error
+    1012,  # Server is restarting
+    1014,  # Handshake failed
+    1015,  # TLS error
+    4007,  # Invalid seq
+)
+# Any close code not in the above two tuples is a non-recoverable close code, and will result in the bot shutting down
+# fmt: on
+
+
+# Sanity check the above constants - only useful during development, but doesn't hurt to leave in
+try:
+    assert set(NON_RESUMABLE_WEBSOCKET_CLOSE_CODES).issubset(set(RECOVERABLE_WEBSOCKET_CLOSE_CODES))
+except AssertionError as e:
+    # find the difference between the two sets
+    diff = set(NON_RESUMABLE_WEBSOCKET_CLOSE_CODES) - set(RECOVERABLE_WEBSOCKET_CLOSE_CODES)
+    raise RuntimeError(
+        f"NON_RESUMABLE_WEBSOCKET_CLOSE_CODES contains codes that are not in RECOVERABLE_WEBSOCKET_CLOSE_CODES: {diff}"
+    ) from e
```

### Comparing `discord-py-interactions-5.3.1/interactions/client/errors.py` & `discord-py-interactions-5.4.0/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/mixins/modal.py` & `discord-py-interactions-5.4.0/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/mixins/send.py` & `discord-py-interactions-5.4.0/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/mixins/serialization.py` & `discord-py-interactions-5.4.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/smart_cache.py` & `discord-py-interactions-5.4.0/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/__init__.py` & `discord-py-interactions-5.4.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/attr_converters.py` & `discord-py-interactions-5.4.0/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/attr_utils.py` & `discord-py-interactions-5.4.0/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/attr_utils.pyi` & `discord-py-interactions-5.4.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/cache.py` & `discord-py-interactions-5.4.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/deserialise_app_cmds.py` & `discord-py-interactions-5.4.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/formatting.py` & `discord-py-interactions-5.4.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/input_utils.py` & `discord-py-interactions-5.4.0/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/misc_utils.py` & `discord-py-interactions-5.4.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/serializer.py` & `discord-py-interactions-5.4.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/client/utils/text_utils.py` & `discord-py-interactions-5.4.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/console.py` & `discord-py-interactions-5.4.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/debug_extension/__init__.py` & `discord-py-interactions-5.4.0/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/debug_extension/debug_application_cmd.py` & `discord-py-interactions-5.4.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/debug_extension/debug_exec.py` & `discord-py-interactions-5.4.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/debug_extension/debug_exts.py` & `discord-py-interactions-5.4.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/debug_extension/utils.py` & `discord-py-interactions-5.4.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/jurigged.py` & `discord-py-interactions-5.4.0/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/mypy/__init__.py` & `discord-py-interactions-5.4.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/paginators.py` & `discord-py-interactions-5.4.0/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/__init__.py` & `discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/command.py` & `discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/context.py` & `discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/help.py` & `discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/manager.py` & `discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/prefixed_commands/utils.py` & `discord-py-interactions-5.4.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/ext/sentry.py` & `discord-py-interactions-5.4.0/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/__init__.py` & `discord-py-interactions-5.4.0/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/__init__.py` & `discord-py-interactions-5.4.0/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/activity.py` & `discord-py-interactions-5.4.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/app_perms.py` & `discord-py-interactions-5.4.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/application.py` & `discord-py-interactions-5.4.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/asset.py` & `discord-py-interactions-5.4.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/auto_mod.py` & `discord-py-interactions-5.4.0/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/base.py` & `discord-py-interactions-5.4.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/channel.py` & `discord-py-interactions-5.4.0/interactions/models/discord/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,19 +400,20 @@
 
     async def purge(
         self,
         deletion_limit: int = 50,
         search_limit: int = 100,
         predicate: Callable[["models.Message"], bool] = MISSING,
         avoid_loading_msg: bool = True,
+        return_messages: bool = False,
         before: Optional[Snowflake_Type] = MISSING,
         after: Optional[Snowflake_Type] = MISSING,
         around: Optional[Snowflake_Type] = MISSING,
         reason: Absent[Optional[str]] = MISSING,
-    ) -> int:
+    ) -> int | List["models.Message"]:
         """
         Bulk delete messages within a channel. If a `predicate` is provided, it will be used to determine which messages to delete, otherwise all messages will be deleted within the `deletion_limit`.
 
         ??? Hint "Example Usage:"
             ```python
             # this will delete the last 20 messages sent by a user with the given ID
             deleted = await channel.purge(deletion_limit=20, predicate=lambda m: m.author.id == 174918559539920897)
@@ -420,14 +421,15 @@
             ```
 
         Args:
             deletion_limit: The target amount of messages to delete
             search_limit: How many messages to search through
             predicate: A function that returns True or False, and takes a message as an argument
             avoid_loading_msg: Should the bot attempt to avoid deleting its own loading messages (recommended enabled)
+            return_messages: Should the bot return the messages that were deleted
             before: Search messages before this ID
             after: Search messages after this ID
             around: Search messages around this ID
             reason: The reason for this deletion
 
         Returns:
             The total amount of messages deleted
@@ -457,21 +459,21 @@
             ):
                 continue
 
             if message.id < fourteen_days_ago:
                 # message is too old to be purged
                 continue
 
-            to_delete.append(message.id)
+            to_delete.append(message)
 
-        count = len(to_delete)
+        out = to_delete.copy()
         while len(to_delete):
-            iteration = [to_delete.pop() for i in range(min(100, len(to_delete)))]
+            iteration = [to_delete.pop().id for i in range(min(100, len(to_delete)))]
             await self.delete_messages(iteration, reason=reason)
-        return count
+        return out if return_messages else len(out)
 
     async def trigger_typing(self) -> None:
         """Trigger a typing animation in this channel."""
         await self._client.http.trigger_typing_indicator(self.id)
 
     @property
     def typing(self) -> Typing:
```

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/color.py` & `discord-py-interactions-5.4.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/components.py` & `discord-py-interactions-5.4.0/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/embed.py` & `discord-py-interactions-5.4.0/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/emoji.py` & `discord-py-interactions-5.4.0/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/enums.py` & `discord-py-interactions-5.4.0/interactions/models/discord/enums.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/file.py` & `discord-py-interactions-5.4.0/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/guild.py` & `discord-py-interactions-5.4.0/interactions/models/discord/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
     def humans(self) -> List["models.Member"]:
         """Returns a list of all humans within this guild"""
         return [member for member in self.members if not member.bot]
 
     @property
     def roles(self) -> List["models.Role"]:
         """Returns a list of roles associated with this guild."""
-        return [self._client.cache.get_role(r_id) for r_id in self._role_ids]
+        return sorted([self._client.cache.get_role(r_id) for r_id in self._role_ids], reverse=True)
 
     @property
     def me(self) -> "models.Member":
         """Returns this bots member object within this guild."""
         return self._client.cache.get_member(self.id, self._client.user.id)
 
     @property
```

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/invite.py` & `discord-py-interactions-5.4.0/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/message.py` & `discord-py-interactions-5.4.0/interactions/models/discord/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Mapping,
 )
 
 import attrs
 
 import interactions.models as models
 from interactions.client.const import GUILD_WELCOME_MESSAGES, MISSING, Absent
-from interactions.client.errors import ThreadOutsideOfGuild
+from interactions.client.errors import ThreadOutsideOfGuild, NotFound
 from interactions.client.mixins.serialization import DictSerializationMixin
 from interactions.client.utils.attr_converters import optional as optional_c
 from interactions.client.utils.attr_converters import timestamp_converter
 from interactions.client.utils.serializer import dict_filter_none
 from interactions.client.utils.text_utils import mentions
 from interactions.models.discord.channel import BaseChannel
 from interactions.models.discord.emoji import process_emoji_req_format
@@ -396,15 +396,19 @@
 
         Returns:
             The referenced message, if found
 
         """
         if self._referenced_message_id is None:
             return None
-        return await self._client.cache.fetch_message(self._channel_id, self._referenced_message_id, force=force)
+
+        try:
+            return await self._client.cache.fetch_message(self._channel_id, self._referenced_message_id, force=force)
+        except NotFound:
+            return None
 
     def get_referenced_message(self) -> Optional["Message"]:
         """
         Get the message this message is referencing, if any.
 
         Returns:
             The referenced message, if found
@@ -488,14 +492,16 @@
         # TODO: Convert to application object
 
         if ref_message_data := data.pop("referenced_message", None):
             if not ref_message_data.get("guild_id"):
                 ref_message_data["guild_id"] = data.get("guild_id")
             _m = client.cache.place_message_data(ref_message_data)
             data["referenced_message_id"] = _m.id
+        elif msg_reference := data.get("message_reference"):
+            data["referenced_message_id"] = msg_reference["message_id"]
 
         if "interaction" in data:
             data["interaction"] = MessageInteraction.from_dict(data["interaction"], client)
 
         if thread_data := data.pop("thread", None):
             data["thread_channel_id"] = client.cache.place_channel_data(thread_data).id
```

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/modal.py` & `discord-py-interactions-5.4.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/reaction.py` & `discord-py-interactions-5.4.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/role.py` & `discord-py-interactions-5.4.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/scheduled_event.py` & `discord-py-interactions-5.4.0/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/snowflake.py` & `discord-py-interactions-5.4.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/stage_instance.py` & `discord-py-interactions-5.4.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/sticker.py` & `discord-py-interactions-5.4.0/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/team.py` & `discord-py-interactions-5.4.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/thread.py` & `discord-py-interactions-5.4.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/timestamp.py` & `discord-py-interactions-5.4.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/user.py` & `discord-py-interactions-5.4.0/interactions/models/discord/user.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/user.pyi` & `discord-py-interactions-5.4.0/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/voice_state.py` & `discord-py-interactions-5.4.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/discord/webhooks.py` & `discord-py-interactions-5.4.0/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/__init__.py` & `discord-py-interactions-5.4.0/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/active_voice_state.py` & `discord-py-interactions-5.4.0/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/annotations/slash.py` & `discord-py-interactions-5.4.0/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/application_commands.py` & `discord-py-interactions-5.4.0/interactions/models/internal/application_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
 
 def desc_validator(_: Any, attr: Attribute, value: str) -> None:
     if value and not 1 <= len(value) <= SLASH_CMD_MAX_DESC_LENGTH:
         raise ValueError(f"Description must be between 1 and {SLASH_CMD_MAX_DESC_LENGTH} characters long")
 
 
+def custom_ids_validator(*custom_id: str | re.Pattern) -> None:
+    if not (all(isinstance(i, re.Pattern) for i in custom_id) or all(isinstance(i, str) for i in custom_id)):
+        raise ValueError("All custom IDs be either a string or a regex pattern, not a mix of both.")
+
+
 @attrs.define(
     eq=False,
     order=False,
     hash=False,
     field_transformer=attrs_validator(name_validator, skip_fields=["default_locale"]),
 )
 class LocalisedName(LocalisedField):
@@ -1141,37 +1146,41 @@
     def wrapper(func: AsyncCallable) -> ComponentCommand:
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         return ComponentCommand(name=f"ComponentCallback::{custom_id}", callback=func, listeners=custom_id)
 
     custom_id = _unpack_helper(custom_id)
-    if not (all(isinstance(i, re.Pattern) for i in custom_id) or all(isinstance(i, str) for i in custom_id)):
-        raise ValueError("All custom IDs be either a string or a regex pattern, not a mix of both.")
+    custom_ids_validator(*custom_id)
     return wrapper
 
 
-def modal_callback(*custom_id: str) -> Callable[[AsyncCallable], ModalCommand]:
+def modal_callback(*custom_id: str | re.Pattern) -> Callable[[AsyncCallable], ModalCommand]:
     """
     Register a coroutine as a modal callback.
 
     Modal callbacks work the same way as commands, just using modals as a way of invoking, instead of messages.
     Your callback will be given a single argument, `ModalContext`
 
+    Note:
+        This can optionally take a regex pattern, which will be used to match against the custom ID of the modal
+
+
     Args:
         *custom_id: The custom ID of the modal to wait for
     """
 
     def wrapper(func: AsyncCallable) -> ModalCommand:
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         return ModalCommand(name=f"ModalCallback::{custom_id}", callback=func, listeners=custom_id)
 
     custom_id = _unpack_helper(custom_id)
+    custom_ids_validator(*custom_id)
     return wrapper
 
 
 InterCommandT = TypeVar("InterCommandT", InteractionCommand, AsyncCallable)
 SlashCommandT = TypeVar("SlashCommandT", SlashCommand, AsyncCallable)
```

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/auto_defer.py` & `discord-py-interactions-5.4.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/callback.py` & `discord-py-interactions-5.4.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/checks.py` & `discord-py-interactions-5.4.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/command.py` & `discord-py-interactions-5.4.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/context.py` & `discord-py-interactions-5.4.0/interactions/models/internal/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,15 +892,15 @@
 
         processed_choices = []
         for choice in choices:
             if isinstance(choice, dict):
                 name = choice["name"]
                 value = choice["value"]
             elif isinstance(choice, SlashCommandChoice):
-                name = choice.name
+                name = choice.name.get_locale(self.locale)
                 value = choice.value
             else:
                 name = str(choice)
                 value = choice
 
             processed_choices.append({"name": name, "value": type_cast(value) if type_cast else value})
```

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/converters.py` & `discord-py-interactions-5.4.0/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/cooldowns.py` & `discord-py-interactions-5.4.0/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/extension.py` & `discord-py-interactions-5.4.0/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/listener.py` & `discord-py-interactions-5.4.0/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/localisation.py` & `discord-py-interactions-5.4.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/protocols.py` & `discord-py-interactions-5.4.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/tasks/task.py` & `discord-py-interactions-5.4.0/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/tasks/triggers.py` & `discord-py-interactions-5.4.0/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/internal/wait.py` & `discord-py-interactions-5.4.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/misc/context_manager.py` & `discord-py-interactions-5.4.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/interactions/models/misc/iterator.py` & `discord-py-interactions-5.4.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/pyproject.toml` & `discord-py-interactions-5.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.3.1"
+version = "5.4.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `discord-py-interactions-5.3.1/setup.py` & `discord-py-interactions-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/consts.py` & `discord-py-interactions-5.4.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/test_bot.py` & `discord-py-interactions-5.4.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/test_cache.py` & `discord-py-interactions-5.4.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/test_contexts.py` & `discord-py-interactions-5.4.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/test_cooldowns.py` & `discord-py-interactions-5.4.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/test_emoji.py` & `discord-py-interactions-5.4.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.3.1/tests/utils.py` & `discord-py-interactions-5.4.0/tests/utils.py`

 * *Files identical despite different names*

