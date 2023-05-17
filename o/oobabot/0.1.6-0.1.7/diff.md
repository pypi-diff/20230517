# Comparing `tmp/oobabot-0.1.6.tar.gz` & `tmp/oobabot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.6.tar", max compression
+gzip compressed data, was "oobabot-0.1.7.tar", max compression
```

## Comparing `oobabot-0.1.6.tar` & `oobabot-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.6/LICENSE
--rw-r--r--   0        0        0    14255 2023-05-14 08:14:21.162473 oobabot-0.1.6/README.md
--rw-r--r--   0        0        0      987 2023-05-14 08:29:00.042268 oobabot-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-14 08:28:58.302268 oobabot-0.1.6/src/oobabot/__init__.py
--rw-r--r--   0        0        0       69 2023-05-14 06:37:29.703837 oobabot-0.1.6/src/oobabot/__main__.py
--rw-r--r--   0        0        0     6229 2023-05-14 05:49:01.714519 oobabot-0.1.6/src/oobabot/bot_commands.py
--rw-r--r--   0        0        0     7043 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/decide_to_respond.py
--rw-r--r--   0        0        0    14456 2023-05-14 05:54:37.044441 oobabot-0.1.6/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     2174 2023-05-14 05:55:27.114429 oobabot-0.1.6/src/oobabot/discord_utils.py
--rw-r--r--   0        0        0     1558 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/fancy_logger.py
--rw-r--r--   0        0        0     2570 2023-05-14 07:14:33.293315 oobabot-0.1.6/src/oobabot/http_client.py
--rw-r--r--   0        0        0     9315 2023-05-14 06:03:07.084322 oobabot-0.1.6/src/oobabot/image_generator.py
--rw-r--r--   0        0        0     4098 2023-05-14 07:14:33.293315 oobabot-0.1.6/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     7661 2023-05-14 07:24:24.833176 oobabot-0.1.6/src/oobabot/oobabot.py
--rw-r--r--   0        0        0     8104 2023-05-14 06:03:31.764314 oobabot-0.1.6/src/oobabot/prompt_generator.py
--rw-r--r--   0        0        0     2861 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/repetition_tracker.py
--rw-r--r--   0        0        0     6647 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/response_stats.py
--rw-r--r--   0        0        0    10298 2023-05-14 07:14:33.293315 oobabot-0.1.6/src/oobabot/sd_client.py
--rw-r--r--   0        0        0     2695 2023-05-09 03:46:59.468832 oobabot-0.1.6/src/oobabot/sentence_splitter.py
--rw-r--r--   0        0        0    12294 2023-05-14 07:23:55.493183 oobabot-0.1.6/src/oobabot/settings.py
--rw-r--r--   0        0        0     6709 2023-05-14 06:04:39.674301 oobabot-0.1.6/src/oobabot/templates.py
--rw-r--r--   0        0        0     1113 2023-05-13 21:40:59.931392 oobabot-0.1.6/src/oobabot/types.py
--rw-r--r--   0        0        0    15045 1970-01-01 00:00:00.000000 oobabot-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.7/LICENSE
+-rw-r--r--   0        0        0    14228 2023-05-17 14:39:21.124910 oobabot-0.1.7/README.md
+-rw-r--r--   0        0        0     1240 2023-05-17 14:40:10.716786 oobabot-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-05-17 14:40:16.710666 oobabot-0.1.7/src/oobabot/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-14 14:34:31.204759 oobabot-0.1.7/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     6141 2023-05-16 18:04:52.618218 oobabot-0.1.7/src/oobabot/bot_commands.py
+-rw-r--r--   0        0        0     7132 2023-05-16 18:45:57.071008 oobabot-0.1.7/src/oobabot/decide_to_respond.py
+-rw-r--r--   0        0        0    17606 2023-05-17 13:55:33.467250 oobabot-0.1.7/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-17 06:48:28.290145 oobabot-0.1.7/src/oobabot/discord_utils.py
+-rw-r--r--   0        0        0     1557 2023-05-14 14:34:31.203723 oobabot-0.1.7/src/oobabot/fancy_logger.py
+-rw-r--r--   0        0        0     2602 2023-05-14 14:34:31.197932 oobabot-0.1.7/src/oobabot/http_client.py
+-rw-r--r--   0        0        0    10740 2023-05-16 12:52:44.722682 oobabot-0.1.7/src/oobabot/image_generator.py
+-rw-r--r--   0        0        0     7927 2023-05-17 06:48:28.291422 oobabot-0.1.7/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     7376 2023-05-17 07:24:58.226500 oobabot-0.1.7/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0     9557 2023-05-17 15:18:05.783839 oobabot-0.1.7/src/oobabot/overengineered_settings_parser.py
+-rw-r--r--   0        0        0     8197 2023-05-17 06:48:28.292148 oobabot-0.1.7/src/oobabot/prompt_generator.py
+-rw-r--r--   0        0        0     2893 2023-05-14 14:34:31.197478 oobabot-0.1.7/src/oobabot/repetition_tracker.py
+-rw-r--r--   0        0        0     6583 2023-05-14 14:34:31.198417 oobabot-0.1.7/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0     9430 2023-05-17 13:29:23.484593 oobabot-0.1.7/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0    24621 2023-05-17 15:18:56.717729 oobabot-0.1.7/src/oobabot/settings.py
+-rw-r--r--   0        0        0     8910 2023-05-17 13:25:50.645781 oobabot-0.1.7/src/oobabot/templates.py
+-rw-r--r--   0        0        0     1153 2023-05-17 06:48:28.293012 oobabot-0.1.7/src/oobabot/types.py
+-rw-r--r--   0        0        0    15065 1970-01-01 00:00:00.000000 oobabot-0.1.7/PKG-INFO
```

### Comparing `oobabot-0.1.6/LICENSE` & `oobabot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.6/README.md` & `oobabot-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -69,94 +69,96 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [--discord-token] [--dont-split-responses]
-               [--history-lines HISTORY_LINES] [--ignore-dms] [--wakewords [WAKEWORDS ...]]
-               [--ai-name AI_NAME] [--base-url BASE_URL] [--log-all-the-things]
-               [--persona PERSONA] [--reply-in-thread] [--diffusion-steps DIFFUSION_STEPS]
-               [--image-height IMAGE_HEIGHT] [--image-width IMAGE_WIDTH]
-               [--image-words [IMAGE_WORDS ...]]
-               [--stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER]
+usage: oobabot [-h] [-c CONFIG] [--generate-config] [--ai-name AI_NAME] [--persona PERSONA]
+               [--wakewords [WAKEWORDS ...]] [--discord-token DISCORD_TOKEN]
+               [--dont-split-responses] [--history-lines HISTORY_LINES] [--ignore-dms]
+               [--reply-in-thread] [--stream-responses] [--base-url BASE_URL]
+               [--log-all-the-things] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
-               [--sd-negative-prompt SD_NEGATIVE_PROMPT]
-               [--sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW]
+               [--extra-prompt-text EXTRA_PROMPT_TEXT]
 
-Discord bot for oobabooga's text-generation-webui
+oobabot v0.1.7: Discord bot for oobabooga's text-generation-webui
 
-options:
-  -h, --help            show this help message and exit
+General Settings:
 
-Discord Settings:
-  --discord-token       Token to log into Discord with. For security purposes it's strongly
-                        recommended that you set this via the DISCORD_TOKEN environment
-                        variable instead, if possible.
-  --dont-split-responses
-                        If set, the bot post its entire response as a single message,
-                        rather than splitting it into seperate messages by sentence.
-  --history-lines HISTORY_LINES
-                        Number of lines of chat history the AI will see when generating a
-                        response. The default is 15.
-  --ignore-dms          If set, the bot will ignore direct messages.
+  -h, --help
+  -c CONFIG, --config CONFIG
+                        Path to a config file to read settings from. Command line settings
+                        will override settings in this file. (default: config.yml)
+  --generate-config     If set, oobabot will print its configuration as a .yml file, then
+                        exit. Any command-line settings also passed will be reflected in
+                        this file. (default: False)
+
+Persona:
+
+  --ai-name AI_NAME     Name the AI will use to refer to itself (default: oobabot)
+  --persona PERSONA     This prefix will be added in front of every user-supplied request.
+                        This is useful for setting up a 'character' for the bot to play.
+                        Alternatively, this can be set with the OOBABOT_PERSONA environment
+                        variable. (default: )
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen
                         in all discord channels can access for one of these words to be
                         mentioned, then reply to any messages it sees with a matching word.
                         The bot will always reply to @-mentions and direct messages, even
-                        if no wakewords are supplied.
+                        if no wakewords are supplied. (default: ['oobabot'])
+
+Discord:
+
+  --discord-token DISCORD_TOKEN
+                        Token to log into Discord with. For security purposes it's strongly
+                        recommended that you set this via the DISCORD_TOKEN environment
+                        variable instead, if possible. (default: )
+  --dont-split-responses
+                        Post the entire response as a single message, rather than splitting
+                        it into seperate messages by sentence. (default: False)
+  --history-lines HISTORY_LINES
+                        Number of lines of chat history the AI will see when generating a
+                        response. (default: 7)
+  --ignore-dms          If set, the bot will not respond to direct messages. (default:
+                        False)
+  --reply-in-thread     If set, the bot will generate a thread to respond in if it is not
+                        already in one. (default: False)
+  --stream-responses    Stream responses into a single message as they are generated.
+                        (default: False)
+
+Oobabooga:
 
-Oobabooga Seetings:
-  --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want,
-                        but might make sense to be the name of the bot in Discord.
   --base-url BASE_URL   Base URL for the oobabooga instance. This should be
                         ws://hostname[:port] for plain websocket connections, or
