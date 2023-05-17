# Comparing `tmp/pydisadm-1.0.6.tar.gz` & `tmp/pydisadm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.0.6.tar", max compression
+gzip compressed data, was "pydisadm-1.0.7.tar", max compression
```

## Comparing `pydisadm-1.0.6.tar` & `pydisadm-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2363 2023-05-17 03:38:22.468533 pydisadm-1.0.6/README.md
--rw-r--r--   0        0        0      111 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/__main__.py
--rw-r--r--   0        0        0     1120 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     5874 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0      539 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      850 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/configuration.py
--rw-r--r--   0        0        0     6012 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-17 03:38:22.472533 pydisadm-1.0.6/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      441 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0      940 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0      947 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     2976 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/services/database.py
--rw-r--r--   0        0        0     1164 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/services/esi.py
--rw-r--r--   0        0        0      372 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      521 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      120 2023-05-17 03:38:22.492533 pydisadm-1.0.6/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      934 2023-05-17 03:38:58.333031 pydisadm-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 pydisadm-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2711 2023-05-17 10:39:05.050201 pydisadm-1.0.7/README.md
+-rw-r--r--   0        0        0      111 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1060 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1541 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     6551 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0      702 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0      816 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/configuration.py
+-rw-r--r--   0        0        0     6872 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1108 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3442 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      472 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-17 10:39:35.706800 pydisadm-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 pydisadm-1.0.7/PKG-INFO
```

### Comparing `pydisadm-1.0.6/README.md` & `pydisadm-1.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -59,14 +59,30 @@
 
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
 ## 🚧 Development
 
