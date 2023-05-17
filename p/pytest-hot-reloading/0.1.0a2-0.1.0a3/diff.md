# Comparing `tmp/pytest_hot_reloading-0.1.0a2.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a2.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a3.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a2.tar` & `pytest_hot_reloading-0.1.0a3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-04-07 00:33:48.326861 pytest_hot_reloading-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     2402 2023-04-21 20:07:47.475596 pytest_hot_reloading-0.1.0a2/README.md
--rw-r--r--   0        0        0      655 2023-04-23 17:25:52.941402 pytest_hot_reloading-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 00:39:23.095602 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-21 18:53:22.219113 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0     4557 2023-04-21 19:45:15.205903 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     6013 2023-04-21 19:51:49.361239 pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0     2848 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     2442 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/README.md
+-rw-r--r--   0        0        0      654 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     1846 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0     4556 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     7672 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a3/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a2/LICENSE` & `pytest_hot_reloading-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a2/README.md` & `pytest_hot_reloading-0.1.0a3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # A PyTest Hot Reloading Plugin
 A hot reloading pytest daemon, implemented as a plugin.
 
-This uses the jurigged library to watch files.
+This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
 
 If it takes less than 5 seconds to do all of the imports
 necessary to run a unit test, then you probably don't need this.
 
 ## Installation
 TBD
```

### Comparing `pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import sys
 import xmlrpc.client
 
 from pytest_hot_reloading.daemon import PytestDaemon
 
 
 class PytestClient:
+    _socket: socket.socket | None
+    _daemon_host: str
+    _daemon_port: int
+    _pytest_name: str
+
     def __init__(
         self, daemon_host: str = "localhost", daemon_port: int = 4852, pytest_name: str = "pytest"
     ) -> None:
         self._socket = None
         self._daemon_host = daemon_host
         self._daemon_port = daemon_port
         self._pytest_name = pytest_name
@@ -26,15 +31,16 @@
         stderr = result["stderr"].data.decode("utf-8")
 
         print(stdout, file=sys.stdout)
         print(stderr, file=sys.stderr)
 
     def abort(self) -> None:
         # Close the socket
-        self._socket.close()
+        if self._socket:
+            self._socket.close()
 
     def _start_daemon_if_needed(self) -> None:
         # check if the daemon is running on the expected host and port
         # if not, start the daemon
 
         # first, try to connect
         try:
```

### Comparing `pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import re
 import socket
 import subprocess
 import sys
 import time
-from shutil import which
 from xmlrpc.server import SimpleXMLRPCServer
 
 import pytest
 
 
 class PytestDaemon:
     def __init__(self, daemon_host: str = "localhost", daemon_port: int = 4852) -> None:
@@ -123,21 +122,21 @@
             # args must omit the calling program
             pytest.main(["--color=yes"] + args)
         finally:
             # restore originals
             sys.stdout = stdout_bak
             sys.stderr = stderr_bak
 
-        stdout.seek(0)
-        stderr.seek(0)
-        stdout_str = stdout.read()
-        stderr_str = stderr.read()
+            stdout.seek(0)
+            stderr.seek(0)
+            stdout_str = stdout.read()
+            stderr_str = stderr.read()
 
-        print(stdout_str, file=sys.stdout)
-        print(stderr_str, file=sys.stderr)
+            print(stdout_str, file=sys.stdout)
+            print(stderr_str, file=sys.stderr)
         return {
             "stdout": self._remove_ansi_escape(stdout_str).encode("utf-8"),
             "stderr": self._remove_ansi_escape(stderr_str).encode("utf-8"),
         }
 
     def _remove_ansi_escape(self, s: str) -> str:
         return re.sub(r"\x1b(\[.*?[@-~]|\].*?(\x07|\x1b\\))", "", s, flags=re.MULTILINE)
