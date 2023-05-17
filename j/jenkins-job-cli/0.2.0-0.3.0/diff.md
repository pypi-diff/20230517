# Comparing `tmp/jenkins-job-cli-0.2.0.tar.gz` & `tmp/jenkins_job_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins-job-cli-0.2.0.tar", max compression
+gzip compressed data, was "jenkins_job_cli-0.3.0.tar", max compression
```

## Comparing `jenkins-job-cli-0.2.0.tar` & `jenkins_job_cli-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1077 2022-02-23 22:48:39.885324 jenkins-job-cli-0.2.0/LICENSE
--rw-r--r--   0        0        0      672 2022-07-17 14:33:58.821978 jenkins-job-cli-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-03-04 11:32:10.563063 jenkins-job-cli-0.2.0/jcli/__init__.py
--rwxr-xr-x   0        0        0     9109 2022-07-17 14:09:40.725356 jenkins-job-cli-0.2.0/jcli/cli.py
--rw-r--r--   0        0        0     2299 2022-03-05 15:18:08.181212 jenkins-job-cli-0.2.0/jcli/config.py
--rw-r--r--   0        0        0       51 2022-07-17 14:11:15.275774 jenkins-job-cli-0.2.0/jcli/version.py
--rw-r--r--   0        0        0      656 2022-07-17 14:22:23.722128 jenkins-job-cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1550 2022-07-17 14:37:51.420199 jenkins-job-cli-0.2.0/setup.py
--rw-r--r--   0        0        0     1465 2022-07-17 14:37:51.420379 jenkins-job-cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0      643 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/jcli/__init__.py
+-rwxr-xr-x   0        0        0    13225 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/jcli/cli.py
+-rw-r--r--   0        0        0     2299 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/jcli/config.py
+-rw-r--r--   0        0        0       75 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/jcli/version.py
+-rw-r--r--   0        0        0      665 2023-05-17 21:49:35.628116 jenkins_job_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 jenkins_job_cli-0.3.0/PKG-INFO
```

### Comparing `jenkins-job-cli-0.2.0/LICENSE` & `jenkins_job_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins-job-cli-0.2.0/jcli/cli.py` & `jenkins_job_cli-0.3.0/jcli/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+from sys import exit
+from time import sleep
+from typing import Optional
 
 import click
-from api4jenkins import Jenkins, exceptions
+import requests as r
+from api4jenkins import exceptions
+from api4jenkins import Jenkins
+from rich import print as pp
 from rich.console import Console
+from rich.markup import escape
+from rich.prompt import Confirm
+from rich.prompt import Prompt
 from rich.table import Table
-from rich.prompt import Prompt, Confirm
-from rich import print as pp
-from time import sleep
-from sys import exit
-import requests as r
 
-from .config import load_and_validate, setup_config
+from .config import load_and_validate
+from .config import setup_config
 from .version import __version__
 
 console = Console()
 error = Console(stderr=True, style="bold red")
 
 
 def init_server_connection(url, user, password):
@@ -44,36 +49,37 @@
         table.add_row("version", server.version)
         for i in infos:
             table.add_row(i, str(server.api_json()[i]))
         console.print(table)
     else:
         pp(server.version)
 
+
 def list_plugins(f: str):
     """
     Grab and list all the plugins
     """
     if f == "table":
         table = Table(show_header=True, box=None)
         table.add_column("NAME")
         table.add_column("VERSION")
         table.add_column("ENABLED")
-        for p in server.plugins.api_json(depth=1)['plugins']:
-            if p['enabled']:
+        for p in server.plugins.api_json(depth=1)["plugins"]:
+            if p["enabled"]:
                 enabled = ":white_check_mark:"
             else:
                 enabled = ":x:"
-            table.add_row(p['longName'], p['version'], enabled)
+            table.add_row(p["longName"], p["version"], enabled)
         console.print(table)
         return
     elif f == "yaml":
         print("---")
         print("plugins:")