-                        wss://hostname[:port] for websocket connections over TLS.
-  --log-all-the-things  Prints all oobabooga requests and responses in their entirety to
-                        STDOUT
-  --persona PERSONA     This prefix will be added in front of every user-supplied request.
-                        This is useful for setting up a 'character' for the bot to play.
-                        Alternatively, this can be set with the OOBABOT_PERSONA environment
-                        variable.
-  --reply-in-thread     When set, the bot will generate a new thread for each response it
-                        generates. But it will only do so if the user who prompted the bot
-                        has thread-create permissions.
-
-Stable Diffusion Settings:
-  --diffusion-steps DIFFUSION_STEPS
-                        Number of diffusion steps to take when generating an image. The
-                        default is 30.
-  --image-height IMAGE_HEIGHT
-                        Size of images to generate. This is the height of the image in
-                        pixels. The default is 512.
-  --image-width IMAGE_WIDTH
-                        Size of images to generate. This is the width of the image in
-                        pixels. The default is 512.
+                        wss://hostname[:port] for websocket connections over TLS. (default:
+                        ws://localhost:5005)
+  --log-all-the-things  Print all AI input and output to STDOUT. (default: False)
+
+Stable Diffusion:
+
   --image-words [IMAGE_WORDS ...]
-                        One or more words that will indicate the user is requeting an image
-                        to be generated.
-  --stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER, --sd-sampler STABLE_DIFFUSION_SAMPLER
-                        Sampler to use when generating images. If not specified, the one
-                        set on the AUTOMATIC1111 server will be used.
-  --stable-diffusion-url STABLE_DIFFUSION_URL, --sd-url STABLE_DIFFUSION_URL
-                        URL for an AUTOMATIC1111 Stable Diffusion server
-  --sd-negative-prompt SD_NEGATIVE_PROMPT
-                        Negative prompt to use when generating images. This will discourage
-                        Stable Diffusion from generating images with the specified content.
-                        By default, this is set to follow Discord's TOS.
-  --sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW
-                        Negative prompt to use when generating images in a channel marked
-                        as'Age-Restricted'.
+                        When one of these words is used in a message, the bot will generate
+                        an image. (default: ['drawing', 'photo', 'pic', 'picture', 'image',
+                        'sketch'])
+  --stable-diffusion-url STABLE_DIFFUSION_URL
+                        URL for an AUTOMATIC1111 Stable Diffusion server. (default: )
+  --extra-prompt-text EXTRA_PROMPT_TEXT
+                        This will be appended to every image generation prompt sent to
+                        Stable Diffusion. (default: )
+
+
+Additional settings can be set in config.yml.  Use the --generate-config option to print a
+new copy of this file to STDOUT.
 
-Also, to authenticate to Discord, you must set the environment variable: DISCORD_TOKEN =
-<your bot's discord token>
+Please set the 'DISCORD_TOKEN' environment variable to your bot's discord token.
 ```
 
+There are **a lot more settings** in the [config.yml file (sample)](./docs/config.sample.yml) here.
+
 ## Required settings
 
 - **`DISCORD_TOKEN`** environment variable
 
    Set your shell environment's **`DISCORD_TOKEN`** to token Discord provided when you set up the bot account.  It should be something like a 72-character-long random-looking string.
 
     **bash example**
@@ -290,16 +292,26 @@
 | **`/lobotomize`** | make the bot forget everything in the channel before the command is run |
 | **`/say "message"`** | speak as the bot |
 
 Oobabot doesn't add any restrictions on who can run these commands, but luckily Discord does!  You can find this inside Discord by visiting "Server Settings" -> Integrations -> Bots and Apps -> hit the icon which looks like [/] next to your bot
 
 If you're running on a large server, you may want to restrict who can run these commands.  I suggest creating a new role, and only allowing that role to run the commands.
 
+## Using a config file
+
+Instead of the command line, you can also use a config file.  This is useful if you want to run multiple instances of the bot, or if you want to run it as a service.
+
+There are also many more settings available in the config file, which are not available on the command line.  See [docs/CONFIG.md](./docs/CONFIG.md) for information on how to use it.
+
+You can also look at a [config.yml file (sample)](./docs/config.sample.yml) here.
+
 ## Known Issues
 
 - detection of requests for photos is very crude, and will likely be improved in the future.
-- some of the default settings are very specific to my use case, and will likely be made
-  configurable in the future
 - public threads in 'age restricted' channels are treated as if they
   were not age-restricted
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
 - found one not listed here?  Have an idea?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
+
+## Contributing
+
+Contributions are welcome!  Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
```

### Comparing `oobabot-0.1.6/src/oobabot/bot_commands.py` & `oobabot-0.1.7/src/oobabot/bot_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+# -*- coding: utf-8 -*-
 import typing
 
 import discord
 
 from oobabot import decide_to_respond
 from oobabot import discord_utils
 from oobabot import fancy_logger
 from oobabot import repetition_tracker
 from oobabot import templates
 
 
 class BotCommands:
     def __init__(
         self,
-        ai_name: str,
         decide_to_respond: decide_to_respond.DecideToRespond,
         repetition_tracker: repetition_tracker.RepetitionTracker,
-        reply_in_thread: bool,
+        persona_settings: dict,
+        discord_settings: dict,
         template_store: templates.TemplateStore,
     ):
-        self.ai_name = ai_name
+        self.ai_name = persona_settings["ai_name"]
         self.decide_to_respond = decide_to_respond
         self.repetition_tracker = repetition_tracker
-        self.reply_in_thread = reply_in_thread
+        self.reply_in_thread = discord_settings["reply_in_thread"]
         self.template_store = template_store
 
     async def on_ready(self, client: discord.Client):
         """
         Register commands with Discord.
         """
 
@@ -91,15 +92,17 @@
             if self.reply_in_thread:
                 channel = await get_messageable(interaction)
                 if channel is None or isinstance(channel, discord.TextChannel):
                     await fail(interaction, f"{self.ai_name} may only speak in threads")
                     return
 
             fancy_logger.get().debug(
-                f"say called by {interaction.user.name} in {interaction.channel_id}"
+                "/say called by user '%s' in channel #%d",
+                interaction.user.name,
+                interaction.channel_id,
             )
             # this will cause the bot to monitor the channel
             # and consider unsolicited responses
             self.decide_to_respond.log_mention_raw(
                 channel_id=interaction.channel_id,
                 send_timestamp=interaction.created_at.timestamp(),
             )
@@ -118,16 +121,17 @@
 
             # find the current message in this channel
             # tell the Repetition Tracker to hide messages
             # before this message
             async for message in channel.history(limit=1):
                 channel_name = discord_utils.get_channel_name(channel)
                 fancy_logger.get().info(
-                    f"lobotomize called in #{channel_name}, "
-                    + f"hiding messages before {message.id}"
+                    "/lobotomize called by user '%s' in #%s",
+                    interaction.user.name,
+                    channel_name,
                 )
                 self.repetition_tracker.hide_messages_before(
                     channel_id=channel.id,
                     message_id=message.id,
                 )
 
             response = self.template_store.format(
@@ -139,23 +143,18 @@
             )
             await interaction.response.send_message(
                 response,
                 silent=True,
             )
 
         fancy_logger.get().debug(
-            "Registering commands, this may take a while sometimes..."
+            "Registering commands, sometimes this takes a while..."
         )
 
         tree = discord.app_commands.CommandTree(client)
         tree.add_command(lobotomize)
         tree.add_command(say)
         commands = await tree.sync(guild=None)
         for command in commands:
             fancy_logger.get().info(
-                f"Registered command: {command.name}: {command.description}"
+                "Registered command: %s: %s", command.name, command.description
             )
-        fancy_logger.get().debug(
-            "If you try to run any command within the first ~5 minutes of "
-            + "the bot starting, it will fail with the error: 'This command "
-            + "is outdated,...'."
-        )
```

### Comparing `oobabot-0.1.6/src/oobabot/decide_to_respond.py` & `oobabot-0.1.7/src/oobabot/decide_to_respond.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import random
 import re
 import typing
 
 from oobabot import fancy_logger
 from oobabot import types
 
@@ -41,21 +42,21 @@
 class DecideToRespond:
     """
     Decide whether to respond to a message.
     """
 
     def __init__(
         self,
-        wakewords: typing.List[str],
-        ignore_dms: bool,
+        discord_settings: dict,
+        persona_settings: dict,
         interrobang_bonus: float,
         time_vs_response_chance: typing.List[typing.Tuple[float, float]],
     ):
-        self.wakewords = wakewords
-        self.ignore_dms = ignore_dms
+        self.wakewords = persona_settings["wakewords"]
+        self.ignore_dms = discord_settings["ignore_dms"]
         self.interrobang_bonus = interrobang_bonus
         self.time_vs_response_chance = time_vs_response_chance
 
         last_reply_cache_timeout = max(time for time, _ in time_vs_response_chance)
         self.last_reply_times = LastReplyTimes(last_reply_cache_timeout)
 
         # match messages that include any `wakeword`, but not as part of
@@ -135,17 +136,19 @@
 
         # if the new message ends with an exclamation point, we'll respond
         if message.body_text.endswith("!"):
             response_chance += self.interrobang_bonus
 
         time_since_last_mention = self.last_reply_times.time_since_last_mention(message)
         fancy_logger.get().debug(
-            f"Considering unsolicited message in channel {message.channel_name} "
-            f"after {time_since_last_mention:2.0f} seconds, "
-            f"with chance {response_chance*100.0:2.0f}%."
+            "Considering unsolicited response in channel %s after %2.0f seconds.  "
+            + "chance: %2.0f%%.",
+            message.channel_name,
+            time_since_last_mention,
+            response_chance * 100.0,
         )
 
         if random.random() < response_chance:
             return True
 
         return False
```

### Comparing `oobabot-0.1.6/src/oobabot/discord_bot.py` & `oobabot-0.1.7/src/oobabot/discord_bot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 # Purpose: Discord client for Rosie
 #
 
 import asyncio
 import typing
 
 import discord
@@ -15,132 +16,128 @@
 from oobabot import prompt_generator
 from oobabot import repetition_tracker
 from oobabot import response_stats
 from oobabot import types
 
 
 class DiscordBot(discord.Client):
