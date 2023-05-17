# Comparing `tmp/dslash-0.6.3.tar.gz` & `tmp/dslash-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslash-0.6.3.tar", max compression
+gzip compressed data, was "dslash-0.6.4.tar", max compression
```

## Comparing `dslash-0.6.3.tar` & `dslash-0.6.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1077 2022-09-01 01:29:39.722384 dslash-0.6.3/LICENSE
--rw-r--r--   0        0        0     5496 2022-09-01 01:29:39.722384 dslash-0.6.3/README.md
--rw-r--r--   0        0        0      815 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/__init__.py
--rw-r--r--   0        0        0     5108 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/choices.py
--rw-r--r--   0        0        0    12730 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/client.py
--rw-r--r--   0        0        0    13747 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/commands.py
--rw-r--r--   0        0        0     3670 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/groups.py
--rw-r--r--   0        0        0     6120 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/options.py
--rw-r--r--   0        0        0      903 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/permissions.py
--rw-r--r--   0        0        0        0 2022-09-01 01:29:39.722384 dslash-0.6.3/dslash/py.typed
--rw-r--r--   0        0        0     1639 2022-09-01 01:29:39.722384 dslash-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6387 1970-01-01 00:00:00.000000 dslash-0.6.3/setup.py
--rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 dslash-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-17 21:21:41.148535 dslash-0.6.4/LICENSE
+-rw-r--r--   0        0        0     5496 2023-05-17 21:21:41.148535 dslash-0.6.4/README.md
+-rw-r--r--   0        0        0      815 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/__init__.py
+-rw-r--r--   0        0        0     5187 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/choices.py
+-rw-r--r--   0        0        0    12730 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/client.py
+-rw-r--r--   0        0        0    13747 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/commands.py
+-rw-r--r--   0        0        0     3670 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/groups.py
+-rw-r--r--   0        0        0     6136 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/options.py
+-rw-r--r--   0        0        0      903 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/permissions.py
+-rw-r--r--   0        0        0        0 2023-05-17 21:21:41.148535 dslash-0.6.4/dslash/py.typed
+-rw-r--r--   0        0        0     1639 2023-05-17 21:21:41.148535 dslash-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6434 1970-01-01 00:00:00.000000 dslash-0.6.4/PKG-INFO
```

### Comparing `dslash-0.6.3/LICENSE` & `dslash-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dslash-0.6.3/README.md` & `dslash-0.6.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DSlash
 
