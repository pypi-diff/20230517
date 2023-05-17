# Comparing `tmp/gpt-convo-reader-0.1.2.tar.gz` & `tmp/gpt-convo-reader-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-convo-reader-0.1.2.tar", last modified: Thu May 11 06:29:24 2023, max compression
+gzip compressed data, was "gpt-convo-reader-0.2.tar", last modified: Wed May 17 10:24:01 2023, max compression
```

## Comparing `gpt-convo-reader-0.1.2.tar` & `gpt-convo-reader-0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.1.2/LICENSE
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2164 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1574 2023-05-08 13:33:05.000000 gpt-convo-reader-0.1.2/README.md
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/setup.cfg
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1067 2023-05-11 06:29:05.000000 gpt-convo-reader-0.1.2/setup.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.667876 gpt-convo-reader-0.1.2/src/
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.719875 gpt-convo-reader-0.1.2/src/converter/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.1.2/src/converter/__init__.py
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2078 2023-05-07 10:27:12.000000 gpt-convo-reader-0.1.2/src/converter/convert.py
--rwxrwxr-x   0 romilly   (1000) romilly   (1000)     3328 2023-05-11 06:28:24.000000 gpt-convo-reader-0.1.2/src/converter/gui.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-11 06:29:24.739875 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2164 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      374 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/entry_points.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       15 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/requires.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-11 06:29:24.000000 gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/top_level.txt
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.2/LICENSE
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     3168 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2580 2023-05-17 10:15:47.000000 gpt-convo-reader-0.2/README.md
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/setup.cfg
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1065 2023-05-17 10:05:52.000000 gpt-convo-reader-0.2/setup.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.841961 gpt-convo-reader-0.2/src/
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/src/converter/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.2/src/converter/__init__.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1542 2023-05-17 10:04:19.000000 gpt-convo-reader-0.2/src/converter/config.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2391 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2/src/converter/convert.py
+-rwxrwxr-x   0 romilly   (1000) romilly   (1000)     4132 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2/src/converter/gui.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 10:24:01.853961 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     3168 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      398 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/entry_points.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       15 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/requires.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-17 10:24:01.000000 gpt-convo-reader-0.2/src/gpt_convo_reader.egg-info/top_level.txt
```

### Comparing `gpt-convo-reader-0.1.2/LICENSE` & `gpt-convo-reader-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.1.2/PKG-INFO` & `gpt-convo-reader-0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-convo-reader
-Version: 0.1.2
-Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
-Home-page: https://github.com/romilly/gpt-convo-reader
-Author: Romilly Cocking
-Author-email: romilly.cocking@gmail.com
-Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChatGPT Convo Reader
 
 The reader lets you find, view and format the conversations you've had with ChatGPT in the playground.
 
 It does so by reading the zip file that ChatGPT saves when you ask it to dump your data.
 
 **Please note:** this is an independently developed project, and it has no official connection with ChatGPT or OpenAI.
@@ -33,29 +18,45 @@
 
 ## Installation
 
 run `pip install gpt-convo-reader`
 
 ## Usage
 
-1. In the directory from which you wish to run the reader, create a file `convert.ini` file with the following format:
+The application now tries to configure itself using data in a config file.
+
+That file is `gpt-convo-reader/config.ini` in the user's config directory.
+
+Typical user config directories are:
+  Mac OS X:               same as user_data_dir:  ~/Library/Application Support/<AppName>
+  Unix:                   ~/.config/<AppName>     # or in $XDG_CONFIG_HOME, if defined
+  Win *:                  same as user_data_dir
 
+
+1. Create a directory gpt-convo directory in your config direectoy
+2. Create a file `convert.ini` file with the following format:
    ```text
    [default directory locations]
    zip directory = foo
    save directory = bar
+   prefix = xhxhazhdsxhnxznsds
    ```
-   
-   where `foo` is the relative path to the directory in which the dumped zip file is located, and `bar`
-   is the default directory into which you will save markdown files.
+   where `foo` is the relative path to the directory in which OpenAI'a dumped zip file is located, `bar`
+   is the default directory into which you will save markdown files, and prefix is set to the prefix that OpenAI adds to the start of the zip files it creates for you.
 1. In your chosen directory, run `gpt_reader_gui`
-2. From the `File\Open` menu, open the dumped zip file you want to examine. A list of title will be displayed.
+2. From the `File/Open` menu, open the dumped zip file you want to examine. A list of title will be displayed.
+5. If you want to load all the files that OpenAI has dumped, select te `File/Load All` option.
 3. Select a conversation you want to examine from the list of titles.