-    # seconds after which we'll lazily purge a channel
-    # from channel_last_direct_response
-
     def __init__(
         self,
         ooba_client: ooba_client.OobaClient,
         decide_to_respond: decide_to_respond.DecideToRespond,
         prompt_generator: prompt_generator.PromptGenerator,
         repetition_tracker: repetition_tracker.RepetitionTracker,
         response_stats: response_stats.AggregateResponseStats,
         bot_commands: bot_commands.BotCommands,
         image_generator: typing.Optional[image_generator.ImageGenerator],
-        ai_name: str,
-        persona: str,
-        ignore_dms: bool,
-        dont_split_responses: bool,
-        reply_in_thread: bool,
-        log_all_the_things: bool,
+        discord_settings: dict,
+        persona_settings: dict,
     ):
-        self.ooba_client = ooba_client
+        self.bot_commands = bot_commands
         self.decide_to_respond = decide_to_respond
+        self.image_generator = image_generator
+        self.ooba_client = ooba_client
         self.prompt_generator = prompt_generator
         self.repetition_tracker = repetition_tracker
         self.response_stats = response_stats
 
-        self.ai_name = ai_name
-        self.persona = persona
+        self.ai_name = persona_settings["ai_name"]
+        self.persona = persona_settings["persona"]
         self.ai_user_id = -1
-        self.image_generator = image_generator
-
-        self.ignore_dms = ignore_dms
-        self.dont_split_responses = dont_split_responses
-        self.reply_in_thread = reply_in_thread
-        self.log_all_the_things = log_all_the_things
 
-        # a list of timestamps in which we last posted to a channel
-        self.channel_last_direct_response = {}
-
-        self.bot_commands = bot_commands
+        self.dont_split_responses = discord_settings["dont_split_responses"]
+        self.ignore_dms = discord_settings["ignore_dms"]
+        self.reply_in_thread = discord_settings["reply_in_thread"]
+        self.stop_markers = discord_settings["stop_markers"]
+        self.stream_responses = discord_settings["stream_responses"]
 
         intents = discord.Intents.default()
         intents.message_content = True
         intents.members = True
 
         super().__init__(intents=intents)
 
     async def on_ready(self) -> None:
         guilds = self.guilds
         num_guilds = len(guilds)
-        num_channels = sum([len(guild.channels) for guild in guilds])
+        num_channels = sum(len(guild.channels) for guild in guilds)
 
         if self.user:
             self.ai_user_id = self.user.id
             user_id_str = str(self.ai_user_id)
         else:
             user_id_str = "<unknown>"
 
         fancy_logger.get().info(
-            f"Connected to discord as {self.user} (ID: {user_id_str})"
+            "Connected to discord as %s (ID: %d)", user_id_str, self.ai_user_id
         )
         fancy_logger.get().debug(
-            f"monitoring {num_channels} channels across " + f"{num_guilds} server(s)"
+            "monitoring %d channels across %d server(s)", num_channels, num_guilds
         )
         if self.ignore_dms:
             fancy_logger.get().debug("Ignoring DMs")
         else:
             fancy_logger.get().debug("listening to DMs")
 
-        if self.dont_split_responses:
+        if self.stream_responses:
+            fancy_logger.get().debug("Responses: streamed live")
+        elif self.dont_split_responses:
             fancy_logger.get().debug("Responses: returned as single messages")
         else:
             fancy_logger.get().debug("Responses: streamed as separate sentences")
 
         if self.image_generator:
             fancy_logger.get().debug("Image generation: enabled")
         else:
             fancy_logger.get().debug("Image generation: disabled")
 
-        fancy_logger.get().debug(f"AI name: {self.ai_name}")
-        fancy_logger.get().debug(f"AI persona: {self.persona}")
+        fancy_logger.get().debug("AI name: %s", self.ai_name)
+        fancy_logger.get().debug("AI persona: %s", self.persona)
+
+        fancy_logger.get().debug(
+            "History: %d lines ", self.prompt_generator.history_lines
+        )
 
         fancy_logger.get().debug(
-            f"History: {self.prompt_generator.history_lines} lines "
+            "Stop markers: %s", ", ".join(self.stop_markers) or "<none>"
         )
 
         str_wakewords = (
             ", ".join(self.decide_to_respond.wakewords)
             if self.decide_to_respond.wakewords
             else "<none>"
         )
-        fancy_logger.get().debug(f"Wakewords: {str_wakewords}")
+        fancy_logger.get().debug("Wakewords: %s", str_wakewords)
 
         # we do this at the very end because when you restart
         # the bot, it can take a while for the commands to
         # register
         try:
             # register the commands
             await self.bot_commands.on_ready(self)
-        except Exception as e:
+        except discord.DiscordException as err:
             fancy_logger.get().warning(
-                f"Failed to register commands: {e} (continuing without commands)"
+                "Failed to register commands: %s (continuing without commands)", err
             )
 
     async def on_message(self, raw_message: discord.Message) -> None:
         try:
             message = discord_utils.discord_message_to_generic_message(raw_message)
             should_respond, is_summon = self.decide_to_respond.should_reply_to_message(
                 self.ai_user_id, message
             )
             if not should_respond:
                 return
 
             async with raw_message.channel.typing():
                 await self._handle_response(message, raw_message, is_summon)
 
-        except Exception as e:
+        except discord.DiscordException as err:
             fancy_logger.get().error(
-                f"Exception while processing message: {e}", exc_info=True
+                "Exception while processing message: %s", err, exc_info=True
             )
 
     async def _handle_response(
         self,
         message: types.GenericMessage,
         raw_message: discord.Message,
         is_summon: bool,
@@ -193,14 +190,28 @@
             )
 
         response_tasks = [
             task for task in [message_task, image_task] if task is not None
         ]
         await asyncio.wait(response_tasks)
 