+### Environment
+The development environment and dependencies is managed using `poetry`. Use the following command to set up environment and install dependencies:
+```shell
+poetry install
+```
+
+A nested poetry shell can be started using this command:
+```shell
+poetry shell
+```
+
+### Run Linting
+```shell
+pylint --rcfile pylint.rc pydisadm/**/*.py
+```
+
 ### Run Unit Tests
 ```shell
 pytest tests/ --cov=pydisadm --cov-branch
 ```
 
 ## 💡 Credits
 Project is forked from and inspired by [@anjode](https://www.github.com/anjode)
```

### Comparing `pydisadm-1.0.6/pydisadm/__main__.py` & `pydisadm-1.0.7/pydisadm/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 
 import signal
 import sys
 import threading
-import logging
 
 from dotenv import load_dotenv
 
 from pydisadm.bot.adm_bot import AdmBot
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 from pydisadm.loader.static_data import update_static_data
 from pydisadm.runnable.runnable_refresh import run_auto_refresh
 from pydisadm.services.database import Database
 
 interrupt_event = threading.Event()
 
-def signal_handler(sig, frame):
+def signal_handler(_1, _2):
     print('Interrupted by CTRL+C')
     interrupt_event.set()
     sys.exit(0)
 
 
 def main() -> int:
     load_dotenv(verbose=True)
@@ -29,26 +28,22 @@
 
     run_auto_refresh(interrupt_event)
 
     configuration = Configuration()
 
     database = Database()
 
-    try:
-        update_static_data(database)
-    except Exception as err:
-        logging.error(err)
-        return 1
+    update_static_data(database)
 
     controller = AdmController(configuration, database)
     controller.update_adm_data()
 
     bot = AdmBot(configuration, controller)
     bot.setup_cogs()
     bot.run()
 
     interrupt_event.set()
 
     return 0
 
 if __name__ == '__main__':
-    sys.exit(main()) 
+    sys.exit(main())
```

### Comparing `pydisadm-1.0.6/pydisadm/bot/adm_bot.py` & `pydisadm-1.0.7/pydisadm/bot/adm_bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,50 @@
+"""Discord bot collecting and posting ADM summaries."""
+
 import asyncio
 import discord
 from discord.ext import commands
 
 from pydisadm.bot.adm_cog import Adm
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 
 def create_intents():
+    """Create discord intents for bot."""
     intents = discord.Intents.default()
     intents.message_content = True
     return intents
 
 class AdmBot:
+    """Discord bot collecting and posting ADM summaries."""
+
     def __init__(self, configuration: Configuration, controller: AdmController):
         self.configuration = configuration
         self.controller = controller
 
         intents = create_intents()
-        self.bot = commands.Bot(application_id=configuration.discord_app_id, command_prefix=None, intents=intents, help_command=None)
-    
+        self.bot = commands.Bot(
+            application_id=configuration.discord_app_id,
+            command_prefix=None,
+            intents=intents,
+            help_command=None
+        )
+
     async def setup_cogs_async(self):
+        """Asynchronously setup cogs"""
         await self.bot.add_cog(Adm(self.bot, self.configuration, self.controller))
 
     def setup_cogs(self):
+        """Setup cogs"""
         return asyncio.run(self.setup_cogs_async())
-    
+
     async def sync_commands_async(self):
+        """Asynchronously synchronize command tree"""
         await self.bot.tree.sync()
 
     def sync_commands(self):
+        """Synchronize command tree"""
         return asyncio.run(self.sync_commands_async())
 
     def run(self):
+        """Run the bot, this function is blocking"""
         self.bot.run(self.configuration.discord_token)
```

### Comparing `pydisadm-1.0.6/pydisadm/bot/adm_cog.py` & `pydisadm-1.0.7/pydisadm/bot/adm_cog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,126 +1,145 @@
+"""Cog providing ADM related commands"""
+
 import discord
 from discord.ext import commands
 from discord import app_commands
 
 from pydisadm.bot.utils import check_allowed_channel, text_channels_with_send_permission
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 from pydisadm.utils.datetime_utils import convert_to_local_timestamp
 
 class Adm(commands.GroupCog):
+    """Cog providing ADM related commands"""
     def __init__(self, bot, configuration: Configuration, controller: AdmController):
         self.bot = bot
         self.configuration = configuration
         self.controller = controller
 
     async def send_tier_list_summary(self, interaction: discord.Interaction):
+        """Send a summary of ADMs organized as a tier list"""
         await interaction.response.defer(thinking=True)
 
         (tier_list, generated_at) = self.controller.generate_tier_list()
         timestamp = convert_to_local_timestamp(generated_at)
 
         file_name = "adm_tier_list.txt"
 
-        with open(file_name, 'w', encoding='UTF-8') as f:
-            f.write(tier_list)
+        with open(file_name, 'w', encoding='UTF-8') as file:
+            file.write(tier_list)
 
         if self.controller.write_file(file_name, tier_list):
-            await interaction.followup.send(file=discord.File(file_name), content=f'ADM @ <t:{timestamp}:F>')
+            await interaction.followup.send(
+                file=discord.File(file_name),
+                content=f'ADM @ <t:{timestamp}:F>'
+            )
             self.controller.delete_file(file_name)
 
     async def send_system_graph(self, interaction: discord.Interaction, what: str):
+        """Send a graph of ADMs matching name"""
         await interaction.response.defer(thinking=True)
 
         file_name = 'adm_history.png'
         if self.controller.create_history_graph(what, file_name):
-            await interaction.followup.send(file=discord.File(file_name), content=f"ADM History")
+            await interaction.followup.send(
+                file=discord.File(file_name),
+                content=f"ADM History of {what}"
+            )
             self.controller.delete_file(file_name)
         else:
             await interaction.followup.send("No data (╯°□°）╯︵ ┻━┻")
 
     async def update_adm(self, interaction: discord.Interaction, system_name: str, adm: float):
+        """Update ADM for system"""
         await interaction.response.defer(thinking=True)
 
         if adm <= 0.0 or adm > 6.0:
             await interaction.followup.send(f"Invalid ADM: {adm} (1.0-6.0 valid)")
             return
 
         if not self.controller.update_system_adm(system_name, adm):
             await interaction.followup.send(f"Couldn't update ADM for {system_name} to {adm}")
         else:
             await interaction.followup.send(f"Manually updated {system_name} ADM to {adm}")
 
     @app_commands.command(description='Recommend where to raise ADM')
     async def recommend(self, interaction: discord.Interaction):
+        """Command recommending which system to raise ADMs"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
-        
+
         await interaction.response.defer()
-        
+
         recommended_system = self.controller.get_recommended_system()
 
         system = recommended_system['solarSystemName']
         region = recommended_system['regionName']
 
         await interaction.followup.send(f'🦀 `{system} in {region}`', tts=True)
 
     @app_commands.command(description='Posts a summary of all system ADM levels')
     async def summary(self, interaction: discord.Interaction):
+        """Command posting a summary of ADMs"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
-        
+
         await self.send_tier_list_summary(interaction)
 
     @app_commands.command(description='Posts a CSV file of all system ADM levels')
     async def csv(self, interaction: discord.Interaction):
+        """Command posting a CSV file of ADMs"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await interaction.response.defer(thinking=True)
 
         file_name = "adm_summary.csv"
         if self.controller.create_spreadsheet(file_name):
-            await interaction.followup.send(file=discord.File(file_name), content=f'ADM Spreadsheet')
+            await interaction.followup.send(file=discord.File(file_name), content='ADM Spreadsheet')
             self.controller.delete_file(file_name)
 
     @app_commands.command(description='Post a graph of system ADM.')
     @app_commands.describe(where='The system, constellation, or region to graph.')
     async def history(self, interaction: discord.Interaction, where: str):
+        """Command posting a graph of ADM history"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await self.send_system_graph(interaction, where)
 
     @app_commands.command(description='Manually refresh all ADM data.')
     async def refresh(self, interaction: discord.Interaction):
+        """Command to manually refresh ADM data"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await interaction.response.defer(thinking=True)
         self.controller.update_adm_data()
         await interaction.followup.send("ADM data manually refreshed 🦀")
 
     @app_commands.command(description='Manually update ADM of system.')
     async def update(self, interaction: discord.Interaction, system_name: str, adm: str):
+        """Command to manually update ADM for system"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await self.update_adm(interaction, system_name, float(adm))
 
     @commands.Cog.listener()
     async def on_ready(self):
+        """cog on_ready event callback"""
         channels = text_channels_with_send_permission(self.bot)
 
         await self.bot.tree.sync()
 
         valid_channels = [
             channel for channel in channels if channel.name == self.configuration.discord_channel]
 
         for channel in valid_channels:
-            await channel.send(f"=== ADM Bot is started 🦀 ===")
+            await channel.send('=== ADM Bot is started 🦀 ===')
```

### Comparing `pydisadm-1.0.6/pydisadm/configuration.py` & `pydisadm-1.0.7/pydisadm/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,17 @@
     def __init__(self):
         self.discord_token = os.getenv('DISCORD_TOKEN')
         self.discord_channel = os.getenv('DISCORD_CHANNEL')
         self.discord_app_id = os.getenv('DISCORD_APP_ID')
 
         alliance_id = os.getenv('ALLIANCE_ID')
 
-        if alliance_id != None:
+        if alliance_id is not None:
             try:
                 alliance_id = int(alliance_id)
             except ValueError as error:
                 raise ValueError('[configuration] invalid `ALLIANCE_ID` value', alliance_id) from error
 
         self.alliance_id = alliance_id
 
     def __str__(self):
-        return '{}(discord_token={}, discord_channel={}, discord_app_id={}, alliance_id={})'.format(
-            self.__class__.__name__, self.discord_token, self.discord_channel, self.discord_app_id, self.alliance_id
-        )
+        return f'{self.__class__.__name__}(discord_token={self.discord_token}, discord_channel={self.discord_channel}, discord_app_id={self.discord_app_id}, alliance_id={self.alliance_id})'
```

### Comparing `pydisadm-1.0.6/pydisadm/controller/adm_controller.py` & `pydisadm-1.0.7/pydisadm/controller/adm_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,98 @@
-
+"""Controller implementation for ADM operations"""
 import os
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
 
 from pydisadm.configuration import Configuration
 from pydisadm.services.database import Database
 from pydisadm.services.esi import sovereignty_structures
 from pydisadm.utils.plot_utils import plot_adm_history_of_systems, plot_save_to_file
 
+
 class AdmController:
+    """Controller implementation for ADM operations"""
+
     def __init__(self, configuration: Configuration, database: Database):
         self.configuration = configuration
         self.database = database
 
     def generate_tier_list(self):
+        """Generate a system tier list based on tier values"""
         system_adms = self.database.select_systems()
 
         system_adms.sort_values(by='adm', inplace=True, ascending=True)
 
         s_tier = system_adms.loc[system_adms['tier'] == 's_tier']
         a_tier = system_adms.loc[system_adms['tier'] == 'a_tier']
         b_tier = system_adms.loc[system_adms['tier'] == 'b_tier']
         c_tier = system_adms.loc[system_adms['tier'] == 'c_tier']
         d_tier = system_adms.loc[system_adms['tier'] == 'd_tier']
 
         sorted_summary = [
-            {'Tier': 'D', 'Systems': '\n'.join(d_tier['solarSystemName']), 'ADM': '\n'.join(d_tier['adm'].map(lambda v: str(
-                v))), 'Constellation': '\n'.join(d_tier['constellationName']), 'Region': '\n'.join(d_tier['regionName'])},
-            {'Tier': 'C', 'Systems': '\n'.join(c_tier['solarSystemName']), 'ADM': '\n'.join(c_tier['adm'].map(lambda v: str(
-                v))), 'Constellation': '\n'.join(c_tier['constellationName']), 'Region': '\n'.join(c_tier['regionName'])},
-            {'Tier': 'B', 'Systems': '\n'.join(b_tier['solarSystemName']), 'ADM': '\n'.join(b_tier['adm'].map(lambda v: str(
-                v))), 'Constellation': '\n'.join(b_tier['constellationName']), 'Region': '\n'.join(b_tier['regionName'])},
-            {'Tier': 'A', 'Systems': '\n'.join(a_tier['solarSystemName']), 'ADM': '\n'.join(a_tier['adm'].map(lambda v: str(
-                v))), 'Constellation': '\n'.join(a_tier['constellationName']), 'Region': '\n'.join(a_tier['regionName'])},
-            {'Tier': 'S', 'Systems': '\n'.join(s_tier['solarSystemName']), 'ADM': '\n'.join(s_tier['adm'].map(lambda v: str(
-                v))), 'Constellation': '\n'.join(s_tier['constellationName']), 'Region': '\n'.join(s_tier['regionName'])}
+            {'Tier': 'D', 'Systems': '\n'.join(d_tier['solarSystemName']),
+             'ADM': '\n'.join(d_tier['adm'].map(str)),
+             'Constellation': '\n'.join(d_tier['constellationName']),
+             'Region': '\n'.join(d_tier['regionName'])},
+            {'Tier': 'C', 'Systems': '\n'.join(c_tier['solarSystemName']),
+             'ADM': '\n'.join(c_tier['adm'].map(str)),
+             'Constellation': '\n'.join(c_tier['constellationName']),
+             'Region': '\n'.join(c_tier['regionName'])},
+            {'Tier': 'B', 'Systems': '\n'.join(b_tier['solarSystemName']),
+             'ADM': '\n'.join(b_tier['adm'].map(str)),
+             'Constellation': '\n'.join(b_tier['constellationName']),
+             'Region': '\n'.join(b_tier['regionName'])},
+            {'Tier': 'A', 'Systems': '\n'.join(a_tier['solarSystemName']),
+             'ADM': '\n'.join(a_tier['adm'].map(str)),
+             'Constellation': '\n'.join(a_tier['constellationName']),
+             'Region': '\n'.join(a_tier['regionName'])},
+            {'Tier': 'S', 'Systems': '\n'.join(s_tier['solarSystemName']),
+             'ADM': '\n'.join(s_tier['adm'].map(str)),
+             'Constellation': '\n'.join(s_tier['constellationName']),
+             'Region': '\n'.join(s_tier['regionName'])}
         ]
 
         table = tabulate(sorted_summary, showindex=False, headers='keys',
-                        tablefmt='fancy_grid', numalign='left', stralign='center')
+                         tablefmt='fancy_grid', numalign='left', stralign='center')
 
         generated_at = self.database.select_most_recent_row()
 
         return (table, generated_at['created_at'][0])
