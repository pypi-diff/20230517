# Comparing `tmp/nextguild-1.1.3.tar.gz` & `tmp/nextguild-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.1.3.tar", last modified: Mon May  1 21:38:00 2023, max compression
+gzip compressed data, was "nextguild-1.1.4.tar", last modified: Wed May 17 13:18:14 2023, max compression
```

## Comparing `nextguild-1.1.3.tar` & `nextguild-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:38:00.486765 nextguild-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 21:37:43.000000 nextguild-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 21:38:00.482765 nextguild-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-01 21:37:43.000000 nextguild-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:38:00.482765 nextguild-1.1.3/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    36828 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:38:00.482765 nextguild-1.1.3/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-01 21:37:43.000000 nextguild-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:38:00.486765 nextguild-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:18:14.220418 nextguild-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 13:18:01.000000 nextguild-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-17 13:18:14.220418 nextguild-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 13:18:01.000000 nextguild-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:18:14.220418 nextguild-1.1.4/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38255 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:18:14.220418 nextguild-1.1.4/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-17 13:18:01.000000 nextguild-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:18:14.220418 nextguild-1.1.4/setup.cfg
```

### Comparing `nextguild-1.1.3/LICENSE` & `nextguild-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/PKG-INFO` & `nextguild-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.3
+Version: 1.1.4
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.3/README.md` & `nextguild-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/nextguild/channel.py` & `nextguild-1.1.4/nextguild/channel.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/nextguild/client.py` & `nextguild-1.1.4/nextguild/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,16 @@
         #     data = response.json()
         #     breakpoint()
         # except json.JSONDecodeError:
         #     data = response.text
         #     breakpoint()
         try:
             data: dict = json.loads(response.content)
-        except: return
+        except:
+            return
         if 200 <= code < 300:
             return data
         raise ValueError(f'Request failed with status {code}: {data}')
 
     def create_channel(
             self,
             name: str,
@@ -577,15 +578,15 @@
             data.update({key: value})
         response = self.request(
             'POST',
             f'{self.base_url}/channels/{channel_id}/events',
             json=data
         )
         return response
-    
+
     def update_event(
             self,
             channel_id: str,
             event_id: int,
             **kwargs
     ):
         data = {}
@@ -598,14 +599,15 @@
         )
         return response
 
     def member_is_owner(self, server_id: str, user_id: str):
         """Checks if a user is the owner of a server."""
         ownerid = self.get_server(server_id).get('server', {}).get('ownerId')
         return ownerid == user_id
+
     def get_events(
             self,
             channel_id: str,
             before: datetime = None,
             after: datetime = None,
             limit: int = None
     ):
@@ -682,92 +684,92 @@
             event_id: int
     ):
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/events/{event_id}/rsvps'
         )
         return response
-    
+
     def create_announcement(self, channel_id: str, title: str, content: str):
         response = self.request(
             'POST',
             f'{self.base_url}/channels/{channel_id}/announcements',
             json={'title': title, 'content': content}
         )
         return response
-    
+
     def get_announcement(self, channel_id: str, announcement_id: str):
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}'
         )
         return response
-    
+
     def get_announcements(self, channel_id: str, before: str = None, limit: str = None):
         params = {}
         if before:
             params['before'] = before
         if limit:
             params['limit'] = limit
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/announcements'
         )
         return response
-    
+
     def update_announcement(self, channel_id: str, announcement_id: str, title: str = None, content: str = None):
         params = {}
         if title:
             params['title'] = title
         if content:
             params['content'] = content
         response = self.request(
             'PATCH',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}',
             json=params
         )
         return response
-    
+
     def delete_announcement(self, channel_id: str, announcement_id: str):
         response = self.request(
             'DELETE',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}'
         )
         return response
-    
+
     def create_announcement_comment(self, channel_id: str, announcement_id: str, content: str):
         response = self.request(
             'POST',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/comments',
             json={'content': content}
         )
         return response
-    
+
     def get_announcement_comment(self, channel_id: str, announcement_id: str, comment_id: int):
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}'
         )
         return response
-    
+
     def get_announcement_comments(self, channel_id: str, announcement_id: str):
         response = self.request(
             'GET',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/comments'
         )
         return response
-    
+
     def update_announcement_comment(self, channel_id: str, announcement_id: str, comment_id: int, content: str):
         response = self.request(
             'PATCH',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}',
             json={'content': content}
         )
         return response
-    
+
     def delete_announcement_comment(self, channel_id: str, announcement_id: str, comment_id: int):
         response = self.request(
             'DELETE',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}'
         )
         return response
 
@@ -858,15 +860,15 @@
             title: str,
             content: str,
     ):
 
         response = self.request(
             'POST',
             f'{self.base_url}/channels/{channel_id}/topics',
-            json= {'title': title, 'content': content}
+            json={'title': title, 'content': content}
         )
         return response
 
     def get_forum_topics(
             self,
             channel_id: str,
             before: datetime = None,
@@ -905,15 +907,15 @@
             title: str = None,
             content: str = None,
     ):
         data = {}
 
         if content:
             data['content'] = content
