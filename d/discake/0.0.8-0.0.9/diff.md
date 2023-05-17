# Comparing `tmp/discake-0.0.8.tar.gz` & `tmp/discake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discake-0.0.8.tar", last modified: Fri May  5 07:49:01 2023, max compression
+gzip compressed data, was "discake-0.0.9.tar", last modified: Wed May 17 11:05:26 2023, max compression
```

## Comparing `discake-0.0.8.tar` & `discake-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 07:48:49.000000 discake-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 07:49:01.808116 discake-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-05 07:48:49.000000 discake-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 07:48:49.000000 discake-0.0.8/discake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-05 07:48:49.000000 discake-0.0.8/discake/paginator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 07:48:49.000000 discake-0.0.8/discake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-05 07:48:49.000000 discake-0.0.8/discake/utils/paginate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:49:01.808116 discake-0.0.8/discake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:49:01.000000 discake-0.0.8/discake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:49:01.808116 discake-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-05 07:48:49.000000 discake-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:05:26.252638 discake-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 11:05:15.000000 discake-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-17 11:05:26.252638 discake-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-17 11:05:15.000000 discake-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:05:26.248638 discake-0.0.9/discake/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 11:05:15.000000 discake-0.0.9/discake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:05:26.252638 discake-0.0.9/discake/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-17 11:05:15.000000 discake-0.0.9/discake/paginator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:05:26.252638 discake-0.0.9/discake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 11:05:15.000000 discake-0.0.9/discake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-17 11:05:15.000000 discake-0.0.9/discake/utils/paginate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:05:26.252638 discake-0.0.9/discake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-17 11:05:26.000000 discake-0.0.9/discake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 11:05:26.000000 discake-0.0.9/discake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:05:26.000000 discake-0.0.9/discake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 11:05:26.000000 discake-0.0.9/discake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 11:05:26.000000 discake-0.0.9/discake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:05:26.252638 discake-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 11:05:15.000000 discake-0.0.9/setup.py
```

### Comparing `discake-0.0.8/LICENSE` & `discake-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `discake-0.0.8/PKG-INFO` & `discake-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discake
-Version: 0.0.8
+Version: 0.0.9
 Summary: A discord py support library containing utilities.
 Home-page: https://github.com/lollipop-69/discake
 Author: Carlos
 License: MIT
 Project-URL: Homepage, https://github.com/lollipop-69/discake/
 Keywords: discord py,discord paginator,paginator,button paginator
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,15 +60,15 @@
 .. code:: py
 
     import discord
     from discord import Embed, Intents
     from discord.ext import commands
     from discake import Paginator
 
-    class MyBot(comamnds.Bot):
+    class MyBot(commands.Bot):
         def __init__(self):
             super().__init__(command_prefix = '!')
             
         async def on_ready(self):
             print('Logged on as', self.user)
 
     client = MyBot(intents=Intents.default())
@@ -86,15 +86,14 @@
         await paginate_object.send(ctx)
     
     
     client.run('TOKEN')
 
 Links
 ------
-
 .. image:: https://invidget.switchblade.xyz/egvmz5NjSZ?theme=light
    :target: https://discord.gg/egvmz5NjSZ
    :alt: Support Server
 
 Author
 ------
 .. image:: https://discord.c99.nl/widget/theme-3/545953035776688139.png
```

### Comparing `discake-0.0.8/README.rst` & `discake-0.0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 .. code:: py
 
     import discord
     from discord import Embed, Intents
     from discord.ext import commands
     from discake import Paginator
 
-    class MyBot(comamnds.Bot):
+    class MyBot(commands.Bot):
         def __init__(self):
             super().__init__(command_prefix = '!')
             
         async def on_ready(self):
             print('Logged on as', self.user)
 
     client = MyBot(intents=Intents.default())
@@ -65,15 +65,14 @@
         await paginate_object.send(ctx)
     
     
     client.run('TOKEN')
 
 Links
 ------
-
 .. image:: https://invidget.switchblade.xyz/egvmz5NjSZ?theme=light
    :target: https://discord.gg/egvmz5NjSZ
    :alt: Support Server
 
 Author
 ------
 .. image:: https://discord.c99.nl/widget/theme-3/545953035776688139.png
