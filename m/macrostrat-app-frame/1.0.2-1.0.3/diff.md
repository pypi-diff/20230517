# Comparing `tmp/macrostrat_app_frame-1.0.2.tar.gz` & `tmp/macrostrat_app_frame-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_app_frame-1.0.2.tar", max compression
+gzip compressed data, was "macrostrat_app_frame-1.0.3.tar", max compression
```

## Comparing `macrostrat_app_frame-1.0.2.tar` & `macrostrat_app_frame-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       59 2023-05-16 20:02:34.747827 macrostrat_app_frame-1.0.2/macrostrat/app_frame/__init__.py
--rw-r--r--   0        0        0      967 2023-05-17 17:57:19.311188 macrostrat_app_frame-1.0.2/macrostrat/app_frame/compose.py
--rw-r--r--   0        0        0     5335 2023-05-17 17:57:37.604819 macrostrat_app_frame-1.0.2/macrostrat/app_frame/control_command.py
--rw-r--r--   0        0        0     3780 2023-05-15 21:31:33.953594 macrostrat_app_frame-1.0.2/macrostrat/app_frame/core.py
--rw-r--r--   0        0        0     2372 2023-05-15 21:32:32.147486 macrostrat_app_frame-1.0.2/macrostrat/app_frame/follow_logs.py
--rw-r--r--   0        0        0      481 2023-05-17 17:57:56.824525 macrostrat_app_frame-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 macrostrat_app_frame-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-16 20:02:34.747827 macrostrat_app_frame-1.0.3/macrostrat/app_frame/__init__.py
+-rw-r--r--   0        0        0      996 2023-05-17 18:01:29.460021 macrostrat_app_frame-1.0.3/macrostrat/app_frame/compose.py
+-rw-r--r--   0        0        0     5361 2023-05-17 18:01:56.665661 macrostrat_app_frame-1.0.3/macrostrat/app_frame/control_command.py
+-rw-r--r--   0        0        0     3780 2023-05-15 21:31:33.953594 macrostrat_app_frame-1.0.3/macrostrat/app_frame/core.py
+-rw-r--r--   0        0        0     2372 2023-05-15 21:32:32.147486 macrostrat_app_frame-1.0.3/macrostrat/app_frame/follow_logs.py
+-rw-r--r--   0        0        0      481 2023-05-17 18:02:24.897094 macrostrat_app_frame-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 macrostrat_app_frame-1.0.3/PKG-INFO
```

### Comparing `macrostrat_app_frame-1.0.2/macrostrat/app_frame/compose.py` & `macrostrat_app_frame-1.0.3/macrostrat/app_frame/compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 
 def compose(*args, **kwargs):
     """Run docker compose commands in the appropriate context"""
     return cmd("docker", "compose", *args, **kwargs)
 
 
-def check_status() -> list[str]:
+def check_status(app_name: str, command_name: str) -> list[str]:
     # Check if containers are running
     res = compose("ps --services --filter status=running", capture_output=True)
     running_containers = res.stdout.decode("utf-8").strip()
     if running_containers == "":
         return []
-    
+
     containers = running_containers.split("\n")
     containers = [c.strip() for c in containers]
 
     console.print("[dim]Some containers are already running and up to date: ")
-    console.print("  " + ", ".join(containers)
+    console.print("  " + ", ".join(containers))
     console.print(
         f"[dim]To fully restart {app_name}, run [cyan]{command_name} restart[/cyan]"
         f" or [cyan]{command_name} up --force-recreate[/cyan]."
     )
 
     return containers
```

### Comparing `macrostrat_app_frame-1.0.2/macrostrat/app_frame/control_command.py` & `macrostrat_app_frame-1.0.3/macrostrat/app_frame/control_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             "One or more containers did not build successfully, aborting.",
             style="red bold",
         )
         sys.exit(res.returncode)
     else:
         app.info("All containers built successfully.", style="green bold")
 
-    running_containers = check_status()
+    running_containers = check_status(app.name, app.command_name)
 
     app.info("Starting :app_name: server...", style="bold")
     compose("start")
 
     for container, command in app.restart_commands.items():
         if container in running_containers:
             app.info(f"Reloading {container}...", style="bold")
```

### Comparing `macrostrat_app_frame-1.0.2/macrostrat/app_frame/core.py` & `macrostrat_app_frame-1.0.3/macrostrat/app_frame/core.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.2/macrostrat/app_frame/follow_logs.py` & `macrostrat_app_frame-1.0.3/macrostrat/app_frame/follow_logs.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.2/PKG-INFO` & `macrostrat_app_frame-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-app-frame
-Version: 1.0.2
+Version: 1.0.3
 Summary: A control script framework for containerized applications.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

