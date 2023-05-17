# Comparing `tmp/mozci-2.2.2.tar.gz` & `tmp/mozci-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozci-2.2.2.tar", max compression
+gzip compressed data, was "mozci-2.3.0.tar", max compression
```

## Comparing `mozci-2.2.2.tar` & `mozci-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    16725 2019-12-03 23:09:31.101080 mozci-2.2.2/LICENSE
--rw-r--r--   0        0        0      133 2020-09-01 14:24:53.684584 mozci-2.2.2/mozci/__init__.py
--rw-r--r--   0        0        0     6852 2022-06-24 14:12:09.370533 mozci-2.2.2/mozci/configuration.py
--rw-r--r--   0        0        0      609 2022-06-24 14:12:09.370533 mozci-2.2.2/mozci/console/application.py
--rw-r--r--   0        0        0    12689 2022-06-24 14:12:09.374533 mozci-2.2.2/mozci/console/commands/batch_execution.py
--rw-r--r--   0        0        0     9655 2022-10-17 16:08:29.587934 mozci-2.2.2/mozci/console/commands/check_backfills.py
--rw-r--r--   0        0        0     5001 2022-03-04 16:49:13.949218 mozci-2.2.2/mozci/console/commands/decision.py
--rw-r--r--   0        0        0    52940 2022-07-15 10:22:42.449111 mozci-2.2.2/mozci/console/commands/push.py
--rw-r--r--   0        0        0      172 2020-09-01 14:24:53.684584 mozci-2.2.2/mozci/data/__init__.py
--rw-r--r--   0        0        0     3470 2022-03-25 23:42:30.024385 mozci-2.2.2/mozci/data/base.py
--rw-r--r--   0        0        0     7042 2022-03-26 00:14:58.682443 mozci-2.2.2/mozci/data/contract.py
--rw-r--r--   0        0        0        0 2020-09-01 14:24:53.684584 mozci-2.2.2/mozci/data/sources/__init__.py
--rw-r--r--   0        0        0     4066 2022-03-22 13:19:27.482042 mozci-2.2.2/mozci/data/sources/artifact/__init__.py
--rw-r--r--   0        0        0     1884 2022-01-13 21:51:04.207686 mozci-2.2.2/mozci/data/sources/bugbug/__init__.py
--rw-r--r--   0        0        0      652 2022-01-13 21:50:58.067723 mozci-2.2.2/mozci/data/sources/hgmo/__init__.py
--rw-r--r--   0        0        0     6213 2022-04-28 11:16:06.676120 mozci-2.2.2/mozci/data/sources/taskcluster/__init__.py
--rw-r--r--   0        0        0     7624 2022-03-25 23:54:19.023597 mozci-2.2.2/mozci/data/sources/treeherder/__init__.py
--rw-r--r--   0        0        0     3135 2022-01-13 21:50:58.071723 mozci-2.2.2/mozci/errors.py
--rw-r--r--   0        0        0    60180 2022-10-17 22:22:09.820387 mozci-2.2.2/mozci/push.py
--rw-r--r--   0        0        0    21211 2022-07-19 09:22:55.113547 mozci-2.2.2/mozci/task.py
--rw-r--r--   0        0        0        0 2019-12-13 09:52:36.469747 mozci-2.2.2/mozci/util/__init__.py
--rw-r--r--   0        0        0     7787 2022-01-13 21:51:14.823622 mozci-2.2.2/mozci/util/cache_stores.py
--rw-r--r--   0        0        0      209 2022-06-24 14:12:09.378533 mozci-2.2.2/mozci/util/defs.py
--rw-r--r--   0        0        0     7168 2022-06-24 14:12:09.378533 mozci-2.2.2/mozci/util/hgmo.py
--rw-r--r--   0        0        0     1093 2020-09-01 14:24:53.692581 mozci-2.2.2/mozci/util/logging.py
--rw-r--r--   0        0        0     1585 2022-01-13 21:50:44.699803 mozci-2.2.2/mozci/util/memoize.py
--rw-r--r--   0        0        0     1025 2022-01-13 21:50:44.699803 mozci-2.2.2/mozci/util/req.py
--rw-r--r--   0        0        0     7139 2022-05-10 10:03:58.721143 mozci-2.2.2/mozci/util/taskcluster.py
--rw-r--r--   0        0        0     1087 2020-02-26 16:06:17.151514 mozci-2.2.2/mozci/util/yaml.py
--rw-r--r--   0        0        0     1169 2022-10-17 22:21:01.244590 mozci-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     1588 2022-10-17 22:23:00.107233 mozci-2.2.2/setup.py
--rw-r--r--   0        0        0     1423 2022-10-17 22:23:00.107473 mozci-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2019-12-03 23:09:31.000000 mozci-2.3.0/LICENSE
+-rw-r--r--   0        0        0      133 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/__init__.py
+-rw-r--r--   0        0        0     6851 2023-04-11 15:35:25.841411 mozci-2.3.0/mozci/configuration.py
+-rw-r--r--   0        0        0      621 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/application.py
+-rw-r--r--   0        0        0    12771 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/commands/batch_execution.py
+-rw-r--r--   0        0        0     9702 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/commands/check_backfills.py
+-rw-r--r--   0        0        0     5040 2023-05-05 21:03:08.495205 mozci-2.3.0/mozci/console/commands/decision.py
+-rw-r--r--   0        0        0    53038 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/console/commands/push.py
+-rw-r--r--   0        0        0      172 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/data/__init__.py
+-rw-r--r--   0        0        0     3470 2022-03-25 23:42:30.000000 mozci-2.3.0/mozci/data/base.py
+-rw-r--r--   0        0        0     7104 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/data/contract.py
+-rw-r--r--   0        0        0        0 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/data/sources/__init__.py
+-rw-r--r--   0        0        0     4065 2023-04-11 15:35:25.751411 mozci-2.3.0/mozci/data/sources/artifact/__init__.py
+-rw-r--r--   0        0        0     1884 2022-01-13 21:51:04.000000 mozci-2.3.0/mozci/data/sources/bugbug/__init__.py
+-rw-r--r--   0        0        0      652 2022-01-13 21:50:58.000000 mozci-2.3.0/mozci/data/sources/hgmo/__init__.py
+-rw-r--r--   0        0        0     6213 2022-04-28 11:16:06.000000 mozci-2.3.0/mozci/data/sources/taskcluster/__init__.py
+-rw-r--r--   0        0        0     7624 2022-03-25 23:54:19.000000 mozci-2.3.0/mozci/data/sources/treeherder/__init__.py
+-rw-r--r--   0        0        0     3135 2022-01-13 21:50:58.000000 mozci-2.3.0/mozci/errors.py
+-rw-r--r--   0        0        0    60180 2023-04-12 14:41:42.404758 mozci-2.3.0/mozci/push.py
+-rw-r--r--   0        0        0    21263 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/task.py
+-rw-r--r--   0        0        0        0 2019-12-13 09:52:36.000000 mozci-2.3.0/mozci/util/__init__.py
+-rw-r--r--   0        0        0     7787 2022-01-13 21:51:14.000000 mozci-2.3.0/mozci/util/cache_stores.py
+-rw-r--r--   0        0        0      239 2023-05-17 18:14:56.605802 mozci-2.3.0/mozci/util/defs.py
+-rw-r--r--   0        0        0     7168 2022-06-24 14:12:09.000000 mozci-2.3.0/mozci/util/hgmo.py
+-rw-r--r--   0        0        0     1093 2020-09-01 14:24:53.000000 mozci-2.3.0/mozci/util/logging.py
+-rw-r--r--   0        0        0     1585 2022-01-13 21:50:44.000000 mozci-2.3.0/mozci/util/memoize.py
+-rw-r--r--   0        0        0     1025 2022-01-13 21:50:44.000000 mozci-2.3.0/mozci/util/req.py
+-rw-r--r--   0        0        0     7139 2022-05-10 10:03:58.000000 mozci-2.3.0/mozci/util/taskcluster.py
+-rw-r--r--   0        0        0     1087 2020-02-26 16:06:17.000000 mozci-2.3.0/mozci/util/yaml.py
+-rw-r--r--   0        0        0     1168 2023-05-17 18:20:46.945702 mozci-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 mozci-2.3.0/PKG-INFO
```

### Comparing `mozci-2.2.2/LICENSE` & `mozci-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/configuration.py` & `mozci-2.3.0/mozci/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     are appended to lists in dest.
 
     Args:
         source (dict): to copy from
         dest (dict): to copy to (modified in place)
     """
     for key, value in source.items():
-
         if key not in dest:
             dest[key] = value
             continue
 
         # Merge dict
         if isinstance(value, dict) and isinstance(dest[key], dict):
             merge_to(value, dest[key])
```

### Comparing `mozci-2.2.2/mozci/console/application.py` & `mozci-2.3.0/mozci/console/application.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
-from cleo import Application
+from cleo.application import Application
 
 from mozci.console.commands.batch_execution import BatchExecutionCommands
 from mozci.console.commands.check_backfills import CheckBackfillsCommand
 from mozci.console.commands.decision import DecisionCommand
 from mozci.console.commands.push import PushCommands
```

### Comparing `mozci-2.2.2/mozci/console/commands/batch_execution.py` & `mozci-2.3.0/mozci/console/commands/batch_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import itertools
 import json
 import os
 import time
 import uuid
 from multiprocessing import Pool
 
-from cleo import Command
+from cleo.commands.command import Command
 from loguru import logger
 
 from mozci.console.commands.push import (
     parse_and_log_details,
     prepare_for_analysis,
     retrieve_sheriff_intermittents,
     retrieve_sheriff_reals,
@@ -121,14 +121,16 @@
     """
     Run the classification algorithm with various parameters combinations for all submitted pushes within the last 30 days
 
     classify
         {--workers= : Number of workers to use in order to parallelize the executions.}
     """
 
+    name = "batch-classification"
+
     csv_header = (
         ["run_uuid", "push_uuid"]
         + PARAMETERS_NAMES
         + ["classification", "time_spent", "now"]
     )
 
     def handle(self) -> None:
@@ -358,14 +360,16 @@
 class BatchExecutionCommands(Command):
     """
     Contains commands that operate on lots of pushes using lots of classification algorithm configurations.
 
     batch-execution
     """
 
+    name = "batch-execution"
+
     commands = [
         BatchClassificationCommand(),
         BatchEvaluationCommand(),
     ]
 
     def handle(self):
         return self.call("help", self._config.name)
```

### Comparing `mozci-2.2.2/mozci/console/commands/check_backfills.py` & `mozci-2.3.0/mozci/console/commands/check_backfills.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 from collections import namedtuple
 from itertools import groupby
 from typing import Any, Dict
 
 import requests
-from cleo import Command
+from cleo.commands.command import Command
 from loguru import logger
 
 from mozci import config
 from mozci.push import make_push_objects
 from mozci.util.defs import TASK_FINAL_STATES
 from mozci.util.taskcluster import (
     COMMUNITY_TASKCLUSTER_ROOT_URL,
@@ -43,14 +43,16 @@
       4. Group them by backfill groups
       => For each backfill group on the Push:
       5. Check if all backfill tasks in this group are completed
       6. If so (and if the notification wasn't already sent), send a notification on Matrix alerting that this backfill group is completed
       7. Add the current task in a dedicated index to avoid sending multiple times the same notification
     """
 