```

### Comparing `discake-0.0.8/discake/paginator/__init__.py` & `discake-0.0.9/discake/paginator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,28 +76,36 @@
             self._pages.append(chunk)
             
         view = ButtonsView(task = self, color = self.color, timeout = self.timeout, previous = self.prev, next = self.next, first = self.first,clear = self.clear, last = self.last)
         
         if isinstance(self._pages[0], Embed):
             if len(self._pages) > 1:
                 if isinstance(interaction, Interaction):
+                    try: await interaction.response.defer()
+                    except: pass
                     self.page = await interaction.followup.send(embed=self._pages[0],view=view) 
                 else:
                     self.page = await interaction.send(embed=self._pages[0],view=view)
             else:
                 if isinstance(interaction, Interaction):
-                    self.page = await interaction.response.send_message(embed=self._pages[0])
+                    try: await interaction.response.defer()
+                    except: pass
+                    self.page = await interaction.followup.send(embed=self._pages[0])
                 else:
                     self.page = await interaction.send(embed=self._pages[0])
         elif isinstance(self._pages[0], Union[str, int]):
             if len(self._pages) > 1:
                 if isinstance(interaction, Interaction):
+                    try: await interaction.response.defer()
+                    except: pass
                     self.page = await interaction.followup.send(content=self._pages[0],view=view)
                 else:
                     self.page = await interaction.send(content=self._pages[0],view=view)
             else:
                 if isinstance(interaction, Interaction):
-                    self.page = await interaction.response.send_message(content=self._pages[0])
+                    try: await interaction.response.defer()
+                    except: pass
+                    self.page = await interaction.followup.send(content=self._pages[0])
                 else:
                     self.page = await interaction.send(content=self._pages[0])
         else:
             raise TypeError("Entries should be of type 'discord.Embed' or 'string'")
```

### Comparing `discake-0.0.8/discake/utils/paginate.py` & `discake-0.0.9/discake/utils/paginate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 
 from discord import Embed, ButtonStyle, Interaction
 from discord.ui import View, Button
 from typing import Literal, Optional
 
+__all__ = (
+    'ButtonsView',
+)
+
 class ButtonsView(View):
     def __init__(
         self,
         task,
         timeout: Optional[float] = 180,
         color: Literal['blurple', 'grey', 'green', 'red'] = 'grey',
         first = '⏮',
```

### Comparing `discake-0.0.8/discake.egg-info/PKG-INFO` & `discake-0.0.9/discake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discake
-Version: 0.0.8
+Version: 0.0.9
 Summary: A discord py support library containing utilities.
 Home-page: https://github.com/lollipop-69/discake
 Author: Carlos
 License: MIT
 Project-URL: Homepage, https://github.com/lollipop-69/discake/
 Keywords: discord py,discord paginator,paginator,button paginator
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,15 +60,15 @@
 .. code:: py
 
     import discord
     from discord import Embed, Intents
     from discord.ext import commands
     from discake import Paginator
 
-    class MyBot(comamnds.Bot):
+    class MyBot(commands.Bot):
         def __init__(self):
             super().__init__(command_prefix = '!')
             
         async def on_ready(self):
             print('Logged on as', self.user)
 
     client = MyBot(intents=Intents.default())
@@ -86,15 +86,14 @@
         await paginate_object.send(ctx)
     
     
     client.run('TOKEN')
 
 Links
 ------
-
 .. image:: https://invidget.switchblade.xyz/egvmz5NjSZ?theme=light
    :target: https://discord.gg/egvmz5NjSZ
    :alt: Support Server
 
 Author
 ------
 .. image:: https://discord.c99.nl/widget/theme-3/545953035776688139.png
```

### Comparing `discake-0.0.8/setup.py` & `discake-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.rst', 'r') as file:
     readme = file.read()
     
 setup(
     name='discake',
     author='Carlos',
     url='https://github.com/lollipop-69/discake',
-    version='0.0.8',
+    version='0.0.9',
     license='MIT',
     description='A discord py support library containing utilities.',
     long_description=readme,
     long_description_content_type='text/x-rst',
     install_requires=[
         'discord.py'
     ],
```