-        for p in server.plugins.api_json(depth=1)['plugins']:
-            if p['enabled']:
+        for p in server.plugins.api_json(depth=1)["plugins"]:
+            if p["enabled"]:
                 print(f"- name: {p['shortName']}")
                 print(f"  version: {p['version']}")
         print("...")
         return
 
 
 def plugins_to_be_updated():
@@ -81,29 +87,99 @@
     Grab and list only the plugins that needs to be updated
     """
     table = Table(show_header=True, box=None)
     table.add_column("SHORT NAME", justify="left", no_wrap=True)
     table.add_column("CURRENT VERSION", style="dim")
     table.add_column("LATEST", style="green")
     with console.status("[bold green]Checking last plugins version, please wait...") as status:
-        #status.update(f"[green]Forcing plugins sync with update center, processing..")
-        #server.plugins.check_updates_server()
-        for p in server.plugins.api_json(depth=1)['plugins']:
-            if p['hasUpdate']:
+        # status.update(f"[green]Forcing plugins sync with update center, processing..")
+        # server.plugins.check_updates_server()
+        for p in server.plugins.api_json(depth=1)["plugins"]:
+            if p["hasUpdate"]:
                 status.update(f"[green]Plugins update found: [bold green]{p['longName']}[/bold green], processing..")
                 u = f"https://plugins.jenkins.io/api/plugin/{p['shortName']}"
                 ru = r.get(u)
                 rj = ru.json()
                 if ru.status_code == 200:
                     outdated = rj["version"]
-                    table.add_row(p['shortName'], p['version'], outdated)
+                    table.add_row(p["shortName"], p["version"], outdated)
         status.update("[bold green]Done!")
         console.print(table)
 
 
+def list_nodes():
+    """
+    Iterate over nodes and print list of nodes with status
+    """
+    table = Table(show_header=True, box=None)
+    table.add_column("NAME")
+    table.add_column("DESCRIPTION", style="dim")
+    table.add_column("STATUS")
+    table.add_column("MEMORY (mb)", style="dim")
+    table.add_column("DISK (gb)", style="dim")
+    table.add_column("ARCH", style="dim")
+    with console.status("[bold green]Scraping all nodes, please wait...") as status:
+        for node in server.nodes:
+            n = node.api_json()
+            status.update(f"[green]Node found: [bold green]{node.name}[/bold green], processing..")
+            _nname = n["displayName"]
+            _ndesc = n["description"]
+            if n["offline"] == True:
+                _nstatus = ":x:"
+            else:
+                _nstatus = ":white_check_mark:"
+                _ntotalmemory = (
+                    int(n["monitorData"]["hudson.node_monitors.SwapSpaceMonitor"]["totalPhysicalMemory"]) / 1024 / 1024
+                )
+                _naivalablememory = (
+                    int(n["monitorData"]["hudson.node_monitors.SwapSpaceMonitor"]["availablePhysicalMemory"])
+                    / 1024
+                    / 1024
+                )
+                _nmemory = f"{int(_ntotalmemory)-int(_naivalablememory)}/{int(_ntotalmemory)}"
+                _ndisk = (
+                    f"{round((n['monitorData']['hudson.node_monitors.DiskSpaceMonitor']['size']/1024/1024/1024), 2)}"
+                )
+                _narch = n["monitorData"]["hudson.node_monitors.ArchitectureMonitor"]
+            table.add_row(_nname, _ndesc, _nstatus, _nmemory, _ndisk, _narch)
+        status.update("[bold green]Done!")
+        console.print(table)
+
+
+def enable_disable_node(node: str, action: str, motivation: Optional[str]):
+    """
+    Enable or disable a node
+    """
+    n = server.nodes.get(node)
+    if n.exists():
+        if action == "enable":
+            n.enable()
+            console.print(f"[bold green]Node {node} enabled!")
+        elif action == "disable":
+            n.disable()
+            console.print(f"[bold green]Node {node} disabled!")
+    else:
+        console.print(f"[bold red]Node {node} not found!")
+        return
+
+
+def node_run_job(node: str):
+    """
+    Ask the command and run a job on a specific node
+    """
+    n = server.nodes.get(node)
+    if n == None:
+        console.print(f"[bold red]Node {node} not found!")
+        return
+    c = Prompt.ask(f"[green] Which command do you want to run?")
+    console.print(f"Running command {c} on node [green]{node}[/green], please wait...")
+    nl = "\n"
+    console.print(f"{nl}{escape(n.run_script(c))}{nl}")
+
+
 def job_health_check(value: int):
     """
     Check health by value according to:
     https://github.com/jenkinsci/jenkins/blob/master/core/src/main/java/hudson/model/HealthReport.java
     and output the corresponding icon
     """
     if value >= 80:
@@ -131,17 +207,21 @@
             jtypes = ["hudson.model.FreeStyleProject", "org.jenkinsci.plugins.workflow.job.WorkflowJob"]
             if job._class in jtypes:
                 status.update(f"[green]Job found: [bold green]{job.display_name}[/bold green], processing..")
                 _jname = job.display_name
                 _jfulln = str(job.api_json()["fullName"])
                 _jdir = _jfulln.split("/")[0] if "/" in _jfulln else ""
                 _jdesc = job.description
-                _jlastb = str(job.api_json()["lastBuild"]["number"])
-                _jhealth = job.api_json()["healthReport"][0]["score"]
-                table.add_row(_jname, _jdesc, _jdir, _jlastb, job_health_check(_jhealth))
+                if job.api_json()["lastBuild"]:
+                    _jlastb = str(job.api_json()["lastBuild"]["number"])
+                    _jhealth = job_health_check(job.api_json()["healthReport"][0]["score"])
+                else:
+                    _jlastb = "-"
+                    _jhealth = "-"
+                table.add_row(_jname, _jdesc, _jdir, _jlastb, _jhealth)
         status.update("[bold green]Done!")
         console.print(table)
 
 
 def job_exist(name: str) -> bool:
     """
     Check if job exist