+        # there may be more than one exception, so be sure to log
+        # them all before raising either of them
+        raise_later = None
+        for task in response_tasks:
+            if task.exception() is not None:
+                fancy_logger.get().error(
+                    f"Exception while running {task.get_coro()} "
+                    + f"response: {task.exception()}",
+                    stack_info=True,
+                )
+                raise_later = task.exception()
+        if raise_later is not None:
+            raise raise_later
+
     async def send_response(
         self,
         message: types.GenericMessage,
         raw_message: discord.Message,
         image_requested: bool,
     ) -> typing.Optional[typing.Tuple[asyncio.Task, discord.abc.Messageable]]:
         """
@@ -240,39 +251,39 @@
                 # second user's response, and again for a third user,
                 # etc.
                 fancy_logger.get().debug("User can't create threads, not responding.")
                 return None
 
         response_coro = self.send_response_in_channel(
             message=message,
-            raw_message=raw_message,
             image_requested=image_requested,
             response_channel=response_channel,
+            response_channel_id=response_channel.id,
         )
         response_task = asyncio.create_task(response_coro)
         return (response_task, response_channel)
 
     async def history_plus_thread_kickoff_message(
         self,
-        aiter: typing.AsyncIterator[discord.Message],
+        aiter_history: typing.AsyncIterator[discord.Message],
         limit: int,
     ) -> typing.AsyncIterator[types.GenericMessage]:
         """
         When returning the history of a thread, Discord
         does not include the message that kicked off the thread.
 
         It will show it in the UI as if it were, but it's not
         one of the messages returned by the history iterator.
 
         This method attempts to return that message as well,
         if we need it.
         """
         items = 0
         last_returned = None
-        async for item in aiter:
+        async for item in aiter_history:
             last_returned = item
             yield discord_utils.discord_message_to_generic_message(item)
             items += 1
         if last_returned is not None and items < limit:
             # we've reached the beginning of the history, but
             # still have space.  If this message was a reply
             # to another message, return that message as well.
@@ -290,94 +301,158 @@
             limit=self.prompt_generator.history_lines,
         )
         return result
 
     async def send_response_in_channel(
         self,
         message: types.GenericMessage,
-        raw_message: discord.Message,
         image_requested: bool,
         response_channel: discord.abc.Messageable,
+        response_channel_id: int,
     ) -> None:
         fancy_logger.get().debug(
-            f"Request from {message.author_name} in {message.channel_name}"
+            "Request from %s in %s", message.author_name, message.channel_name
         )
 
         recent_messages = await self.recent_messages_following_thread(response_channel)
 
         repeated_id = self.repetition_tracker.get_throttle_message_id(
-            raw_message.channel.id
+            response_channel_id
         )
 
         prompt_prefix = await self.prompt_generator.generate(
             ai_user_id=self.ai_user_id,
             message_history=recent_messages,
             image_requested=image_requested,
             throttle_message_id=repeated_id,
         )
 
         this_response_stat = self.response_stats.log_request_arrived(prompt_prefix)
-        if self.log_all_the_things:
-            print("prompt_prefix:\n----------\n")
-            print(prompt_prefix)
-            print("Response:\n----------\n")
 
         try:
-            if self.dont_split_responses:
-                generator = self.ooba_client.request_as_string(prompt_prefix)
-            else:
-                generator = self.ooba_client.request_by_sentence(prompt_prefix)
-
-            async for sentence in generator:
-                if self.log_all_the_things:
-                    print(sentence)
-
-                sentence = self.filter_immersion_breaking_lines(sentence)
-                if not sentence:
-                    # we can't send an empty message
-                    continue
-
-                response_message = await response_channel.send(sentence)
-                generic_response_message = (
-                    discord_utils.discord_message_to_generic_message(response_message)
+            if self.stream_responses:
+                generator = self.ooba_client.request_as_grouped_tokens(prompt_prefix)
+                await self.render_streaming_response(
+                    generator,
+                    this_response_stat,
+                    response_channel,
+                    response_channel_id,
                 )
-                self.repetition_tracker.log_message(
-                    raw_message.channel.id, generic_response_message
+            else:
+                if self.dont_split_responses:
+                    generator = self.ooba_client.request_as_string(prompt_prefix)
+                else:
+                    generator = self.ooba_client.request_by_sentence(prompt_prefix)
+                await self.render_response(
+                    generator, this_response_stat, response_channel, response_channel_id
                 )
 
-                this_response_stat.log_response_part()
-
-        except Exception as err:
-            fancy_logger.get().error(f"Error: {str(err)}")
+        except discord.DiscordException as err:
+            fancy_logger.get().error("Error: %s", err, exc_info=True)
             self.response_stats.log_response_failure()
             return
 
         this_response_stat.write_to_log(f"Response to {message.author_name} done!  ")
         self.response_stats.log_response_success(this_response_stat)
 
-    def filter_immersion_breaking_lines(self, sentence: str) -> str:
+    async def render_response(
+        self,
+        response_iterator: typing.AsyncIterator[str],
+        this_response_stat: response_stats.ResponseStats,
+        response_channel: discord.abc.Messageable,
+        response_channel_id: int,
+    ):
+        async for sentence in response_iterator:
+            (sentence, abort_response) = self.filter_immersion_breaking_lines(sentence)
+            if abort_response:
+                break
+            if not sentence:
+                # we can't send an empty message
+                continue
+
+            response_message = await response_channel.send(sentence)
+            generic_response_message = discord_utils.discord_message_to_generic_message(
+                response_message
+            )
+            self.repetition_tracker.log_message(
+                response_channel_id, generic_response_message
+            )
+
+            this_response_stat.log_response_part()
+
+    async def render_streaming_response(
+        self,
+        response_iterator: typing.AsyncIterator[str],
+        this_response_stat: response_stats.ResponseStats,
+        response_channel: discord.abc.Messageable,
+        response_channel_id: int,
+    ):
+        response = ""
+        last_message = None
+        async for token in response_iterator:
+            if "" == token:
+                continue
+
+            response += token
+            (response, abort_response) = self.filter_immersion_breaking_lines(response)
+            if abort_response:
+                break
+            if not response:
+                # we can't send an empty message
+                continue
+
+            if last_message is None:
+                # when we send the first message, we don't want to send a notification,
+                # as it will only include the first token of the response.  This will
+                # not be very useful to anyone.
+                last_message = await response_channel.send(response, silent=True)
+            else:
+                await last_message.edit(content=response)
+
+            this_response_stat.log_response_part()
+
+        if last_message is None:
+            raise discord.DiscordException("No response was generated")
+
+        generic_response_message = discord_utils.discord_message_to_generic_message(
+            last_message
+        )
+        self.repetition_tracker.log_message(
+            response_channel_id, generic_response_message
+        )
+
+    def filter_immersion_breaking_lines(self, sentence: str) -> typing.Tuple[str, bool]:
         lines = sentence.split("\n")
         good_lines = []
         previous_line = ""
+        abort_response = False
         for line in lines:
             # if the AI gives itself a second line, just ignore
             # the line instruction and continue
             if self.prompt_generator.bot_prompt_line == line:
                 fancy_logger.get().warning(
-                    f'Filtered out "{line}" from response, continuing'
+                    "Filtered out %s from response, continuing", line
                 )
                 continue
 
             # hack: abort response if it looks like the AI is
             # continuing the conversation as someone else
             if line.endswith(" says:"):
                 fancy_logger.get().warning(
-                    f'Filtered out "{line}" from response, aborting'
+                    'Filtered out "%s" from response, aborting', line
+                )
+                abort_response = True
+                break
+
+            if line in self.stop_markers:
+                fancy_logger.get().warning(
+                    'Filtered out "%s" from response, aborting', line
                 )
+                abort_response = True
                 break
 
             if not line and not previous_line:
                 # filter out multiple blank lines in a row
                 continue
 
             good_lines.append(line)
-        return "\n".join(good_lines)
+        return ("\n".join(good_lines), abort_response)
```

### Comparing `oobabot-0.1.6/src/oobabot/discord_utils.py` & `oobabot-0.1.7/src/oobabot/discord_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import re
 import typing
 
 import discord
 
 from oobabot import fancy_logger
 from oobabot import types
@@ -40,21 +41,22 @@
         "author_name": sanitize_string(raw_message.author.display_name),
         "channel_id": raw_message.channel.id,
         "channel_name": get_channel_name(raw_message.channel),
         "message_id": raw_message.id,
         "body_text": sanitize_string(raw_message.content),
         "author_is_bot": raw_message.author.bot,
         "send_timestamp": raw_message.created_at.timestamp(),
+        "reference_message_id": raw_message.reference.message_id
+        if raw_message.reference
+        else "",
     }
     if isinstance(raw_message.channel, discord.DMChannel):
         return types.DirectMessage(**generic_args)
-    if (
-        isinstance(raw_message.channel, discord.TextChannel)
-        or isinstance(raw_message.channel, discord.GroupChannel)
-        or isinstance(raw_message.channel, discord.Thread)
+    if isinstance(
+        raw_message.channel, (discord.TextChannel, discord.GroupChannel, discord.Thread)
     ):
         return types.ChannelMessage(
             mentions=[mention.id for mention in raw_message.mentions],
             **generic_args,
         )
     fancy_logger.get().warning(
         f"Unknown channel type {type(raw_message.channel)}, "
```

### Comparing `oobabot-0.1.6/src/oobabot/fancy_logger.py` & `oobabot-0.1.7/src/oobabot/fancy_logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import logging
 
 FOREGROUND_COLORS = {
     "black": 30,
     "red": 31,
     "green": 32,
     "yellow": 33,
@@ -27,25 +28,24 @@
 }
 
 
 class ColorfulLoggingFormatter(logging.Formatter):
     def __init__(self) -> None:
         super().__init__()
         self.formatters = {}
-        for logging_level in FORMATS.keys():
+        for logging_level in FORMATS:
             self.formatters[logging_level] = logging.Formatter(
                 FORMATS.get(logging_level)
             )
 
     def format(self, record: logging.LogRecord) -> str:
         formatter = self.formatters.get(record.levelno)
         if formatter:
             return formatter.format(record)
-        else:
-            return record.getMessage()
+        return record.getMessage()
 
 
 def get(name: str = "oobabot") -> logging.Logger:
     return logging.getLogger(name)
 
 
 def init_logging() -> logging.Logger:
```

### Comparing `oobabot-0.1.6/src/oobabot/http_client.py` & `oobabot-0.1.7/src/oobabot/http_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import abc
 import asyncio
 import socket
 
 import aiohttp
 
 
@@ -41,18 +42,18 @@
             await self._setup()
         except (
             aiohttp.ClientConnectionError,
             aiohttp.ClientError,
             ConnectionRefusedError,
             socket.gaierror,
             asyncio.exceptions.TimeoutError,
-        ) as e:
+        ) as err:
             raise OobaHttpClientError(
                 f"Could not connect to {self.service_name} server: [{self.base_url}]"
-            ) from e
+            ) from err
 
     def __init__(self, sevice_name: str, base_url: str):
         self.service_name = sevice_name
         self.base_url = base_url
         self._session = None
 
     def get_session(self) -> aiohttp.ClientSession:
@@ -77,14 +78,14 @@
     def test_connection(self) -> None:
         async def try_setup():
             async with self:
                 await self.setup()
 
         try:
             asyncio.run(try_setup())
-        except AssertionError as e:
+        except AssertionError as err:
             # asyncio will throw an AssertionError if we try to run
             # with a base_url that has a path.  This is a user-supplied
             # value, so catching this is grody but necessary.
             raise OobaHttpClientError(
                 f"Could not connect to {self.service_name} server: [{self.base_url}]"
-            ) from e
+            ) from err
```

### Comparing `oobabot-0.1.6/src/oobabot/image_generator.py` & `oobabot-0.1.7/src/oobabot/image_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+# -*- coding: utf-8 -*-
 import asyncio
 import io
 import re
 import typing
 
 import discord
 
 from oobabot import fancy_logger
+from oobabot import http_client
 from oobabot import sd_client
 from oobabot import templates
 
 
 async def image_task_to_file(image_task: "asyncio.Task[bytes]", image_request: str):
     await image_task
     img_bytes = image_task.result()
@@ -23,17 +25,28 @@
 class StableDiffusionImageView(discord.ui.View):
     """
     A View that displays buttons to regenerate an image
     from Stable Diffusion with a new seed, or to lock
     in the current image.
     """
 
+    LABEL_ACCEPT = "Accept"
+    LABEL_DELETE = "Delete"
+
+    # these two phrases (along with exactly two periods)
+    # in "Drawing.." were chosen because they render at
+    # the exact same width as each other.  If they don't,
+    # the buttons will shift to the left and right as the
+    # labels are swapped.
+    LABEL_TRY_AGAIN = "Try Again"
+    LABEL_DRAWING = "Drawing.."
+
     def __init__(
         self,
-        sd_client: sd_client.StableDiffusionClient,
+        stable_diffusion_client: sd_client.StableDiffusionClient,
         is_channel_nsfw: bool,
         image_prompt: str,
         requesting_user_id: int,
         requesting_user_name: str,
         template_store: templates.TemplateStore,
     ):
         super().__init__(timeout=120.0)
@@ -47,42 +60,65 @@
         self.image_prompt = image_prompt
         self.photo_accepted = False
 
         #####################################################
         # "Try Again" button
         #
         btn_try_again = discord.ui.Button(
-            label="Try Again",
+            label=self.LABEL_TRY_AGAIN,
             style=discord.ButtonStyle.blurple,
             row=1,
         )
         self.image_message = None
 
         async def on_try_again(interaction: discord.Interaction):
             result = await self.diy_interaction_check(interaction)
             if not result:
                 # unauthorized user
                 return
 
             try:
+                btn_try_again.label = self.LABEL_DRAWING
+
+                # we disable all three buttons because otherwise
+                # the lock_in and delete buttons will flicker
+                # when we disable the try_again button.  And it
+                # doesn't make much sense for them to work anyway
+                # when the button is being regenerated.
+                btn_try_again.disabled = True
+                btn_lock_in.disabled = True
+                btn_delete.disabled = True
+
+                await interaction.response.defer()
+                await self.get_image_message().edit(view=self)
+
                 # generate a new image
-                regen_task = sd_client.generate_image(image_prompt, is_channel_nsfw)
+                regen_task = stable_diffusion_client.generate_image(
+                    image_prompt, is_channel_nsfw
+                )
                 regen_file = await image_task_to_file(regen_task, image_prompt)
-                await interaction.response.defer()
-                await self.get_image_message().edit(attachments=[regen_file])
-            except Exception as e:
-                fancy_logger.get().error(f"Could not regenerate image: {e}")
+
+                btn_try_again.label = self.LABEL_TRY_AGAIN
+                btn_try_again.disabled = False
+                btn_lock_in.disabled = False
+                btn_delete.disabled = False
+
+                await self.get_image_message().edit(attachments=[regen_file], view=self)
+            except (http_client.OobaHttpClientError, discord.DiscordException) as err:
+                fancy_logger.get().error(
+                    "Could not regenerate image: %s", err, exc_info=True
+                )
 
         btn_try_again.callback = on_try_again
 
         #####################################################
         # "Accept" button
         #
         btn_lock_in = discord.ui.Button(
-            label="Accept",
+            label=self.LABEL_ACCEPT,
             style=discord.ButtonStyle.success,
             row=1,
         )
 
         async def on_lock_in(interaction: discord.Interaction):
             result = await self.diy_interaction_check(interaction)
             if not result:
@@ -93,15 +129,15 @@
 
         btn_lock_in.callback = on_lock_in
 
         #####################################################
         # "Delete" button
         #
         btn_delete = discord.ui.Button(
-            label="Delete",
+            label=self.LABEL_DELETE,
             style=discord.ButtonStyle.danger,
             row=1,
         )
 
         async def on_delete(interaction: discord.Interaction):
             result = await self.diy_interaction_check(interaction)
             if not result:
@@ -202,16 +238,16 @@
             is_channel_nsfw = raw_message.channel.is_nsfw()
 
         image_task = self.stable_diffusion_client.generate_image(
             image_prompt, is_channel_nsfw=is_channel_nsfw
         )
         try:
             file = await image_task_to_file(image_task, image_prompt)
-        except Exception as e:
-            fancy_logger.get().error(f"Could not generate image: {e}")
+        except (http_client.OobaHttpClientError, discord.DiscordException) as err:
+            fancy_logger.get().error("Could not generate image: %s", err, exc_info=True)
             error_message = self.template_store.format(
                 templates.Templates.IMAGE_GENERATION_ERROR,
                 {
                     templates.TemplateToken.USER_NAME: raw_message.author.display_name,
                     templates.TemplateToken.IMAGE_PROMPT: image_prompt,
                 },
             )
@@ -241,24 +277,21 @@
         )
         regen_view.image_message = image_message
         return image_message
 
     def maybe_get_image_prompt(
         self, raw_message: discord.Message
     ) -> typing.Optional[str]:
-        image_prompt = None
         for image_pattern in self.image_patterns:
             match = image_pattern.search(raw_message.content)
             if match:
                 image_prompt = match.group(2)
+                fancy_logger.get().debug("Found image prompt: %s", image_prompt)
                 return image_prompt
-        if image_prompt is None:
-            return None
-
-        fancy_logger.get().debug("Found image prompt: %s", image_prompt)
+        return None
 
     async def generate_image(
         self,
         image_prompt: str,
         raw_message: discord.Message,
         response_channel: discord.abc.Messageable,
     ) -> typing.Optional["asyncio.Task[discord.Message]"]:
```

### Comparing `oobabot-0.1.6/src/oobabot/oobabot.py` & `oobabot-0.1.7/src/oobabot/oobabot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 
 import asyncio
+import contextlib
 import signal
 import sys
+import typing
 
 from oobabot import bot_commands
 from oobabot import decide_to_respond
 from oobabot import discord_bot
 from oobabot import fancy_logger
 from oobabot import http_client
 from oobabot import image_generator
@@ -18,176 +20,173 @@
 from oobabot import response_stats
 from oobabot import sd_client
 from oobabot import settings
 from oobabot import templates
 
 
 class OobaBot:
-    def __init__(self, cli_args=None):
+    def __init__(self, cli_args: typing.List[str]):
         fancy_logger.init_logging()
 
         self.settings = settings.Settings()
         self.settings.load(cli_args)
-        if not self.settings.discord_token:
-            msg = (
-                f"Please set the '{self.settings.DISCORD_TOKEN_ENV_VAR}' "
-                + "environment variable to your bot's discord token."
-            )
-            # will exit() after printing
-            self.settings.error(msg)
-
-        self.response_stats = None
-
-        def sigint_handler(_signum, _frame):
-            fancy_logger.get().info("Received SIGINT, exiting...")
-            if self.response_stats is not None:
-                self.response_stats.write_stat_summary_to_log()
-            exit(1)
 
-        signal.signal(signal.SIGINT, sigint_handler)
+        # templates used to generate prompts to send to the AI
+        # as well as for some UI elements
+        self.template_store = templates.TemplateStore(
+            settings=self.settings.template_settings.get_all()
+        )
 
         ########################################################
         # Connect to Oobabooga
 
         self.ooba_client = ooba_client.OobaClient(
-            self.settings.base_url, self.settings.OOBABOOGA_DEFAULT_REQUEST_PARAMS
+            settings=self.settings.oobabooga_settings.get_all(),
         )
 
         ########################################################
         # Connect to Stable Diffusion, if configured
 
         self.stable_diffusion_client = None
-        if self.settings.stable_diffusion_url:
+        sd_settings = self.settings.stable_diffusion_settings.get_all()
+        if sd_settings["stable_diffusion_url"]:
             self.stable_diffusion_client = sd_client.StableDiffusionClient(
-                base_url=self.settings.stable_diffusion_url,
-                negative_prompt=self.settings.stable_diffusion_negative_prompt,
-                negative_prompt_nsfw=self.settings.stable_diffusion_negative_prompt_nsfw,  # noqa: E501
-                image_width=self.settings.image_width,
-                image_height=self.settings.image_height,
-                steps=self.settings.diffusion_steps,
-                desired_sampler=self.settings.stable_diffusion_sampler,
+                settings=sd_settings,
             )
 
         ########################################################
         # Bot logic
 
         # decides which messages the bot will respond to
         self.decide_to_respond = decide_to_respond.DecideToRespond(
-            self.settings.wakewords,
-            self.settings.ignore_dms,
-            self.settings.DECIDE_TO_RESPOND_INTERROBANG_BONUS,
-            self.settings.DECIDE_TO_RESPOND_TIME_VS_RESPONSE_CHANCE,
+            discord_settings=self.settings.discord_settings.get_all(),
+            persona_settings=self.settings.persona_settings.get_all(),
+            interrobang_bonus=self.settings.DECIDE_TO_RESPOND_INTERROBANG_BONUS,
+            time_vs_response_chance=self.settings.TIME_VS_RESPONSE_CHANCE,
         )
 
-        # templates used to generate prompts to send to the AI
-        # as well as for some UI elements
-        self.template_store = templates.TemplateStore()
-
         # once we decide to respond, this generates a prompt
         # to send to the AI, given a message history
         self.prompt_generator = prompt_generator.PromptGenerator(
-            ai_name=self.settings.ai_name,
-            persona=self.settings.persona,
-            history_lines=self.settings.history_lines,
-            token_space=self.settings.OOBABOT_MAX_AI_TOKEN_SPACE,
+            discord_settings=self.settings.discord_settings.get_all(),
+            oobabooga_settings=self.settings.oobabooga_settings.get_all(),
+            persona_settings=self.settings.persona_settings.get_all(),
             template_store=self.template_store,
-            dont_split_responses=self.settings.dont_split_responses,
         )
 
         # tracks of the time spent on responding, success rate, etc.
         self.response_stats = response_stats.AggregateResponseStats(
             fn_get_total_tokens=lambda: self.ooba_client.total_response_tokens
         )
 
         # generates images, if stable diffusion is configured
         # also includes a UI to regenerate images on demand
         self.image_generator = None
         if self.stable_diffusion_client is not None:
             self.image_generator = image_generator.ImageGenerator(
                 stable_diffusion_client=self.stable_diffusion_client,
-                image_words=self.settings.image_words,
+                image_words=[
+                    str(w)
+                    for w in self.settings.stable_diffusion_settings.get_list(
+                        "image_words"
+                    )
+                ],
                 template_store=self.template_store,
             )
 
         # if a bot sees itself repeating a message over and over,
         # it will keep doing so forever.  This attempts to fix that.
         # by looking for repeated responses, and deciding how far
         # back in history the bot can see.
         self.repetition_tracker = repetition_tracker.RepetitionTracker(
             repetition_threshold=self.settings.REPETITION_TRACKER_THRESHOLD
         )
 
         self.bot_commands = bot_commands.BotCommands(
-            ai_name=self.settings.ai_name,
             decide_to_respond=self.decide_to_respond,
             repetition_tracker=self.repetition_tracker,
-            reply_in_thread=self.settings.reply_in_thread,
+            persona_settings=self.settings.persona_settings.get_all(),
+            discord_settings=self.settings.discord_settings.get_all(),
             template_store=self.template_store,
         )
 
+        def sigint_handler(_signum, _frame):
+            fancy_logger.get().info("Received SIGINT, exiting...")
+            self.response_stats.write_stat_summary_to_log()
+            sys.exit(1)
+
+        signal.signal(signal.SIGINT, sigint_handler)
+
     def run(self):
+        if self.settings.general_settings.get("generate_config"):
+            self.settings.write_sample_config(out_stream=sys.stdout)
+            sys.exit(0)
+
+        if not self.settings.discord_settings.get("discord_token"):
+            msg = (
+                f"Please set the '{self.settings.DISCORD_TOKEN_ENV_VAR}' "
+                + "environment variable to your bot's discord token."
+            )
+            print(msg, file=sys.stderr)
+            sys.exit(1)
+
         ########################################################
         # Test connection to services
         for client in [self.ooba_client, self.stable_diffusion_client]:
             if client is None:
                 continue
 
-            fancy_logger.get().info(f"{client.service_name} is at {client.base_url}")
+            fancy_logger.get().info("%s is at %s", client.service_name, client.base_url)
             try:
                 client.test_connection()
-                fancy_logger.get().info(f"Connected to {client.service_name}!")
-            except http_client.OobaHttpClientError as e:
+                fancy_logger.get().info("Connected to %s!", client.service_name)
+            except http_client.OobaHttpClientError as err:
                 fancy_logger.get().error(
-                    f"Could not connect to {client.service_name} "
-                    + f"server: [{client.base_url}]"
+                    "Could not connect to %s server: [%s]",
+                    client.service_name,
+                    client.base_url,
                 )
                 fancy_logger.get().error("Please check the URL and try again.")
-                if e.__cause__ is not None:
-                    fancy_logger.get().error(f"Reason: {e.__cause__}")
+                if err.__cause__ is not None:
+                    fancy_logger.get().error("Reason: %s", err.__cause__)
                 sys.exit(1)
 
         ########################################################
         # Connect to Discord
 
         fancy_logger.get().info("Connecting to Discord... ")
         bot = discord_bot.DiscordBot(
             self.ooba_client,
             decide_to_respond=self.decide_to_respond,
             prompt_generator=self.prompt_generator,
             repetition_tracker=self.repetition_tracker,
             response_stats=self.response_stats,
             image_generator=self.image_generator,
             bot_commands=self.bot_commands,
-            ai_name=self.settings.ai_name,
-            persona=self.settings.persona,
-            ignore_dms=self.settings.ignore_dms,
-            dont_split_responses=self.settings.dont_split_responses,
-            reply_in_thread=self.settings.reply_in_thread,
-            log_all_the_things=self.settings.log_all_the_things,
+            persona_settings=self.settings.persona_settings.get_all(),
+            discord_settings=self.settings.discord_settings.get_all(),
         )
 
         # opens http connections to our services,
         # then connects to Discord
         async def init_then_start():
-            try:
-                if self.stable_diffusion_client is not None:
-                    async with self.stable_diffusion_client:
-                        async with self.ooba_client:
-                            try:
-                                await bot.start(self.settings.discord_token)
-                            finally:
-                                await bot.close()
-                else:
-                    async with self.ooba_client:
-                        try:
-                            await bot.start(self.settings.discord_token)
-                        finally:
-                            await bot.close()
-            except Exception as e:
-                fancy_logger.get().error(f"Error starting bot: {e}")
+            async with contextlib.AsyncExitStack() as stack:
+                for context_manager in [
+                    self.ooba_client,
+                    self.stable_diffusion_client,
+                ]:
+                    if context_manager is not None:
+                        await stack.enter_async_context(context_manager)
+
+                try:
+                    await bot.start(
+                        self.settings.discord_settings.get_str("discord_token")
+                    )
+                finally:
+                    await bot.close()
 
         asyncio.run(init_then_start())
 
 
 def main():
-    oobabot = OobaBot()
+    oobabot = OobaBot(sys.argv[1:])
     oobabot.run()
```

### Comparing `oobabot-0.1.6/src/oobabot/prompt_generator.py` & `oobabot-0.1.7/src/oobabot/prompt_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 # purpose: generate a prompt for the AI to respond to, given
 # the message history and persona.
 import typing
 
 from oobabot import fancy_logger
 from oobabot import templates
 from oobabot import types
@@ -34,27 +35,26 @@
     # when we're not splitting responses, each history line is
     # much larger, and it's easier to run out of token space,
     # so we use a different estimate
     EST_CHARACTERS_PER_HISTORY_LINE_NOT_SPLITTING_RESPONSES = 180
 
     def __init__(
         self,
-        ai_name: str,
-        persona: str,
-        history_lines: int,
-        token_space: int,
+        discord_settings: dict,
+        oobabooga_settings: dict,
+        persona_settings: dict,
         template_store: templates.TemplateStore,
-        dont_split_responses: bool,
     ):
-        self.ai_name = ai_name
-        self.persona = persona
-        self.history_lines = history_lines
-        self.token_space = token_space
+        self.ai_name = persona_settings["ai_name"]
+        self.dont_split_responses = discord_settings["dont_split_responses"]
+        self.history_lines = discord_settings["history_lines"]
+        self.persona = persona_settings["persona"]
+        self.token_space = oobabooga_settings["request_params"]["truncation_length"]
+
         self.template_store = template_store
-        self.dont_split_responses = dont_split_responses
 
         # this will be also used when sending message
         # to suppress sending the prompt text to the user
         self.bot_prompt_line = self.template_store.format(
             templates.Templates.PROMPT_HISTORY_LINE,
             {
                 templates.TemplateToken.USER_NAME: self.ai_name,
@@ -64,14 +64,15 @@
 
         self.image_request_made = self.template_store.format(
             templates.Templates.PROMPT_IMAGE_COMING,
             {
                 templates.TemplateToken.AI_NAME: self.ai_name,
             },
         )
+
         self._init_history_available_chars()
 
     def _init_history_available_chars(self) -> None:
         """
         Calculate the number of characters we have available
         for history, and raise an exception if we don't have
         enough.
