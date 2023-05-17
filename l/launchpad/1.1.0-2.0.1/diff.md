# Comparing `tmp/launchpad-1.1.0.tar.gz` & `tmp/launchpad-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\launchpad-1.1.0.tar", last modified: Tue May 18 06:34:45 2021, max compression
+gzip compressed data, was "C:\Users\mikem\Documents\techdev\launchpad\dist\.tmp-ixho78k1\launchpad-2.0.1.tar", last modified: Wed May 17 07:52:30 2023, max compression
```

## Comparing `launchpad-1.1.0.tar` & `launchpad-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-05-18 06:34:45.000000 launchpad-1.1.0/
--rw-rw-rw-   0        0        0     5127 2021-05-18 06:34:45.000000 launchpad-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3650 2021-05-18 06:22:40.000000 launchpad-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad/
--rw-rw-rw-   0        0        0     1303 2021-05-18 06:25:16.000000 launchpad-1.1.0/launchpad/__init__.py
--r--r--r--   0        0        0     6463 2021-03-25 10:31:22.000000 launchpad-1.1.0/launchpad/core.py
-drwxrwxrwx   0        0        0        0 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad.egg-info/
--rw-rw-rw-   0        0        0     5127 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-05-18 06:34:45.000000 launchpad-1.1.0/launchpad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-18 06:34:45.000000 launchpad-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      961 2021-05-18 06:26:35.000000 launchpad-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:52:30.000000 launchpad-2.0.1/
+-rw-rw-rw-   0        0        0     1096 2023-05-16 14:45:34.000000 launchpad-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4188 2023-05-17 07:52:30.000000 launchpad-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3650 2023-05-16 14:45:34.000000 launchpad-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad/
+-rw-rw-rw-   0        0        0     1350 2023-05-17 06:46:58.000000 launchpad-2.0.1/launchpad/__init__.py
+-rw-rw-rw-   0        0        0      574 2023-05-17 07:14:33.000000 launchpad-2.0.1/launchpad/constants.py
+-rw-rw-rw-   0        0        0     6244 2023-05-17 07:17:07.000000 launchpad-2.0.1/launchpad/core.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad.egg-info/
+-rw-rw-rw-   0        0        0     4188 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 07:52:30.000000 launchpad-2.0.1/launchpad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:52:30.000000 launchpad-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-05-17 07:11:26.000000 launchpad-2.0.1/setup.py
```

### Comparing `launchpad-1.1.0/PKG-INFO` & `launchpad-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,128 @@
 Metadata-Version: 2.1
 Name: launchpad
-Version: 1.1.0
+Version: 2.0.1
 Summary: Launchpad represents a small factory and a distinct abstract for defining actionable items
 Home-page: https://github.com/mikemalinowski/launchpad
 Author: Mike Malinowski
 Author-email: mike.malinowski@outlook.com
