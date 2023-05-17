# Comparing `tmp/iconoclast-2.0.1.tar.gz` & `tmp/iconoclast-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iconoclast-2.0.1.tar", max compression
+gzip compressed data, was "iconoclast-2.0.2.tar", max compression
```

## Comparing `iconoclast-2.0.1.tar` & `iconoclast-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1091 2023-05-11 17:01:03.168348 iconoclast-2.0.1/LICENSE.md
--rw-r--r--   0        0        0     1254 2023-05-11 17:01:03.168348 iconoclast-2.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/__init__.py
--rw-r--r--   0        0        0     3674 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/app.py
--rw-r--r--   0        0        0      247 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/context.py
--rw-r--r--   0        0        0      285 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/exceptions.py
--rw-r--r--   0        0        0       96 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/graphql/__init__.py
--rw-r--r--   0        0        0    12875 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/graphql/schema.py
--rw-r--r--   0        0        0      298 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/iconokit/iconokit/__init__.py
--rw-r--r--   0        0        0      209 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/iconokit/pyproject.toml
--rw-r--r--   0        0        0     1665 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/prompts.py
--rw-r--r--   0        0        0        0 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/plugins/__init__.py
--rw-r--r--   0        0        0      584 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/plugins/iconocards.py
--rw-r--r--   0        0        0     3203 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/plugins/iconoclast.py
--rw-r--r--   0        0        0     1907 2023-05-11 17:01:03.176348 iconoclast-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 iconoclast-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-17 01:54:42.807254 iconoclast-2.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1254 2023-05-17 01:54:42.807254 iconoclast-2.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/__init__.py
+-rw-r--r--   0        0        0     3876 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/app.py
+-rw-r--r--   0        0        0      247 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/context.py
+-rw-r--r--   0        0        0      285 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/exceptions.py
+-rw-r--r--   0        0        0       96 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/graphql/__init__.py
+-rw-r--r--   0        0        0    12875 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/graphql/schema.py
+-rw-r--r--   0        0        0      298 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/iconokit/iconokit/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/iconokit/pyproject.toml
+-rw-r--r--   0        0        0     1665 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/cli/prompts.py
+-rw-r--r--   0        0        0      189 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/plugins/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/plugins/iconocards.py
+-rw-r--r--   0        0        0     3403 2023-05-17 01:54:42.815254 iconoclast-2.0.2/iconoclast/plugins/iconoclast.py
+-rw-r--r--   0        0        0     1891 2023-05-17 01:54:42.815254 iconoclast-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 iconoclast-2.0.2/PKG-INFO
```

### Comparing `iconoclast-2.0.1/LICENSE.md` & `iconoclast-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.1/README.md` & `iconoclast-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.1/iconoclast/cli/app.py` & `iconoclast-2.0.2/iconoclast/cli/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 
     api_url = URL("https://api.fontawesome.com")
 
     resp = requests.post(
         api_url / "token",
         headers={"Authorization": f"Bearer {kit_config.token}"},
     )
+
+    if resp.status_code == 403:
+        raise Iconoquit("Your Font Awesome API token is invalid.")
+    elif resp.status_code != 200:
+        raise Iconoquit("Couldn't communicate with Font Awesome.")
+
     access_token = resp.json()["access_token"]
 
     endpoint = RequestsEndpoint(
         str(api_url), base_headers={"Authorization": f"Bearer {access_token}"}
     )
 
     op = Operation(schema.RootQueryType)
```

### Comparing `iconoclast-2.0.1/iconoclast/cli/graphql/schema.py` & `iconoclast-2.0.2/iconoclast/cli/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.1/iconoclast/cli/prompts.py` & `iconoclast-2.0.2/iconoclast/cli/prompts.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.1/iconoclast/plugins/iconoclast.py` & `iconoclast-2.0.2/iconoclast/plugins/iconoclast.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import inspect
+import logging
 import os
 import sys
 from typing import Optional, Tuple
 
 from dict_deep import deep_get, deep_set
