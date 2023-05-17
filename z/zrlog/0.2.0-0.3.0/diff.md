# Comparing `tmp/zrlog-0.2.0.tar.gz` & `tmp/zrlog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrlog-0.2.0.tar", last modified: Tue May 16 14:03:35 2023, max compression
+gzip compressed data, was "zrlog-0.3.0.tar", last modified: Wed May 17 15:33:32 2023, max compression
```

## Comparing `zrlog-0.2.0.tar` & `zrlog-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.411049 zrlog-0.2.0/
--rw-rw-rw-   0        0        0     1069 2023-05-16 13:38:24.000000 zrlog-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     5167 2023-05-16 14:03:35.411049 zrlog-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4608 2023-05-16 14:01:40.000000 zrlog-0.2.0/README.md
--rw-rw-rw-   0        0        0       88 2023-05-16 13:38:24.000000 zrlog-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      763 2023-05-16 14:03:35.413049 zrlog-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.395049 zrlog-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.404049 zrlog-0.2.0/src/zrlog/
--rw-rw-rw-   0        0        0       57 2023-05-16 13:45:41.000000 zrlog-0.2.0/src/zrlog/__init__.py
--rw-rw-rw-   0        0        0      969 2023-05-16 13:38:24.000000 zrlog-0.2.0/src/zrlog/logger.py
--rw-rw-rw-   0        0        0     4710 2023-05-16 14:00:09.000000 zrlog-0.2.0/src/zrlog/logs.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.410049 zrlog-0.2.0/src/zrlog.egg-info/
--rw-rw-rw-   0        0        0     5167 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:33:32.775572 zrlog-0.3.0/
+-rw-rw-rw-   0        0        0     1069 2023-05-16 13:38:24.000000 zrlog-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5883 2023-05-17 15:33:32.776538 zrlog-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5324 2023-05-17 15:33:12.000000 zrlog-0.3.0/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-16 13:38:24.000000 zrlog-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      763 2023-05-17 15:33:32.777571 zrlog-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 15:33:32.761579 zrlog-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:33:32.769572 zrlog-0.3.0/src/zrlog/
+-rw-rw-rw-   0        0        0      131 2023-05-17 14:57:06.000000 zrlog-0.3.0/src/zrlog/__init__.py
+-rw-rw-rw-   0        0        0     5281 2023-05-17 15:13:47.000000 zrlog-0.3.0/src/zrlog/logger.py
+-rw-rw-rw-   0        0        0     4436 2023-05-17 15:14:36.000000 zrlog-0.3.0/src/zrlog/logs.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:33:32.775572 zrlog-0.3.0/src/zrlog.egg-info/
+-rw-rw-rw-   0        0        0     5883 2023-05-17 15:33:32.000000 zrlog-0.3.0/src/zrlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-17 15:33:32.000000 zrlog-0.3.0/src/zrlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:33:32.000000 zrlog-0.3.0/src/zrlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-17 15:33:32.000000 zrlog-0.3.0/src/zrlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-17 15:33:32.000000 zrlog-0.3.0/src/zrlog.egg-info/top_level.txt
```

### Comparing `zrlog-0.2.0/LICENSE` & `zrlog-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zrlog-0.2.0/PKG-INFO` & `zrlog-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,89 @@
 Metadata-Version: 2.1
 Name: zrlog
-Version: 0.2.0
+Version: 0.3.0
 Summary: Logging with Zirconium-based configuration and supports audit logging
 Home-page: https://github.com/turnbullerin/zrlog
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zrlog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zirconium Logging (ZrLog)
-This package adds logging support using the Zirconium configuration tool and TOML, with an extension for supporting
-logging audit events.
+Logging configuration is often complex and Python is missing a few "nice" features that exist in 
+other languages logging systems. This package hopes to simplify the experience of configuring logging while adding a few
+nice features:
+
+* Loading logging configuration from TOML or YAML (via `zirconium`) instead of the older `configparser` format
+* `TRACE` level for very fine-grained output (more so that `DEBUG`)
+* `NOTICE` level for normal conditions that should always be output
+* `OUT` level for logging user messages
+* `AUDIT` level for interacting with Python's audit hooks
+* A threaded audit hook that logs most audit messages
+* The ability to disable stack trace output
+* The ability to set context-specific "extra" variables on all loggers and to provide defaults for these
+  so that they can be added to all logging messages within that context (e.g. for usernames)
 