-    
+
     def create_history_graph(self, name, file_name):
+        """Generate an ADM history graph and save to file"""
         systems_by_name = self.database.select_system_by_name(name)
-        
+
         if plot_adm_history_of_systems(systems_by_name):
             plot_save_to_file('ADM History', file_name)
 
         return os.path.isfile(file_name)
-    
+
     def create_spreadsheet(self, file_name):
+        """Generate a spreadsheet of ADM data and save to file"""
         system_adms = self.database.select_systems()
         system_adms.sort_values(by='adm', inplace=True, ascending=False)
 
-        system_adms.to_csv(file_name, index=False, columns=[
-                        'system_id', 'adm', 'tier', 'created_at', 'solarSystemName', 'constellationName', 'regionName'])
+        csv_columns = [
+            'system_id',
+            'adm',
+            'tier',
+            'created_at',
+            'solarSystemName',
+            'constellationName',
+            'regionName'
+        ]
+
+        system_adms.to_csv(file_name, index=False, columns=csv_columns)
 
         return os.path.isfile(file_name)
-    
+
     def tier_list(self, systems):
+        """Assign tier column based on system ADM"""
         conditions = [
             (systems['adm'] >= 6.0),
             (systems['adm'] >= 5.0) & (systems['adm'] < 6.0),
             (systems['adm'] >= 4.0) & (systems['adm'] < 5.0),
             (systems['adm'] >= 3.5) & (systems['adm'] < 4.0),
             (systems['adm'] < 3.5)
         ]
