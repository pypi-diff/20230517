# Comparing `tmp/hack_mentor-0.1.tar.gz` & `tmp/hack_mentor-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hack_mentor-0.1.tar", last modified: Tue May 16 21:13:39 2023, max compression
+gzip compressed data, was "hack_mentor-0.2.tar", last modified: Tue May 16 21:57:20 2023, max compression
```

## Comparing `hack_mentor-0.1.tar` & `hack_mentor-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 21:13:39.056923 hack_mentor-0.1/
--rw-r--r--   0 georgepickett   (502) staff       (20)       53 2023-05-16 21:13:39.056259 hack_mentor-0.1/PKG-INFO
--rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:17.000000 hack_mentor-0.1/README.md
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 21:13:39.051594 hack_mentor-0.1/hack_mentor/
--rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:27.000000 hack_mentor-0.1/hack_mentor/__init__.py
--rw-r--r--   0 georgepickett   (502) staff       (20)     2909 2023-05-16 21:12:57.000000 hack_mentor-0.1/hack_mentor/main.py
-drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 21:13:39.055540 hack_mentor-0.1/hack_mentor.egg-info/
--rw-r--r--   0 georgepickett   (502) staff       (20)       53 2023-05-16 21:13:38.000000 hack_mentor-0.1/hack_mentor.egg-info/PKG-INFO
--rw-r--r--   0 georgepickett   (502) staff       (20)      274 2023-05-16 21:13:39.000000 hack_mentor-0.1/hack_mentor.egg-info/SOURCES.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)        1 2023-05-16 21:13:38.000000 hack_mentor-0.1/hack_mentor.egg-info/dependency_links.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       54 2023-05-16 21:13:38.000000 hack_mentor-0.1/hack_mentor.egg-info/entry_points.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       42 2023-05-16 21:13:38.000000 hack_mentor-0.1/hack_mentor.egg-info/requires.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       12 2023-05-16 21:13:38.000000 hack_mentor-0.1/hack_mentor.egg-info/top_level.txt
--rw-r--r--   0 georgepickett   (502) staff       (20)       38 2023-05-16 21:13:39.057165 hack_mentor-0.1/setup.cfg
--rw-r--r--   0 georgepickett   (502) staff       (20)      371 2023-05-16 21:12:21.000000 hack_mentor-0.1/setup.py
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 21:57:20.589099 hack_mentor-0.2/
+-rw-r--r--   0 georgepickett   (502) staff       (20)       53 2023-05-16 21:57:20.588703 hack_mentor-0.2/PKG-INFO
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2101 2023-05-16 21:52:38.000000 hack_mentor-0.2/README.md
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 21:57:20.583528 hack_mentor-0.2/hack_mentor/
+-rw-r--r--   0 georgepickett   (502) staff       (20)        0 2023-05-16 19:34:27.000000 hack_mentor-0.2/hack_mentor/__init__.py
+-rw-r--r--   0 georgepickett   (502) staff       (20)     2382 2023-05-16 21:39:13.000000 hack_mentor-0.2/hack_mentor/main.py
+-rw-r--r--   0 georgepickett   (502) staff       (20)     1570 2023-05-16 21:29:27.000000 hack_mentor-0.2/hack_mentor/prompts.py
+drwxr-xr-x   0 georgepickett   (502) staff       (20)        0 2023-05-16 21:57:20.587813 hack_mentor-0.2/hack_mentor.egg-info/
+-rw-r--r--   0 georgepickett   (502) staff       (20)       53 2023-05-16 21:57:20.000000 hack_mentor-0.2/hack_mentor.egg-info/PKG-INFO
+-rw-r--r--   0 georgepickett   (502) staff       (20)      297 2023-05-16 21:57:20.000000 hack_mentor-0.2/hack_mentor.egg-info/SOURCES.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)        1 2023-05-16 21:57:20.000000 hack_mentor-0.2/hack_mentor.egg-info/dependency_links.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       54 2023-05-16 21:57:20.000000 hack_mentor-0.2/hack_mentor.egg-info/entry_points.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       42 2023-05-16 21:57:20.000000 hack_mentor-0.2/hack_mentor.egg-info/requires.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       12 2023-05-16 21:57:20.000000 hack_mentor-0.2/hack_mentor.egg-info/top_level.txt
+-rw-r--r--   0 georgepickett   (502) staff       (20)       38 2023-05-16 21:57:20.589208 hack_mentor-0.2/setup.cfg
+-rw-r--r--   0 georgepickett   (502) staff       (20)      371 2023-05-16 21:55:31.000000 hack_mentor-0.2/setup.py
```

### Comparing `hack_mentor-0.1/hack_mentor/main.py` & `hack_mentor-0.2/hack_mentor/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 from dotenv import load_dotenv
 from flask import Flask
 from rich.console import Console
 from rich.markdown import Markdown
 import os
 import sys
 import argparse