-4. If you want to export a conversation as a neatly formatted markdown file, you can do so from the `File\Save` menu.
+4. If you want to export a conversation as a neatly formatted markdown file, you can do so from the `File/Save` menu.
+
+If you are only interested in converations containing a given string, type the string in the entry field by the search buton and press `Search`.
+
+The list will show only those converastions that contain that string.
 
+If you want to see all the conversations again, delete the search string and press `Search The full list of converations will be displayed.`
 ## How to contribute
 
 Please raise any issues (bugs or feature requests) on GitHub.
 
 ## Contact details
 
 I'm Romilly Cocking: @RAREblog on twitter, @romilly@fosstodon.org
```

### Comparing `gpt-convo-reader-0.1.2/setup.cfg` & `gpt-convo-reader-0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.1.2/setup.py` & `gpt-convo-reader-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-convo-reader",
-    version="0.1.2",
+    version="0.2",
     author="Romilly Cocking",
     author_email="romilly.cocking@gmail.com",
     description="Lets you find, view and format the conversations you've had with ChatGPT in the playground.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/romilly/gpt-convo-reader",
     project_urls={
```

### Comparing `gpt-convo-reader-0.1.2/src/converter/convert.py` & `gpt-convo-reader-0.2/src/converter/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # coding: utf-8
-
+import os
 import zipfile
 import json
 import datetime
 from io import StringIO
 from typing import List, Dict, Any
 from pathlib import Path
 
@@ -66,7 +66,17 @@
         with zip_file.open(file_to_extract) as file:
             data = json.load(file)
     result = {}
     for item in data:
         convo= conversation(item)
         result[convo.title] = convo
     return result
+
+def convert_all(directory: str, prefix: str) -> Dict[str, Conversation]:
+    result = {}
+    for name in os.listdir(directory):
+        if name.startswith(prefix) and name.endswith('.zip'):
+            pathname = os.path.join(directory, name)
+            result |= convert(pathname)
+    return result
+
+
```

### Comparing `gpt-convo-reader-0.1.2/src/converter/gui.py` & `gpt-convo-reader-0.2/src/converter/gui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 #!/usr/bin/env python
 # coding: utf-8
+import time
+
 import os.path
 from configparser import ConfigParser
-from guizero import App, ListBox, TextBox, TitleBox, MenuBar
+from guizero import App, ListBox, TextBox, TitleBox, MenuBar, PushButton
 
-from converter.convert import convert
+from converter import config
+from converter.config import Configuration
+from converter.convert import convert, convert_all
 
 
 class ConversationGUI(App):
-    def __init__(self):
+    def __init__(self, testing=False):
         super().__init__(title='ChatGPT Conversation Reader', height=800, width=1400)
-        self.zip_folder, self.save_folder = self.get_default_directories()
+        if testing:
+            self.configuration = Configuration()
+        else:
+            self.configuration = config.get_configuration()
         self.conversations = {}
         self.selected_conversation = None
         menubar = MenuBar(self,
                           toplevel=["File"],
                           options=[
-                              [["Open", self.open_function],["Save", self.save_function]],
+                              [["Open", self.open_function],
+                               ['Load all', self.load_all],
+                               ["Save", self.save_function]],
                           ])
         # Create a Box to contain the ListBox and TextBox
         self.conversation_box = TitleBox(self, 'Conversations', width='fill')
         # Create a ListBox to display the conversation titles
         self.conversation_list = ListBox(self.conversation_box, command=self.show_conversation, width = 'fill')
+        self.search_box = TitleBox(self.conversation_box,'Search', width='fill')
+        self.search_button= PushButton(self.search_box, text='Search', command=self.filter_convos, align='left')
+        self.search_field = TextBox(self.search_box, width='fill', align='left')
         # Create a TextBox to display the conversation messages
         self.conversation_text = TextBox(self.conversation_box, multiline=True, scrollbar=True, width= 'fill', height='fill')
 
-    def get_default_directories(self):
-        config = ConfigParser()
-        if os.path.exists('convert.ini'):
-            config.read('convert.ini')
-            zip_folder = config['default directory locations']['zip directory']
-            save_folder = config['default directory locations']['save directory']
-        else:
-            zip_folder = '.'
-            save_folder = '.'
-            print('using current directory as default')
-        return zip_folder, save_folder
-
+    def filter_convos(self):
+        self.conversation_list.clear()
+        wanted = self.search_field.value.strip()
+        if len(wanted) == 0:
+            self.show_full_convo_list()
+            return
+        for title in self.conversations:
+            for message in self.conversations[title].messages:
+                if wanted in message.text():
+                    self.conversation_list.append(title)
+                    break
 
     def show_conversation(self):
         # Get the selected conversation from the ListBox
         title = self.conversation_list.value
         # Get the conversation object from the dictionary
         self.selected_conversation = self.conversations[title]
         # Clear the TextBox
@@ -48,24 +59,32 @@
         # Add the messages to the TextBox
         for message in self.selected_conversation.messages:
             self.conversation_text.append(str(message))
             self.conversation_text.append('\n')
 
     def open_function(self):
         file_name = self.select_file(filetypes=[['zip files', '*.zip']],
-                                     folder=self.zip_folder)
+                                     folder=self.configuration.zip_directory)
         if len(file_name) > 0:
             self.conversations = convert(file_name)
             # Add the conversation titles to the ListBox