-License: UNKNOWN
-Description: 
-        # Overview
-        
-        
-        Launchpad represents a small factory and a distinct abstract for defining
-        actionable items. This is particularly useful when creating libraries of
-        tools or processes which need to be exposed and invokable.
-        
-        Each action contains general details such as name, description etc as well
-        as some richer functionality to invoke the action or for the action to expose
-        further sub-actions or properties.
-        
-        As the LaunchPad class is just a factory its population is dynamic based
-        upon the paths your feed it (or expose through the LAUNCHPAD_PLUGIN_PATHS
-        variable).
-        
-        An example of use might be...
-        
-        ```python
-        import launchpad
-        
-        # -- Instance launchpad, this gives access to all the
-        # -- actions
-        lp = launchpad.LaunchPad('/usr/my_actions')
-        
-        # -- We can cycle over all the actions
-        for action in lp.identifiers():
-            print(action)
-        
-            # -- We can get an action and run it
-            lp.request(action).run()
-        
-        # -- We can access actions direclty too
-        action = lp.request('My Action Name')
-        action.run()
-        ```
-        
-        # Installation
-        
-        If you use pip, you can simply run ```pip install launchpad```. That will 
-        pull down the required dependencies (scribble & factories) automatically.
-        
-        Note: If you install ```launchpanel``` this module will be pulled down
-        automatically as a dependency. Therefore you only need to pull down this
-        module explicitly if you do not plan to utilise the launchpanel ui.
-        
-        # The Abstract
-        
-        To define an action you must implement a Launch Action. The process of 
-        implementing an action is just a case of creating a python file and inheriting
-        from the LaunchAction object, like this:
-        
-        ```python
-        import launchpad
-        
-        # ------------------------------------------------------------------------------
-        class MyAction(launchpad):
-            Name = ''
-            Description = __doc__
-            Icon = ''
-            Groups = []
-        
-            @classmethod
-            def run(cls):
-                pass
-        
-            @classmethod
-            def actions(cls):
-                return dict()
-        
-            @classmethod
-            def properties(cls):
-                return dict()
-        
-            @classmethod
-            def viability(cls):
-                return cls.VALID
-        
-        ```
-        
-        The properties are very much about giving descriptive information about your
-        action. Description, Icon and Groups are all optional and can be left out
-        entirely if desired - but Name must always be filled in.
-        
-        __run()__ is where you perform the default action for this action.
-        
-        __actions()__ allows you to return a dictionary of key value pairs where the
-        key is the action label and the value is the function/callable. This allows
-        you to give your action variations or extended behaviour which is accessible
-        in a consistent way.
-        
-        __viability()__ is the mechanism to give an indiciation as to whether your 
-        action is valid within the current environment. For example, if your action
-        relies on paths existing, or environment variables being set, you can run those
-        tests there are return the Action Viability (VALID, INVALID, DISABLED).
-        
-        __properties()__ is a mechanism for storing blind data. It should always return
-        a dictionary but there is not formal structure for that dictionary. This is
-        implemented to give you the oppotunity to store tool specific data within the 
-        action depending upon your needs.
-        
-        
-        # Credits & Collaboration
-        
-        This module was inspired by some excellent collaborative projects with a 
-        fantastic tech-artist called __Toby Harrison-Banfield__.
-        
-        I am always open to collaboration, so if you spot bugs lets me know, or if
-        you would like to contribute or get involved just shout!
-        
-        
-        # Compatibility
-        
-        Launchpad has been tested under Python 2.7 and Python 3.7 on Windows and Ubuntu.
-        
 Keywords: launch launchpad pad action actions
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Overview
+
+
+Launchpad represents a small factory and a distinct abstract for defining
+actionable items. This is particularly useful when creating libraries of
+tools or processes which need to be exposed and invokable.
+
+Each action contains general details such as name, description etc as well
+as some richer functionality to invoke the action or for the action to expose
+further sub-actions or properties.
+
+As the LaunchPad class is just a factory its population is dynamic based
+upon the paths your feed it (or expose through the LAUNCHPAD_PLUGIN_PATHS
+variable).
+
+An example of use might be...
+
+```python
+import launchpad
+
+# -- Instance launchpad, this gives access to all the
+# -- actions
+lp = launchpad.LaunchPad('/usr/my_actions')
+
+# -- We can cycle over all the actions
+for action in lp.identifiers():
+    print(action)
+
+    # -- We can get an action and run it
+    lp.request(action).run()
+
+# -- We can access actions direclty too
+action = lp.request('My Action Name')
+action.run()
+```
+
+# Installation
+
+If you use pip, you can simply run ```pip install launchpad```. That will 
+pull down the required dependencies (scribble & factories) automatically.
+
+Note: If you install ```launchpanel``` this module will be pulled down
+automatically as a dependency. Therefore you only need to pull down this
+module explicitly if you do not plan to utilise the launchpanel ui.
+
+# The Abstract
+
+To define an action you must implement a Launch Action. The process of 
+implementing an action is just a case of creating a python file and inheriting
+from the LaunchAction object, like this:
+
+```python
+import launchpad
+
+# ------------------------------------------------------------------------------
+class MyAction(launchpad):
+    Name = ''
+    Description = __doc__
+    Icon = ''
+    Groups = []
+
+    @classmethod
+    def run(cls):
+        pass
+
+    @classmethod
+    def actions(cls):
+        return dict()
+
+    @classmethod
+    def properties(cls):
+        return dict()
+
+    @classmethod
+    def viability(cls):
+        return cls.VALID
+
+```
+
+The properties are very much about giving descriptive information about your
+action. Description, Icon and Groups are all optional and can be left out
+entirely if desired - but Name must always be filled in.
+
+__run()__ is where you perform the default action for this action.
+
+__actions()__ allows you to return a dictionary of key value pairs where the
+key is the action label and the value is the function/callable. This allows
+you to give your action variations or extended behaviour which is accessible
+in a consistent way.
+
+__viability()__ is the mechanism to give an indiciation as to whether your 
+action is valid within the current environment. For example, if your action
+relies on paths existing, or environment variables being set, you can run those
+tests there are return the Action Viability (VALID, INVALID, DISABLED).
+
+__properties()__ is a mechanism for storing blind data. It should always return
+a dictionary but there is not formal structure for that dictionary. This is
+implemented to give you the oppotunity to store tool specific data within the 
+action depending upon your needs.
+
+
+# Credits & Collaboration
+
+This module was inspired by some excellent collaborative projects with a 
+fantastic tech-artist called __Toby Harrison-Banfield__.
+
+I am always open to collaboration, so if you spot bugs lets me know, or if
+you would like to contribute or get involved just shout!
+
+
+# Compatibility
+
+Launchpad has been tested under Python 2.7 and Python 3.7 on Windows and Ubuntu.
```

### Comparing `launchpad-1.1.0/README.md` & `launchpad-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `launchpad-1.1.0/launchpad/__init__.py` & `launchpad-2.0.1/launchpad/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,13 +33,14 @@
 ```
 
 
 # Compatibility
 
 Launchpad has been tested under Python 2.7 and Python 3.7 on Windows and Ubuntu.
 """
-__version__ = "1.1.0"
+__version__ = "2.0.1"
 
 from .core import LaunchPad
 from .core import LaunchAction
-from .core import LAUNCHPAD_PLUGIN_ENVVAR
-from .core import LAUNCHPAD_USER_PLUGIN_DIR
+from .constants import LAUNCHPAD_PLUGIN_ENVVAR
+from .constants import LAUNCHPAD_USER_PLUGIN_DIR
+from .constants import PluginStates
```

### Comparing `launchpad-1.1.0/launchpad/core.py` & `launchpad-2.0.1/launchpad/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,110 +8,108 @@
 further sub-actions or properties.
 
 As the LaunchPad class is just a factory its population is dynamic based
 upon the paths your feed it (or expose through the LAUNCHPAD_PLUGIN_PATHS
 variable).
 """
 import os