+    name = "check-backfills"
+
     def handle(self) -> None:
         branch = self.option("branch")
         environment = self.option("environment")
         matrix_room = config.get("matrix-room-id")
         current_task_id = os.environ.get("TASK_ID")
 
         try:
```

### Comparing `mozci-2.2.2/mozci/console/commands/decision.py` & `mozci-2.3.0/mozci/console/commands/decision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import os
 from datetime import datetime
 
 import taskcluster
-from cleo import Command
+from cleo.commands.command import Command
 
 from mozci.push import Push, make_push_objects
 from mozci.util.memoize import memoized_property
 from mozci.util.taskcluster import get_taskcluster_options
 
 
 class DecisionCommand(Command):
@@ -18,28 +18,29 @@
     decision
         {branch=autoland : Branch the push belongs to (e.g autoland, try, etc).}
         {--nb-pushes=15 : Do not create tasks on taskcluster, simply output actions.}
         {--dry-run : Do not create tasks on taskcluster, simply output actions.}
         {--environment=testing : Environment in which the analysis is running (testing, production, ...)}
     """
 
+    name = "decision"
+
     def handle(self):
         branch = self.argument("branch")
         dry_run = self.option("dry-run")
         nb_pushes = int(self.option("nb-pushes"))
 
         self.queue = (
             not dry_run and taskcluster.Queue(get_taskcluster_options()) or None
         )
 
         self.line(f"Process pushes from {branch}")
 
         # List most recent pushes
         for push in make_push_objects(nb=nb_pushes, branch=branch):
-
             if dry_run:
                 self.line(f"Would classify {push.branch}@{push.rev}")
                 continue
 
             # Create a child task to classify that push
             task_id = self.create_task(push)
             self.line(f"<info>Created task {task_id}</info>")
```

### Comparing `mozci-2.2.2/mozci/console/commands/push.py` & `mozci-2.3.0/mozci/console/commands/push.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import traceback
 from inspect import signature
 from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import urlencode
 
 import arrow
 import taskcluster
-from cleo import Command
-from clikit.api.args.exceptions import NoSuchOptionException
+from cleo.commands.command import Command
+from cleo.exceptions import CleoNoSuchOptionError
 from loguru import logger
 from tabulate import tabulate
 from taskcluster.exceptions import TaskclusterRestFailure
 
 from mozci import config
 from mozci.errors import PushNotFound, SourcesNotFound, TaskNotFound
 from mozci.push import (
@@ -163,15 +163,15 @@
     classify_parameters = {}
     for parameter in default_parameters:
         parameter_name = parameter.name
         parameter_type = parameter.annotation
         option_name = parameter_name.replace("_", "-")
         try:
             option = options(option_name)
-        except NoSuchOptionException:
+        except CleoNoSuchOptionError:
             option = None
 
         if config.get(parameter_name) is not None and option is not None:
             raise Exception(
                 f"You should provide either --{option_name} CLI option OR '{parameter_name}' in the config secret not both."
             )
 
@@ -605,15 +605,18 @@
     pending = []
     for group in predicted_groups:
         classifications_set = set(
             task.classification for task in group_summaries[group].tasks if task.failed
         )
         if len(classifications_set) == 0:
             continue
-        if classifications_set == {"not classified"}:
+        if (
+            len(classifications_set - {"not classified", "new failure not classified"})
+            == 0
+        ):
             pending.append(group)
         elif len(classifications_set) != 1:
             conflicting.append(group)
         elif classifications_set.isdisjoint(expected):
             differing.append(group)
 
     missed = []
@@ -1143,15 +1146,14 @@
         verb = "were" if backedout else "weren't"
         line = f"{nb} out of {len(self.pushes)} pushes {verb} backed-out by a sheriff and were classified as {status.name}."
         self.line(line)
 
         return line
 
     def send_emails(self, total, stats, error_line):
-
         today = datetime.datetime.strftime(datetime.datetime.now(), "%Y-%m-%d")
 
         stats = "\n".join([f"- {stat}" for stat in stats])
 
         environment = self.option("environment")
         notify_email(
             emails=config.get("emails", {}).get("monitoring"),
@@ -1266,15 +1268,14 @@
 
             progress.advance()
 
         # Cleanup progress bar
         progress.finish()
 
     def list_classification_tasks(self, group_id):
-
         # Check cache first
         cache_key = f"perf/task_group/{group_id}"
         tasks = config.cache.get(cache_key, [])
 
         if not tasks:
             queue = taskcluster.Queue(get_taskcluster_options())
             token = False
@@ -1316,14 +1317,16 @@
 class PushCommands(Command):
     """
     Contains commands that operate on a single push.
 
     push
     """
 
+    name = "push"
+
     commands = [
         PushTasksCommand(),
         ClassifyCommand(),
         ClassifyEvalCommand(),
         ClassifyPerfCommand(),
     ]
```

### Comparing `mozci-2.2.2/mozci/data/base.py` & `mozci-2.3.0/mozci/data/base.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/data/contract.py` & `mozci-2.3.0/mozci/data/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
                             options=[
                                 "autoclassified intermittent",
                                 "infra",
                                 "intermittent",
                                 "expected fail",
                                 "fixed by commit",
                                 "not classified",
+                                "new failure not classified",
                             ],
                         ),
                         "classification_note": v.Str(),
                     },
                     optional=["classification_note"],
                 ),
             )
```

### Comparing `mozci-2.2.2/mozci/data/sources/artifact/__init__.py` & `mozci-2.3.0/mozci/data/sources/artifact/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         )
 
         for line in lines:
             if line["action"] == "test_groups":
                 groups |= set(line["groups"]) - {"default"}
 
             elif line["action"] == "group_result":
-
                 group = line["group"]
                 if group not in group_results or line["status"] != "OK":
                     group_results[group] = (line["status"], line["duration"])
 
             elif line["action"] == "log":
                 if task_id not in self.TASK_ERRORS:
                     self.TASK_ERRORS[task_id] = []
```

### Comparing `mozci-2.2.2/mozci/data/sources/bugbug/__init__.py` & `mozci-2.3.0/mozci/data/sources/bugbug/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/data/sources/hgmo/__init__.py` & `mozci-2.3.0/mozci/data/sources/hgmo/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/data/sources/taskcluster/__init__.py` & `mozci-2.3.0/mozci/data/sources/taskcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/data/sources/treeherder/__init__.py` & `mozci-2.3.0/mozci/data/sources/treeherder/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/errors.py` & `mozci-2.3.0/mozci/errors.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/push.py` & `mozci-2.3.0/mozci/push.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/task.py` & `mozci-2.3.0/mozci/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,16 @@
         hook_payload = jsone.render(
             backfill_action["hookPayload"],
             context={
                 "taskId": self.id,
                 "taskGroupId": decision_task.id,
                 "input": {
                     "times": 5
-                    if self.classification == "not classified"
+                    if self.classification
+                    in ("not classified", "new failure not classified")
                     or self.classification in INTERMITTENT_CLASSES
                     else 1
                 },
             },
         )
 
         logger.info("Backfilling task '{}'".format(self.tags.get("label", "")))
```

### Comparing `mozci-2.2.2/mozci/util/cache_stores.py` & `mozci-2.3.0/mozci/util/cache_stores.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/util/hgmo.py` & `mozci-2.3.0/mozci/util/hgmo.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/util/logging.py` & `mozci-2.3.0/mozci/util/logging.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/util/memoize.py` & `mozci-2.3.0/mozci/util/memoize.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/util/req.py` & `mozci-2.3.0/mozci/util/req.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/util/taskcluster.py` & `mozci-2.3.0/mozci/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/mozci/util/yaml.py` & `mozci-2.3.0/mozci/util/yaml.py`

 * *Files identical despite different names*

### Comparing `mozci-2.2.2/pyproject.toml` & `mozci-2.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mozci"
-version = "2.2.2"
+version = "2.3.0"
 description = ""
 authors = [
   "Andrew Halberstadt <ahal@mozilla.com>",
   "Marco Castelluccio <marco@mozilla.com>",
 ]
 
 [tool.poetry.scripts]
@@ -25,24 +25,24 @@
 flake8 = ">=3,<5"
 pyyaml = ">=5,<7"
 taskcluster = ">=38"
 lru-dict = "^1.1.7"
 
 # Optional dependencies
 ValidX = "^0.7"
-cleo = "^0.8.1"
+cleo = "^2.0.1"
 tabulate = ">=0.8.9,<0.10.0"
 arrow = "^1.2.2"
 markdown2 = "^2.4.2"
 json-e = "^4.4.3"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20"
-pytest = "^7.1"
-tox = "^3.26"
+pytest = "^7.3"
+tox = "^4.5"
 responses = "^0.20"
 sphinx = "^5.3.0"
 
 [tool.poetry.extras]
 cache = ["boto3", "python3-memcached", "redis", "zstandard"]
 cache-s3 = ["boto3"]
 cache-memcached = ["python3-memcached"]
```

### Comparing `mozci-2.2.2/PKG-INFO` & `mozci-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: mozci
-Version: 2.2.2
+Version: 2.3.0
 Summary: 
 Author: Andrew Halberstadt
 Author-email: ahal@mozilla.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cache
 Provides-Extra: cache-memcached
 Provides-Extra: cache-redis
 Provides-Extra: cache-s3
 Provides-Extra: cache-seeded-file
 Requires-Dist: ValidX (>=0.7,<0.8)
 Requires-Dist: appdirs (>=1,<2)
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
-Requires-Dist: boto3 (>=1,<2); extra == "cache" or extra == "cache-s3"
+Requires-Dist: boto3 (>=1,<2) ; extra == "cache" or extra == "cache-s3"
 Requires-Dist: cachy (>=0,<1)
-Requires-Dist: cleo (>=0.8.1,<0.9.0)
+Requires-Dist: cleo (>=2.0.1,<3.0.0)
 Requires-Dist: flake8 (>=3,<5)
 Requires-Dist: json-e (>=4.4.3,<5.0.0)
 Requires-Dist: loguru (>=0,<1)
 Requires-Dist: lru-dict (>=1.1.7,<2.0.0)
 Requires-Dist: markdown2 (>=2.4.2,<3.0.0)
-Requires-Dist: python3-memcached (>=1,<2); extra == "cache" or extra == "cache-memcached"
+Requires-Dist: python3-memcached (>=1,<2) ; extra == "cache" or extra == "cache-memcached"
 Requires-Dist: pyyaml (>=5,<7)
-Requires-Dist: redis (>=3,<5); extra == "cache" or extra == "cache-redis"
+Requires-Dist: redis (>=3,<5) ; extra == "cache" or extra == "cache-redis"
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: tabulate (>=0.8.9,<0.10.0)
 Requires-Dist: taskcluster (>=38)
 Requires-Dist: taskcluster_urls (>=13,<14)
 Requires-Dist: tomlkit (>=0,<1)
-Requires-Dist: zstandard (>=0,<1); extra == "cache" or extra == "cache-seeded-file"
+Requires-Dist: zstandard (>=0,<1) ; extra == "cache" or extra == "cache-seeded-file"
```