@@ -143,18 +144,18 @@
             adjusted_author_name = message.author_name
             if message.author_id == ai_user_id:
                 # make sure the AI always sees its persona name
                 # in the transcript, even if the chat program
                 # has it under a different account name
                 adjusted_author_name = self.ai_name
 
-                # hack: if the message includes the text
-                # "tried to make an image with the prompt",
-                # ignore it
-                if "tried to make an image with the prompt" in message.body_text:
+                # we'll ignore any messages we generate which refer
+                # another message, since those are ones our image
+                # generation code generated
+                if message.reference_message_id:
                     continue
 
             if not message.body_text:
                 continue
 
             line = self.template_store.format(
                 templates.Templates.PROMPT_HISTORY_LINE,
@@ -162,18 +163,17 @@
                     templates.TemplateToken.USER_NAME: adjusted_author_name,
                     templates.TemplateToken.USER_MESSAGE: message.body_text,
                 },
             )
 
             if len(line) > prompt_len_remaining:
                 num_discarded_lines = self.history_lines - len(history_lines)
-                fancy_logger.get().warn(
-                    "ran out of prompt space, discarding "
-                    + f"{num_discarded_lines} lines "
-                    + "of chat history"
+                fancy_logger.get().warning(
+                    "ran out of prompt space, discarding {%d} lines of chat history",
+                    num_discarded_lines,
                 )
                 break
 
             prompt_len_remaining -= len(line)
             history_lines.append(line)
 
         history_lines.reverse()
```

### Comparing `oobabot-0.1.6/src/oobabot/repetition_tracker.py` & `oobabot-0.1.7/src/oobabot/repetition_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import typing
 
 from oobabot import fancy_logger
 from oobabot import types
 
 
 class RepetitionTracker:
@@ -41,21 +42,22 @@
         if last_message == sentence:
             repetition_count += 1
         else:
             repetition_count = 0
 
         if repetition_count > 0:
             fancy_logger.get().debug(
-                f"Repetition count for channel {channel_id} is {repetition_count}"
+                "Repetition count for channel %d is %d", channel_id, repetition_count
             )
 
         if self.should_throttle(repetition_count):
             fancy_logger.get().warning(
-                "Repetition found, will throttle history for channel "
-                + f"{channel_id} in next request"
+                "Repetition found, will throttle history for channel #%d "
+                + "in next request",
+                channel_id,
             )
             throttle_message_id = response_message.message_id
 
         self.repetition_count[channel_id] = (
             sentence,
             throttle_message_id,
             repetition_count,
@@ -65,16 +67,15 @@
         """
         Hides all messages before the given message ID in the given channel
         """
         sentence, _, repetition_count = self.repetition_count.get(
             channel_id, ("", 0, 0)
         )
         fancy_logger.get().info(
-            "Hiding messages before message ID "
-            + f"{message_id} in channel {channel_id}"
+            "Hiding messages before message ID %d in channel %d", message_id, channel_id
         )
         self.repetition_count[channel_id] = (sentence, message_id, repetition_count)
 
     def should_throttle(self, repetition_count: int) -> bool:
         """
         Returns whether the bot should throttle history for a given repetition count
         """
```

### Comparing `oobabot-0.1.6/src/oobabot/response_stats.py` & `oobabot-0.1.7/src/oobabot/response_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import time
 import typing
 
 from oobabot import fancy_logger
 
 
 class ResponseStats:
@@ -159,35 +160,31 @@
             f"Recevied {self.total_requests_received} request(s), "
             + f"sent {self.total_successful_responses} successful responses "
             + f"and failed to send one {self.total_failed_responses} times(s)"
         )
 
         if self.total_failed_responses > 0:
             fancy_logger.get().error(
-                "Error rate:                  " + f"{self.error_rate()}%"
+                "Error rate:                  %0.2f%%", self.error_rate()
             )
 
         if self.total_successful_responses > 0:
             fancy_logger.get().debug(
-                "Average response time:       "
-                + f"{self.average_response_time():6.2f}s"
+                "Average response time:       %6.2fs", self.average_response_time()
             )
             fancy_logger.get().debug(
-                "Average response latency:    "
-                + f"{self.average_response_latency():6.2f}s"
+                "Average response latency:    %6.2fs", self.average_response_latency()
             )
             fancy_logger.get().debug(
-                "Average tokens per response: "
-                + f"{self.average_tokens_per_second():6.2f}"
+                "Average tokens per response: %6.2f", self.average_tokens_per_second()
             )
 
         if self.total_response_time_seconds > 0:
             fancy_logger.get().debug(
-                "Average tokens per second:   "
-                + f"{self.average_tokens_per_second():6.2f}"
+                "Average tokens per second:   %6.2f", self.average_tokens_per_second()
             )
 
         fancy_logger.get().debug(
             "Prompt length: "
             + f"max: {self.prompt_max_chars}, "
             + f"min: {self.prompt_min_chars}, "
             + f"avg: {self.average_prompt_length():.2f}"
```

### Comparing `oobabot-0.1.6/src/oobabot/sd_client.py` & `oobabot-0.1.7/src/oobabot/sd_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 # Purpose: Client for generating images using the AUTOMATIC1111
 # API.  Takes a prompt and returns image binary data in PNG format.
 #
 
 import asyncio
 import base64
 import time
@@ -18,15 +19,14 @@
 class StableDiffusionClient(http_client.SerializedHttpClient):
     """
     Purpose: Client for generating images using the AUTOMATIC1111
     API.  Takes a prompt and returns image binary data in PNG format.
     """
 
     SERVICE_NAME = "Stable Diffusion"
-    LOG_PREFIX = SERVICE_NAME + ": "
     STABLE_DIFFUSION_API_URI_PATH: str = "/sdapi/v1/"
 
     API_COMMAND_URLS = {
         "get_samplers": STABLE_DIFFUSION_API_URI_PATH + "samplers",
         # get_samplers: GET only
         #   returns a list of samplers which we can use
         #   in text2img
@@ -41,53 +41,26 @@
         "txt2img": STABLE_DIFFUSION_API_URI_PATH + "txt2img",
         # txt2img: POST only
         #   takes a prompt, generates an image and returns it
     }
 
     def __init__(
         self,
-        base_url: str,
-        negative_prompt: str,
-        negative_prompt_nsfw: str,
-        image_width: int,
-        image_height: int,
-        steps: int,
-        desired_sampler: typing.Optional[str] = None,
+        settings: typing.Dict[str, typing.Any],
     ):
-        super().__init__(self.SERVICE_NAME, base_url)
+        super().__init__(self.SERVICE_NAME, settings["stable_diffusion_url"])
 
-        self.negative_prompt = negative_prompt
-        self.negative_prompt_nsfw = negative_prompt_nsfw
+        self.extra_prompt_text = settings["extra_prompt_text"]
+        self.request_params = settings["request_params"]
 
-        self._sampler = None
-        self.desired_sampler = desired_sampler
-
-        self.image_width = image_width
-        self.image_height = image_height
-
-        self._steps = steps
-
-    # set default negative prompts to make it more difficult
-    # to create content against the discord TOS
-    # https://discord.com/guidelines
-
-    DEFAULT_REQUEST_PARAMS: typing.Dict[str, typing.Union[bool, int, str]] = {
-        # default values are commented out
-        #
-        # "do_not_save_samples": False,
-        #    This is a privacy concern for the users of the service.
-        #    We don't want to save the generated images anyway, since they
-        #    are going to be on Discord.  Also, we don't want to use the
-        #    disk space.
-        "do_not_save_samples": True,
-        #
-        # "do_not_save_grid": False,
-        #    Sames as above.
-        "do_not_save_grid": True,
-    }
+        # when we're in a "age restricted" channel, we'll swap
+        # the "negative_prompt" in the request_params with this
+        # value.  Otherwise we'll use the one already in
+        # request_params["negative_prompt"]
+        self.negative_prompt_nsfw = self.request_params.pop("negative_prompt_nsfw", "")
 
     DEFAULT_OPTIONS = {
         #
         # - "enable_pnginfo"
         #   by default, this will store the parameters used to generate the image.
         #   For instance:
         #         Parameters: zombie taylor swift pinup movie posterSteps: 30,
@@ -136,22 +109,23 @@
         for k, v in self.DEFAULT_OPTIONS.items():
             if k not in current_options:
                 continue
             if v == current_options[k]:
                 continue
             options_to_set[k] = v
             fancy_logger.get().info(
-                self.LOG_PREFIX
-                + f" changing option '{k}' from to "
-                + f"'{current_options[k]}' to '{v}'"
+                "Stable Diffusion:  changing option '%s' from to '%s' to '%s'",
+                k,
+                current_options[k],
+                v,
             )
 
         if not options_to_set:
             fancy_logger.get().debug(
-                self.LOG_PREFIX + "Options are already set correctly, no changes made."
+                "Stable Diffusion: Options are already set correctly, no changes made."
             )
             return
 
         async with self.get_session().post(url, json=options_to_set) as response:
             if response.status != 200:
                 raise http_client.OobaHttpClientError(response)
             await response.json()
@@ -169,109 +143,105 @@
         self,
         prompt: str,
         is_channel_nsfw: bool = False,
     ) -> "asyncio.Task[bytes]":
         # Purpose: Generate an image from a prompt.
         # Args:
         #     prompt: The prompt to generate an image from.
-        #     negative_prompt: The negative prompt to use.
-        #     sampler_name: The sampler to use.
-        #     steps: The number of steps to use.
-        #     width: The width of the image.
-        #     height: The height of the image.
+        #     is_channel_nsfw: Whether the channel is NSFW.
+        #     this will change the negative prompt.
         # Returns:
         #     The image as bytes.
         # Raises:
         #     OobaHttpClientError, if the request fails.
-        request = self.DEFAULT_REQUEST_PARAMS.copy()
-        negative_prompt = self.negative_prompt
+        request = self.request_params.copy()
+        request["prompt"] = prompt
         if is_channel_nsfw:
-            negative_prompt = self.negative_prompt_nsfw
-        request.update(
-            {
-                "prompt": prompt,
-                "negative_prompt": negative_prompt,
-                "steps": self._steps,
-                "width": self.image_width,
-                "height": self.image_height,
-            }
-        )
-        if self._sampler is not None:
-            request["sampler_name"] = self._sampler
+            request["negative_prompt"] = self.negative_prompt_nsfw
+
+        if self.extra_prompt_text:
+            request["prompt"] += ", " + self.extra_prompt_text
 
         async def do_post() -> bytes:
             fancy_logger.get().debug(
-                self.LOG_PREFIX
-                + f"Image request (nsfw: {is_channel_nsfw}): {request['prompt']}"
+                "Stable Diffusion: Image request (nsfw: %r): %s",
+                is_channel_nsfw,
+                request["prompt"],
             )
             start_time = time.time()
 
             async with self.get_session().post(
                 self.API_COMMAND_URLS["txt2img"],
                 json=request,
             ) as response:
                 if response.status != 200:
                     raise http_client.OobaHttpClientError(response)
                 duration = time.time() - start_time
                 json_body = await response.json()
-                bytes = base64.b64decode(json_body["images"][0])
+                image_bytes = base64.b64decode(json_body["images"][0])
                 fancy_logger.get().debug(
-                    self.LOG_PREFIX
-                    + "Image generated, {} bytes in {:.2f} seconds".format(
-                        len(bytes), duration
-                    )
+                    "Stable Diffusion: Image generated, %d bytes in %.2f seconds",
+                    len(image_bytes),
+                    duration,
                 )
-                return bytes
+                return image_bytes
 
         # works around aiohttp being bad
         async def do_post_with_retry() -> bytes:
             tries = 0
             while True:
                 try:
                     return await do_post()
-                except aiohttp.ClientOSError as e:
-                    if e.__cause__ is not ConnectionResetError:
-                        raise e
-                    if tries > 2:
-                        raise e
+                except aiohttp.ClientError as err:
+                    if tries > 2 or err.__cause__ is not ConnectionResetError:
+                        raise http_client.OobaHttpClientError(err) from err
                     fancy_logger.get().warning(
-                        self.LOG_PREFIX
-                        + f"Connection reset error: {e}, retrying in 1 second"
+                        "Stable Diffusion: Connection reset error: %s, "
+                        + "retrying in 1 second",
+                        err,
                     )
                     await asyncio.sleep(1)
                     tries += 1
 
         return asyncio.create_task(do_post_with_retry())
 
-    async def set_sampler(self):
-        """Sets the sampler to use, if it is available."""
+    async def verify_sampler_available(self):
+        """
+        Checks that the requested sampler is available on the server.
+        If it isn't, logs a warning and sets the sampler to the default.
+        """
         samplers = await self.get_samplers()
-        if self.desired_sampler is not None:
-            if self.desired_sampler in samplers:
-                fancy_logger.get().debug(
-                    self.LOG_PREFIX + "Using desired sampler '%s'", self.desired_sampler
-                )
-                self._sampler = self.desired_sampler
-            else:
-                fancy_logger.get().warn(
-                    self.LOG_PREFIX + "Desired sampler '%s' not available",
-                    self.desired_sampler,
-                )
-                self._sampler = None
-        if self._sampler is None:
+
+        desired_sampler = self.request_params.get("sampler")
+        if not desired_sampler:
             fancy_logger.get().debug(
-                self.LOG_PREFIX + "Using default sampler on SD server"
+                "Stable Diffusion: Using default sampler on SD server"
             )
+            return
+
+        if desired_sampler in samplers:
             fancy_logger.get().debug(
-                self.LOG_PREFIX + "Available samplers: %s", ", ".join(samplers)
+                "Stable Diffusion: Using desired sampler '%s'", desired_sampler
             )
-            self._sampler = None
+            return
+
+        fancy_logger.get().warning(
+            "Stable Diffusion: Desired sampler '%s' not available",
+            desired_sampler,
+        )
+        fancy_logger.get().info(
+            "Stable Diffusion: Available samplers: %s", ", ".join(samplers)
+        )
+        self.request_params["sampler"] = ""
 
     async def _setup(self):
-        await self.set_sampler()
+        await self.verify_sampler_available()
         await self.set_options()
         fancy_logger.get().debug(
-            self.LOG_PREFIX
-            + "Using negative prompt: "
-            + self.negative_prompt[:20]
-            + "..."
+            "Stable Diffusion: Using negative prompt: %s...",
+            str(self.request_params.get("negative_prompt", ""))[:20],
         )
+        if self.extra_prompt_text:
+            fancy_logger.get().debug(
+                "Stable Diffusion: will append to every prompt: '%s'",
+                self.extra_prompt_text,
+            )
```

### Comparing `oobabot-0.1.6/src/oobabot/types.py` & `oobabot-0.1.7/src/oobabot/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,40 @@
+# -*- coding: utf-8 -*-
 import typing
 
 
-class GenericMessage(object):
+class GenericMessage:
     def __init__(
         self,
         author_id: int,
         author_name: str,
         channel_id: int,
         channel_name: str,
         message_id: int,
+        reference_message_id,
         body_text: str,
         author_is_bot: bool,
         send_timestamp: float,
     ):
         self.author_id = author_id
         self.author_name = author_name
         self.message_id = message_id
         self.body_text = body_text
         self.author_is_bot = author_is_bot
+        self.reference_message_id = reference_message_id
         self.send_timestamp = send_timestamp
         self.channel_id = channel_id
         self.channel_name = channel_name
 
     def is_empty(self) -> bool:
         return not self.body_text.strip()
 
 
 class DirectMessage(GenericMessage):
-    def __init__(self, /, **kwargs):
-        super().__init__(**kwargs)
+    pass
 
 
 class ChannelMessage(GenericMessage):
     def __init__(
         self,
         /,
         mentions: typing.List[int],
```

### Comparing `oobabot-0.1.6/PKG-INFO` & `oobabot-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: discord.py (>=2.2.2,<3.0.0)
 Requires-Dist: pysbd (>=0.3.4,<0.4.0)
+Requires-Dist: ruamel-yaml (>=0.17.26,<0.18.0)
 Project-URL: Repository, https://github.com/chrisrude/oobabot
 Description-Content-Type: text/markdown
 
 # `oobabot`
 
 **`oobabot`** is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
 
@@ -89,94 +90,96 @@
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
 You should now be able to run oobabot from wherever pip installed it.
 
 ```none
-usage: oobabot [-h] [--discord-token] [--dont-split-responses]
-               [--history-lines HISTORY_LINES] [--ignore-dms] [--wakewords [WAKEWORDS ...]]
-               [--ai-name AI_NAME] [--base-url BASE_URL] [--log-all-the-things]
-               [--persona PERSONA] [--reply-in-thread] [--diffusion-steps DIFFUSION_STEPS]
-               [--image-height IMAGE_HEIGHT] [--image-width IMAGE_WIDTH]
-               [--image-words [IMAGE_WORDS ...]]
-               [--stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER]
+usage: oobabot [-h] [-c CONFIG] [--generate-config] [--ai-name AI_NAME] [--persona PERSONA]
+               [--wakewords [WAKEWORDS ...]] [--discord-token DISCORD_TOKEN]
+               [--dont-split-responses] [--history-lines HISTORY_LINES] [--ignore-dms]
+               [--reply-in-thread] [--stream-responses] [--base-url BASE_URL]
+               [--log-all-the-things] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
-               [--sd-negative-prompt SD_NEGATIVE_PROMPT]
-               [--sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW]
+               [--extra-prompt-text EXTRA_PROMPT_TEXT]
 
-Discord bot for oobabooga's text-generation-webui
+oobabot v0.1.7: Discord bot for oobabooga's text-generation-webui
 
-options:
-  -h, --help            show this help message and exit
+General Settings:
 
-Discord Settings:
-  --discord-token       Token to log into Discord with. For security purposes it's strongly
-                        recommended that you set this via the DISCORD_TOKEN environment
-                        variable instead, if possible.
-  --dont-split-responses
-                        If set, the bot post its entire response as a single message,
-                        rather than splitting it into seperate messages by sentence.
-  --history-lines HISTORY_LINES
-                        Number of lines of chat history the AI will see when generating a
-                        response. The default is 15.
-  --ignore-dms          If set, the bot will ignore direct messages.
+  -h, --help
+  -c CONFIG, --config CONFIG
+                        Path to a config file to read settings from. Command line settings
+                        will override settings in this file. (default: config.yml)
+  --generate-config     If set, oobabot will print its configuration as a .yml file, then
+                        exit. Any command-line settings also passed will be reflected in
+                        this file. (default: False)
+
+Persona:
+
+  --ai-name AI_NAME     Name the AI will use to refer to itself (default: oobabot)
+  --persona PERSONA     This prefix will be added in front of every user-supplied request.
+                        This is useful for setting up a 'character' for the bot to play.
+                        Alternatively, this can be set with the OOBABOT_PERSONA environment
+                        variable. (default: )
   --wakewords [WAKEWORDS ...]
                         One or more words that the bot will listen for. The bot will listen
                         in all discord channels can access for one of these words to be
                         mentioned, then reply to any messages it sees with a matching word.
                         The bot will always reply to @-mentions and direct messages, even
-                        if no wakewords are supplied.
+                        if no wakewords are supplied. (default: ['oobabot'])
+
+Discord:
+
+  --discord-token DISCORD_TOKEN
+                        Token to log into Discord with. For security purposes it's strongly
+                        recommended that you set this via the DISCORD_TOKEN environment
+                        variable instead, if possible. (default: )
+  --dont-split-responses
+                        Post the entire response as a single message, rather than splitting
+                        it into seperate messages by sentence. (default: False)
+  --history-lines HISTORY_LINES
+                        Number of lines of chat history the AI will see when generating a
+                        response. (default: 7)
+  --ignore-dms          If set, the bot will not respond to direct messages. (default:
+                        False)
+  --reply-in-thread     If set, the bot will generate a thread to respond in if it is not
+                        already in one. (default: False)
+  --stream-responses    Stream responses into a single message as they are generated.
+                        (default: False)
+
+Oobabooga:
 
-Oobabooga Seetings:
-  --ai-name AI_NAME     Name of the AI to use for requests. This can be whatever you want,
-                        but might make sense to be the name of the bot in Discord.
   --base-url BASE_URL   Base URL for the oobabooga instance. This should be
                         ws://hostname[:port] for plain websocket connections, or
-                        wss://hostname[:port] for websocket connections over TLS.
-  --log-all-the-things  Prints all oobabooga requests and responses in their entirety to
-                        STDOUT
-  --persona PERSONA     This prefix will be added in front of every user-supplied request.
-                        This is useful for setting up a 'character' for the bot to play.
-                        Alternatively, this can be set with the OOBABOT_PERSONA environment
-                        variable.
-  --reply-in-thread     When set, the bot will generate a new thread for each response it
-                        generates. But it will only do so if the user who prompted the bot
-                        has thread-create permissions.
-
-Stable Diffusion Settings:
-  --diffusion-steps DIFFUSION_STEPS
-                        Number of diffusion steps to take when generating an image. The
-                        default is 30.
-  --image-height IMAGE_HEIGHT
-                        Size of images to generate. This is the height of the image in
-                        pixels. The default is 512.
-  --image-width IMAGE_WIDTH
-                        Size of images to generate. This is the width of the image in
-                        pixels. The default is 512.
+                        wss://hostname[:port] for websocket connections over TLS. (default:
+                        ws://localhost:5005)
+  --log-all-the-things  Print all AI input and output to STDOUT. (default: False)
+
+Stable Diffusion:
+
   --image-words [IMAGE_WORDS ...]
-                        One or more words that will indicate the user is requeting an image
-                        to be generated.
-  --stable-diffusion-sampler STABLE_DIFFUSION_SAMPLER, --sd-sampler STABLE_DIFFUSION_SAMPLER
-                        Sampler to use when generating images. If not specified, the one
-                        set on the AUTOMATIC1111 server will be used.
-  --stable-diffusion-url STABLE_DIFFUSION_URL, --sd-url STABLE_DIFFUSION_URL
-                        URL for an AUTOMATIC1111 Stable Diffusion server
-  --sd-negative-prompt SD_NEGATIVE_PROMPT
-                        Negative prompt to use when generating images. This will discourage
-                        Stable Diffusion from generating images with the specified content.
-                        By default, this is set to follow Discord's TOS.
-  --sd-negative-prompt-nsfw SD_NEGATIVE_PROMPT_NSFW
-                        Negative prompt to use when generating images in a channel marked
-                        as'Age-Restricted'.
+                        When one of these words is used in a message, the bot will generate
+                        an image. (default: ['drawing', 'photo', 'pic', 'picture', 'image',
+                        'sketch'])
+  --stable-diffusion-url STABLE_DIFFUSION_URL
+                        URL for an AUTOMATIC1111 Stable Diffusion server. (default: )
+  --extra-prompt-text EXTRA_PROMPT_TEXT
+                        This will be appended to every image generation prompt sent to
+                        Stable Diffusion. (default: )
+
+
+Additional settings can be set in config.yml.  Use the --generate-config option to print a
+new copy of this file to STDOUT.
 
-Also, to authenticate to Discord, you must set the environment variable: DISCORD_TOKEN =
-<your bot's discord token>
+Please set the 'DISCORD_TOKEN' environment variable to your bot's discord token.
 ```
 
+There are **a lot more settings** in the [config.yml file (sample)](./docs/config.sample.yml) here.
+
 ## Required settings
 
 - **`DISCORD_TOKEN`** environment variable
 
    Set your shell environment's **`DISCORD_TOKEN`** to token Discord provided when you set up the bot account.  It should be something like a 72-character-long random-looking string.
 
     **bash example**
@@ -310,17 +313,27 @@
 | **`/lobotomize`** | make the bot forget everything in the channel before the command is run |
 | **`/say "message"`** | speak as the bot |
 
 Oobabot doesn't add any restrictions on who can run these commands, but luckily Discord does!  You can find this inside Discord by visiting "Server Settings" -> Integrations -> Bots and Apps -> hit the icon which looks like [/] next to your bot
 
 If you're running on a large server, you may want to restrict who can run these commands.  I suggest creating a new role, and only allowing that role to run the commands.
 
+## Using a config file
+
+Instead of the command line, you can also use a config file.  This is useful if you want to run multiple instances of the bot, or if you want to run it as a service.
+
+There are also many more settings available in the config file, which are not available on the command line.  See [docs/CONFIG.md](./docs/CONFIG.md) for information on how to use it.
+
+You can also look at a [config.yml file (sample)](./docs/config.sample.yml) here.
+
 ## Known Issues
 
 - detection of requests for photos is very crude, and will likely be improved in the future.
-- some of the default settings are very specific to my use case, and will likely be made
-  configurable in the future
 - public threads in 'age restricted' channels are treated as if they
   were not age-restricted
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
 - found one not listed here?  Have an idea?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
 
+## Contributing
+
+Contributions are welcome!  Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
+
```

