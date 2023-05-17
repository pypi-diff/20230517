# Comparing `tmp/launchpanel-1.1.0.tar.gz` & `tmp/launchpanel-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\launchpanel-1.1.0.tar", last modified: Tue May 18 06:35:01 2021, max compression
+gzip compressed data, was "C:\Users\mikem\Documents\techdev\launchpanel\dist\.tmp-dpbehflp\launchpanel-2.0.1.tar", last modified: Wed May 17 07:53:03 2023, max compression
```

## Comparing `launchpanel-1.1.0.tar` & `launchpanel-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2021-05-18 06:35:01.000000 launchpanel-1.1.0/
--rw-rw-rw-   0        0        0     4207 2021-05-18 06:35:01.000000 launchpanel-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2021-05-18 06:28:57.000000 launchpanel-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel/
--rw-rw-rw-   0        0        0     1700 2021-05-18 06:25:20.000000 launchpanel-1.1.0/launchpanel/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel/_resources/
--r--r--r--   0        0        0     3779 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/alert.png
--r--r--r--   0        0        0     2840 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/bg.png
--r--r--r--   0        0        0    15040 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/launch.png
--r--r--r--   0        0        0    11451 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/launchpad.ui
--r--r--r--   0        0        0      628 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/north.qss
--r--r--r--   0        0        0    18972 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/options.png
--r--r--r--   0        0        0    71776 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/splash.png
--r--r--r--   0        0        0      217 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/style.qss
--r--r--r--   0        0        0      568 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/west.qss
--r--r--r--   0        0        0    21463 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard.png
--r--r--r--   0        0        0      106 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard.qss
--r--r--r--   0        0        0     4150 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard_page_five.ui
--r--r--r--   0        0        0     4418 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard_page_four.ui
--r--r--r--   0        0        0     2282 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard_page_one.ui
--r--r--r--   0        0        0     2225 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard_page_three.ui
--r--r--r--   0        0        0     2277 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/_resources/wizard_page_two.ui
--r--r--r--   0        0        0       41 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/constants.py
--r--r--r--   0        0        0    45715 2021-04-26 15:42:49.000000 launchpanel-1.1.0/launchpanel/core.py
--r--r--r--   0        0        0    12295 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/create.py
--r--r--r--   0        0        0      323 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/run.py
--r--r--r--   0        0        0      303 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/run_tray.py
--r--r--r--   0        0        0     2565 2021-04-26 15:42:49.000000 launchpanel-1.1.0/launchpanel/tray.py
--r--r--r--   0        0        0     1133 2021-03-25 10:31:22.000000 launchpanel-1.1.0/launchpanel/utils.py
-drwxrwxrwx   0        0        0        0 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel.egg-info/
--rw-rw-rw-   0        0        0     4207 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      949 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-05-18 06:35:01.000000 launchpanel-1.1.0/launchpanel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-18 06:35:01.000000 launchpanel-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1109 2021-05-18 06:29:31.000000 launchpanel-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:53:03.000000 launchpanel-2.0.1/
+-rw-rw-rw-   0        0        0     1096 2023-05-16 14:45:45.000000 launchpanel-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-05-17 07:53:03.000000 launchpanel-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2023-05-16 14:45:45.000000 launchpanel-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 07:53:03.000000 launchpanel-2.0.1/launchpanel/
+-rw-rw-rw-   0        0        0     1700 2023-05-16 14:58:31.000000 launchpanel-2.0.1/launchpanel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:53:03.000000 launchpanel-2.0.1/launchpanel/_resources/
+-rw-rw-rw-   0        0        0     3779 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/alert.png
+-rw-rw-rw-   0        0        0     2840 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/bg.png
+-rw-rw-rw-   0        0        0    15040 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/launch.png
+-rw-rw-rw-   0        0        0    12722 2023-05-17 06:45:23.000000 launchpanel-2.0.1/launchpanel/_resources/launchpad.ui
+-rw-rw-rw-   0        0        0      628 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/north.qss
+-rw-rw-rw-   0        0        0    18972 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/options.png
+-rw-rw-rw-   0        0        0    71776 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/splash.png
+-rw-rw-rw-   0        0        0      217 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/style.qss
+-rw-rw-rw-   0        0        0      568 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/west.qss
+-rw-rw-rw-   0        0        0    21463 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard.png
+-rw-rw-rw-   0        0        0      106 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard.qss
+-rw-rw-rw-   0        0        0     4150 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard_page_five.ui
+-rw-rw-rw-   0        0        0     4418 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard_page_four.ui
+-rw-rw-rw-   0        0        0     2282 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard_page_one.ui
+-rw-rw-rw-   0        0        0     2225 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard_page_three.ui
+-rw-rw-rw-   0        0        0     2277 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/_resources/wizard_page_two.ui
+-rw-rw-rw-   0        0        0       41 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/constants.py
+-rw-rw-rw-   0        0        0    46821 2023-05-17 07:18:16.000000 launchpanel-2.0.1/launchpanel/core.py
+-rw-rw-rw-   0        0        0    12295 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/create.py
+-rw-rw-rw-   0        0        0      323 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/run.py
+-rw-rw-rw-   0        0        0      303 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/run_tray.py
+-rw-rw-rw-   0        0        0     2570 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/tray.py
+-rw-rw-rw-   0        0        0     1410 2023-05-16 14:45:45.000000 launchpanel-2.0.1/launchpanel/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:53:03.000000 launchpanel-2.0.1/launchpanel.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-05-17 07:53:02.000000 launchpanel-2.0.1/launchpanel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      957 2023-05-17 07:53:03.000000 launchpanel-2.0.1/launchpanel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:53:02.000000 launchpanel-2.0.1/launchpanel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-17 07:53:02.000000 launchpanel-2.0.1/launchpanel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 07:53:02.000000 launchpanel-2.0.1/launchpanel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:53:03.000000 launchpanel-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2023-05-17 07:11:26.000000 launchpanel-2.0.1/setup.py
```

### Comparing `launchpanel-1.1.0/README.md` & `launchpanel-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/__init__.py` & `launchpanel-2.0.1/launchpanel/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,12 +58,12 @@
     * scribble (pip install scribble)
 
 
 # Compatibility
 
 Launchpad has been tested under Python 2.7 and Python 3.7 on Windows and Ubuntu.
 """
-__version__ = "1.1.0"
+__version__ = "2.0.1"
 
 from .core import launch
 from . import utils
 from .tray import launch_tray
```

### Comparing `launchpanel-1.1.0/launchpanel/_resources/alert.png` & `launchpanel-2.0.1/launchpanel/_resources/alert.png`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/bg.png` & `launchpanel-2.0.1/launchpanel/_resources/bg.png`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/launch.png` & `launchpanel-2.0.1/launchpanel/_resources/launch.png`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/launchpad.ui` & `launchpanel-2.0.1/launchpanel/_resources/launchpad.ui`

 * *Files 3% similar despite different names*

#### Comparing `launchpanel-1.1.0/launchpanel/_resources/launchpad.ui` & `launchpanel-2.0.1/launchpanel/_resources/launchpad.ui`

```diff
@@ -13,15 +13,24 @@
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout_2">
       <property name="spacing">
         <number>0</number>
       </property>
-      <property name="margin">
+      <property name="leftMargin">
+        <number>0</number>
+      </property>
+      <property name="topMargin">
+        <number>0</number>
+      </property>
+      <property name="rightMargin">
+        <number>0</number>
+      </property>
+      <property name="bottomMargin">
         <number>0</number>
       </property>
       <item>
         <layout class="QVBoxLayout" name="verticalLayout">
           <property name="spacing">
             <number>0</number>
           </property>
@@ -52,15 +61,24 @@
                 <attribute name="title">
                   <string/>
                 </attribute>
                 <layout class="QVBoxLayout" name="verticalLayout_8">
                   <property name="spacing">
                     <number>0</number>
                   </property>
-                  <property name="margin">
+                  <property name="leftMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="topMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="rightMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="bottomMargin">
                     <number>0</number>
                   </property>
                   <item>
                     <widget class="QScrollArea" name="scrollArea">
                       <property name="widgetResizable">
                         <bool>true</bool>
                       </property>
@@ -138,14 +156,32 @@
                                                   <number>60</number>
                                                 </property>
                                               </widget>
                                             </item>
                                           </layout>
                                         </item>
                                         <item>
+                                          <layout class="QHBoxLayout" name="horizontalLayout_6" stretch="1,0">
+                                            <item>
+                                              <widget class="QLabel" name="label_5">
+                                                <property name="text">
+                                                  <string>Show Beta Actions</string>
+                                                </property>
+                                              </widget>
+                                            </item>
+                                            <item>
+                                              <widget class="QCheckBox" name="showBeta">
+                                                <property name="text">
+                                                  <string/>
+                                                </property>
+                                              </widget>
+                                            </item>
+                                          </layout>
+                                        </item>
+                                        <item>
                                           <layout class="QHBoxLayout" name="horizontalLayout_5" stretch="1,0">
                                             <item>
                                               <widget class="QLabel" name="label_4">
                                                 <property name="text">
                                                   <string>Status Check Interval (seconds)</string>
                                                 </property>
                                               </widget>
```

### Comparing `launchpanel-1.1.0/launchpanel/_resources/north.qss` & `launchpanel-2.0.1/launchpanel/_resources/north.qss`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/options.png` & `launchpanel-2.0.1/launchpanel/_resources/options.png`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/splash.png` & `launchpanel-2.0.1/launchpanel/_resources/splash.png`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/west.qss` & `launchpanel-2.0.1/launchpanel/_resources/west.qss`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/wizard.png` & `launchpanel-2.0.1/launchpanel/_resources/wizard.png`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/wizard_page_five.ui` & `launchpanel-2.0.1/launchpanel/_resources/wizard_page_five.ui`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/wizard_page_four.ui` & `launchpanel-2.0.1/launchpanel/_resources/wizard_page_four.ui`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/wizard_page_one.ui` & `launchpanel-2.0.1/launchpanel/_resources/wizard_page_one.ui`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/wizard_page_three.ui` & `launchpanel-2.0.1/launchpanel/_resources/wizard_page_three.ui`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/_resources/wizard_page_two.ui` & `launchpanel-2.0.1/launchpanel/_resources/wizard_page_two.ui`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/core.py` & `launchpanel-2.0.1/launchpanel/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import ctypes
 import scribble
 import launchpad
 import functools
 import collections
 
 from . import create
-from . import constants
+from . import constants as c
 
 
 # ------------------------------------------------------------------------------
 def _get_resource(name):
     """
     This is a convinience function to get files from the resources directory
     and correct handle the slashing.