@@ -78,80 +104,88 @@
             'c_tier',
             'd_tier'
         ]
 
         systems['tier'] = np.select(conditions, values)
 
         return systems
-    
+
     def create_system_adm(self, system, adm):
+        """Create a DataFrame for system ADM data"""
         system_adm = pd.DataFrame(columns=['system_id', 'adm'])
         system_adm['system_id'] = system['solarSystemID']
         system_adm['adm'] = [adm]
 
         self.tier_list(system_adm)
 
         return system_adm
-    
+
     def get_alliance_structures(self, structures, alliance_id):
-        df = pd.DataFrame.from_dict(structures)
+        """Retrieve a list of alliance sovreignty structures"""
+        structure_data = pd.DataFrame.from_dict(structures)
 
         drop_columns = [
             'structure_id',
             'structure_type_id',
             'vulnerable_end_time',
             'vulnerable_start_time',
         ]
 
-        df.drop(columns=drop_columns, inplace=True)
+        structure_data.drop(columns=drop_columns, inplace=True)
+
+        return structure_data[structure_data['alliance_id'] == alliance_id]
 
-        return df[df['alliance_id'] == alliance_id]
-    
     def update_system_adm(self, system_name: str, adm: float) -> bool:
+        """Update ADM for system with name"""
         system = self.database.select_system_with_name(system_name)
 
         if system.empty:
             return False
