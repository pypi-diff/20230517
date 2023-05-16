# Comparing `tmp/hack_mentor-0.5.tar.gz` & `tmp/hack_mentor-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hack_mentor-0.5.tar", last modified: Tue May 16 22:25:27 2023, max compression
+gzip compressed data, was "hack_mentor-0.7.tar", last modified: Tue May 16 22:36:37 2023, max compression
```

## Comparing `hack_mentor-0.5.tar` & `hack_mentor-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:25:27.465521 hack_mentor-0.5/
--rw-r--r--   0 georgepickett   (502) staff       (20)     2484 2023-05-16 22:25:27.464976 hack_mentor-0.5/PKG-INFO
--rw-r--r--   0 georgepickett   (502) staff       (20)     1969 2023-05-16 22:19:14.000000 hack_mentor-0.5/README.md
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:25:27.459811 hack_mentor-0.5/hack_mentor/
--rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:27.000000 hack_mentor-0.5/hack_mentor/__init__.py
--rw-r--r--   0 georgepickett   (502) staff       (20)     2382 2023-05-16 21:39:13.000000 hack_mentor-0.5/hack_mentor/main.py
--rw-r--r--   0 georgepickett   (502) staff       (20)     1570 2023-05-16 21:29:27.000000 hack_mentor-0.5/hack_mentor/prompts.py
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:25:27.463995 hack_mentor-0.5/hack_mentor.egg-info/
--rw-r--r--   0 georgepickett   (502) staff       (20)     2484 2023-05-16 22:25:27.000000 hack_mentor-0.5/hack_mentor.egg-info/PKG-INFO
--rw-r--r--   0 georgepickett   (502) staff       (20)      312 2023-05-16 22:25:27.000000 hack_mentor-0.5/hack_mentor.egg-info/SOURCES.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)        1 2023-05-16 22:25:27.000000 hack_mentor-0.5/hack_mentor.egg-info/dependency_links.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       54 2023-05-16 22:25:27.000000 hack_mentor-0.5/hack_mentor.egg-info/entry_points.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       42 2023-05-16 22:25:27.000000 hack_mentor-0.5/hack_mentor.egg-info/requires.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       12 2023-05-16 22:25:27.000000 hack_mentor-0.5/hack_mentor.egg-info/top_level.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)      522 2023-05-16 22:25:20.000000 hack_mentor-0.5/pyproject.toml
--rw-r--r--   0 georgepickett   (502) staff       (20)       38 2023-05-16 22:25:27.465791 hack_mentor-0.5/setup.cfg
--rw-r--r--   0 georgepickett   (502) staff       (20)      371 2023-05-16 22:25:03.000000 hack_mentor-0.5/setup.py
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:36:37.724049 hack_mentor-0.7/
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2535 2023-05-16 22:36:37.722426 hack_mentor-0.7/PKG-INFO
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2020 2023-05-16 22:36:17.000000 hack_mentor-0.7/README.md
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:36:37.717354 hack_mentor-0.7/hack_mentor/
+-rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:27.000000 hack_mentor-0.7/hack_mentor/__init__.py
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2366 2023-05-16 22:35:03.000000 hack_mentor-0.7/hack_mentor/main.py
+-rw-r--r--   0 georgepickett   (502) staff       (20)     1570 2023-05-16 21:29:27.000000 hack_mentor-0.7/hack_mentor/prompts.py
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 22:36:37.721297 hack_mentor-0.7/hack_mentor.egg-info/
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2535 2023-05-16 22:36:37.000000 hack_mentor-0.7/hack_mentor.egg-info/PKG-INFO
+-rw-r--r--   0 georgepickett   (502) staff       (20)      312 2023-05-16 22:36:37.000000 hack_mentor-0.7/hack_mentor.egg-info/SOURCES.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)        1 2023-05-16 22:36:37.000000 hack_mentor-0.7/hack_mentor.egg-info/dependency_links.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       54 2023-05-16 22:36:37.000000 hack_mentor-0.7/hack_mentor.egg-info/entry_points.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       42 2023-05-16 22:36:37.000000 hack_mentor-0.7/hack_mentor.egg-info/requires.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       12 2023-05-16 22:36:37.000000 hack_mentor-0.7/hack_mentor.egg-info/top_level.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)      522 2023-05-16 22:35:17.000000 hack_mentor-0.7/pyproject.toml
+-rw-r--r--   0 georgepickett   (502) staff       (20)       38 2023-05-16 22:36:37.724433 hack_mentor-0.7/setup.cfg
+-rw-r--r--   0 georgepickett   (502) staff       (20)      371 2023-05-16 22:35:12.000000 hack_mentor-0.7/setup.py
```

### Comparing `hack_mentor-0.5/PKG-INFO` & `hack_mentor-0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hack_mentor
-Version: 0.5
+Version: 0.7
 Summary: GPT4 in your terminal, watching you code and giving feedback
 Author-email: George Pickett <gpickett00@gmail.com>
 Project-URL: Homepage, https://github.com/grp06/hack_mentor
 Project-URL: Bug Tracker, https://github.com/grp06/hack_mentor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,18 @@
 
 ## Quickstart
 
 ```bash
 pip install hack_mentor
 ```
 