@@ -90,15 +90,15 @@
         # -- Set the window properties
         self.setWindowTitle('Launch Panel')
         self.setWindowIcon(qute.QIcon(_get_resource('launch.png')))
 
         # -- If we're on windows we need to tell windows that python is actually just
         # -- hosting an application and is not the application itself.
         if sys.platform == 'win32':
-            ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(constants.APP_ID)
+            ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(c.APP_ID)
 
         # -- Create a default layout
         self.setLayout(qute.slimify(qute.QVBoxLayout()))
         
         # -- Load in the ui
         self.ui = qute.loadUi(_get_resource('launchpad.ui'))
         self.layout().addWidget(self.ui)
@@ -138,14 +138,15 @@
             )
         )
 
         # -- Update the icon size variable to reflect what it actually
         # -- is
         self.ui.iconSize.setValue(settings.get('icon_size', 50))
         self.ui.statusInterval.setValue(settings.get('status_inverval', 1800))
+        self.ui.showBeta.setChecked(settings.get('show_beta', False))
 
         # -- Combine any paths we're given with any stored paths
         # -- and then ensure we remove any duplicates
         stored_plugin_paths = settings.get('plugin_locations', [])
         stored_plugin_paths.extend(plugin_locations or list())
         stored_plugin_paths = list(set(stored_plugin_paths))
 