-import sys
+import typing
 import factories
 
-
-# -- Define the environment variable we will use when looking
-# -- for plugin paths
-LAUNCHPAD_PLUGIN_ENVVAR = 'LAUNCHPAD_PLUGIN_PATHS'
-
-# -- This is a default location we always look in for user placed
-# -- actions
-LAUNCHPAD_USER_PLUGIN_DIR = os.path.join(
-    os.path.expanduser('~'),
-    '.launchpad',
-)
+from . import constants as c
 
 
 # ------------------------------------------------------------------------------
 class LaunchPad(factories.Factory):
 
     # --------------------------------------------------------------------------
-    def __init__(self, plugin_locations=None):
+    def __init__(self, plugin_locations: typing.List[str] = None):
 
         # -- Define the variable we will use to pass all our
         # -- plugin paths to
-        paths = [LAUNCHPAD_USER_PLUGIN_DIR]
+        paths = [c.LAUNCHPAD_USER_PLUGIN_DIR]
 
         # -- Add any user defined plugin locations
         if plugin_locations:
 
             # -- Quick safety check to ensure we're passing a list
             # -- of locations rather than just a single string
             if not isinstance(plugin_locations, (list, tuple)):
                 plugin_locations = [plugin_locations]
 
             paths.extend(plugin_locations)
 
         # -- Add any paths defined in the environment