-        
+
         if title:
             data['title'] = title
 
         response = self.request(
             'PATCH',
             f'{self.base_url}/channels/{channel_id}/topics/{forum_topic_id}',
             json=data
@@ -1047,15 +1049,15 @@
             emote_id: int
     ):
         response = self.request(
             'PUT',
             f'{self.base_url}/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'
         )
         return response
-    
+
     def delete_message_reaction(
             self,
             channel_id: str,
             message_id: str,
             emote_id: int,
             user_id: str
     ):
@@ -1164,15 +1166,15 @@
     ):
         response = self.request(
             'DELETE',
             f'{self.base_url}/channels/{channel_id}/events/{event_id}'
             f'/comments/{comment_id}/emotes/{emote_id}'
         )
         return response
-    
+
     def create_announcement_reaction(
             self,
             channel_id: str,
             announcement_id: str,
             emote_id: int
     ):
         response = self.request(
@@ -1188,28 +1190,28 @@
             emote_id: int
     ):
         response = self.request(
             'DELETE',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/emotes/{emote_id}'
         )
         return response
-    
+
     def create_announcement_comment_reaction(
             self,
             channel_id: str,
             announcement_id: str,
             comment_id: int,
             emote_id: int
     ):
         response = self.request(
             'PUT',
             f'{self.base_url}/channels/{channel_id}/announcements/{announcement_id}/comments/{comment_id}/emotes/{emote_id}'
         )
         return response
-    
+
     def delete_announcement_comment_reaction(
             self,
             channel_id: str,
             announcement_id: str,
             comment_id: int,
             emote_id: int
     ):
@@ -1222,15 +1224,14 @@
     def create_doc(
             self,
             channel_id: str,
             title: str,
             content: str
     ):
 
-
         response = self.request(
             'POST',
             f'{self.base_url}/channels/{channel_id}/docs',
             json={'title': title, 'content': content}
         )
         return response
 
@@ -1334,32 +1335,68 @@
             f'{comment_id}'
         )
         return response
 
     def get_bot_user_id(self):
         response = self.request('GET', f'{self.base_url}/users/@me')
         return response['user']['id']
-    
+
     def get_user_servers(self, user_id: str):
         response = self.request('GET', f'{self.base_url}users/{user_id}/servers')
         return response
 
     def get_bot_servers(self):
         response = self.request('GET', f'{self.base_url}/users/@me/servers')
         return response
-    
+
     def get_default_channel(self, server_id: str):
         r = self.request('GET', f'{self.base_url}/servers/{server_id}')
         try:
             print(r)
             response = r['server']['defaultChannelId']
         except:
             response = 'No default channel found'
         return response
-    
+
+
+    def create_group(self, server_id: str, name: str, description: str, emote_id: int, is_public: bool):
+        response = self.request('POST', f'{self.base_url}/servers/{server_id}/groups', json={'name': name, 'description': description, 'emoteId': emote_id, 'isPublic': is_public})
+        return response
+
+    def get_groups(self, server_id: str):
+        response = self.request('GET', f'{self.base_url}/servers/{server_id}/groups')
+        return response
+
+
+    def get_group(self, server_id: str, group_id: str):
+        response = self.request('GET', f'{self.base_url}/servers/{server_id}/groups/{group_id}')
+        return response
+
+    def update_group(self, server_id: str, group_id: str, name: str, description: str, emote_id: int, is_public: bool):
+
+        response = self.request('PATCH', f'{self.base_url}/servers/{server_id}/groups/{group_id}', json={'name': name, 'description': description, 'emoteId': emote_id, 'isPublic': is_public})
+        return response
+
+
+    def delete_group(self, server_id: str, group_id: str):
+        response = self.request('DELETE', f'{self.base_url}/servers/{server_id}/groups/{group_id}')
+        return response
+
+
+
+    def update_status(self, content: str, emote_id: int):
+        response = self.request('PUT', f'{self.base_url}/users/@me/status', json={'content': content, 'emoteId': emote_id})
+        return response
+
+
+    def delete_status(self):
+        response = self.request('DELETE', f'{self.base_url}/users/@me/status')
+        return response
+
+
     def member_has_role(self, server_id: str, user_id: str, role_id: int or list, type: str = 'any'):
         r = self.get_member_roles(server_id, user_id)
         if isinstance(role_id, list):
             if type == 'any':
                 for i in role_id:
                     if i in r:
                         return True
@@ -1369,16 +1406,18 @@
                     if i not in r:
                         return False
                 return True
         if role_id in r:
             return True
         else:
             return False
-        
+
     def member_is_owner(self, server_id: str, user_id: str):
         r = self.get_server(server_id)
         if r['server']['ownerId'] == user_id:
             return True
         else:
             return False
-        
+
+
+
```

### Comparing `nextguild-1.1.3/nextguild/embed.py` & `nextguild-1.1.4/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/nextguild/events.py` & `nextguild-1.1.4/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/nextguild/message.py` & `nextguild-1.1.4/nextguild/message.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/nextguild/reaction.py` & `nextguild-1.1.4/nextguild/reaction.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.3/nextguild.egg-info/PKG-INFO` & `nextguild-1.1.4/nextguild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.3
+Version: 1.1.4
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.3/pyproject.toml` & `nextguild-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