@@ -184,14 +185,15 @@
         self.ui.iconSize.valueChanged.connect(self.resizeIcons)
         self.ui.addPluginPath.clicked.connect(self.addPluginPath)
         self.ui.actionWizard.clicked.connect(self.initiateWizard)
         self.ui.tabPanel.currentChanged.connect(self.storeActiveTab)
         self.ui.removePluginPath.clicked.connect(self.removePluginPath)
         self.ui.tabModeCombo.currentIndexChanged.connect(self.setTabMode)
         self.ui.statusInterval.valueChanged.connect(self.updateStatusInterval)
+        self.ui.showBeta.stateChanged.connect(self.toggleBetaPlugins)
 
         # -- Begin with a status check
         self.performStatusCheck()
 
     # --------------------------------------------------------------------------
     def setTabMode(self, tab_mode=None):
         """
@@ -281,41 +283,46 @@
         settings = scribble.get(self.environment_id)
 
         # -- Now we can begin populating all the tabs. We start by adding
         # -- the persistent 'All' tab which shows all actions
         widget = ActionListWidget(
             factory=self.factory,
             action_list=None,
+            show_beta=self.ui.showBeta.isChecked(),
             size=settings.get('icon_size', 75),
             parent=self,
         )
         self._action_lists.append(widget)
 
         # -- Add the tab into the ui
         self.ui.tabPanel.insertTab(
             0,
             widget,
             'All',
         )
 
         # -- We now need to cycle over all the grouped identifiers
         # -- and create a ListWidget containing them.
-        groups = self.factory.grouped_identifiers()
+        groups = self.factory.grouped_identifiers(
+            show_beta=self.ui.showBeta.isChecked(),
+        )
+
         group_names = reversed(sorted(list(groups.keys())))
 
         for group_name in group_names:
 
             # -- We do not show uncategorised items. They will
             # -- show in the 'All' tab
             if group_name == 'Uncategorised':
                 continue
 
             widget = ActionListWidget(
                 factory=self.factory,
                 action_list=groups[group_name],
+                show_beta=self.ui.showBeta.isChecked(),
                 size=settings.get('icon_size', 75),
                 parent=self,
             )
 
             # -- Hook up event signals specific to this widget type
             widget.alertPropogation.connect(self.updateTabState)
 
@@ -348,14 +355,15 @@
         if not user_picked_actions:
             return
 
         # -- Build the tab
         widget = ActionListWidget(
             factory=self.factory,
             action_list=user_picked_actions,
+            show_beta=self.ui.showBeta.isChecked(),
             size=settings.get('icon_size', 75),
             parent=self,
         )
 
         # -- Hook up event signals specific to this widget type
         widget.alertPropogation.connect(self.updateTabState)
 
@@ -493,14 +501,24 @@
         # -- If no tab information is stored we do not do anything
         if not tab_name:
             return
 
         # -- Cycle our tabs, and attempt to match it via name
         self._setTabByName(tab_name)
 
+    # ----------------------------------------------------------------------------------
+    def toggleBetaPlugins(self):
+
+        settings = scribble.get(self.environment_id)
+        settings['show_beta'] = self.ui.showBeta.isChecked()
+        settings.save()
+
+        self.populate()
+        self.populateUserActions()
+
     # --------------------------------------------------------------------------
     def resizeIcons(self, icon_size=None):
         """
         Resizes the icons to the given size (or to the ui settings if no
         size is given). All changes through this method will be stored
         ready for the next run.
 