-
-## Defining Logging Parameters
-Configuration for the logging module can be added in TOML under the `logging` key. The entries correspond to those 
-supported by `logging.config.dictConfig()` with a few additions to support audit logging. For example:
-
-```toml 
-# .logging.toml (or your own app configuration file that you've registered) 
-[logging]
-version = 1
-
-[logging.root]
-level = "INFO"
-handlers = ["console"]
-
-[logging.handlers.console]
-class = "logging.StreamHandler"
-formatter = "brief"
-level = "WARNING"
-stream = "ext://sys.stdout"
-
-[logging.formatters.brief]
-format = "%(message)s [%(levelname)s]"
-```
-
-Of note, if you want to change a specific logger (which often have dots in the name), you must quote the key:
-
-```toml 
-[logging.loggers."module.foo.bar"]
-level = "WARNING"
-```
-
-## Setting up logging
-
-Logging can be initialized at the appropriate place in your code. This should be AFTER you have registered all your
-configuration with Zirconium but before you want to do any logging.
+## Basic Usage
 
 ```python 
+# Do this at the start of any run of your code
 import zrlog
-zrlog.init_logging()
-```
-
-For test cases, configuration is often not done until the test case level, but you can use the `no_config` parameter
-to tell ZrLog to ignore the configuration.
-
-```python
-import zrlog
-zrlog.init_logging(no_config=True)
-```
-
 
-## Additional Logging Levels
-This package adds three additional levels of logging:
+# Imports logging configuration from TOML and sets up the logging system for you.
+zrlog.init_logging()
 
-- `audit()`, which is intended to be used only with the Python auditing system as described below. The logging level is 
-  set to 1.
-- `trace()`, which is intended to be even more detailed than debug(). The logging level is set to 5.
-- `out()`, which is ranked between INFO and WARNING and is intended to be used to log user output for command-line 
-  applications or key events that need to be tracked for auditing purposes. The logging level is set to 25.
+# Set a default username
+zrlog.set_default_extra('username', '**anonymous**')
 
-These are configured as methods on the `getLogger()` class as well as on `logging` itself for the root logger. Putting
-these together with existing levels, we recommend the following usages:
+# logging.getLogger() works as well, this version is a wrapper that (a) makes sure that `zrlog.init_logging()` was 
+# called and (b) provides a better type hint for the logger class.
+logger = zrlog.get_logger(__name__)
+```
+
+## Configuration File
+By default, logging configuration comes from a TOML file in up to three places:
+
+* `[HOME_DIRECTORY]/.logging.toml`
+* `[CURRENT_WORKING_DIRECTORY]/.logging.toml`
+* Value of the `ZRLOG_CONFIG_FILE` environment variable. This file may also be a YAML or other formats supported by 
+  `zirconium`
+  
+If you use `zirconium` for your project configuration, it can also be in any configuration file specified by your
+project.
+  
+The logging configuration file is similar to that defined by `logging.config.dictConfig()`, with a few extensions. See 
+the `.logging.example.toml` file for configuration.
+
+
+## Performance impact
+Testing suggests that the impact of replacing the typical `logging` approach with this module is about 14% slower to 
+get a logger and 10% slower to make a logging call with extras. However, the time to make a log to `stdout` is 
+still only 0.013 ms (compared to 0.012 ms for the standard logging package), therefore this performance impact is 
+probably insignificant in most use cases.
 
-| Level | Meaning |
+## Log Level Recommendations
+| Level | Use Case |
 | --- | --- |
-| critical | An error so severe has occurred that the system may now crash. |
-| error | An error has occurred and something that was expected to happen did not happen. |
-| warning | Something unexpected happen or a problem may occur in the future. |
-| out | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| critical | An error so severe has occurred that the application may now crash. |
+| error | An error has occurred and may have created unexpected behaviour. |
+| warning | Something unexpected happen but it is recoverable, or a problem may occur in the future. |
+| notice | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| out | Something expected has happened in a command line environment that the user needs to be notified of. |
 | info | Something expected has happened that does not need tracking but can be useful to confirm normal operation. |
 | debug | Additional detail for debugging an issue |
 | trace | Even more detail for debugging an issue |
 | audit | Python auditing output only |
 
 
-
 ## Logging Audit Events
 This package provides a system for turning `sys.audit()` events into log records using a thread-based queue. This is 
 necessary because audit events don't play nicely with the logging subsystem, leading to inconsistent errors if the
 logger `log()` method is called directly from the audit hook. Audit logging must be enabled specifically by setting
 the `with_audit` flag:
 
 ```toml