-        
+
         insert_systems = self.create_system_adm(system, adm)
 
         self.database.insert_systems(insert_systems)
 
         return True
 
     def get_system_adms(self, alliance_id):
+        """Retrieve ADM for systems controlled by alliance"""
         structures = sovereignty_structures()
         system_adms = self.get_alliance_structures(structures, alliance_id)
 
         system_adms.drop_duplicates(inplace=True)
 
         drop_columns = ['alliance_id']
         system_adms.drop(columns=drop_columns, inplace=True)
 
         rename_columns = {'solar_system_id': 'system_id',
-                        'vulnerability_occupancy_level': 'adm'}
+                          'vulnerability_occupancy_level': 'adm'}
         system_adms.rename(columns=rename_columns, inplace=True)
 
         self.tier_list(system_adms)
 
         return system_adms
-    
+
     def get_recommended_system(self):
+        """Retrieve recommended system to raise ADM"""
         systems = self.database.select_systems()
         systems.sort_values(by='adm', inplace=True, ascending=True)
-        
+
         return systems.iloc[0]
 
     def update_adm_data(self):
+        """Update ADM data"""
         alliance_id = self.configuration.alliance_id
         system_adms = self.get_system_adms(alliance_id)
 
         self.database.insert_systems(system_adms)
-    
+
     def write_file(self, file_name, content) -> bool:
-        with open(file_name, 'w', encoding='UTF-8') as f:
-            f.write(content)
-        
+        """Write content to file"""
+        with open(file_name, 'w', encoding='UTF-8') as file:
+            file.write(content)
+
         return os.path.isfile(file_name)
-    
+
     def delete_file(self, file_name):
+        """Delete file"""
         os.remove(file_name)