@@ -641,20 +659,21 @@
     launchpad factory and list of actions to be shown.
     """
     # -- This signal is used to alert that changes in
     # -- state have occured
     alertPropogation = qute.Signal(object)
 
     # --------------------------------------------------------------------------
-    def __init__(self, factory, action_list, size=75, parent=None):
+    def __init__(self, factory, action_list, show_beta=False, size=75, parent=None):
         super(ActionListWidget, self).__init__(parent=parent)
 
         # -- store the launch panel
         self._launch_panel = parent
         self._parent = parent
+        self._show_beta = show_beta
 
         # -- This variable can be used to query whether this widget has any items
         # -- within it which have alerts
         self.status_threads = list()
         self.status_tracker = dict()
 
         # -- Define some optimisation variables
@@ -667,15 +686,15 @@
         self.setSortingEnabled(False)
         self.setMouseTracking(True)
         self.setSelectionMode(self.NoSelection)
         self.setContextMenuPolicy(qute.Qt.DefaultContextMenu)
 
         # -- Store our factory and list of actions
         self.factory = factory
-        self.action_list = action_list or factory.identifiers()
+        self.action_list = action_list or factory.identifiers(show_beta=show_beta)
 
         # -- Populate the panel
         self.populate()
 
         self.setStyleSheet(
             """
                 background-image: url(%s);