@@ -138,11 +126,16 @@
 formatter = "brief"
 level = "AUDIT"
 stream = "ext://sys.stdout"
 ```
 
 ## Change Log
 
+### version 0.3.0
+- Added logger extra handling via `set_logger_extra` and `set_default_logger_extra`
+- Added the `NOTICE` level to correspond with more typical usage. `OUT` should be used for user output where it needs
+  to be logged and `NOTICE` for normal conditions that need to be logged even in production.
+
 ### version 0.2.0
 - Updated the audit handling thread to use a `threading.Event` to end itself rather than a boolean flag.
 - Added the `no_config` flag, mostly to be used in test suites to ensure everything still works properly.
 - Several documentation cleanup items
```

### Comparing `zrlog-0.2.0/README.md` & `zrlog-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,74 @@
 # Zirconium Logging (ZrLog)
-This package adds logging support using the Zirconium configuration tool and TOML, with an extension for supporting
-logging audit events.
+Logging configuration is often complex and Python is missing a few "nice" features that exist in 
+other languages logging systems. This package hopes to simplify the experience of configuring logging while adding a few
+nice features:
+
+* Loading logging configuration from TOML or YAML (via `zirconium`) instead of the older `configparser` format
+* `TRACE` level for very fine-grained output (more so that `DEBUG`)
+* `NOTICE` level for normal conditions that should always be output
+* `OUT` level for logging user messages
+* `AUDIT` level for interacting with Python's audit hooks
+* A threaded audit hook that logs most audit messages
+* The ability to disable stack trace output
+* The ability to set context-specific "extra" variables on all loggers and to provide defaults for these
+  so that they can be added to all logging messages within that context (e.g. for usernames)
 
-
-## Defining Logging Parameters
-Configuration for the logging module can be added in TOML under the `logging` key. The entries correspond to those 
-supported by `logging.config.dictConfig()` with a few additions to support audit logging. For example:
-
-```toml 
-# .logging.toml (or your own app configuration file that you've registered) 
-[logging]
-version = 1
-
-[logging.root]
-level = "INFO"
-handlers = ["console"]
-
-[logging.handlers.console]
-class = "logging.StreamHandler"
-formatter = "brief"
-level = "WARNING"
-stream = "ext://sys.stdout"
-
-[logging.formatters.brief]
-format = "%(message)s [%(levelname)s]"
-```
-
-Of note, if you want to change a specific logger (which often have dots in the name), you must quote the key:
-
-```toml 
-[logging.loggers."module.foo.bar"]
-level = "WARNING"
-```
-
-## Setting up logging
-
-Logging can be initialized at the appropriate place in your code. This should be AFTER you have registered all your
-configuration with Zirconium but before you want to do any logging.
+## Basic Usage
 
 ```python 
+# Do this at the start of any run of your code
 import zrlog
-zrlog.init_logging()
-```
-
-For test cases, configuration is often not done until the test case level, but you can use the `no_config` parameter
-to tell ZrLog to ignore the configuration.
-
-```python
-import zrlog
-zrlog.init_logging(no_config=True)
-```
-
 
-## Additional Logging Levels
-This package adds three additional levels of logging:
+# Imports logging configuration from TOML and sets up the logging system for you.
+zrlog.init_logging()
 
-- `audit()`, which is intended to be used only with the Python auditing system as described below. The logging level is 
-  set to 1.
-- `trace()`, which is intended to be even more detailed than debug(). The logging level is set to 5.
-- `out()`, which is ranked between INFO and WARNING and is intended to be used to log user output for command-line 
-  applications or key events that need to be tracked for auditing purposes. The logging level is set to 25.
+# Set a default username
+zrlog.set_default_extra('username', '**anonymous**')
 