```

### Comparing `pydisadm-1.0.6/pydisadm/data/mapConstellations.csv` & `pydisadm-1.0.7/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.6/pydisadm/data/mapRegions.csv` & `pydisadm-1.0.7/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.6/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.0.7/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.6/pydisadm/loader/static_data.py` & `pydisadm-1.0.7/pydisadm/loader/static_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+"""Utilities for loading static data"""
 import pandas as pd
 
 from pydisadm.loader.datasets import get_constellations, get_regions, get_solar_systems
 
 def load_solar_systems() -> pd.DataFrame:
-    solar_systems = pd.read_csv(get_solar_systems(), usecols=['regionID','constellationID','solarSystemID','solarSystemName'])
+    """Load solar systems data"""
+    solar_systems = pd.read_csv(get_solar_systems(), usecols=[
+        'regionID','constellationID','solarSystemID','solarSystemName'])
     solar_systems.set_index('solarSystemID', inplace=True)
 
-    constellations = pd.read_csv(get_constellations(), usecols=['constellationID','constellationName'])
+    constellations = pd.read_csv(get_constellations(), usecols=[
+        'constellationID','constellationName'])
     constellations.set_index('constellationID', inplace=True)
 
     regions = pd.read_csv(get_regions(), usecols=['regionID','regionName'])
     regions.set_index('regionID', inplace=True)
 
     solar_systems = solar_systems.join(constellations, on='constellationID', how='left')
     solar_systems = solar_systems.join(regions, on='regionID', how='left')
 
     return solar_systems
 
 def update_static_data(database):
+    """Populate database with solar systems data"""
     solar_systems = load_solar_systems()
-    database.insert_map_data(solar_systems)
+    database.insert_map_data(solar_systems)
```

### Comparing `pydisadm-1.0.6/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.0.7/pydisadm/runnable/runnable_refresh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-import schedule
+"""Module for running scheduled refresh"""
 import logging
+import schedule
 
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 from pydisadm.services.database import Database
 from pydisadm.utils.thread_utils import run_threaded
 
 logger = logging.getLogger('adm_auto_refresh')
 
 def scheduler_loop(interrupt_event):
+    """Scheduler main loop"""
     configuration = Configuration()
     database = Database()
 
     controller = AdmController(configuration, database)
 
     schedule.every().day.at('11:30', tz='UTC').do(refresh_job, controller)
 
     while True:
         schedule.run_pending()
         if interrupt_event.wait(timeout=1000):
             break
 
 def refresh_job(controller: AdmController):
+    """Refresh adm data"""
     logger.info('updating adm data...')
     controller.update_adm_data()
     logger.info('adm data update finished')
 
 def run_auto_refresh(interrupt_event):
+    """Run automatic adm data refresh in separate thread"""
     logger.info('starting adm data update thread')
-    run_threaded(lambda: scheduler_loop(interrupt_event))
+    run_threaded(lambda: scheduler_loop(interrupt_event))
```

### Comparing `pydisadm-1.0.6/pydisadm/services/database.py` & `pydisadm-1.0.7/pydisadm/services/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,82 @@
+"""Database service"""
 import sqlite3
 import pandas as pd
 
 class Database:
+    """Database service implementation"""
+
     def __init__(self):
         self.conn = sqlite3.connect('adm-data.sqlite')
         self.setup()
 
     def setup(self):
+        """Setup database schema"""
         cur = self.conn.cursor()
         cur.execute("""
                         CREATE TABLE IF NOT EXISTS systems (
                             id INTEGER PRIMARY KEY AUTOINCREMENT, 
                             system_id INTEGER NOT NULL, 
                             adm REAL NOT NULL, 
                             tier TEXT NOT NULL,
                             created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
                         )
                     """)
-        
+
         cur.execute("""
                         CREATE TABLE IF NOT EXISTS map (
                             solarSystemID INTEGER PRIMARY KEY NOT NULL, 
                             constellationID INTEGER NOT NULL, 
                             regionID INTEGER NOT NULL, 
                             solarSystemName TEXT NOT NULL,
                             constellationName TEXT NOT NULL,
                             regionName TEXT NOT NULL
                         )
                     """)
         self.conn.commit()
 
     def insert_systems(self, systems):
+        """Insert system ADM records"""
         systems.to_sql('systems', self.conn, index=False, if_exists='append')
 
         self.conn.commit()
 
