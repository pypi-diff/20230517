# Comparing `tmp/swgoh_comlink-1.8.0.tar.gz` & `tmp/swgoh_comlink-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/comlink-python/comlink-python/dist/.tmp-paj2_r6d/swgoh_comlink-1.8.0.tar", last modified: Tue Jan 31 16:55:33 2023, max compression
+gzip compressed data, was "/home/runner/work/comlink-python/comlink-python/dist/.tmp-syg88egc/swgoh_comlink-1.9.0.tar", last modified: Tue Jan 31 18:32:57 2023, max compression
```

## Comparing `swgoh_comlink-1.8.0.tar` & `swgoh_comlink-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-01-31 16:55:03.000000 swgoh_comlink-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-01-31 16:55:03.000000 swgoh_comlink-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-01-31 16:55:03.000000 swgoh_comlink-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/swgoh_comlink/
--rw-r--r--   0 runner    (1001) docker     (122)    13656 2023-01-31 16:55:03.000000 swgoh_comlink-1.8.0/src/swgoh_comlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-31 16:55:23.000000 swgoh_comlink-1.8.0/src/swgoh_comlink/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/swgoh_comlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/swgoh_comlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/swgoh_comlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/swgoh_comlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-01-31 16:55:33.000000 swgoh_comlink-1.8.0/src/swgoh_comlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-01-31 18:32:30.000000 swgoh_comlink-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-01-31 18:32:30.000000 swgoh_comlink-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-01-31 18:32:30.000000 swgoh_comlink-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/swgoh_comlink/
+-rw-r--r--   0 runner    (1001) docker     (122)    15088 2023-01-31 18:32:30.000000 swgoh_comlink-1.9.0/src/swgoh_comlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-31 18:32:48.000000 swgoh_comlink-1.9.0/src/swgoh_comlink/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/swgoh_comlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/swgoh_comlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/swgoh_comlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/swgoh_comlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-01-31 18:32:57.000000 swgoh_comlink-1.9.0/src/swgoh_comlink.egg-info/top_level.txt
```

### Comparing `swgoh_comlink-1.8.0/LICENSE` & `swgoh_comlink-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swgoh_comlink-1.8.0/PKG-INFO` & `swgoh_comlink-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swgoh_comlink
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python 3 interface library for swgoh-comlink (https://github.com/swgoh-utils/swgoh-comlink)
 Author-email: Mar Trepodi <martrepodi@gmail.com>
 Project-URL: Homepage, https://github.com/swgoh-utils/comlink-python
 Project-URL: Bug Tracker, https://github.com/swgoh-utils/comlink-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swgoh_comlink-1.8.0/README.md` & `swgoh_comlink-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `swgoh_comlink-1.8.0/pyproject.toml` & `swgoh_comlink-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swgoh_comlink-1.8.0/src/swgoh_comlink/__init__.py` & `swgoh_comlink-1.9.0/src/swgoh_comlink/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -146,23 +146,35 @@
             query_string = f'?' + '&'.join(filter(None, [flags, language]))
         endpoint_string = f'api' + query_string if query_string else 'api'
         return self._post(url_base=self.stats_url_base, endpoint=endpoint_string, payload=request_payload)
 
     def get_enums(self):
         """
         Get an object containing the game data enums
-        :return: dict
+        :return: object
         """
         url = self.url_base + '/enums'
         try:
             r = requests.request('GET', url)
             return loads(r.content.decode('utf-8'))
         except Exception as e:
             raise e
 
+    # alias for non PEP usage of direct endpoint calls
+    getEnums = get_enums
+    def get_events(self):
+        """
+        Get an object containing the events game data
+        :return: object
+        """
+        return self._post('getEvents', {})
+
+    # alias for non PEP usage of direct endpoint calls
+    getEvents = get_events
+
     def get_game_data(self,
                             version: str = "",
                             include_pve_units=True,
                             request_segment: int = 0,
                             enums=False
                             ):
         """
@@ -182,14 +194,16 @@
                 "includePveUnits": include_pve_units,
                 "requestSegment": request_segment
             },
             "enums": enums
         }
         return self._post(endpoint='data', payload=payload)
 
+    # alias for non PEP usage of direct endpoint calls
+    getGameData = get_game_data
     def get_localization(self,
                                id: str,
                                unzip=False,
                                enums=False
                                ):
         """
         Get localization data from game
@@ -203,14 +217,17 @@
             'enums': enums,
             'payload': {
                 'id': id
             }
         }
         return self._post(endpoint='localization', payload=payload)
 