+from .prompts import mentor_prompt, architect_prompt
+
 
 load_dotenv()
 api_key = os.environ['OPENAI_API_KEY']
 app = Flask(__name__)
 console = Console()
 
 def write_with_code_block(text):
-    start_code_block = '\033[1;37;40m'  # White text with black background
-    end_code_block = '\033[0m'  # Reset to default colors
+    start_code_block = '\033[1;37;40m'
+    end_code_block = '\033[0m'
     sys.stdout.write(start_code_block + text + end_code_block)
     sys.stdout.flush()
 
 
 class CustomStreamingStdOutCallbackHandler(StreamingStdOutCallbackHandler):
     def on_llm_new_token(self, token, **kwargs):
         pass
@@ -35,46 +37,42 @@
 
         if callback:
             callback(result)
 
         return result
     
     
-def call_gpt(code):
-    print(code)
+def call_gpt(code, prompt):
+    print(prompt)
     chat = CustomChatOpenAI(streaming=True, model_name="gpt-3.5-turbo", callback_manager=BaseCallbackManager([StreamingStdOutCallbackHandler()]), verbose=True)
-    chat([HumanMessage(content=f"""The following code may have a bug. If it exists, tell me exactly where to look. In your response only tell me concisely exactly where to look. Be as concise as possible. Respond like, You may want to look at _____ where there's an issue with ____ and you can fix it by _____. Be specific with your suggested fix. Show a minimal representation of the fixed code.
-                                              
-    If there is no obvious bug simply reply, "no bug".
-    
-    Next you'll play the role of a software architect. You'll take a second look at our architecture decisions and recommend alternatives if there's something better.
-    
-    If there is no obvious recommendation, simply reply, "no rec"
-    
-    Below I will paste the contents from a bunch of my files. If I show you errors pay special attention to the errors and help me fix them.
-{code}""")])
+    chat([HumanMessage(content=prompt)])
 
 
 def get_file_content(file_names):
     content = ""
     for file in file_names:
         with open(file, 'r') as f:
             content += f"### {os.path.basename(file)}\n\n\n" + f.read() + "\n"
     return content
 
 
 
 def main(args=None):
     print('app started')
     parser = argparse.ArgumentParser(description='Process some files.')
+    parser.add_argument('mode', metavar='M', type=str, choices=['mentor', 'architect'],
+                        help='Mode of operation: mentor or architect')
     parser.add_argument('file_names', metavar='N', type=str, nargs='+',
                         help='Files to process')
 
     args = parser.parse_args(args)
     while True:
         file_content = get_file_content(args.file_names)
-        call_gpt(file_content)
+        if args.mode == 'mentor':
+            call_gpt(file_content, mentor_prompt(file_content))
+        elif args.mode == 'architect':
+            call_gpt(file_content, architect_prompt(file_content))
         input("Press Enter to continue...")
 
 
 if __name__ == '__main__':
     main()
```