-These are configured as methods on the `getLogger()` class as well as on `logging` itself for the root logger. Putting
-these together with existing levels, we recommend the following usages:
+# logging.getLogger() works as well, this version is a wrapper that (a) makes sure that `zrlog.init_logging()` was 
+# called and (b) provides a better type hint for the logger class.
+logger = zrlog.get_logger(__name__)
+```
+
+## Configuration File
+By default, logging configuration comes from a TOML file in up to three places:
+
+* `[HOME_DIRECTORY]/.logging.toml`
+* `[CURRENT_WORKING_DIRECTORY]/.logging.toml`
+* Value of the `ZRLOG_CONFIG_FILE` environment variable. This file may also be a YAML or other formats supported by 
+  `zirconium`
+  
+If you use `zirconium` for your project configuration, it can also be in any configuration file specified by your
+project.
+  
+The logging configuration file is similar to that defined by `logging.config.dictConfig()`, with a few extensions. See 
+the `.logging.example.toml` file for configuration.
+
+
+## Performance impact
+Testing suggests that the impact of replacing the typical `logging` approach with this module is about 14% slower to 
+get a logger and 10% slower to make a logging call with extras. However, the time to make a log to `stdout` is 
+still only 0.013 ms (compared to 0.012 ms for the standard logging package), therefore this performance impact is 
+probably insignificant in most use cases.
 
-| Level | Meaning |
+## Log Level Recommendations
+| Level | Use Case |
 | --- | --- |
-| critical | An error so severe has occurred that the system may now crash. |
-| error | An error has occurred and something that was expected to happen did not happen. |
-| warning | Something unexpected happen or a problem may occur in the future. |
-| out | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| critical | An error so severe has occurred that the application may now crash. |
+| error | An error has occurred and may have created unexpected behaviour. |
+| warning | Something unexpected happen but it is recoverable, or a problem may occur in the future. |
+| notice | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| out | Something expected has happened in a command line environment that the user needs to be notified of. |
 | info | Something expected has happened that does not need tracking but can be useful to confirm normal operation. |
 | debug | Additional detail for debugging an issue |
 | trace | Even more detail for debugging an issue |
 | audit | Python auditing output only |
 
 
-
 ## Logging Audit Events
 This package provides a system for turning `sys.audit()` events into log records using a thread-based queue. This is 
 necessary because audit events don't play nicely with the logging subsystem, leading to inconsistent errors if the
 logger `log()` method is called directly from the audit hook. Audit logging must be enabled specifically by setting
 the `with_audit` flag:
 
 ```toml
@@ -123,11 +111,16 @@
 formatter = "brief"
 level = "AUDIT"
 stream = "ext://sys.stdout"
 ```
 
 ## Change Log
 
+### version 0.3.0
+- Added logger extra handling via `set_logger_extra` and `set_default_logger_extra`
+- Added the `NOTICE` level to correspond with more typical usage. `OUT` should be used for user output where it needs
+  to be logged and `NOTICE` for normal conditions that need to be logged even in production.
+
 ### version 0.2.0
 - Updated the audit handling thread to use a `threading.Event` to end itself rather than a boolean flag.
 - Added the `no_config` flag, mostly to be used in test suites to ensure everything still works properly.
 - Several documentation cleanup items
```

### Comparing `zrlog-0.2.0/setup.cfg` & `zrlog-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 726c 6f67 0d0a 7665 7273 696f   = zrlog..versio
-00000020: 6e20 3d20 302e 322e 300d 0a61 7574 686f  n = 0.2.0..autho
+00000020: 6e20 3d20 302e 332e 300d 0a61 7574 686f  n = 0.3.0..autho
 00000030: 7220 3d20 4572 696e 2054 7572 6e62 756c  r = Erin Turnbul
 00000040: 6c0d 0a61 7574 686f 725f 656d 6169 6c20  l..author_email 
 00000050: 3d20 6572 696e 2e61 2e74 7572 6e62 756c  = erin.a.turnbul
 00000060: 6c40 676d 6169 6c2e 636f 6d0d 0a64 6573  l@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 204c 6f67 6769  cription = Loggi
 00000080: 6e67 2077 6974 6820 5a69 7263 6f6e 6975  ng with Zirconiu
 00000090: 6d2d 6261 7365 6420 636f 6e66 6967 7572  m-based configur
```

### Comparing `zrlog-0.2.0/src/zrlog/logs.py` & `zrlog-0.3.0/src/zrlog/logs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ Logging management compatible with Zirconium with additional features"""
 from autoinject import injector
 import zirconium as zr
 import logging.config
+from zrlog.logger import ImprovedLogger, _LogSettingManager
 import logging
 import threading
 import queue
 import sys
 import atexit
-import time
+import os
 
 
 class AuditLog(threading.Thread):
     """ Responsible for managing a queue of audit messages from sys.audit() and passing them to the logging.
 
         Note that this is necessary because calls directly to logging.audit() will cause an error, so we will
         manage them in a thread instead.
@@ -61,49 +62,42 @@
 
 
 @zr.configure
 def config_logging(config: zr.ApplicationConfig):
     """ Configuration for zirconium """
     config.register_file("~/.logging.toml")
     config.register_file("./.logging.toml")