+    # aliases for non PEP usage of direct endpoint calls
+    getLocalization = get_localization
+    getLocalizationBundle = get_localization
     get_localization_bundle = get_localization
 
     def get_game_metadata(self, client_specs = None, enums = False):
         """
         Get the game metadata. Game metadata contains the current game and localization versions.
         :param client_specs:  Optional dictionary containing
         :param enums: Boolean signifying whether enums in response should be translated to text. [Default: False]
@@ -231,14 +248,17 @@
         """
         if client_specs:
             payload = { "payload": { "client_specs": client_specs}, "enums": enums }
         else:
             payload = {}
         return self._post(endpoint='metadata', payload=payload)
 
+    # alias for non PEP usage of direct endpoint calls
+    getGameMetaData = get_game_metadata
+    getMetaData = get_game_metadata
     get_metadata = get_game_metadata
 
     def get_player(self,
                          allycode: str or int = None,
                          player_id: str = None,
                          enums=False
                          ):
@@ -248,31 +268,40 @@
         :param player_id: string representing player game ID
         :param enums: boolean [Defaults to False]
         :return: dict
         """
         payload = _get_player_payload(allycode=allycode, player_id=player_id, enums=enums)
         return self._post(endpoint='player', payload=payload)
 
+    # alias for non PEP usage of direct endpoint calls
+    getPlayer = get_player
+
     def get_player_arena(self,
                                allycode: int = None,
                                player_id: str = None,
+                               playerDetailsOnly = False,
                                enums=False
                                ):
         """
         Get player arena information from game
         :param allycode: integer or string representing player allycode
         :param player_id: string representing player game ID
+        :param playerDetailsOnly: filter results to only player details [Defaults to False]
         :param enums: boolean [Defaults to False]
         :return: dict
         """
         payload = _get_player_payload(allycode=allycode, player_id=player_id, enums=enums)
+        payload['payload']['playerDetailsOnly'] = playerDetailsOnly
         return self._post(endpoint='playerArena', payload=payload)
 
-    # alias to allow for get_arena() calls as a shortcut for get_player_arena()
+    # alias to allow for get_arena() calls as a shortcut for get_player_arena() and non PEP variations
     get_arena = get_player_arena
+    get_player_arena_profile = get_player_arena
+    getPlayerArena = get_player_arena
+    getPlayerArenaProfile = get_player_arena
 
     def get_guild(self,
                         guild_id: str,
                         include_recent_guild_activity_info=False,
                         enums=False
                         ):
         """
@@ -290,14 +319,17 @@
             "enums": enums
         }
         guild = self._post(endpoint='guild', payload=payload)
         if 'guild' in guild.keys():
             guild = guild['guild']
         return guild
 
+    # alias for non PEP usage of direct endpoint calls
+    getGuild = get_guild
+
     def get_guilds_by_name(self,
                                  name: str,
                                  start_index: int = 0,
                                  count: int = 10,
                                  enums=False
                                  ):
         """
@@ -315,14 +347,17 @@
                 "startIndex": start_index,
                 "count": count
             },
             "enums": enums
         }
         return self._post(endpoint='getGuilds', payload=payload)
 
+    # alias for non PEP usage of direct endpoint calls
+    getGuildByName = get_guilds_by_name
+
     def get_guilds_by_criteria(self,
                                      search_criteria: dict,
                                      start_index: int = 0,
                                      count: int = 10,
                                      enums=False
                                      ):
         """
@@ -348,7 +383,10 @@
                 "filterType": 5,
                 "startIndex": start_index,
                 "count": count
             },
             "enums": enums
         }
         return self._post(endpoint='getGuilds', payload=payload)
+
+    # alias for non PEP usage of direct endpoint calls
+    getGuildByCriteria = get_guilds_by_criteria
```

### Comparing `swgoh_comlink-1.8.0/src/swgoh_comlink.egg-info/PKG-INFO` & `swgoh_comlink-1.9.0/src/swgoh_comlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swgoh-comlink
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python 3 interface library for swgoh-comlink (https://github.com/swgoh-utils/swgoh-comlink)
 Author-email: Mar Trepodi <martrepodi@gmail.com>
 Project-URL: Homepage, https://github.com/swgoh-utils/comlink-python
 Project-URL: Bug Tracker, https://github.com/swgoh-utils/comlink-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

