# Comparing `tmp/simplesystray-0.0.7.tar.gz` & `tmp/simplesystray-0.0.8.tar.gz`

## Comparing `simplesystray-0.0.7.tar` & `simplesystray-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/systrayv2.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simplesystray-0.0.7/src/simplesystray/__init__.py
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 simplesystray-0.0.7/src/simplesystray/traybar.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 simplesystray-0.0.7/src/simplesystray/win32_adapter.py
--rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 simplesystray-0.0.7/tests/test.ico
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 simplesystray-0.0.7/tests/test.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 simplesystray-0.0.7/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 simplesystray-0.0.7/LICENSE
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 simplesystray-0.0.7/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 simplesystray-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 simplesystray-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/systrayv2.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simplesystray-0.0.8/src/simplesystray/__init__.py
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 simplesystray-0.0.8/src/simplesystray/traybar.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 simplesystray-0.0.8/src/simplesystray/win32_adapter.py
+-rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 simplesystray-0.0.8/tests/test.ico
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 simplesystray-0.0.8/tests/test.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 simplesystray-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 simplesystray-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 simplesystray-0.0.8/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 simplesystray-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 simplesystray-0.0.8/PKG-INFO
```

### Comparing `simplesystray-0.0.7/.idea/workspace.xml` & `simplesystray-0.0.8/.idea/workspace.xml`

 * *Files 24% similar despite different names*

#### Comparing `simplesystray-0.0.7/.idea/workspace.xml` & `simplesystray-0.0.8/.idea/workspace.xml`

```diff
@@ -1,18 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="3adf79f7-ff10-4044-ae51-9ecc614ccb4f" name="Changes" comment="">
-      <change afterPath="$PROJECT_DIR$/src/simplesystray/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/infi/__init__.py" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/infi/systray/__init__.py" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/infi/systray/traybar.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/simplesystray/traybar.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/infi/systray/win32_adapter.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/simplesystray/win32_adapter.py" afterDir="false"/>
-    </list>
+    <list default="true" id="3adf79f7-ff10-4044-ae51-9ecc614ccb4f" name="Changes" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -29,24 +22,24 @@
   </component>
   <component name="ProjectId" id="2PtJq1xlau3tb2PXWOXgHJc1iXE"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
     <option name="showMembers" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false",
-    "last_opened_file_path": "C:/Users/Alex/Desktop/github/systrayv2",
-    "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
+    &quot;last_opened_file_path&quot;: &quot;C:/Users/Alex/Desktop/github/systrayv2&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\Alex\Desktop\github\systrayv2\src\simplesystray"/>
       <recent name="C:\Users\Alex\Desktop\github\systrayv2\src"/>
     </key>
   </component>
   <component name="RunManager">
@@ -87,30 +80,39 @@
       <option name="presentableId" value="Default"/>
       <updated>1684270631737</updated>
       <workItem from="1684270632852" duration="2846000"/>
       <workItem from="1684274432230" duration="247000"/>
       <workItem from="1684274858562" duration="560000"/>
       <workItem from="1684275538743" duration="420000"/>
       <workItem from="1684275968191" duration="27000"/>
-      <workItem from="1684276004831" duration="137000"/>
+      <workItem from="1684276004831" duration="229000"/>
+      <workItem from="1684276302374" duration="64000"/>
+      <workItem from="1684276392867" duration="11000"/>
     </task>
     <task id="LOCAL-00001" summary=".">
       <created>1684273300086</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1684273300086</updated>
     </task>
-    <option name="localTasksCounter" value="2"/>
+    <task id="LOCAL-00002" summary=".">
+      <created>1684276159018</created>
+      <option name="number" value="00002"/>
+      <option name="presentableId" value="LOCAL-00002"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1684276159018</updated>
+    </task>
+    <option name="localTasksCounter" value="3"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="."/>
     <option name="LAST_COMMIT_MESSAGE" value="."/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
-    <SUITE FILE_PATH="coverage/systrayv2$test.coverage" NAME="test Coverage Results" MODIFIED="1684276122122" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/systrayv2$test.coverage" NAME="test Coverage Results" MODIFIED="1684276314323" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `simplesystray-0.0.7/.idea/inspectionProfiles/Project_Default.xml` & `simplesystray-0.0.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/src/simplesystray/traybar.py` & `simplesystray-0.0.8/src/simplesystray/traybar.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/src/simplesystray/win32_adapter.py` & `simplesystray-0.0.8/src/simplesystray/win32_adapter.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/tests/test.ico` & `simplesystray-0.0.8/tests/test.ico`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/tests/test.py` & `simplesystray-0.0.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/.gitignore` & `simplesystray-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/LICENSE` & `simplesystray-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/README.md` & `simplesystray-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.7/pyproject.toml` & `simplesystray-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "simplesystray"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="actorpus", email="alex@actorpus.com" },
 ]
 description = "Adds support for a simple icon on the system tray, clone of infi-systray but maintained"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplesystray-0.0.7/PKG-INFO` & `simplesystray-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesystray
-Version: 0.0.7
+Version: 0.0.8
 Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
 Project-URL: Homepage, https://github.com/actorpus/systrayv2
 Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
 Author-email: actorpus <alex@actorpus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