+    custom_path = os.environ.get("ZRLOG_CONFIG_FILE")
+    if custom_path:
+        config.register_file(custom_path)
 
 
-def _add_logging_level(level_name, level_no):
-    """ Adds a logging level """
-
-    def log_at_level(message, *args, **kwargs):
-        logging.log(level_no, message, *args, **kwargs)
-
-    level_name = level_name.upper()
-    method_name = level_name.lower()
-    logging.addLevelName(level_no, level_name)
-    setattr(logging, level_name, level_no)
-    setattr(logging, method_name, log_at_level)
+def get_logger(name: str) -> ImprovedLogger:
+    _LogSettingManager.get().init()
+    return logging.getLogger(name)
 
 
 @injector.inject
-def init_logging(no_config: bool = False, config: zr.ApplicationConfig = None):
+def init_logging(config: zr.ApplicationConfig = None):
     """ Initializes logging from the configuration file as well as adding our custom levels and, if specified, audit
         output
     """
-    #Audit is for the sys.audit(), if enabled
-    _add_logging_level("AUDIT", 1)
-    # Trace is a lower level than debug for even more information
-    _add_logging_level("TRACE", 5)
-    # Out is a level higher than info but lower than warning for what a CLI user might want to see
-    _add_logging_level("OUT", 25)
-    # Import is done here in case something else has overridden the default logging class
-    from .logger import ImprovedLogger
-    logging.setLoggerClass(ImprovedLogger)
-    if (not no_config) and "logging" in config:
+    # Add the additional logging levels
+    instance = _LogSettingManager.get()
+    instance.init()
+    if "logging" in config:
         # Load our logging configuration
         logging.config.dictConfig(config["logging"])
         # If we want to include audit events, set up the logging for them
         if config.as_bool(("logging", "with_audit"), False) and sys.version_info.major >= 3 and sys.version_info.minor >= 8:
             audit_logger = AuditLog(
                 config.as_bool(("logging", "omit_logging_frames"), True),
                 config.as_str(("logging", "audit_level"), "AUDIT")
             )
             audit_logger.start()
             sys.addaudithook(audit_logger.audit_hook)
             atexit.register(audit_logger.halt)
+        # Load defaults for extras
+        instance.set_defaults(config.as_dict(("logging", "default_extras"), default={}))
+        # Load stack trace visibility setting
+        instance.show_stack_traces = config.as_bool(("logging", "show_stack_traces"), default=True)
     logging.getLogger("zrlog").debug("Zirconium-based logging initialized")
```

### Comparing `zrlog-0.2.0/src/zrlog.egg-info/PKG-INFO` & `zrlog-0.3.0/src/zrlog.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,89 @@
 Metadata-Version: 2.1
 Name: zrlog
-Version: 0.2.0
+Version: 0.3.0
 Summary: Logging with Zirconium-based configuration and supports audit logging
 Home-page: https://github.com/turnbullerin/zrlog
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zrlog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Zirconium Logging (ZrLog)
-This package adds logging support using the Zirconium configuration tool and TOML, with an extension for supporting
-logging audit events.
+Logging configuration is often complex and Python is missing a few "nice" features that exist in 
+other languages logging systems. This package hopes to simplify the experience of configuring logging while adding a few
+nice features:
+
+* Loading logging configuration from TOML or YAML (via `zirconium`) instead of the older `configparser` format
+* `TRACE` level for very fine-grained output (more so that `DEBUG`)
+* `NOTICE` level for normal conditions that should always be output
+* `OUT` level for logging user messages
+* `AUDIT` level for interacting with Python's audit hooks
+* A threaded audit hook that logs most audit messages
+* The ability to disable stack trace output
+* The ability to set context-specific "extra" variables on all loggers and to provide defaults for these
+  so that they can be added to all logging messages within that context (e.g. for usernames)
 
-
-## Defining Logging Parameters
-Configuration for the logging module can be added in TOML under the `logging` key. The entries correspond to those 
-supported by `logging.config.dictConfig()` with a few additions to support audit logging. For example:
-
-```toml 
-# .logging.toml (or your own app configuration file that you've registered) 
-[logging]
-version = 1
-
-[logging.root]
-level = "INFO"
-handlers = ["console"]
-
-[logging.handlers.console]
-class = "logging.StreamHandler"
-formatter = "brief"
-level = "WARNING"
-stream = "ext://sys.stdout"
-
-[logging.formatters.brief]
-format = "%(message)s [%(levelname)s]"
-```
-
-Of note, if you want to change a specific logger (which often have dots in the name), you must quote the key:
-
-```toml 
-[logging.loggers."module.foo.bar"]
-level = "WARNING"
-```
-
-## Setting up logging
-
-Logging can be initialized at the appropriate place in your code. This should be AFTER you have registered all your
-configuration with Zirconium but before you want to do any logging.
+## Basic Usage
 
 ```python 
+# Do this at the start of any run of your code
 import zrlog
-zrlog.init_logging()
-```
-
-For test cases, configuration is often not done until the test case level, but you can use the `no_config` parameter
-to tell ZrLog to ignore the configuration.
-
-```python
-import zrlog
-zrlog.init_logging(no_config=True)
-```
-
 