+```bash
+export OPENAI_API_KEY="your-key-here"
+```
+
 ## Description
 
 This project ues GPT-4 to actively watch you code in your terminal, providing real-time feedback and suggestions.
 
 There are two key modes in Hack Mentor:
 
 - **Bug Mode**: Here, Hack Mentor will look for bugs and give concise suggestions for how to fix.
```

### Comparing `hack_mentor-0.5/README.md` & `hack_mentor-0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 ## Quickstart
 
 ```bash
 pip install hack_mentor
 ```
 
+```bash
+export OPENAI_API_KEY="your-key-here"
+```
+
 ## Description
 
 This project ues GPT-4 to actively watch you code in your terminal, providing real-time feedback and suggestions.
 
 There are two key modes in Hack Mentor:
 
 - **Bug Mode**: Here, Hack Mentor will look for bugs and give concise suggestions for how to fix.
```

### Comparing `hack_mentor-0.5/hack_mentor/main.py` & `hack_mentor-0.7/hack_mentor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langchain.callbacks.base import BaseCallbackManager
+from langchain.callbacks.base import CallbackManager
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import (
     HumanMessage,
     AIMessage
 )
 from dotenv import load_dotenv
@@ -39,15 +39,15 @@
             callback(result)
 
         return result
     
     
 def call_gpt(code, prompt):
     print(prompt)
-    chat = CustomChatOpenAI(streaming=True, model_name="gpt-3.5-turbo", callback_manager=BaseCallbackManager([StreamingStdOutCallbackHandler()]), verbose=True)
+    chat = CustomChatOpenAI(streaming=True, model_name="gpt-4", callback_manager=CallbackManager([StreamingStdOutCallbackHandler()]), verbose=True)
     chat([HumanMessage(content=prompt)])
 
 
 def get_file_content(file_names):
     content = ""
     for file in file_names:
         with open(file, 'r') as f:
```

### Comparing `hack_mentor-0.5/hack_mentor/prompts.py` & `hack_mentor-0.7/hack_mentor/prompts.py`

 * *Files identical despite different names*

### Comparing `hack_mentor-0.5/hack_mentor.egg-info/PKG-INFO` & `hack_mentor-0.7/hack_mentor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hack-mentor
-Version: 0.5
+Version: 0.7
 Summary: GPT4 in your terminal, watching you code and giving feedback
 Author-email: George Pickett <gpickett00@gmail.com>
 Project-URL: Homepage, https://github.com/grp06/hack_mentor
 Project-URL: Bug Tracker, https://github.com/grp06/hack_mentor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,18 @@
 
 ## Quickstart
 
 ```bash
 pip install hack_mentor
 ```
 
+```bash
+export OPENAI_API_KEY="your-key-here"
+```
+
 ## Description
 
 This project ues GPT-4 to actively watch you code in your terminal, providing real-time feedback and suggestions.
 
 There are two key modes in Hack Mentor:
 
 - **Bug Mode**: Here, Hack Mentor will look for bugs and give concise suggestions for how to fix.
```

### Comparing `hack_mentor-0.5/pyproject.toml` & `hack_mentor-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hack_mentor"
-version = "0.5"
+version = "0.7"
 authors = [
   { name="George Pickett", email="gpickett00@gmail.com" },
 ]
 description = "GPT4 in your terminal, watching you code and giving feedback"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