@@ -237,32 +317,84 @@
 
 @jenkins.command(help="Get generic info", name="info")
 def info():
     cfg = load_and_validate()
     init_server_connection(cfg["server"], cfg["user"], cfg["password"])
     get_server_info(a=True)
 
+
+@main.group(help="Nodes management")
+@click.pass_context
+def nodes(ctx):
+    pass
+
+
+@nodes.command(help="List nodes", name="ls")
+def listnodes():
+    cfg = load_and_validate()
+    init_server_connection(cfg["server"], cfg["user"], cfg["password"])
+    list_nodes()
+
+
+@nodes.command(help="Enable node", name="enable")
+@click.argument("node")
+def enablenode(node, motivation: Optional[str] = None):
+    cfg = load_and_validate()
+    init_server_connection(cfg["server"], cfg["user"], cfg["password"])
+    enable_disable_node(node, "enable", motivation)
+
+
+@nodes.command(help="Disable node", name="disable")
+@click.argument("node")
+@click.argument("motivation", required=False)
+def disablenode(node, motivation: Optional[str] = None):
+    cfg = load_and_validate()
+    init_server_connection(cfg["server"], cfg["user"], cfg["password"])
+    enable_disable_node(node, "disable", motivation)
+
+
+@nodes.command(help="Run a command", name="run")
+@click.argument("node")
+def runcommand(node):
+    cfg = load_and_validate()
+    init_server_connection(cfg["server"], cfg["user"], cfg["password"])
+    node_run_job(node)
+
+
 @main.group(help="Plugins management")
 @click.pass_context
 def plugins(ctx):
     pass
 
+
 @plugins.command(help="List plugins", name="ls")