-        if LAUNCHPAD_PLUGIN_ENVVAR in os.environ:
+        if c.LAUNCHPAD_PLUGIN_ENVVAR in os.environ:
             paths.extend(
                 [
                     os.path.abspath(path)
-                    for path in os.environ[LAUNCHPAD_PLUGIN_ENVVAR].split(';')
+                    for path in os.environ[c.LAUNCHPAD_PLUGIN_ENVVAR].split(';')
                     if path.strip()
                 ]
             )
 
         # -- Initiate the factory
         super(LaunchPad, self).__init__(
             abstract=LaunchAction,
             plugin_identifier='Name',
             versioning_identifier='Version',
             paths=paths,
         )
 
     # --------------------------------------------------------------------------
-    def identifiers(self):
+    def identifiers(self, show_beta=False) -> typing.List[str]:
         """
         We overload this function because we want to omit any invalid
         actions
 
         :return: list(str, str, ...)
         """
         filtered_actions = list()
+        all_actions = sorted(
+            super(
+                LaunchPad,
+                self,
+            ).identifiers(),
+            key=lambda t: t.lower(),
+        )
 
-        for action_name in sorted(super(LaunchPad, self).identifiers(), key=lambda t: t.lower()):
+        for action_name in all_actions:
             action = self.request(action_name)
+            action_state = action.state()
 
-            if action.viability() != LaunchAction.INVALID:
-                filtered_actions.append(
-                    [
-                        action_name,
-                        action.Priority,
-                    ],
-                )
+            if not show_beta and c.PluginStates.BETA in action_state:
+                continue
 
-        final_results = list()
+            if action.state() == c.PluginStates.INVALID:
+                continue
 
-        for action, _ in sorted(filtered_actions, key=lambda t: t[1], reverse=True):
-            final_results.append(action)
+            filtered_actions.append(action_name)
 
-        return final_results
+        return filtered_actions
 
     # --------------------------------------------------------------------------
-    def grouped_identifiers(self):
+    def grouped_identifiers(self, show_beta=False) -> typing.Dict[str, str]:
         """
         This will create a dictionary of groups, where the keys are the groups
         defined in the actions and the values are lists of identifiers.
 
         :return: dict(group_name: [name, name, name]
         """
         data = {'Uncategorised': list()}
 
         for action in self.plugins():
 
+            action_state = action.state()
+
+            if not show_beta and c.PluginStates.BETA in action_state:
+                continue
+
             # -- Ignore invalid actions
-            if action.viability() == LaunchAction.INVALID:
+            if action.state() != c.PluginStates.INVALID:
                 continue
 
             if action.Groups:
                 for group in action.Groups:
                     if group not in data:
                         data[group] = list()
 
@@ -134,61 +132,47 @@
     Description = __doc__
     Icon = ''
     Groups = []
 
     # -- This allows you to re-implement the same plugin multiple
     # -- times and always get the highest priority plugin
     Version = 0
-    Priority = 0
-
-    # -- This is an enum of validity, which you should not
-    # -- change, but one of these should be returned by the
-    # -- viability method
-    INVALID = 0
-    DISABLED = 1
-    VALID = 2
 
+    # -- This property allows a plugin to override how often the status
+    # -- should be pinged. This is additive on top of the value defined
+    # -- by the user in the settings. For instance, if hte user has a
+    # -- status wait time of five seconds, and this is set to 1000 then this
+    # -- plugin would be checked every six seconds.
     STATUS_DELAY = 0
 
     # --------------------------------------------------------------------------
     @classmethod
-    def run(cls):
+    def run(cls) -> bool:
         """
         This is used to initiate the default action for this plugin.
         """
         pass
 
     # --------------------------------------------------------------------------
     @classmethod
-    def actions(cls):
+    def actions(cls) -> typing.Dict[str, callable]:
         """
         This can return a dictionary of sub-actions for this plugin. The
         format of the dictionary is expected to be dict(label=callable)
         """
         return dict()
 
     # --------------------------------------------------------------------------
     @classmethod
-    def properties(cls):
-        """
-        This allows plugins to utilise blind property data which may be
-        utilised by different interfaces for your specific needs.
-
-        This should return a dictionary of the form dict(prop_name=prop_value)
-        """
-        return dict()
-
-    # --------------------------------------------------------------------------
-    @classmethod
-    def viability(cls):
-        return cls.VALID
+    def state(cls) -> "launchpad.PluginStates":
+        return c.PluginStates.VALID
 
     # --------------------------------------------------------------------------
     @classmethod