```

### Comparing `pytest_hot_reloading-0.1.0a2/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Pytest Hot Reloading plugin
 """
+import ast
 import fnmatch
 import os
 import re
 import sys
 from typing import Callable
 
 import jurigged
+import jurigged.codetools as jurigged_codetools
 from pytest import Config, Item, Session
 
 from pytest_hot_reloading.client import PytestClient
 from pytest_hot_reloading.daemon import PytestDaemon
 
 # this is modified by the daemon so that the pytest_collection hooks does not run
 i_am_server = False
@@ -59,54 +61,98 @@
     )
 
 
 # list of pytest hooks
 # https://docs.pytest.org/en/stable/reference.html#_pytest.hookspec.pytest_addhooks
 
 
-def pytest_collection(session: Session) -> None:
+def pytest_cmdline_main(config: Config) -> None:
     """
     This hook is called by pytest and is one of the first hooks.
     """
     # early escapes
-    if session.config.option.collectonly:
+    if config.option.collectonly:
         return
     if i_am_server:
         return
-    _plugin_logic(session)
+    _plugin_logic(config)
 
 
 def _jurigged_logger(x: str) -> None:
     """
     Jurigged behavior is to both print and log.
 
     By default this creates duplicated output.
 
     Pass in a no-op logger to prevent this.
     """
 
 
-def _plugin_logic(session: Session) -> None:
+OrigFunctionDefinition = jurigged_codetools.FunctionDefinition
+
+
+class NewFunctionDefinition(OrigFunctionDefinition):
+    def reevaluate(self, new_node, glb):
+        new_node = self.apply_assertion_rewrite(new_node, glb)
+        return super().reevaluate(new_node, glb)
+
+    def apply_assertion_rewrite(self, ast_func, glb):
+        from _pytest.assertion.rewrite import AssertionRewriter
+
+        nodes: list[ast.AST] = [ast_func]
+        while nodes:
+            node = nodes.pop()
+            for name, field in ast.iter_fields(node):
+                if isinstance(field, list):
+                    new: list[ast.AST] = []
+                    for i, child in enumerate(field):
+                        if isinstance(child, ast.Assert):
+                            # Transform assert.
+                            new.extend(
+                                AssertionRewriter(glb["__file__"], None, None).visit(child)
+                            )
+                        else:
+                            new.append(child)
+                            if isinstance(child, ast.AST):
+                                nodes.append(child)
+                    setattr(node, name, new)
+                elif (
+                    isinstance(field, ast.AST)
+                    # Don't recurse into expressions as they can't contain
+                    # asserts.
+                    and not isinstance(field, ast.expr)
+                ):
+                    nodes.append(field)
+        return ast_func
+
+
+# monkey patch in new definition
+jurigged_codetools.FunctionDefinition = NewFunctionDefinition
+
+
+def _plugin_logic(config: Config) -> None:
     """
     The core plugin logic. This is where it splits based on whether we are the server or client.
 
     In either case, the pytest logic will not continue after this.
     """
     # if daemon is passed, then we are the daemon / server
     # if daemon is not passed, then we are the client
-    daemon_port = int(session.config.option.daemon_port)
-    if session.config.option.daemon:
+    daemon_port = int(config.option.daemon_port)
+    if config.option.daemon:
         # pytest prints out "collecting ...". The leading \r prevents that
         print("\rStarting daemon...")
-        pattern = _get_pattern_filters(session)
-        jurigged.watch(pattern=pattern, logger=_jurigged_logger)
+        pattern = _get_pattern_filters(config)
+        # TODO: intelligently use poll versus watchman
+        jurigged.watch(pattern=pattern, logger=_jurigged_logger, poll=True)
         daemon = PytestDaemon(daemon_port=daemon_port)
+
         daemon.run_forever()
     else:
-        pytest_name = session.config.option.pytest_name
+        pytest_name = config.option.pytest_name
         client = PytestClient(daemon_port=daemon_port, pytest_name=pytest_name)
         # find the index of the first value that is not None
         for idx, val in enumerate(
             [
                 x.endswith(pytest_name) or x.endswith(f"{pytest_name}/__main__.py")
                 for x in sys.argv
             ]
@@ -122,15 +168,15 @@
             )
         client.run(sys.argv[pytest_name_index + 1 :])
 
         # dont do any more work. Don't let pytest continue
         os._exit(0)
 
 
-def _get_pattern_filters(session: Session) -> str | Callable[[str], bool]:
+def _get_pattern_filters(config: Config) -> str | Callable[[str], bool]:
     """
     Jurigged takes in a pattern argument. The argument is either a glob string
     or a function that returns True if the path passed into it should be watched.
 
     This creates a function filter that will return True if the path matches.
 
     The logic takes in the --daemon-watch-globs and --daemon-ignore-watch-globs options
@@ -146,20 +192,20 @@
             glob = os.path.expanduser(glob)
         elif not glob.startswith("/"):
             glob = os.path.abspath(glob)
         if os.path.isdir(glob):
             glob = os.path.join(glob, "*")
         return glob
 
-    watch_globs = session.config.option.daemon_watch_globs.split(":")
+    watch_globs = config.option.daemon_watch_globs.split(":")
     regex_matches = [re.compile(fnmatch.translate(normalize(glob))).match for glob in watch_globs]
 
-    ignore_watch_globs = session.config.option.daemon_ignore_watch_globs
+    ignore_watch_globs = config.option.daemon_ignore_watch_globs
     if ignore_watch_globs:
-        ignore_globs = session.config.option.daemon_ignore_watch_globs.split(":")
+        ignore_globs = config.option.daemon_ignore_watch_globs.split(":")
         ignore_regex_matches = [
             re.compile(fnmatch.translate(normalize(glob))).match for glob in ignore_globs
         ]
     else:
         ignore_regex_matches = []
 
     def matcher(filename) -> bool:
```

### Comparing `pytest_hot_reloading-0.1.0a2/PKG-INFO` & `pytest_hot_reloading-0.1.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a2
-Summary: A pytest plugin to enable a hot reloading daemon.
+Version: 0.1.0a3
+Summary: 
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jurigged (>=0.5.5,<0.6.0)
 Description-Content-Type: text/markdown
 
 # A PyTest Hot Reloading Plugin
 A hot reloading pytest daemon, implemented as a plugin.
 
-This uses the jurigged library to watch files.
+This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
 
 If it takes less than 5 seconds to do all of the imports
 necessary to run a unit test, then you probably don't need this.
 
 ## Installation
 TBD
```

