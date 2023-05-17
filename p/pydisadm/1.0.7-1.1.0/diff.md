# Comparing `tmp/pydisadm-1.0.7.tar.gz` & `tmp/pydisadm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.0.7.tar", max compression
+gzip compressed data, was "pydisadm-1.1.0.tar", max compression
```

## Comparing `pydisadm-1.0.7.tar` & `pydisadm-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     2711 2023-05-17 10:39:05.050201 pydisadm-1.0.7/README.md
--rw-r--r--   0        0        0      111 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/__init__.py
--rw-r--r--   0        0        0     1060 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/__main__.py
--rw-r--r--   0        0        0     1541 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     6551 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0      702 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      816 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/configuration.py
--rw-r--r--   0        0        0     6872 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-17 10:39:05.054201 pydisadm-1.0.7/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1108 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3442 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/services/esi.py
--rw-r--r--   0        0        0      472 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-17 10:39:05.070201 pydisadm-1.0.7/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-17 10:39:35.706800 pydisadm-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 pydisadm-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2711 2023-05-17 11:44:06.264630 pydisadm-1.1.0/README.md
+-rw-r--r--   0        0        0      111 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1060 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1541 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     6691 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0      816 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/configuration.py
+-rw-r--r--   0        0        0     7883 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-17 11:44:06.268630 pydisadm-1.1.0/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-17 11:44:06.284630 pydisadm-1.1.0/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1108 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3442 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-17 11:44:06.288630 pydisadm-1.1.0/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-17 11:44:37.684786 pydisadm-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 pydisadm-1.1.0/PKG-INFO
```

### Comparing `pydisadm-1.0.7/README.md` & `pydisadm-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/__main__.py` & `pydisadm-1.1.0/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/bot/adm_bot.py` & `pydisadm-1.1.0/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/bot/adm_cog.py` & `pydisadm-1.1.0/pydisadm/bot/adm_cog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Cog providing ADM related commands"""
 
 import discord
 from discord.ext import commands
 from discord import app_commands
+from pydisadm.bot.update_adm_modal import UpdateAdmModal
 
 from pydisadm.bot.utils import check_allowed_channel, text_channels_with_send_permission
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 from pydisadm.utils.datetime_utils import convert_to_local_timestamp
 
 class Adm(commands.GroupCog):
@@ -119,21 +120,22 @@
             return
 
         await interaction.response.defer(thinking=True)
         self.controller.update_adm_data()
         await interaction.followup.send("ADM data manually refreshed 🦀")
 
     @app_commands.command(description='Manually update ADM of system.')
-    async def update(self, interaction: discord.Interaction, system_name: str, adm: str):
+    @app_commands.describe(system_name='Which system to update ADM')
+    async def update(self, interaction: discord.Interaction, system_name: str):
         """Command to manually update ADM for system"""
         if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
-        await self.update_adm(interaction, system_name, float(adm))
+        await interaction.response.send_modal(UpdateAdmModal(system_name, self.controller))
 
     @commands.Cog.listener()
     async def on_ready(self):
         """cog on_ready event callback"""
         channels = text_channels_with_send_permission(self.bot)
 
         await self.bot.tree.sync()
```

### Comparing `pydisadm-1.0.7/pydisadm/bot/utils.py` & `pydisadm-1.1.0/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/configuration.py` & `pydisadm-1.1.0/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/controller/adm_controller.py` & `pydisadm-1.1.0/pydisadm/controller/adm_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
 
 from pydisadm.configuration import Configuration
 from pydisadm.services.database import Database
 from pydisadm.services.esi import sovereignty_structures
+from pydisadm.utils.adm_utils import adm_from_index
 from pydisadm.utils.plot_utils import plot_adm_history_of_systems, plot_save_to_file
 
 
 class AdmController:
     """Controller implementation for ADM operations"""
 
     def __init__(self, configuration: Configuration, database: Database):
@@ -105,14 +106,21 @@
             'd_tier'
         ]
 
         systems['tier'] = np.select(conditions, values)
 
         return systems
 
+    def create_system_adm_from_index(self, system, military: int, industrial: int, strategic: int):
+        """Create a DataFrame for system ADM data from index values"""
+        adm = adm_from_index(military, industrial, strategic)
+
+        return self.create_system_adm(system, adm)
+
+
     def create_system_adm(self, system, adm):
         """Create a DataFrame for system ADM data"""
         system_adm = pd.DataFrame(columns=['system_id', 'adm'])
         system_adm['system_id'] = system['solarSystemID']
         system_adm['adm'] = [adm]
 
         self.tier_list(system_adm)
@@ -143,14 +151,32 @@
 
         insert_systems = self.create_system_adm(system, adm)
 
         self.database.insert_systems(insert_systems)
 
         return True
 
+    def update_system_adm_from_index(self,
+                                     system_name: str,
+                                     military: int,
+                                     industrial: int,
+                                     strategic: int) -> bool:
+        """Update ADM for system with name from index values"""
+        system = self.database.select_system_with_name(system_name)
+
+        if system.empty:
+            return (False, 0)
+
+        insert_systems = self.create_system_adm_from_index(
+            system, military, industrial, strategic)
+
+        self.database.insert_systems(insert_systems)
+
+        return (True, insert_systems['adm'][0])
+
     def get_system_adms(self, alliance_id):
         """Retrieve ADM for systems controlled by alliance"""
         structures = sovereignty_structures()
         system_adms = self.get_alliance_structures(structures, alliance_id)
 
         system_adms.drop_duplicates(inplace=True)
```

### Comparing `pydisadm-1.0.7/pydisadm/data/mapConstellations.csv` & `pydisadm-1.1.0/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/data/mapRegions.csv` & `pydisadm-1.1.0/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.1.0/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/loader/datasets.py` & `pydisadm-1.1.0/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/loader/static_data.py` & `pydisadm-1.1.0/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.1.0/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/services/database.py` & `pydisadm-1.1.0/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/services/esi.py` & `pydisadm-1.1.0/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pydisadm/utils/plot_utils.py` & `pydisadm-1.1.0/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.7/pyproject.toml` & `pydisadm-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.0.7"
+version = "1.1.0"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.0.7/PKG-INFO` & `pydisadm-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.0.7
+Version: 1.1.0
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