-    def status(cls):
+    def status_message(cls) -> str or None:
         """
         This allows for important information to be passed up. Examples may be
         when a user is expected to update a tool etc.
 
         Returning None means the status is normal, any other value will be passed
         up to the user in whichever way is relevant for the view, therefore in most
         cases this should be a string if the status is anything other than normal.
```

### Comparing `launchpad-1.1.0/launchpad.egg-info/PKG-INFO` & `launchpad-2.0.1/launchpad.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,128 @@
 Metadata-Version: 2.1
 Name: launchpad
-Version: 1.1.0
+Version: 2.0.1
 Summary: Launchpad represents a small factory and a distinct abstract for defining actionable items
 Home-page: https://github.com/mikemalinowski/launchpad
 Author: Mike Malinowski
 Author-email: mike.malinowski@outlook.com
-License: UNKNOWN
-Description: 
-        # Overview
-        
-        
-        Launchpad represents a small factory and a distinct abstract for defining
-        actionable items. This is particularly useful when creating libraries of
-        tools or processes which need to be exposed and invokable.
-        
-        Each action contains general details such as name, description etc as well
-        as some richer functionality to invoke the action or for the action to expose
-        further sub-actions or properties.
-        
-        As the LaunchPad class is just a factory its population is dynamic based
-        upon the paths your feed it (or expose through the LAUNCHPAD_PLUGIN_PATHS
-        variable).
-        
-        An example of use might be...
-        
-        ```python
-        import launchpad
-        
-        # -- Instance launchpad, this gives access to all the
-        # -- actions
-        lp = launchpad.LaunchPad('/usr/my_actions')
-        
-        # -- We can cycle over all the actions
-        for action in lp.identifiers():
-            print(action)
-        
-            # -- We can get an action and run it
-            lp.request(action).run()
-        
-        # -- We can access actions direclty too
-        action = lp.request('My Action Name')
-        action.run()
-        ```
-        
-        # Installation
-        
-        If you use pip, you can simply run ```pip install launchpad```. That will 
-        pull down the required dependencies (scribble & factories) automatically.
-        
-        Note: If you install ```launchpanel``` this module will be pulled down
-        automatically as a dependency. Therefore you only need to pull down this
-        module explicitly if you do not plan to utilise the launchpanel ui.
-        
-        # The Abstract
-        
-        To define an action you must implement a Launch Action. The process of 
-        implementing an action is just a case of creating a python file and inheriting
-        from the LaunchAction object, like this:
-        
-        ```python
-        import launchpad
-        
-        # ------------------------------------------------------------------------------
-        class MyAction(launchpad):
-            Name = ''
-            Description = __doc__
-            Icon = ''
-            Groups = []
-        
-            @classmethod
-            def run(cls):
-                pass
-        
-            @classmethod
-            def actions(cls):
-                return dict()
-        
-            @classmethod
-            def properties(cls):
-                return dict()
-        
-            @classmethod
-            def viability(cls):
-                return cls.VALID
-        
-        ```
-        
-        The properties are very much about giving descriptive information about your
-        action. Description, Icon and Groups are all optional and can be left out
-        entirely if desired - but Name must always be filled in.
-        
-        __run()__ is where you perform the default action for this action.
-        
-        __actions()__ allows you to return a dictionary of key value pairs where the
-        key is the action label and the value is the function/callable. This allows
-        you to give your action variations or extended behaviour which is accessible
-        in a consistent way.
-        
-        __viability()__ is the mechanism to give an indiciation as to whether your 
-        action is valid within the current environment. For example, if your action
-        relies on paths existing, or environment variables being set, you can run those
-        tests there are return the Action Viability (VALID, INVALID, DISABLED).
-        
-        __properties()__ is a mechanism for storing blind data. It should always return
-        a dictionary but there is not formal structure for that dictionary. This is
-        implemented to give you the oppotunity to store tool specific data within the 
-        action depending upon your needs.
-        
-        
-        # Credits & Collaboration
-        
-        This module was inspired by some excellent collaborative projects with a 
-        fantastic tech-artist called __Toby Harrison-Banfield__.
-        
-        I am always open to collaboration, so if you spot bugs lets me know, or if
-        you would like to contribute or get involved just shout!
-        
-        
-        # Compatibility
-        
-        Launchpad has been tested under Python 2.7 and Python 3.7 on Windows and Ubuntu.
-        
 Keywords: launch launchpad pad action actions
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Overview
+
+
+Launchpad represents a small factory and a distinct abstract for defining
+actionable items. This is particularly useful when creating libraries of
+tools or processes which need to be exposed and invokable.
+
+Each action contains general details such as name, description etc as well
+as some richer functionality to invoke the action or for the action to expose
+further sub-actions or properties.
+
+As the LaunchPad class is just a factory its population is dynamic based
+upon the paths your feed it (or expose through the LAUNCHPAD_PLUGIN_PATHS
+variable).
+
+An example of use might be...
+
+```python
+import launchpad
+
+# -- Instance launchpad, this gives access to all the
+# -- actions
+lp = launchpad.LaunchPad('/usr/my_actions')
+
+# -- We can cycle over all the actions
+for action in lp.identifiers():
+    print(action)
+
+    # -- We can get an action and run it
+    lp.request(action).run()
+
+# -- We can access actions direclty too
+action = lp.request('My Action Name')
+action.run()
+```
+
+# Installation
+
+If you use pip, you can simply run ```pip install launchpad```. That will 
+pull down the required dependencies (scribble & factories) automatically.
+
+Note: If you install ```launchpanel``` this module will be pulled down
+automatically as a dependency. Therefore you only need to pull down this
+module explicitly if you do not plan to utilise the launchpanel ui.
+
+# The Abstract
+
+To define an action you must implement a Launch Action. The process of 
+implementing an action is just a case of creating a python file and inheriting
+from the LaunchAction object, like this:
+
+```python
+import launchpad
+
+# ------------------------------------------------------------------------------
+class MyAction(launchpad):
+    Name = ''
+    Description = __doc__
+    Icon = ''
+    Groups = []
+
+    @classmethod
+    def run(cls):
+        pass
+
+    @classmethod
+    def actions(cls):
+        return dict()
+
+    @classmethod
+    def properties(cls):
+        return dict()
+
+    @classmethod
+    def viability(cls):
+        return cls.VALID
+
+```
+
+The properties are very much about giving descriptive information about your
+action. Description, Icon and Groups are all optional and can be left out
+entirely if desired - but Name must always be filled in.
+
+__run()__ is where you perform the default action for this action.
+
+__actions()__ allows you to return a dictionary of key value pairs where the
+key is the action label and the value is the function/callable. This allows
+you to give your action variations or extended behaviour which is accessible
+in a consistent way.
+
+__viability()__ is the mechanism to give an indiciation as to whether your 
+action is valid within the current environment. For example, if your action
+relies on paths existing, or environment variables being set, you can run those
+tests there are return the Action Viability (VALID, INVALID, DISABLED).
+
+__properties()__ is a mechanism for storing blind data. It should always return
+a dictionary but there is not formal structure for that dictionary. This is
+implemented to give you the oppotunity to store tool specific data within the 
+action depending upon your needs.
+
+
+# Credits & Collaboration
+
+This module was inspired by some excellent collaborative projects with a 
+fantastic tech-artist called __Toby Harrison-Banfield__.
+
+I am always open to collaboration, so if you spot bugs lets me know, or if
+you would like to contribute or get involved just shout!
+
+
+# Compatibility
+
+Launchpad has been tested under Python 2.7 and Python 3.7 on Windows and Ubuntu.
```

### Comparing `launchpad-1.1.0/setup.py` & `launchpad-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_description = fh.read()
 
 else:
     long_description = short_description
 
 setuptools.setup(
     name='launchpad',
-    version='1.1.0',
+    version='2.0.1',
     author='Mike Malinowski',
     author_email='mike.malinowski@outlook.com',
     description=short_description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mikemalinowski/launchpad',
     packages=setuptools.find_packages(),
```