-            for title in self.conversations:
-                self.conversation_list.append(title)
+            self.show_full_convo_list()
+
+    def load_all(self):
+        self.conversations = convert_all(self.configuration.zip_directory, self.configuration.prefix)
+        self.show_full_convo_list()
+
+    def show_full_convo_list(self):
+        for title in self.conversations:
+            self.conversation_list.append(title)
 
     def save_function(self):
+        time.sleep(0.1)
         file_name = self.select_file(filetypes=[['Markdown Files', '*.md']], save=True,
-                                     folder=self.save_folder)
+                                     folder=self.configuration.save_directory)
         if len(file_name) > 0:
             with open(file_name, 'w') as mdf:
                 mdf.write(f'# {self.selected_conversation.title}\n\n')
                 mdf.write(f'{self.selected_conversation.updated()}\n\n')
                 for message in self.selected_conversation.messages:
                     mdf.write(message.markdown())
                     mdf.write('\n\n')
```

### Comparing `gpt-convo-reader-0.1.2/src/gpt_convo_reader.egg-info/PKG-INFO` & `gpt-convo-reader-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.1.2
+Version: 0.2
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,29 +33,45 @@
 
 ## Installation
 
 run `pip install gpt-convo-reader`
 
 ## Usage
 
-1. In the directory from which you wish to run the reader, create a file `convert.ini` file with the following format:
+The application now tries to configure itself using data in a config file.
 
+That file is `gpt-convo-reader/config.ini` in the user's config directory.
+
+Typical user config directories are:
+  Mac OS X:               same as user_data_dir:  ~/Library/Application Support/<AppName>
+  Unix:                   ~/.config/<AppName>     # or in $XDG_CONFIG_HOME, if defined
+  Win *:                  same as user_data_dir
+
+
+1. Create a directory gpt-convo directory in your config direectoy
+2. Create a file `convert.ini` file with the following format:
    ```text
    [default directory locations]
    zip directory = foo
    save directory = bar
+   prefix = xhxhazhdsxhnxznsds
    ```
-   
-   where `foo` is the relative path to the directory in which the dumped zip file is located, and `bar`
-   is the default directory into which you will save markdown files.
+   where `foo` is the relative path to the directory in which OpenAI'a dumped zip file is located, `bar`
+   is the default directory into which you will save markdown files, and prefix is set to the prefix that OpenAI adds to the start of the zip files it creates for you.
 1. In your chosen directory, run `gpt_reader_gui`
-2. From the `File\Open` menu, open the dumped zip file you want to examine. A list of title will be displayed.
+2. From the `File/Open` menu, open the dumped zip file you want to examine. A list of title will be displayed.
+5. If you want to load all the files that OpenAI has dumped, select te `File/Load All` option.
 3. Select a conversation you want to examine from the list of titles.
-4. If you want to export a conversation as a neatly formatted markdown file, you can do so from the `File\Save` menu.
+4. If you want to export a conversation as a neatly formatted markdown file, you can do so from the `File/Save` menu.
+
+If you are only interested in converations containing a given string, type the string in the entry field by the search buton and press `Search`.
+
+The list will show only those converastions that contain that string.
 
+If you want to see all the conversations again, delete the search string and press `Search The full list of converations will be displayed.`
 ## How to contribute
 
 Please raise any issues (bugs or feature requests) on GitHub.
 
 ## Contact details
 
 I'm Romilly Cocking: @RAREblog on twitter, @romilly@fosstodon.org
```