-## Additional Logging Levels
-This package adds three additional levels of logging:
+# Imports logging configuration from TOML and sets up the logging system for you.
+zrlog.init_logging()
 
-- `audit()`, which is intended to be used only with the Python auditing system as described below. The logging level is 
-  set to 1.
-- `trace()`, which is intended to be even more detailed than debug(). The logging level is set to 5.
-- `out()`, which is ranked between INFO and WARNING and is intended to be used to log user output for command-line 
-  applications or key events that need to be tracked for auditing purposes. The logging level is set to 25.
+# Set a default username
+zrlog.set_default_extra('username', '**anonymous**')
 
-These are configured as methods on the `getLogger()` class as well as on `logging` itself for the root logger. Putting
-these together with existing levels, we recommend the following usages:
+# logging.getLogger() works as well, this version is a wrapper that (a) makes sure that `zrlog.init_logging()` was 
+# called and (b) provides a better type hint for the logger class.
+logger = zrlog.get_logger(__name__)
+```
+
+## Configuration File
+By default, logging configuration comes from a TOML file in up to three places:
+
+* `[HOME_DIRECTORY]/.logging.toml`
+* `[CURRENT_WORKING_DIRECTORY]/.logging.toml`
+* Value of the `ZRLOG_CONFIG_FILE` environment variable. This file may also be a YAML or other formats supported by 
+  `zirconium`
+  
+If you use `zirconium` for your project configuration, it can also be in any configuration file specified by your
+project.
+  
+The logging configuration file is similar to that defined by `logging.config.dictConfig()`, with a few extensions. See 
+the `.logging.example.toml` file for configuration.
+
+
+## Performance impact
+Testing suggests that the impact of replacing the typical `logging` approach with this module is about 14% slower to 
+get a logger and 10% slower to make a logging call with extras. However, the time to make a log to `stdout` is 
+still only 0.013 ms (compared to 0.012 ms for the standard logging package), therefore this performance impact is 
+probably insignificant in most use cases.
 
-| Level | Meaning |
+## Log Level Recommendations
+| Level | Use Case |
 | --- | --- |
-| critical | An error so severe has occurred that the system may now crash. |
-| error | An error has occurred and something that was expected to happen did not happen. |
-| warning | Something unexpected happen or a problem may occur in the future. |
-| out | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| critical | An error so severe has occurred that the application may now crash. |
+| error | An error has occurred and may have created unexpected behaviour. |
+| warning | Something unexpected happen but it is recoverable, or a problem may occur in the future. |
+| notice | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| out | Something expected has happened in a command line environment that the user needs to be notified of. |
 | info | Something expected has happened that does not need tracking but can be useful to confirm normal operation. |
 | debug | Additional detail for debugging an issue |
 | trace | Even more detail for debugging an issue |
 | audit | Python auditing output only |
 
 
-
 ## Logging Audit Events
 This package provides a system for turning `sys.audit()` events into log records using a thread-based queue. This is 
 necessary because audit events don't play nicely with the logging subsystem, leading to inconsistent errors if the
 logger `log()` method is called directly from the audit hook. Audit logging must be enabled specifically by setting
 the `with_audit` flag:
 
 ```toml
@@ -138,11 +126,16 @@
 formatter = "brief"
 level = "AUDIT"
 stream = "ext://sys.stdout"
 ```
 
 ## Change Log
 
+### version 0.3.0
+- Added logger extra handling via `set_logger_extra` and `set_default_logger_extra`
+- Added the `NOTICE` level to correspond with more typical usage. `OUT` should be used for user output where it needs
+  to be logged and `NOTICE` for normal conditions that need to be logged even in production.
+
 ### version 0.2.0
 - Updated the audit handling thread to use a `threading.Event` to end itself rather than a boolean flag.
 - Added the `no_config` flag, mostly to be used in test suites to ensure everything still works properly.
 - Several documentation cleanup items
```

