# Comparing `tmp/simplesystray-0.0.6.tar.gz` & `tmp/simplesystray-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesystray-0.0.6.tar", last modified: Tue May 16 22:14:08 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `simplesystray-0.0.6.tar` & `simplesystray-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.706091 simplesystray-0.0.6/
--rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5764 2023-05-16 22:14:08.706091 simplesystray-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5189 2023-05-16 21:39:36.000000 simplesystray-0.0.6/README.md
--rw-rw-rw-   0        0        0      653 2023-05-16 22:13:50.000000 simplesystray-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 22:14:08.706091 simplesystray-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.697091 simplesystray-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.701090 simplesystray-0.0.6/src/simplesystray/
--rw-rw-rw-   0        0        0        0 2023-05-16 22:13:24.000000 simplesystray-0.0.6/src/simplesystray/__init__.py
--rw-rw-rw-   0        0        0    12084 2023-05-16 21:40:55.000000 simplesystray-0.0.6/src/simplesystray/traybar.py
--rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.6/src/simplesystray/win32_adapter.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.704093 simplesystray-0.0.6/src/simplesystray.egg-info/
--rw-rw-rw-   0        0        0     5764 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-16 22:14:08.000000 simplesystray-0.0.6/src/simplesystray.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 22:14:08.705092 simplesystray-0.0.6/tests/
--rw-rw-rw-   0        0        0      756 2023-05-16 21:23:04.000000 simplesystray-0.0.6/tests/test.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/systrayv2.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simplesystray-0.0.7/src/simplesystray/__init__.py
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 simplesystray-0.0.7/src/simplesystray/traybar.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 simplesystray-0.0.7/src/simplesystray/win32_adapter.py
+-rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 simplesystray-0.0.7/tests/test.ico
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 simplesystray-0.0.7/tests/test.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 simplesystray-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 simplesystray-0.0.7/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 simplesystray-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 simplesystray-0.0.7/PKG-INFO
```

### Comparing `simplesystray-0.0.6/LICENSE` & `simplesystray-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.6/PKG-INFO` & `simplesystray-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: simplesystray
-Version: 0.0.6
-Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
-Author-email: actorpus <alex@actorpus.com>
-Project-URL: Homepage, https://github.com/actorpus/systrayv2
-Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
 To install simplesystray, run:
```

### Comparing `simplesystray-0.0.6/README.md` & `simplesystray-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,142 +1,156 @@
-# `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
-
-This module implements a Windows system tray icon with a right-click context menu.
-
-## Installation
-
-To install simplesystray, run:
-
-```
-pip install simplesystray
-```
-
-## Usage
-
-### Creating an icon with one option in the context menu:
-
-```python
-from simplesystray import SysTrayIcon
-
-def say_hello(systray):
-    print("Hello, World!")
-    
-menu_options = (("Say Hello", "hello.ico", say_hello),)
-systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
-systray.start()
-```
-
-The first parameter to SysTrayIcon is a path to the icon to show in the systray. If the icon is not found, or
-if None is specified, a default system icon will be displayed.
-The second parameter is the hover text to show when the mouse is hovered over the systray icon.
-The traybar will run in its own thread, so the using script can continue to run.
-
-For the parameters of `menu_options`: cf the section **Menu** below
-
-### Updating : icon, hover text and/or menu options
-The icon and/or hover text and/or menu options can be updated using the update() method with the appropriate `hover_text` or `icon` or  `menu_options` keyword argument:
-
-#### Updating the hover_text:
-```python
-for item in ['item1', 'item2', 'item3']:
-    systray.update(hover_text=item)
-    do_something(item)
-```
-
-#### Updating the menu options:
-```python
-def say_hello(systray):
-    systray.update(menu_options=menu_optionsbye)
-    
-def say_bye(systray):
-    systray.update(menu_options=menu_optionshello)
-    
-menu_optionshello = (("Say Hello","hello.ico", say_hello),)
-menu_optionsbye = (("Say Bye", "bye.ico", say_bye),)
-systray = SysTrayIcon("icon.ico", "Hello/Bye", menu_optionshello)   
-systray.start()
-```
-
-### Shutting down
-To destroy the icon when the program ends, call
-
-```python
-systray.shutdown()
-```
-
-SysTrayIcon can be used as a context manager to start and shutdown the tray, which also prevents hung tray threads should the parent thread fail or otherwise not close the tray process:
-
-```python
-with SysTrayIcon(icon, hover_text) as systray:
-    for item in ['item1', 'item2', 'item3']:
-        systray.update(hover_text=item)
-        do_something(item)
-```
-
-A "Quit" command is always appended to the end of the icon context menu, after the menu options specified by the user.
-To perform operations when Quit is selected, pass "on_quit=callback" as a parameter, e.g.:
-
-```python
-def on_quit_callback(systray):
-    program.shutdown()
-    
-systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options, on_quit=on_quit_callback)
-```
-
-When the user double-clicks the systray icon, the first option specified in menu_options will be executed. The default
-command may be changed to a different option by setting the parameter "default_menu_index", e.g.:
-
-```python
-systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options, default_menu_index=2)
-```
-
-menu_options must be a list of 3-tuples. Each 3-tuple specifies a context menu options. The first value in each tuple
-is the context menu string.
-Some versions of Windows can show icons next to each option in the context menu. This icon can be specified in
-the second value of the tuples. If None is passed, no icon is displayed for the option.
-The third value is the command to execute when the context menu is selected by the user.
-
-It is possible to create sub-menus in the context menu by recursively passing a list of 3-tuple options as the third
-value of an option, instead of passing a callback function. e.g.
-
-```python
-from simplesystray import SysTrayIcon
-
-hover_text = "SysTrayIcon Demo"
-
-
-def hello(sysTrayIcon):
-    print("Hello World.")
-    
-def simon(sysTrayIcon):
-    print("Hello Simon.")
-    
-def bye(sysTrayIcon):
-    print('Bye, then.')
-    
-def do_nothing(sysTrayIcon):
-    pass
-
-
-menu_options = (('Say Hello', "hello.ico", hello),
-                ('Do nothing', None, do_nothing),
-                ('A sub-menu', "submenu.ico", (('Say Hello to Simon', "simon.ico", simon),
-                                               ('Do nothing', None, do_nothing),
-                                              ))
-               )
-
-sysTrayIcon = SysTrayIcon("main.ico", hover_text, menu_options, on_quit=bye, default_menu_index=1)
-sysTrayIcon.start()
-```
-
-Note that in the previous examples, if no code is executed after calling systray.start(), the main thread will
-exit and the icon thread will continue to exist until the Quit option is selected. In order to catch keyboard
-interrupts, some code must be written that will call systray.shutdown when the program should quit.
-Using SysTrayIcon as a context manager automates the start and shutdown of the tray.
-
-This module can only be used in Windows systems, otherwise the import statement will fail.
-
-## Credit
-
-This module is adapted from an implementation by Infinidat Ltd. this was a clone on Simon Brunning's version, which in turn was adapted from Mark Hammond's
-win32gui_taskbar.py and win32gui_menu.py demos from PyWin32.
-
+Metadata-Version: 2.1
+Name: simplesystray
+Version: 0.0.7
+Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
+Project-URL: Homepage, https://github.com/actorpus/systrayv2
+Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
+Author-email: actorpus <alex@actorpus.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
+
+This module implements a Windows system tray icon with a right-click context menu.
+
+## Installation
+
+To install simplesystray, run:
+
+```
+pip install simplesystray
+```
+
+## Usage
+
+### Creating an icon with one option in the context menu:
+
+```python
+from simplesystray import SysTrayIcon
+
+def say_hello(systray):
+    print("Hello, World!")
+    
+menu_options = (("Say Hello", "hello.ico", say_hello),)
+systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
+systray.start()
+```
+
+The first parameter to SysTrayIcon is a path to the icon to show in the systray. If the icon is not found, or
+if None is specified, a default system icon will be displayed.
+The second parameter is the hover text to show when the mouse is hovered over the systray icon.
+The traybar will run in its own thread, so the using script can continue to run.
+
+For the parameters of `menu_options`: cf the section **Menu** below
+
+### Updating : icon, hover text and/or menu options
+The icon and/or hover text and/or menu options can be updated using the update() method with the appropriate `hover_text` or `icon` or  `menu_options` keyword argument:
+
+#### Updating the hover_text:
+```python
+for item in ['item1', 'item2', 'item3']:
+    systray.update(hover_text=item)
+    do_something(item)
+```
+
+#### Updating the menu options:
+```python
+def say_hello(systray):
+    systray.update(menu_options=menu_optionsbye)
+    
+def say_bye(systray):
+    systray.update(menu_options=menu_optionshello)
+    
+menu_optionshello = (("Say Hello","hello.ico", say_hello),)
+menu_optionsbye = (("Say Bye", "bye.ico", say_bye),)
+systray = SysTrayIcon("icon.ico", "Hello/Bye", menu_optionshello)   
+systray.start()
+```
+
+### Shutting down
+To destroy the icon when the program ends, call
+
+```python
+systray.shutdown()
+```
+
+SysTrayIcon can be used as a context manager to start and shutdown the tray, which also prevents hung tray threads should the parent thread fail or otherwise not close the tray process:
+
+```python
+with SysTrayIcon(icon, hover_text) as systray:
+    for item in ['item1', 'item2', 'item3']:
+        systray.update(hover_text=item)
+        do_something(item)
+```
+
+A "Quit" command is always appended to the end of the icon context menu, after the menu options specified by the user.
+To perform operations when Quit is selected, pass "on_quit=callback" as a parameter, e.g.:
+
+```python
+def on_quit_callback(systray):
+    program.shutdown()
+    
+systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options, on_quit=on_quit_callback)
+```
+
+When the user double-clicks the systray icon, the first option specified in menu_options will be executed. The default
+command may be changed to a different option by setting the parameter "default_menu_index", e.g.:
+
+```python
+systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options, default_menu_index=2)
+```
+
+menu_options must be a list of 3-tuples. Each 3-tuple specifies a context menu options. The first value in each tuple
+is the context menu string.
+Some versions of Windows can show icons next to each option in the context menu. This icon can be specified in
+the second value of the tuples. If None is passed, no icon is displayed for the option.
+The third value is the command to execute when the context menu is selected by the user.
+
+It is possible to create sub-menus in the context menu by recursively passing a list of 3-tuple options as the third
+value of an option, instead of passing a callback function. e.g.
+
+```python
+from simplesystray import SysTrayIcon
+
+hover_text = "SysTrayIcon Demo"
+
+
+def hello(sysTrayIcon):
+    print("Hello World.")
+    
+def simon(sysTrayIcon):
+    print("Hello Simon.")
+    
+def bye(sysTrayIcon):
+    print('Bye, then.')
+    
+def do_nothing(sysTrayIcon):
+    pass
+
+
+menu_options = (('Say Hello', "hello.ico", hello),
+                ('Do nothing', None, do_nothing),
+                ('A sub-menu', "submenu.ico", (('Say Hello to Simon', "simon.ico", simon),
+                                               ('Do nothing', None, do_nothing),
+                                              ))
+               )
+
+sysTrayIcon = SysTrayIcon("main.ico", hover_text, menu_options, on_quit=bye, default_menu_index=1)
+sysTrayIcon.start()
+```
+
+Note that in the previous examples, if no code is executed after calling systray.start(), the main thread will
+exit and the icon thread will continue to exist until the Quit option is selected. In order to catch keyboard
+interrupts, some code must be written that will call systray.shutdown when the program should quit.
+Using SysTrayIcon as a context manager automates the start and shutdown of the tray.
+
+This module can only be used in Windows systems, otherwise the import statement will fail.
+
+## Credit
+
+This module is adapted from an implementation by Infinidat Ltd. this was a clone on Simon Brunning's version, which in turn was adapted from Mark Hammond's
+win32gui_taskbar.py and win32gui_menu.py demos from PyWin32.
+
```

### Comparing `simplesystray-0.0.6/pyproject.toml` & `simplesystray-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 [project]
 name = "simplesystray"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="actorpus", email="alex@actorpus.com" },
 ]
 description = "Adds support for a simple icon on the system tray, clone of infi-systray but maintained"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplesystray-0.0.6/src/simplesystray/traybar.py` & `simplesystray-0.0.7/src/simplesystray/traybar.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.6/src/simplesystray/win32_adapter.py` & `simplesystray-0.0.7/src/simplesystray/win32_adapter.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.6/tests/test.py` & `simplesystray-0.0.7/tests/test.py`

 * *Files identical despite different names*