@@ -692,15 +711,17 @@
     # --------------------------------------------------------------------------
     def populate(self):
         """
         This will populate the list widget with all the elements defined
         in the action list during initialisation.
         """
         self.clear()
-        valid_actions = self.factory.identifiers()
+        valid_actions = self.factory.identifiers(
+            show_beta=self._show_beta
+        )
 
         # -- Start by adding all the required items
         for idx, action_name in enumerate(self.action_list):
 
             if action_name not in valid_actions:
                 continue
 
@@ -755,14 +776,19 @@
         """
 
         # -- pass a NoneType item
         if not item:
             return
 
         action = self.factory.request(item.identifier)
+
+        # -- check we have not disabled the action
+        if launchpad.PluginStates.DISABLED in action.state():
+            return
+
         action.run()
 
         # -- Trigger a status check for this item
         self._parent.performStatusCheckOfActionType(item.identifier)
 
     # --------------------------------------------------------------------------
     def mousePressEvent(self, event):
@@ -923,15 +949,15 @@
             # -- Ensure we remove this thread once we're done with it
             threads_to_remove.append(thread)
 
             thread.delegate.requires_attention = thread.status
 
             # -- Update the tooltip. If there is no alert state it can
             # -- simply by blank
-            thread.item.setToolTip(thread.status)
+            thread.item.setToolTip(str(thread.status))
             thread.item.status = thread.status
 
             # -- Finally we trigger a redraw of this item
             self.update(self.indexFromItem(thread.item))
 
             # -- If the status is different we need to emit a status
             # -- change
@@ -985,15 +1011,15 @@
 
     # --------------------------------------------------------------------------
     def __init__(self, action, size, parent=None):
         super(ActionDelegate, self).__init__(parent=parent)
 
         # -- Store the action, as this is used during painting
         self.action = action
-        self.viability = action.viability()
+        self.state = action.state()
         self.requires_attention = False
 
         # -- Extract the icon, and create the pixmaps for the
         # -- icons
         self.icon_colour = None
         self.icon_bw = None
         self.size = size
@@ -1094,16 +1120,16 @@
         # -- defaults
         hovering = False
         icon_opacity = 0.5
         icon_px = self.icon_bw
 
         # -- If we're hovering lets increase the opacity and use
         # -- the colour icon
-        disabled = self.viability == launchpad.LaunchAction.DISABLED
-
+        disabled =  launchpad.PluginStates.DISABLED in self.state
+        print(disabled)
         if option.state & qute.QStyle.State_MouseOver:
             hovering = True
             icon_opacity = 1
             icon_px = self.icon_colour
 
         if disabled:
             icon_opacity = 0.25
@@ -1113,15 +1139,15 @@
             gradient = qute.QLinearGradient(
                 0,
                 option.rect.y(),
                 0,
                 option.rect.y() + option.rect.height(),
             )
 
-            if self.highlight:
+            if self.highlight and not disabled:
                 gradient.setColorAt(0, self.highlight)
                 gradient.setColorAt(1, qute.QColor(0, 0, 0, a=0))
                 painter.setBrush(gradient)
                 painter.setPen(qute.QColor(0, 0, 0, a=0))
                 painter.drawRect(
                     option.rect,
                 )
@@ -1208,19 +1234,24 @@
         self.status = None
 
     # --------------------------------------------------------------------------
     def runAfterDelay(self):
         # -- We're running code from within a plugin, so we wrap it as we
         # -- cannot guarantee its quality
         try:
-            if self.plugin.viability() == self.plugin.VALID:
-                self.status = self.plugin.status()
+            # -- skip any INVALID plugins
+            if self.plugin.state() == launchpad.PluginStates.INVALID:
+                return
+
+            # -- only update the tooltip if we have a Status to report
+            self.status = self.plugin.status_message() or None
 
         except:
             print('Failed to get status for {}'.format(self.item.identifier))
+            print(sys.exc_info())
 
     # --------------------------------------------------------------------------
     def run(self):
         time.sleep(self.plugin.STATUS_DELAY)
         self.runAfterDelay()
 
 
@@ -1235,25 +1266,23 @@
     :return:
     """
     q_app = qute.qApp()
 
     splash_screen = None
 
     if show_splash:
-        # -- Allow the user to give their own splash screen
-        splash_path = _get_resource('splash.png')
-
         try:
             if show_splash and os.path.exists(show_splash):
                 splash_path = show_splash
 
-        except: pass
+                splash_screen = qute.QSplashScreen(splash_path)
+                splash_screen.show()
 
-        splash_screen = qute.QSplashScreen(splash_path)
-        splash_screen.show()
+        except:
+            pass
 
     # -- get any passed args that we can use
     title = kwargs.pop('title', '')
     icon = kwargs.pop('icon', '')
 
     # -- Create a window and embed our widget into it
     launch_widget = LaunchPanel(*args, **kwargs)
```

### Comparing `launchpanel-1.1.0/launchpanel/create.py` & `launchpanel-2.0.1/launchpanel/create.py`

 * *Files identical despite different names*

### Comparing `launchpanel-1.1.0/launchpanel/tray.py` & `launchpanel-2.0.1/launchpanel/tray.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # --------------------------------------------------------------------------
     def updateTabState(self, action_list):
         for idx in range(action_list.count()):
             # -- Get the item, and check if there is a status
             item = action_list.item(idx)
             try:
                 if item.status:
-                    self.show_message(item.status)
+                    self.show_message(str(item.status))
             except:
                 self.show_message(traceback.format_exc())
 
     # --------------------------------------------------------------------------
     def onActivate(self, reason):
         if reason == self.DoubleClick:
             self.widget.setVisible(not self.widget.isVisible())
```

### Comparing `launchpanel-1.1.0/launchpanel/utils.py` & `launchpanel-2.0.1/launchpanel/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,21 @@
     args = list()
     kwargs = dict()
 
     for arg in all_args:
 
         # -- If it has an =, its a kwarg
         if '=' in arg:
-            kwargs[arg.split('=')[0]] = arg.split('=')[1]
+            # -- we need to convert our plugin paths arg to a list
+            if arg.split('=')[0] == 'plugin_locations':
+                plugin_locations = arg.split('=')[1].split(';')
+                kwargs[arg.split('=')[0]] = plugin_locations
+
+            else:
+                kwargs[arg.split('=')[0]] = arg.split('=')[1]
 
         else:
             # -- We're dealing with an arg, so just
             # -- add it
             args.append(arg)
 
     return args, kwargs
```

### Comparing `launchpanel-1.1.0/launchpanel.egg-info/SOURCES.txt` & `launchpanel-2.0.1/launchpanel.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 launchpanel/__init__.py
 launchpanel/constants.py
 launchpanel/core.py
 launchpanel/create.py
 launchpanel/run.py
```

### Comparing `launchpanel-1.1.0/setup.py` & `launchpanel-2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_description = fh.read()
 
 else:
     long_description = short_description
 
 setuptools.setup(
     name='launchpanel',
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