-@click.option('--format', "-f", default="table", required=False, help="Output format", type=click.Choice(["table", "yaml"], case_sensitive=False, ))
+@click.option(
+    "--format",
+    "-f",
+    default="table",
+    required=False,
+    help="Output format",
+    type=click.Choice(
+        ["table", "yaml"],
+        case_sensitive=False,
+    ),
+)
 def listplugin(format):
     cfg = load_and_validate()
     init_server_connection(cfg["server"], cfg["user"], cfg["password"])
     list_plugins(f=format)
 
+
 @plugins.command(help="List only outdated plugins and latest version", name="check")
 def listpluginupdate():
     cfg = load_and_validate()
     init_server_connection(cfg["server"], cfg["user"], cfg["password"])
     plugins_to_be_updated()
 
+
 @main.group(help="List and execute jobs")
 @click.pass_context
 def jobs(ctx):
     pass
 
 
 @jobs.command(help="Run jenkins jobs", name="run")
```

### Comparing `jenkins-job-cli-0.2.0/jcli/config.py` & `jenkins_job_cli-0.3.0/jcli/config.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # adjusted from https://raw.githubusercontent.com/mbovo/pdh/main/src/pdh/config.py
-
-import yaml
 import os
 import sys
 from typing import Any
+
+import yaml
+from appdirs import AppDirs
 from rich import print
 from rich.prompt import Prompt
-from appdirs import AppDirs
 
 _APPNAME = "jcli"
 _AUTHOR = "brokenpip3"
 dirs = AppDirs(_APPNAME, _AUTHOR)
 
 REQUIRED_KEYS = ["server", "user", "password"]
```

### Comparing `jenkins-job-cli-0.2.0/pyproject.toml` & `jenkins_job_cli-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "jenkins-job-cli"
-version = "0.2.0"
-description = "Jcli: list, run, and check jenkins jobs"
+version = "0.3.0"
+description = "Jcli: Alternative Jenkins CLI written in Python"
 authors = ["Brokenpip3 <brokenpip3@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/brokenpip3/jcli"
 readme = "README.md"
 packages = [
     {include = "jcli"}
 ]
 
 [tool.poetry.scripts]
 jcli = "jcli.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 api4jenkins = "^1.9"
-rich = "^12.0.0"
+rich = ">=12,<14"
 click = "^8.0.4"
 appdirs = "^1.4.4"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
-mock = "^4.0.3"
-pytest = "^7.1.0"
+mock = "^5.0.2"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `jenkins-job-cli-0.2.0/PKG-INFO` & `jenkins_job_cli-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: jenkins-job-cli
-Version: 0.2.0
-Summary: Jcli: list, run, and check jenkins jobs
+Version: 0.3.0
+Summary: Jcli: Alternative Jenkins CLI written in Python
 Home-page: https://github.com/brokenpip3/jcli
 License: MIT
 Author: Brokenpip3
 Author-email: brokenpip3@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: api4jenkins (>=1.9,<2.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.4,<9.0.0)
-Requires-Dist: rich (>=12.0.0,<13.0.0)
+Requires-Dist: rich (>=12,<14)
 Project-URL: Repository, https://github.com/brokenpip3/jcli
 Description-Content-Type: text/markdown
 
 # Jcli
 
 
 Small cli to list, run, and check jenkins jobs
@@ -32,19 +33,24 @@
 
 `pip install jenkins-job-cli`
 
 Archlinux users: you can find the pkgbuild [here](https://aur.archlinux.org/packages/jcli)
 
 ## Usage
 
-* `config`: setup the `jcli` configuration
-
-* `jobs`:
-  * `list`: list all jenkins jobs (default deep = 1)
-  * `run`: run a specific jenkins job
+```
+Usage: jcli [OPTIONS] COMMAND [ARGS]...
 
-* `jenkins`: show jenkins server info like version (`version`) and security options (`info`)
+  jcli - Jenkins job cli
 
-* `plugins`:
-  * `ls`: List plugins name, status and version
-  * `check`:  List only outdated plugins and latest version
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  config   Create jcli config
+  jenkins  Get Jenkins server info
+  jobs     List and execute jobs
+  nodes    Nodes management
+  plugins  Plugins management
+```
```