-![Version: 0.6.3](https://img.shields.io/badge/Version-0.6.3-red?style=flat-square)
+![Version: 0.6.4](https://img.shields.io/badge/Version-0.6.4-red?style=flat-square)
 [![Code Style: black](https://img.shields.io/badge/Code%20Style-black-black?style=flat-square)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-orange?style=flat-square)](./LICENSE)
 [![PyPI: dslash](https://img.shields.io/badge/PyPI-dslash-green?style=flat-square)](https://pypi.org/project/dslash)
 ![Python: ^3.9](https://img.shields.io/badge/python-%5E3.9-blue?style=flat-square)
 
 > **THIS PROJECT IS NO LONGER MAINTAINED**
 >
```

### Comparing `dslash-0.6.3/dslash/__init__.py` & `dslash-0.6.4/dslash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     allow_users,
     disallow_roles,
     disallow_users,
     global_permissions,
     guild_permissions,
 )
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 __all__ = (
     "__version__",
     "CommandClient",
     "CommandGroup",
     "CommandSubGroup",
     "subcommand",
     "Channel",
```

### Comparing `dslash-0.6.3/dslash/choices.py` & `dslash-0.6.4/dslash/choices.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,16 @@
             choice = new_cls(choice_data.name, choice_data.value)
             value_map[choice_data.value] = choice
             name_map[name] = choice
         return new_cls
 
     def __getattr__(cls: Type[Choices[CT]], name: str) -> Choices[CT]:
         """Get a choice by name."""
+        if name.startswith("__"):
+            return super().__getattr__(name)
         return cls._name_map[name]  # type: ignore
 
 
 class Choices(Generic[CT], metaclass=ChoicesMeta, abstract=True):
     """A class containing each of the choices for some option.
 
     Example usage:
```

### Comparing `dslash-0.6.3/dslash/client.py` & `dslash-0.6.4/dslash/client.py`

 * *Files identical despite different names*

### Comparing `dslash-0.6.3/dslash/commands.py` & `dslash-0.6.4/dslash/commands.py`

 * *Files identical despite different names*

### Comparing `dslash-0.6.3/dslash/groups.py` & `dslash-0.6.4/dslash/groups.py`

 * *Files identical despite different names*

### Comparing `dslash-0.6.3/dslash/options.py` & `dslash-0.6.4/dslash/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,16 @@
         ):
             if self.choices:
                 return self.choices._get_by_value(value)
             return value
         if type == ApplicationCommandOptionType.attachment:
             data = (
                 interaction.data.get("resolved", {}).get("attachments", {}).get(value)
-                if interaction.data else None
+                if interaction.data
+                else None
             )
             if data:
                 return nextcord.Attachment(data=data, state=interaction._state)
             raise ValueError("Attachment option recieved without resolved attachment.")
         # We could use `resolved` for users/roles/channels, but working with
         # discord.py/nextcord internals is more hassle than it's worth.
         value = int(value)
```

### Comparing `dslash-0.6.3/dslash/permissions.py` & `dslash-0.6.4/dslash/permissions.py`

 * *Files identical despite different names*

### Comparing `dslash-0.6.3/pyproject.toml` & `dslash-0.6.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dslash"
-version = "0.6.3"
+version = "0.6.4"
 description = "A library which supplements Nextcord by adding support for slash commands."
 authors = ["Artemis <me@arty.li>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/artemis21/dslash"
 repository = "https://github.com/artemis21/dslash"
 keywords = ["discord", "discord.py", "nextcord", "slash commands", "extension"]
@@ -20,15 +20,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nextcord = "^2.0.0-alpha.3"
 docstring-parser = "^0.12"
 
 [tool.poetry.dev-dependencies]
-black = "^21.7b0"
+black = "^23.3.0"
 isort = "^5.9.3"
 flake8 = "^3.9.2"
 flake8-annotations = "^2.6.2"
 flake8-bugbear = "^21.4.3"
 flake8-comprehensions = "^3.5.0"
 flake8-datetimez = "^20.10.0"
 flake8-docstrings = "^1.6.0"
```

### Comparing `dslash-0.6.3/setup.py` & `dslash-0.6.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,196 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dslash
+Version: 0.6.4
+Summary: A library which supplements Nextcord by adding support for slash commands.
+Home-page: https://github.com/artemis21/dslash
+License: MIT
+Keywords: discord,discord.py,nextcord,slash commands,extension
+Author: Artemis
+Author-email: me@arty.li
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Dist: docstring-parser (>=0.12,<0.13)
+Requires-Dist: nextcord (>=2.0.0-alpha.3,<3.0.0)
+Project-URL: Repository, https://github.com/artemis21/dslash
+Description-Content-Type: text/markdown
+
+# DSlash
+
+![Version: 0.6.4](https://img.shields.io/badge/Version-0.6.4-red?style=flat-square)
+[![Code Style: black](https://img.shields.io/badge/Code%20Style-black-black?style=flat-square)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-orange?style=flat-square)](./LICENSE)
+[![PyPI: dslash](https://img.shields.io/badge/PyPI-dslash-green?style=flat-square)](https://pypi.org/project/dslash)
+![Python: ^3.9](https://img.shields.io/badge/python-%5E3.9-blue?style=flat-square)
+
+> **THIS PROJECT IS NO LONGER MAINTAINED**
+>
+> Danny has returned from a break, and [Discord.py](https://github.com/rapptz/discord.py)
+> is now being maintained again, with support for slash commands. Nextcord also
+> now has built-in support for slash commands. For new projects, you should use
+> one of these options (or another).
+>
+> Dslash will continue to receive minimal updates to keep it working, at least
+> for the near future, but it will not receive support for new features.
+>
+> One change Discord has made since this library stopped being maintained was
+> to remove support for bots configuring permissions for their own commands. In
+> order to avoid breaking bots, Dslash still allows permissions to be
+> configured as before, but will now ignore them. The `allow_roles`,
+> `allow_users`, `disallow_roles`, `disallow_users`, `global_permissions` and
+> `guild_permissions` wrappers, as well as the `default_permission` and
+> `permissions` parameters are all deprecated and should not be used.
+
+A library which supplements [Nextcord](https://github.com/nextcord/nextcord)
+(a fork of Discord.py) by adding support for slash commands.
+
+Documentation is still a work in progress, and the library should currently be
+considered unstable.
+
+You can install it using pip, eg. `pip install dslash`.
+
+## Example
+
+```python
+import logging
+import random
+import typing
+
+from dslash import Choices, CommandClient, CommandGroup, CommandSubGroup, subcommand
+from nextcord import Embed, Interaction, Member, Role, Attachment
+
+GUILD_ID = ...
+TOKEN = ...
+
+logging.basicConfig(level=logging.INFO)
+client = CommandClient(guild_id=GUILD_ID)
+
+
+@client.event
+async def on_ready():
+    print(f"Logged in as {client.user}.")
+
+
+@client.command()
+async def roll(interaction: Interaction, sides: typing.Optional[int]):
+    """Roll a dice.
+
+    :param sides: How many sides (default 6).
+    """
+    value = random.randint(1, sides or 6)
+    await interaction.response.send_message(f"You got: {value}")
+
+
+@client.group
+class Images(CommandGroup):
+    """Cute image commands."""
+
+    @subcommand()
+    async def cat(self, interaction: Interaction):
+        """Get a cat image."""
+        await interaction.response.send_message(
+            embed=Embed().set_image(url="https://cataas.com/cat")
+        )
+
+    @subcommand()
+    async def dog(self, interaction: Interaction):
+        """Get a dog image."""
+        await interaction.response.send_message(
+            embed=Embed().set_image(url="https://placedog.net/500?random")
+        )
+
+    @subcommand(name="any")
+    async def any_(self, interaction: Interaction):
+        """Get any random image."""
+        await interaction.response.send_message(
+            embed=Embed().set_image(url="https://picsum.photos/600")
+        )
+
+    @subcommand()
+    async def upload(self, interaction: Interaction, image: Attachment):
+        """Upload a new cute image."""
+        print(f"Uploading {image.proxy_url!r}...")
+        await interaction.response.send_message("All done!")
+
+
+@client.group
+class Admin(CommandGroup):
+    """Admin-only commands."""
+
+    class Roles(CommandSubGroup):
+        """Commands to manage roles."""
+
+        @subcommand(name="del")
+        async def del_(self, interaction: Interaction, role: Role):
+            """Delete a role.
+
+            :param role: The role to delete.
+            """
+            await role.delete()
+            await interaction.response.send_message("Deleted the role.", ephemeral=True)
+
+
+@client.command()
+async def ban(interaction: Interaction, user: Member):
+    """Ban a user.
+
+    :param user: The user to ban.
+    """
+    await user.ban()
+    await interaction.response.send_message("Banned the user.", ephemeral=True)
+
+
+class RPSChoices(Choices):
+    rock = "Rock"
+    paper = "Paper"
+    scissors = "Scissors"
+    gun = "Gun"
+
+
+@client.command()
+async def rps(interaction: Interaction, choice: RPSChoices):
+    """Play rock, paper, scissors.
+
+    :param choice: Your choice.
+    """
+    if choice == RPSChoices.gun:
+        await interaction.response.send_message("That's cheating!")
+    else:
+        await interaction.response.send_message(f"You picked {choice.name}.")
+
+
+client.run(TOKEN)
+```
+
+## Development
+
+As well as Python 3.9+, this project requires Poetry for development.
+[Click this link for installation instructions](https://python-poetry.org/docs/master/#installation),
+or:
+
+- #### \*nix (Linux/MacOS)
+
+  `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python -`
+
+- #### Windows Powershell
+
+  `(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py -UseBasicParsing).Content | python -`
+
+Once you have Poetry installed:
 
-packages = \
-['dslash']
+1. **Create a virtual environment:** `poetry shell`
+2. **Install dependencies:** `poetry install`
 
-package_data = \
-{'': ['*']}
+The following commands are then available:
 
-install_requires = \
-['docstring-parser>=0.12,<0.13', 'nextcord>=2.0.0-alpha.3,<3.0.0']
-
-setup_kwargs = {
-    'name': 'dslash',
-    'version': '0.6.3',
-    'description': 'A library which supplements Nextcord by adding support for slash commands.',
-    'long_description': '# DSlash\n\n![Version: 0.6.3](https://img.shields.io/badge/Version-0.6.3-red?style=flat-square)\n[![Code Style: black](https://img.shields.io/badge/Code%20Style-black-black?style=flat-square)](https://github.com/psf/black)\n[![License: MIT](https://img.shields.io/badge/License-MIT-orange?style=flat-square)](./LICENSE)\n[![PyPI: dslash](https://img.shields.io/badge/PyPI-dslash-green?style=flat-square)](https://pypi.org/project/dslash)\n![Python: ^3.9](https://img.shields.io/badge/python-%5E3.9-blue?style=flat-square)\n\n> **THIS PROJECT IS NO LONGER MAINTAINED**\n>\n> Danny has returned from a break, and [Discord.py](https://github.com/rapptz/discord.py)\n> is now being maintained again, with support for slash commands. Nextcord also\n> now has built-in support for slash commands. For new projects, you should use\n> one of these options (or another).\n>\n> Dslash will continue to receive minimal updates to keep it working, at least\n> for the near future, but it will not receive support for new features.\n>\n> One change Discord has made since this library stopped being maintained was\n> to remove support for bots configuring permissions for their own commands. In\n> order to avoid breaking bots, Dslash still allows permissions to be\n> configured as before, but will now ignore them. The `allow_roles`,\n> `allow_users`, `disallow_roles`, `disallow_users`, `global_permissions` and\n> `guild_permissions` wrappers, as well as the `default_permission` and\n> `permissions` parameters are all deprecated and should not be used.\n\nA library which supplements [Nextcord](https://github.com/nextcord/nextcord)\n(a fork of Discord.py) by adding support for slash commands.\n\nDocumentation is still a work in progress, and the library should currently be\nconsidered unstable.\n\nYou can install it using pip, eg. `pip install dslash`.\n\n## Example\n\n```python\nimport logging\nimport random\nimport typing\n\nfrom dslash import Choices, CommandClient, CommandGroup, CommandSubGroup, subcommand\nfrom nextcord import Embed, Interaction, Member, Role, Attachment\n\nGUILD_ID = ...\nTOKEN = ...\n\nlogging.basicConfig(level=logging.INFO)\nclient = CommandClient(guild_id=GUILD_ID)\n\n\n@client.event\nasync def on_ready():\n    print(f"Logged in as {client.user}.")\n\n\n@client.command()\nasync def roll(interaction: Interaction, sides: typing.Optional[int]):\n    """Roll a dice.\n\n    :param sides: How many sides (default 6).\n    """\n    value = random.randint(1, sides or 6)\n    await interaction.response.send_message(f"You got: {value}")\n\n\n@client.group\nclass Images(CommandGroup):\n    """Cute image commands."""\n\n    @subcommand()\n    async def cat(self, interaction: Interaction):\n        """Get a cat image."""\n        await interaction.response.send_message(\n            embed=Embed().set_image(url="https://cataas.com/cat")\n        )\n\n    @subcommand()\n    async def dog(self, interaction: Interaction):\n        """Get a dog image."""\n        await interaction.response.send_message(\n            embed=Embed().set_image(url="https://placedog.net/500?random")\n        )\n\n    @subcommand(name="any")\n    async def any_(self, interaction: Interaction):\n        """Get any random image."""\n        await interaction.response.send_message(\n            embed=Embed().set_image(url="https://picsum.photos/600")\n        )\n\n    @subcommand()\n    async def upload(self, interaction: Interaction, image: Attachment):\n        """Upload a new cute image."""\n        print(f"Uploading {image.proxy_url!r}...")\n        await interaction.response.send_message("All done!")\n\n\n@client.group\nclass Admin(CommandGroup):\n    """Admin-only commands."""\n\n    class Roles(CommandSubGroup):\n        """Commands to manage roles."""\n\n        @subcommand(name="del")\n        async def del_(self, interaction: Interaction, role: Role):\n            """Delete a role.\n\n            :param role: The role to delete.\n            """\n            await role.delete()\n            await interaction.response.send_message("Deleted the role.", ephemeral=True)\n\n\n@client.command()\nasync def ban(interaction: Interaction, user: Member):\n    """Ban a user.\n\n    :param user: The user to ban.\n    """\n    await user.ban()\n    await interaction.response.send_message("Banned the user.", ephemeral=True)\n\n\nclass RPSChoices(Choices):\n    rock = "Rock"\n    paper = "Paper"\n    scissors = "Scissors"\n    gun = "Gun"\n\n\n@client.command()\nasync def rps(interaction: Interaction, choice: RPSChoices):\n    """Play rock, paper, scissors.\n\n    :param choice: Your choice.\n    """\n    if choice == RPSChoices.gun:\n        await interaction.response.send_message("That\'s cheating!")\n    else:\n        await interaction.response.send_message(f"You picked {choice.name}.")\n\n\nclient.run(TOKEN)\n```\n\n## Development\n\nAs well as Python 3.9+, this project requires Poetry for development.\n[Click this link for installation instructions](https://python-poetry.org/docs/master/#installation),\nor:\n\n- #### \\*nix (Linux/MacOS)\n\n  `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python -`\n\n- #### Windows Powershell\n\n  `(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py -UseBasicParsing).Content | python -`\n\nOnce you have Poetry installed:\n\n1. **Create a virtual environment:** `poetry shell`\n2. **Install dependencies:** `poetry install`\n\nThe following commands are then available:\n\n- `poe format` - Run auto-formatting and linting.\n\nPrefix these with `poetry run` if outside of the Poetry shell.\n',
-    'author': 'Artemis',
-    'author_email': 'me@arty.li',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/artemis21/dslash',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+- `poe format` - Run auto-formatting and linting.
 
+Prefix these with `poetry run` if outside of the Poetry shell.
 
-setup(**setup_kwargs)
```