-    def insert_map_data(self, map):
-        map.to_sql('map', self.conn, index=True, if_exists='replace')
+    def insert_map_data(self, map_data):
+        """Insert map data"""
+        map_data.to_sql('map', self.conn, index=True, if_exists='replace')
 
         self.conn.commit()
 
     def select_system_with_name(self, system_name) -> pd.DataFrame:
-        return pd.read_sql_query("SELECT * FROM map WHERE solarSystemName = ?", self.conn, params=[system_name])
+        """Select system matching name"""
+        return pd.read_sql_query("SELECT * FROM map WHERE solarSystemName = ?",
+                                 self.conn, params=[system_name])
 
     def select_most_recent_row(self) -> pd.DataFrame:
-        return pd.read_sql_query("SELECT created_at FROM systems ORDER BY created_at DESC LIMIT 1", self.conn)
+        """Select the most recent ADM record"""
+        return pd.read_sql_query("SELECT created_at FROM systems ORDER BY created_at DESC LIMIT 1",
+                                 self.conn)
 
     def select_systems(self) -> pd.DataFrame:
+        """Select most recent record of all systems"""
         return pd.read_sql_query("""
             SELECT t1.*, t2.solarSystemName, t2.constellationName, t2.regionName FROM systems t1 
             LEFT JOIN map t2 ON t1.system_id = t2.solarSystemID 
             WHERE t1.created_at = (SELECT MAX(t3.created_at) FROM systems t3 WHERE t3.system_id = t1.system_id);
         """, self.conn)
-    
+
     def select_system_by_name(self, name) -> pd.DataFrame:
+        """Select systems by name"""
         sql = """
             SELECT map.solarSystemName system_name, adm, tier, created_at FROM systems
             INNER JOIN map ON map.solarSystemID = systems.system_id
             WHERE map.solarSystemName=? OR map.constellationName=? OR map.regionName=? ORDER BY created_at
         """
         return pd.read_sql_query(sql, self.conn, params=[name, name, name])
 
     def select_system_history(self, system, limit) -> pd.DataFrame:
+        """Select history of a single system"""
         return pd.read_sql_query("""
             SELECT system_id, adm, tier, created_at FROM systems
             INNER JOIN map ON map.solarSystemID = systems.system_id
             WHERE map.solarSystemName=? ORDER BY created_at DESC LIMIT ?
         """, self.conn, params=[system, limit])
```

### Comparing `pydisadm-1.0.6/pydisadm/utils/plot_utils.py` & `pydisadm-1.0.7/pydisadm/utils/plot_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Plotting utility functions"""
 import pandas as pd
 import matplotlib.pyplot as plt
 
 def plot_save_to_file(name, file_name):
+    """Save plot to file"""
     plt.title(name)
     plt.savefig(file_name, bbox_inches='tight')
 
 def plot_adm_history_of_systems(systems: pd.DataFrame) -> bool:
+    """Generate plot of system ADM levels"""
     if (len(systems)) < 1:
         return False
-    
+
     systems.created_at = pd.to_datetime(systems.created_at)
     systems.pivot(index='created_at', columns='system_name', values='adm').plot(
         ylim=(1.0, 6.0), xlabel='Date', ylabel='ADM').legend(bbox_to_anchor=(1, 1))
 
     return True
```

### Comparing `pydisadm-1.0.6/pyproject.toml` & `pydisadm-1.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.0.6"
+version = "1.0.7"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
 
@@ -20,14 +20,15 @@
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.4"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
+pylint = "^2.17.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
```

### Comparing `pydisadm-1.0.6/PKG-INFO` & `pydisadm-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -82,14 +82,30 @@
 
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
 ## 🚧 Development
 
+### Environment
+The development environment and dependencies is managed using `poetry`. Use the following command to set up environment and install dependencies:
+```shell
+poetry install
+```
+
+A nested poetry shell can be started using this command:
+```shell
+poetry shell
+```
+
+### Run Linting
+```shell
+pylint --rcfile pylint.rc pydisadm/**/*.py
+```
+
 ### Run Unit Tests
 ```shell
 pytest tests/ --cov=pydisadm --cov-branch
 ```
 
 ## 💡 Credits
 Project is forked from and inspired by [@anjode](https://www.github.com/anjode)
```