+from mkdocs.commands.build import DuplicateFilter
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config, ConfigErrors, ConfigWarnings
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from path import Path
-from rich import print
-from rich.panel import Panel
+
+from iconoclast.plugins import new_console
 
 symlink = Path(__file__).parent / ".overrides" / ".icons" / "fontawesome"
 
 
 class IconokitConfig(Config):
     name = c.Type(str, default="")
     token = c.Type(str, default=os.getenv("FONTAWESOME_API_TOKEN") or "")
@@ -43,24 +45,22 @@
 
         (get_package_path() / "svgs").symlink(symlink)
 
         if self.config.kit.enabled:
             try:
                 import iconokit
             except ImportError:
-                print(
-                    Panel(
-                        "You haven't installed a Kit. Run [cyan]iconoclast install[/cyan], then try again.",
-                        title="Iconoclast Error",
-                        title_align="left",
-                        border_style="red",
+                with new_console() as console:
+                    console.print(
+                        "You haven't installed a Font Awesome kit. "
+                        "Run [cyan]iconoclast install[/] or change your settings "
+                        "for the [magenta]iconoclast[/] plugin.",
                     )
-                )
-
-                sys.exit(1)
+                    log.error(console.export_text(styles=True))
+                    sys.exit(1)
             else:
                 icon_dirs.append(iconokit.icons())
                 css = iconokit.kit("css")
 
         key = "mdx_configs|pymdownx.emoji|options|custom_icons"
 
         for icon_dir in icon_dirs:
@@ -87,21 +87,21 @@
             (fa_path / "webfonts").copytree(site_dir / "webfonts")
 
 
 def get_package_path() -> Path:
     try:
         import fontawesomepro
     except ImportError:
-        print(
-            Panel(
-                "Font Awesome Pro is not installed.",
-                title="Iconoclast Error",
-                title_align="left",
-                border_style="red",
+        with new_console() as console:
+            console.print(
+                "Font Awesome Pro is not installed. Install it or remove the [magenta]iconoclast[/] plugin."
             )
-        )
-
-        sys.exit(1)
+            log.error(console.export_text(styles=True))
+            sys.exit(1)
     else:
         return (
             Path(inspect.getfile(fontawesomepro)).parent / "static" / "fontawesomepro"
         )
+
+
+log = logging.getLogger("mkdocs")
+log.addFilter(DuplicateFilter())
```

### Comparing `iconoclast-2.0.1/pyproject.toml` & `iconoclast-2.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "iconoclast"
-version = "2.0.1"
+version = "2.0.2"
 description = "Font Awesome Pro integration for Material for MkDocs"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 decorator = "^5.1.1"
 dict-deep = "^4.1.2"
 halo = "^0.0.31"
+importlib-metadata = "^6.6.0"
 mkdocs = "^1.4"
 path = "^16.6.0"
+semver = "^3.0.0"
 sgqlc = "^16.1"
 yarl = "^1.9.2"
 typer = { extras = ["all"], version = "^0.9.0" }
 
 [tool.poetry.group.dev.dependencies]
 doppler-env = "^0.3.1"
 mkdocs-material = "^9.1.8"
 rich-tracebacks = "^1.2.1"
-fontawesomepro = { version = "^6.4.0", source = "fontawesome" }
 
 [tool.poetry.group.docs.dependencies]
 cairosvg = "^2.7.0"
 pillow = "^9.5.0"
 poethepoet = "^0.19.0"
 fontawesomepro = { version = "^6.4.0", source = "fontawesome" }
 mkdocs-material = { git = "https://github.com/squidfunk/mkdocs-material-insiders" }
```

### Comparing `iconoclast-2.0.1/PKG-INFO` & `iconoclast-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconoclast
-Version: 2.0.1
+Version: 2.0.2
 Summary: Font Awesome Pro integration for Material for MkDocs
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
+Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
 Requires-Dist: mkdocs (>=1.4,<2.0)
 Requires-Dist: path (>=16.6.0,<17.0.0)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Iconoclast
```

