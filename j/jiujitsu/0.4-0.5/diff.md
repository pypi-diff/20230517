# Comparing `tmp/jiujitsu-0.4.tar.gz` & `tmp/jiujitsu-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiujitsu-0.4.tar", last modified: Tue May 16 22:40:40 2023, max compression
+gzip compressed data, was "jiujitsu-0.5.tar", last modified: Wed May 17 16:09:11 2023, max compression
```

## Comparing `jiujitsu-0.4.tar` & `jiujitsu-0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:40:40.173093 jiujitsu-0.4/
--rw-r--r--   0 adam      (1000) users      (984)      479 2023-05-16 22:40:40.173093 jiujitsu-0.4/PKG-INFO
--rw-r--r--   0 adam      (1000) users      (984)     6367 2023-05-16 16:51:46.000000 jiujitsu-0.4/README.md
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:40:40.173093 jiujitsu-0.4/jiujitsu/
--rw-r--r--   0 adam      (1000) users      (984)      515 2023-05-16 17:27:01.000000 jiujitsu-0.4/jiujitsu/__init__.py
--rw-r--r--   0 adam      (1000) users      (984)     1669 2023-05-16 16:52:45.000000 jiujitsu-0.4/jiujitsu/bpFileSystem.py
--rw-r--r--   0 adam      (1000) users      (984)     4535 2023-05-16 17:17:28.000000 jiujitsu-0.4/jiujitsu/bpInterpreter.py
--rw-r--r--   0 adam      (1000) users      (984)    31109 2023-05-16 17:28:34.000000 jiujitsu-0.4/jiujitsu/bpInterpreterBase.py
--rw-r--r--   0 adam      (1000) users      (984)    11559 2023-05-16 17:17:50.000000 jiujitsu-0.4/jiujitsu/bpPrimitives.py
--rwxr-xr-x   0 adam      (1000) users      (984)    24302 2023-05-16 20:09:57.000000 jiujitsu-0.4/jiujitsu/jInterpreter.py
--rw-r--r--   0 adam      (1000) users      (984)     2647 2023-05-16 16:52:45.000000 jiujitsu-0.4/jiujitsu/jNode.py
--rw-r--r--   0 adam      (1000) users      (984)     5163 2023-05-16 17:18:46.000000 jiujitsu-0.4/jiujitsu/jParser.py
--rw-r--r--   0 adam      (1000) users      (984)     1161 2023-05-16 17:18:52.000000 jiujitsu-0.4/jiujitsu/jRecord.py
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:40:40.173093 jiujitsu-0.4/jiujitsu/test/
--rw-r--r--   0 adam      (1000) users      (984)        0 2023-05-16 16:51:46.000000 jiujitsu-0.4/jiujitsu/test/__init__.py
--rw-r--r--   0 adam      (1000) users      (984)    14839 2023-05-16 17:21:29.000000 jiujitsu-0.4/jiujitsu/test/test_bpInterpreterBase.py
--rw-r--r--   0 adam      (1000) users      (984)     6025 2023-05-16 17:22:31.000000 jiujitsu-0.4/jiujitsu/test/test_bpPrimitives.py
--rw-r--r--   0 adam      (1000) users      (984)    17534 2023-05-16 17:32:42.000000 jiujitsu-0.4/jiujitsu/test/test_jInterpreter.py
--rw-r--r--   0 adam      (1000) users      (984)      886 2023-05-16 17:25:00.000000 jiujitsu-0.4/jiujitsu/test/test_jParser.py
-drwxr-xr-x   0 adam      (1000) users      (984)        0 2023-05-16 22:40:40.173093 jiujitsu-0.4/jiujitsu.egg-info/
--rw-r--r--   0 adam      (1000) users      (984)      479 2023-05-16 22:40:40.000000 jiujitsu-0.4/jiujitsu.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) users      (984)      598 2023-05-16 22:40:40.000000 jiujitsu-0.4/jiujitsu.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) users      (984)        1 2023-05-16 22:40:40.000000 jiujitsu-0.4/jiujitsu.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) users      (984)       50 2023-05-16 22:40:40.000000 jiujitsu-0.4/jiujitsu.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1000) users      (984)       19 2023-05-16 22:40:40.000000 jiujitsu-0.4/jiujitsu.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) users      (984)        9 2023-05-16 22:40:40.000000 jiujitsu-0.4/jiujitsu.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) users      (984)      590 2023-05-16 22:40:40.173093 jiujitsu-0.4/setup.cfg
--rw-r--r--   0 adam      (1000) users      (984)      897 2023-05-16 22:40:25.000000 jiujitsu-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.757191 jiujitsu-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:09:11.757191 jiujitsu-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-17 16:08:58.000000 jiujitsu-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.753191 jiujitsu-0.5/jiujitsu/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpFileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpInterpreterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/bpPrimitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24426 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/jRecord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.753191 jiujitsu-0.5/jiujitsu/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_bpInterpreterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_bpPrimitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_jInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-17 16:08:58.000000 jiujitsu-0.5/jiujitsu/test/test_jParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:09:11.753191 jiujitsu-0.5/jiujitsu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 16:09:11.000000 jiujitsu-0.5/jiujitsu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 16:09:11.757191 jiujitsu-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-17 16:08:58.000000 jiujitsu-0.5/setup.py
```

### Comparing `jiujitsu-0.4/README.md` & `jiujitsu-0.5/README.md`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/__init__.py` & `jiujitsu-0.5/jiujitsu/__init__.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/bpFileSystem.py` & `jiujitsu-0.5/jiujitsu/bpFileSystem.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/bpInterpreter.py` & `jiujitsu-0.5/jiujitsu/bpInterpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         documents = []
         for arg in args:
             if arg.word[0] == '-': 
                 flags += [ arg ]
             else:
                 documents += [ arg ]
         if documents[0].word == '/': self.state.fs = {}
-        elif documents[0].word in self.state.fs or self.state.working_dir+'/'+documents[0].word in self.state.fs: self.state.fs.pop(document[0].word)
+        elif documents[0].word in self.state.fs or self.state.working_dir+'/'+documents[0].word in self.state.fs: self.state.fs.pop(documents[0].word)
         else: print("rm: cannot remove '" + documents[0].word + "': No such file or directory")
 
     def f_mv(self, node):
         command, args = self.parse_node(node)
         self.state.copy_file(args[0].word, args[1].word)
         self.state.remove_file(args[0].word)
```

### Comparing `jiujitsu-0.4/jiujitsu/bpInterpreterBase.py` & `jiujitsu-0.5/jiujitsu/bpInterpreterBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# from bpFileSystem import FileSocket
 from jiujitsu.bpFileSystem import FileSocket
 from jiujitsu.bpPrimitives import ActionEntry, State
+
 from bashparser import NodeVisitor
+
 import copy, bashparser, subprocess
 
 
 class InterpreterError(Exception):
     pass
 
 
@@ -164,23 +165,23 @@
         if not len(self.action_stack):
             output += 'Empty' + '\n'
         return output
 
 
     def shell(self, text, forward_stdio = True):
         repl_nodes = self.replace(bashparser.parse(text), full = True)
-
+        
         for node in repl_nodes:
             repl_text = str(bashparser.NodeVisitor(node))
             if forward_stdio:
                 repl_text = 'echo "' + self.stdin() + '" | ' + repl_text
-
+            
             """ Execute the code """
             result = subprocess.run(repl_text, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
+            
             """ Put results in the STDIO """
             output = result.stdout
             if len(str(result.stderr)): output += result.stderr
             self.state.STDOUT(output)
 
     def set_variable(self, name, value):
         if type(name) is not str: raise InterpreterError('Interpreter.set_variable(name != str)')
@@ -557,21 +558,27 @@
  
                 def replace_cmd_sub_results(node, part, index):
                     screen_string = ' '.join(self.state.get_screen().split('\n'))
                     results = screen_string + ' ' + self.stdout() if len(screen_string) else self.stdout()
                     if self.stdout() == '' and len(screen_string): results = results[:-1] # remove bad trailing space
                     self.stdout('')
                     self.state.screen = "" # empty screen so it doesn't get appended to
+                    
                     # Adjust the tree with the replaced results
                     index_one = part.pos[0] - node.pos[0]
-                    #if part.pos[1] - part.pos[0] != len(str(part.command)):
-                    #    index_one -= 1
-                    #print('index one: ', index_one)
-                    #print('index two: ', index_one + (part.pos[1] - node.pos[0]))
-                    quoted_delta = 0
+                    orig_index_one = index_one  # sloppy coding but it works so whatever
+
+                    # If the string is quoted in any way the $ will be offset from the actual pos
+                    # This is how we identify if we need to verify pos and find new pos
+                    starting_offset = -1
+                    while node.word[index_one] != '$':
+                        index_one = orig_index_one + starting_offset
+                        starting_offset = abs(starting_offset) if starting_offset < 0 else -(starting_offset + 1)
+ 
+
 
                     node.word = node.word[:index_one] + results + node.word[index_one + (part.pos[1] - node.pos[0]):]
                     node.parts = node.parts[:index] + node.parts[index + 1:]
                     # Exit the subshell env
                     self.state.raise_scope()
 
                 action = ActionEntry(func=build_cmd_sub, args=[node,part], text='Enter Command Substitution Env: ' + str(bashparser.NodeVisitor(node)), code=str(bashparser.NodeVisitor(node)))
```

### Comparing `jiujitsu-0.4/jiujitsu/bpPrimitives.py` & `jiujitsu-0.5/jiujitsu/bpPrimitives.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/jInterpreter.py` & `jiujitsu-0.5/jiujitsu/jInterpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         """ Converts arguments to strings. A necessary wrapper cause escape characters """
         text = ''
         for arg in args:
             if unescape:
                 text += arg.unescape() + ' '
             else:
                 text += arg.value + ' '
-        text = text[:-1]    # last space is wrong plz remove
+        if len(text):
+            text = text[:-1]    # last space is wrong plz remove
         return text
     
     def get_next_node(self):
         # if self.prog_nodes is None or len(self.prog_nodes) == 0: return None
         if self.index >= len(self.prog_nodes): return None
         node = self.prog_nodes[self.index]
         return node
@@ -152,15 +153,16 @@
                         print('=>', self.env.action_stack[0])
                     else:
                         print('=> Action stack empty')
                 else:
                     self.env.run(node)
             
             else:
-                while len(self.env.action_stack): self.do_inch(text)
+                while len(self.env.action_stack): 
+                    self.do_inch(text)
 
             if Flag('p') in flags:
                 return self.state([])
 
             if self.get_next_node():
                 print('=>', str(bashparser.NodeVisitor(self.get_next_node())))
 
@@ -220,16 +222,18 @@
         itrs = self.args_to_str(args)
         if not itrs.isdigit():
             itrs = 1
         else: itrs = int(itrs)
         
         for i in range(0, itrs):
             if Flag('e') in flags:
-                node_str = self.env.action_stack[0].code
-                self.do_shell(node_str)
+                node_str = self.env.action_stack[0].code 
+                print('entered shell')
+                if node_str:
+                    self.do_shell(node_str)
                 self.env.action_stack.pop(0)
                 self.env.stdin('')
 
             else:
                 res = self.env.inch()
             
             if len(self.env.action_stack):
@@ -318,15 +322,15 @@
     def do_shell(self, text):
         """Runs a (real) command on your host system.  Note that the ! must be followed by a space.
                 STDIO will be passed into the command unless the -n flag is specified """
         
         flags, args = self.parser.parse(text)
         text = self.args_to_str(args)
         
-        self.env.shell(text, Flag('n') in flags)
+        self.env.shell(text, Flag('n') not in flags)
         
     def do_dir(self, text):
         """ Deals with the printing and modificaiton of the interpreters working directory """
         flags, args = self.parser.parse(text)   # Do it this way cause escaping
         if len(args) == 1:
             self.env.working_dir(args[0].value)
             print('Working dir: ' + self.env.working_dir())
```

### Comparing `jiujitsu-0.4/jiujitsu/jNode.py` & `jiujitsu-0.5/jiujitsu/jNode.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/jParser.py` & `jiujitsu-0.5/jiujitsu/jParser.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/jRecord.py` & `jiujitsu-0.5/jiujitsu/jRecord.py`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/jiujitsu/test/test_bpInterpreterBase.py` & `jiujitsu-0.5/jiujitsu/test/test_bpInterpreterBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 from unittest import TestCase
+
 from jiujitsu import InterpreterBase, InterpreterError
-# from bpInterpreter import Interpreter as Full_Interpreter
 from jiujitsu import FullInterpreter as Full_Interpreter
-# from bpPrimitives import State
 from jiujitsu import State
-
-# from bpFileSystem import File, FileSocket
 from jiujitsu import File, FileSocket
 
 import bashparser
 
 class TestBpInterpreterBase(TestCase):
-
     def test_init(self):
-        """ Verify all the objects are created correctly with no arguments """
+        # Verify all the objects are created correctly with no arguments #
         intr = InterpreterBase()
         state = State()
         self.assertTrue(intr.state == state)
         self.assertTrue(intr.action_stack == [])
         self.assertTrue(intr.execute == True)
 
-        """ Verify the passed in arguments work well """
+        # Verify the passed in arguments work well #
         stdio = FileSocket(id_num = 1)
         working_dir = '~/some/where'
         variables = {
             'name1':['value1'],
             'name2':['value2', 'value3']
         }
-        """ Test loading the state from a json """
+        # Test loading the state from a json #
         fs = [
             { 
                 "name": "~/name1",
                 "contents": "value1",
                 "permissions": "rw-rw-rw-"
             }
         ]
-        """ Actual fs form """
+        # Actual fs form #
         fs2 = {
             "~/name1": File("~/name1", "value1", "rw-rw-rw-")
         }
         open_socket = []
         truths = {
             'something':True,
             'else':False,
@@ -55,55 +51,55 @@
         self.assertTrue(intr.state == expected_state2)
         self.assertTrue(intr.execute == True)
         self.assertTrue(intr.action_stack == [])
         self.assertTrue(intr.state.fs == expected_state.fs)
 
 
     def test_json(self):
-        """ Only need to verify execute wraps properly. state is checked in bpPrimatives """
+        # Only need to verify execute wraps properly. state is checked in bpPrimatives #
         intr = InterpreterBase(execute = False)
         self.assertTrue(intr.json()['execute'] == 'f')
         intr = InterpreterBase(execute = True)
         self.assertTrue(intr.json()['execute'] == 't')
 
 
     def test_working_dir(self):
         intr = InterpreterBase()
         self.assertTrue(intr.working_dir() == '~')
         self.assertTrue(intr.working_dir('~/some/where') == '~/some/where')
 
 
     def test_update_file_system(self):
-        """ This should mirror test_bpPrimitives.test_update_file_system """
+        # This should mirror test_bpPrimitives.test_update_file_system #
         intr = InterpreterBase()
 
         self.assertRaises(InterpreterError, intr.update_file_system, 1234, 'contents')
         self.assertRaises(InterpreterError, intr.update_file_system, 'name', 1234)
         self.assertRaises(InterpreterError, intr.update_file_system, 'name', 'contents', 1234)
         self.assertRaises(InterpreterError, intr.update_file_system, 'name', 'contents', 'permissions', 1234)
 
-        """ Try it with all arguments """
+        # Try it with all arguments #
         intr.update_file_system('name1', 'contents1', permissions='rwxrw-rw-', location='~/new/place')
         self.assertTrue(intr.state.fs['~/new/place/name1'] == File('~/new/place/name1', 'contents1', 'rwxrw-rw-'))
 
-        """ Try it without location """
+        # Try it without location #
         intr.update_file_system('name2', 'contents2', permissions='rwxrw-rw-')
         self.assertTrue(intr.state.fs['~/name2'] == File('~/name2', 'contents2', 'rwxrw-rw-'))
 
-        """ Try it without permissions """
+        # Try it without permissions #
         intr.update_file_system('name3', 'contents3')
         self.assertTrue(intr.state.fs['~/name3'] == File('~/name3', 'contents3', 'rw-rw-rw-'))
 
-        """ Update a file already in the file system """
+        # Update a file already in the file system #
         intr.update_file_system('name3', 'contents4')
         self.assertTrue(intr.state.fs['~/name3'] == File('~/name3', 'contents4', 'rw-rw-rw-'))
 
 
     def test_replace(self):
-        """ This should mirror test_bpPrimitives.test_replace """
+        # This should mirror test_bpPrimitives.test_replace #
         self.assertRaises(InterpreterError, InterpreterBase().replace, 1234)
         var_list = {'one':['two']}
         intr = InterpreterBase(variables=var_list)
         node = bashparser.parse("echo $one")
         replaced = intr.replace(node)
         self.assertTrue(replaced[0] == bashparser.parse('echo two')[0])
 
@@ -119,24 +115,27 @@
         intr = Full_Interpreter()               # Need to use full interpreter so echo command is known
         node = bashparser.parse("echo $one")[0]
 
         self.assertRaises(InterpreterError, intr.build, 1234)
         self.assertRaises(InterpreterError, intr.build, node, 1234)
 
         intr.build(node)
-        self.assertTrue(len(intr.action_stack) == 2)
+        self.assertTrue(len(intr.action_stack) == 3)
         self.assertTrue(intr.action_stack[0] == 'Initialize state for command')
         self.assertTrue(intr.action_stack[1] == 'Command node: echo')
+        self.assertTrue(intr.action_stack[2] == 'Exit Node Cleanup')
 
         intr.build(node, append = True)
-        self.assertTrue(len(intr.action_stack) == 4)
+        self.assertTrue(len(intr.action_stack) == 6)
         self.assertTrue(intr.action_stack[0] == 'Initialize state for command')
         self.assertTrue(intr.action_stack[1] == 'Command node: echo')
-        self.assertTrue(intr.action_stack[2] == 'Initialize state for command')
-        self.assertTrue(intr.action_stack[3] == 'Command node: echo')
+        self.assertTrue(intr.action_stack[2] == 'Exit Node Cleanup')
+        self.assertTrue(intr.action_stack[3] == 'Initialize state for command')
+        self.assertTrue(intr.action_stack[4] == 'Command node: echo')
+        self.assertTrue(intr.action_stack[5] == 'Exit Node Cleanup')
 
 
     def test_set_variable(self):
         self.assertRaises(InterpreterError, InterpreterBase().set_variable, 1234, 'value')
         self.assertRaises(InterpreterError, InterpreterBase().set_variable, 'name', 1234)
 
         intr = InterpreterBase()
@@ -186,53 +185,54 @@
     def test_run(self):
         intr = Full_Interpreter()
         self.assertRaises(InterpreterError, intr.run, 1234)
 
         node1 = bashparser.parse('echo hello world')[0]
         node2 = bashparser.parse('echo this')[0]
         
-        """ Verify it works normally """
+        # Verify it works normally #
         intr.run(node1)
-        self.assertTrue(intr.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.get_screen() == 'hello world\n')
         intr.state.STDIO.OUT = ''
 
-        """ Verify it overrides build stack """
+        # Verify it overrides build stack #
         intr.build(node1)
         intr.run(node2)
-        self.assertTrue(intr.state.STDIO.OUT == 'this')
+        self.assertTrue(intr.get_screen() == 'hello world\nthis\n')
         intr.state.STDIO.OUT = ''
         
-        """ Verify it works if command is pre-built """
+        # Verify it works if command is pre-built #
+        intr.state.screen = ""
         intr.build(node1)
         intr.run()
-        self.assertTrue(intr.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.get_screen() == 'hello world\n')
 
 
     def test_run_command(self):
-        """ Test valid command pushed onto stack """
+        # Test valid command pushed onto stack #
         cmd_node = bashparser.parse('echo this')[0]
         intr = Full_Interpreter()
         intr.run_command(cmd_node.parts[0], cmd_node.parts[1:], cmd_node)
 
         self.assertTrue(len(intr.action_stack) == 1)
         self.assertTrue(str(intr.action_stack[-1]) == 'Command node: echo')
 
-        """ Test assignment node """
+        # Test assignment node #
         assign_node = bashparser.parse('a=b')[0]
         intr.run_command(assign_node.parts[0], assign_node.parts[1:], assign_node)
         self.assertTrue(len(intr.action_stack) == 3)
         self.assertTrue(str(intr.action_stack[-1]) == 'Variable Assignment')
 
-        """ Test invalid command push onto stack """
+        # Test invalid command push onto stack #
         unknown_node = bashparser.parse('TestingCommand -flg arg ument')[0]
         intr.run_command(unknown_node.parts[0], unknown_node.parts[1:], unknown_node)
         self.assertTrue(len(intr.action_stack) == 4)
         self.assertTrue(str(intr.action_stack[-1]) == 'Command node: TestingCommand')
 
-        """ Verify command substitution pushing onto the stack """
+        # Verify command substitution pushing onto the stack #
         intr.action_stack = []
         cmd_sub_node = bashparser.parse('a=$(echo this)')[0]
         intr.run_command(cmd_sub_node.parts[0], cmd_sub_node.parts[1:], cmd_sub_node)
         self.assertTrue(str(intr.action_stack[0]) == 'Entering Assignment Node: a=$(echo this)')
         self.assertTrue(str(intr.action_stack[1]) == 'Enter Command Substitution Env: a=$(echo this)')
         self.assertTrue(str(intr.action_stack[2]) == 'Exiting Command Substitution Env: a=$(echo this)')
         self.assertTrue(str(intr.action_stack[3]) == 'Variable Assignment')
@@ -245,29 +245,28 @@
 
         intr.set_truth('something', True)
         self.assertTrue(intr.test_truth('something'))
 
 
     def test_test_truth(self):
         intr = InterpreterBase()
-        self.assertRaises(InterpreterError, intr.test_truth, 1234)
 
         intr.set_truth('something', True)
         self.assertTrue(intr.test_truth('something'))
 
         intr.set_truth('something', False)
         self.assertTrue(not intr.test_truth('something'))
 
 
     def test_command_substitution(self):
         # Verify the replacement works
         node = bashparser.parse("f=$(cd $b)")[0]
         intr = Full_Interpreter()
         intr.run(node)
-        self.assertTrue(intr.state.variables == {'f':[''], 'b':['']})
+        self.assertTrue(intr.state.variables == {'f':['']})
 
         # Verify the file system changes properly with cp
         intr = Full_Interpreter()
         node = bashparser.parse("$(cp this that)")[0]
         intr.run(node)
         expected_intr = Full_Interpreter()
         expected_intr.run(bashparser.parse("cp this that")[0])
@@ -281,22 +280,22 @@
         expected_intr.run(bashparser.parse("mv over rainbow")[0])
         self.assertTrue(intr.state.fs == expected_intr.state.fs)
 
         # Verify the stdout is replaced properly with echo
         intr = Full_Interpreter()
         node = bashparser.parse("echo $(echo this)")[0]
         intr.run(node)
-        self.assertTrue(intr.stdout() == 'this')
+        self.assertTrue(intr.get_screen() == 'this\n')
 
 
     def test_interpreter(self):
-        """ Add random edge cases to this section """
+        # Add random edge cases to this section #
 
-        """ Verify the variable assignment only happens when inched through. 
-            This was a bug that happened """
+        # Verify the variable assignment only happens when inched through. 
+            # This was a bug that happened #
         bash_node = bashparser.parse('echo a; b=3; echo $b; b=4; echo $b')[0]
         intr = Full_Interpreter()
         expected_state = State()
         intr.build(bash_node)
         self.assertTrue(expected_state == intr.state)
         intr.inch() # init state for command
         self.assertTrue(expected_state == intr.state)
@@ -363,7 +362,76 @@
         # Now the function should be replaced
         self.assertTrue(str(intr.action_stack[0] == 'Enter the function scope'))
         self.assertTrue(str(intr.action_stack[0] == 'Command node: echo'))
         self.assertTrue(str(intr.action_stack[0] == 'Exit the function scope'))
         intr.inch()
         intr.inch()
         self.assertTrue(intr.stdout() == 'this wordsIn')
+
+
+    def test_file_redirects(self):
+        code = '( echo "text for the file" ) > ~/testing'
+        nodes = bashparser.parse(code)
+        intr = Full_Interpreter()
+        intr.run(nodes[0])
+        self.assertTrue('~/testing' in intr.state.fs)
+
+
+    def test_variable_scoping(self):
+        # just regular scoping
+        code = 'a="upper scope"; b=$(a="lower scope"; echo $a)'
+        nodes = bashparser.parse(code)
+        intr = Full_Interpreter()
+        intr.run(nodes[0])
+        self.assertTrue(intr.state.variables == {'a':['upper scope'], 'b':['lower scope']})
+
+        # Variable scoping and function scoping in one go
+        code = """Print1() {
+                    echo $a
+                  }
+                  a="upper scope"; b=$(a="lower scope"; Print1)"""
+        nodes = bashparser.parse(code)
+        intr = Full_Interpreter()
+        intr.run(nodes[0])
+        intr.run(nodes[1])
+        self.assertTrue(intr.state.variables == {'a':['upper scope'], 'b':['lower scope ']})
+
+
+    def test_substringing(self):
+        code = 'a="this node"; b=${a:0:4}'
+        nodes = bashparser.parse(code)
+        intr = Full_Interpreter()
+        intr.run(nodes[0])
+        self.assertTrue(intr.state.variables == {'a':['this node'], 'b':['this']})
+        
+    def test_array_indexing(self):
+        code = 'a="not an array"; b=${a[2]}'
+        nodes = bashparser.parse(code)
+        intr = Full_Interpreter()
+        intr.run(nodes[0])
+        self.assertTrue(intr.state.variables == {'a':['not an array'], 'b':['']})
+
+    def test_quoted_command_substitution_replacement(self):
+        code = """Print1() {
+                    echo $a
+                  }
+                  a="upper scope"; b=\"$(a="lower scope"; Print1)\""""
+        nodes = bashparser.parse(code)
+        intr = Full_Interpreter()
+        intr.run(nodes[0])
+        intr.run(nodes[1])
+        self.assertTrue(intr.state.variables == {'a':['upper scope'], 'b':['lower scope ']})
+
+
+
+    # This test requires user interaction so its been removed
+    # Just verify it every one in  while
+    # Could also consider adding functionality to execute automatically
+    # def test_commands_in_if_statements(self):
+    #     code = 'if echo "this"; then echo success; else echo failed; fi'
+    #     nodes = bashparser.parse(code)
+    #     intr = Full_Interpreter()
+    #     intr.run(nodes[0])
+    #     self.assertTrue(intr.state.get_screen() == 'success\n')
+        
+
+
```

### Comparing `jiujitsu-0.4/jiujitsu/test/test_bpPrimitives.py` & `jiujitsu-0.5/jiujitsu/test/test_bpPrimitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from unittest import TestCase
-# from bpPrimitives import State
-# from bpFileSystem import File, FileSocket
+
 from jiujitsu import State, File, FileSocket
+
 import bashparser
 
 class TestState(TestCase):
-    
     def test_init(self):
         stdio = FileSocket(id_num = 1)
         working_dir = '~/some/where'
         variables = {
             'name1':['value1'],
             'name2':['value2', 'value3']
         }
-        """ Test loading the state from a json """
+        # Test loading the state from a json #
         fs = [
             { 
                 "name": "~/name1",
                 "contents": "value1",
                 "permissions": "rw-rw-rw-"
             }
         ]
-        """ Actual fs form """
+        # Actual fs form #
         fs2 = {
             "~/name1": File("~/name1", "value1", "rw-rw-rw-")
         }
         open_socket = []
         truths = {
             'something':True,
             'else':False,
@@ -37,77 +36,77 @@
         self.assertTrue(new_state.working_dir == working_dir)
         self.assertTrue(new_state.variables == variables)
         self.assertTrue(new_state.fs == fs2)    # Verify the file has been unpacked correctly
         self.assertTrue(new_state.open_sockets == open_socket)
         self.assertTrue(new_state.truths == truths)
 
 
-        """ Verify not unpacking fs also works """
+        # Verify not unpacking fs also works #
         new_state2 = State(STDIO=stdio, working_dir=working_dir, variables=variables, 
                         fs=fs2, open_sockets=open_socket, truths=truths)
         self.assertTrue(new_state2.STDIO == stdio)
         self.assertTrue(new_state2.working_dir == working_dir)
         self.assertTrue(new_state2.variables == variables)
         self.assertTrue(new_state2.fs == new_state.fs)    # Verify the file has been unpacked correctly
         self.assertTrue(new_state2.open_sockets == open_socket)
         self.assertTrue(new_state2.truths == truths)
 
 
     def test_update_file_system(self):
-        """ This should mirror test_bpInterpreterBase.test_update_file_system """
+        # This should mirror test_bpInterpreterBase.test_update_file_system #
         stdio = State()
         
-        """ Try it with all arguments """
+        # Try it with all arguments #
         stdio.update_file_system('name1', 'contents1', permissions='rwxrw-rw-', location='~/new/place')
         self.assertTrue(stdio.fs['~/new/place/name1'] == File('~/new/place/name1', 'contents1', 'rwxrw-rw-'))
 
 
-        """ Try it without location """
+        # Try it without location #
         stdio.update_file_system('name2', 'contents2', permissions='rwxrw-rw-')
         self.assertTrue(stdio.fs['~/name2'] == File('~/name2', 'contents2', 'rwxrw-rw-'))
 
-        """ Try it without permissions """
+        # Try it without permissions #
         stdio.update_file_system('name3', 'contents3')
         self.assertTrue(stdio.fs['~/name3'] == File('~/name3', 'contents3', 'rw-rw-rw-'))
 
-        """ Update a file already in the file system """
+        # Update a file already in the file system #
         stdio.update_file_system('name3', 'contents4')
         self.assertTrue(stdio.fs['~/name3'] == File('~/name3', 'contents4', 'rw-rw-rw-'))
 
-        """ Verify ./ gets replaced properly """
+        # Verify ./ gets replaced properly #
         stdio.update_file_system('./name4', 'contents4')
         self.assertTrue(stdio.fs['~/name4'] == File('~/name4', 'contents4', 'rw-rw-rw-'))
 
-        """ Verify trailing slash gets removed properly """
+        # Verify trailing slash gets removed properly #
         stdio.update_file_system('./name5/', 'contents5')
         self.assertTrue(stdio.fs['~/name5'] == File('~/name5', 'contents5', 'rw-rw-rw-'))
 
 
     def test_replace(self):
-        """ Most of the replacement testing is actually in bashparser """
-        """ This should mirror test_bpInterpreterBase.test_replace """
+        # Most of the replacement testing is actually in bashparser #
+        # This should mirror test_bpInterpreterBase.test_replace #
         var_list = {'one':['two']}
         stdio = State(variables=var_list)
         node = bashparser.parse("echo $one")
         replaced = stdio.replace(node)
         self.assertTrue(replaced[0] == bashparser.parse('echo two')[0])
 
-        """ Thanks Wes for finding this bug """
+        # Thanks Wes for finding this bug #
         node = bashparser.parse("echo a; b=3; echo $b")
-        replaced = stdio.replace(node)
+        replaced = stdio.replace(node, full=True)
         self.assertTrue(replaced[0] == bashparser.parse('echo a; b=3; echo 3')[0])
 
 
     def test_set_variable(self):
         stdio = State()
-        """ Make sure it gets wrapped in an array """
+        # Make sure it gets wrapped in an array #
         stdio.set_variable('name', 'value1')
         self.assertTrue(stdio.variables['name'] == ['value1'])
 
-        """ Verify the default case """
+        # Verify the default case #
         stdio.set_variable('name2', ['value2', 'value3'])
         self.assertTrue(stdio.variables['name2'] == ['value2', 'value3'])
 
 
     def test_update_variable_list(self):
          stdio = State()
          node = bashparser.parse('a=b')[0]
```

### Comparing `jiujitsu-0.4/jiujitsu/test/test_jInterpreter.py` & `jiujitsu-0.5/jiujitsu/test/test_jInterpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,182 +1,178 @@
 from unittest import TestCase
-# from jInterpreter import Interpreter
-# from jParser import Parser
-# from jNode import Flag, Arg
-# from bpFileSystem import File, FileSocket
+
 from jiujitsu import jjInterpreter as Interpreter
 from jiujitsu import File, FileSocket
 from jiujitsu import Parser, Flag, Arg
+
 import bashparser, os, copy, sys
 
 old_stdout = sys.stdout # backup current stdout
 
 class TestjInterpreter(TestCase):
-
     def squelch(self):
         sys.stdout = open(os.devnull, "w")
         
     def unsquelch(self):
         sys.stdout = old_stdout # reset old stdout
 
     def test_args_to_str(self):
-        """ Test with unescaping the text """
+        # Test with unescaping the text
         string = r'arg1 arg2 "arg3.1 \t\"arg3.2\"" arg4'
         flags, args = Parser().parse(string)
         expected_string = r'arg1 arg2 "arg3.1 \t\"arg3.2\"" arg4'
         result_string = Interpreter().args_to_str(args, unescape=True)
         self.assertTrue(result_string == expected_string)
 
-        """ Test without unescaping the string """
+        # Test without unescaping the string #
         result_string = Interpreter().args_to_str(args, unescape=False)
         expected_string = 'arg1 arg2 arg3.1 \t"arg3.2" arg4'
         self.assertTrue(result_string == expected_string)
         
-        """ Verify the default value """
+        # Verify the default value #
         result_string = Interpreter().args_to_str(args)
         expected_string = 'arg1 arg2 arg3.1 \t"arg3.2" arg4'
         self.assertTrue(result_string == expected_string)
 
-
     def test_load(self):
         self.squelch()
         intr = Interpreter()
         intr.do_load('test.sh')
         self.unsquelch()
-        """ Build correct answers """
+        # Build correct answers #
         nodes = bashparser.parse('mv /usr/bin/something /usr/bin/else') + bashparser.parse('echo this') + bashparser.parse('cat test.sh | grep grep')
         nodes[1] = bashparser.align(nodes[1], nodes[0].pos[1] + 1)
         nodes[2] = bashparser.align(nodes[2], nodes[1].pos[1] + 1)
         
-        """  Verify the nodes properly loaded into Interpreter.prog_nodes """
+        #  Verify the nodes properly loaded into Interpreter.prog_nodes #
         self.assertTrue(len(intr.prog_nodes) == len(nodes))
         for i, node in enumerate(nodes):
             self.assertTrue(intr.prog_nodes[i] == nodes[i])
 
-        """ Verify nothing happens if not text for filename """
+        # Verify nothing happens if not text for filename #
         self.squelch()
         intr.do_load('')
         self.unsquelch()
         for i, node in enumerate(nodes):
             self.assertTrue(intr.prog_nodes[i] == nodes[i])
 
 
     def test_next(self):
         intr = Interpreter()
 
         intr.maintain_history = False
         initial_env_len = len(intr.history_stack)
 
-        """ Run the command flat out. No new history should be added """
+        # Run the command flat out. No new history should be added #
         intr.prog_nodes = bashparser.parse('echo hello world')
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.state.get_screen() == 'hello world\n')
         self.assertTrue(initial_env_len == len(intr.history_stack))
 
-        """ Verify h flag will create a new history entry """
+        # Verify h flag will create a new history entry #
         intr.prog_nodes = bashparser.parse('echo hello world')
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('-h')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.state.get_screen() == 'hello world\n')
         self.assertTrue(initial_env_len + 1 == len(intr.history_stack))
         intr.history_stack = intr.history_stack[:-1]
 
-        """ Verify i flag will alias to build """
+        # Verify i flag will alias to build #
         intr.prog_nodes = bashparser.parse('echo hello world')
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('-i')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == '')
-        self.assertTrue(1 == len(intr.env.action_stack))
+        self.assertTrue(intr.env.state.get_screen() == '')
+        self.assertTrue(3 == len(intr.env.action_stack))
         intr.history_stack = intr.history_stack[:-1]
 
-        """ Verify the e flag will execute in the environment """
-        """ Actually move a file in the env """
+        # Verify the e flag will execute in the environment #
+        # Actually move a file in the env #
         intr.env.state.update_file_system('test.sh', 'some contents', location='.')
         intr.prog_nodes = bashparser.parse('cp ./test.sh ./test2.sh')
+        intr.env.action_stack = []
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('-e')
         self.unsquelch()
 
-        """ Verify the move file exists in the env """
+        # Verify the move file exists in the env #
         files = [f for f in os.listdir('.') if os.path.isfile(f)]
         self.assertTrue('test2.sh' in files)
 
-        """ Delete the file in the env """
+        # Delete the file in the env #
         intr.prog_nodes = bashparser.parse('rm ./test2.sh')
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('-e')
         self.unsquelch()
         intr.history_stack = intr.history_stack[:-2]
 
-        """ Verify maintain_history = True will add an entry into the history """
+        # Verify maintain_history = True will add an entry into the history #
         intr.maintain_history = True
         intr.prog_nodes = bashparser.parse('echo hello world')
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.get_screen() == 'hello world\n')
         self.assertTrue(initial_env_len == len(intr.history_stack))
 
 
     def test_undo(self):
-        """ Verify undo works in the init case """
+        # Verify undo works in the init case #
         intr = Interpreter(config_file='./judo_config')
         intr.env.state.STDIO.IN = "something random"
         self.squelch()
         intr.do_undo('')
         self.unsquelch()
         intr2 = Interpreter(config_file='./judo_config')
         self.assertTrue(intr.env == intr2.env)
         self.assertTrue(intr.index == intr2.index)
         self.assertTrue(len(intr.history_stack) == len(intr2.history_stack))
         for i, el in enumerate(intr.history_stack):
             self.assertTrue(intr.history_stack[i] == intr2.history_stack[i])
         
 
-        """ Verify undo works with more than 1 entry """
+        # Verify undo works with more than 1 entry #
         intr.prog_nodes = bashparser.parse('echo hello world')
         intr.index = 0
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_next('')
         self.unsquelch()
 
         intr.prog_nodes = bashparser.parse('echo hello world')
         intr.index = 0
         self.squelch()
         intr.do_next('')
         self.unsquelch()
 
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.get_screen() == 'hello world\nhello world\n')
         self.assertTrue(3 == len(intr.history_stack))
 
         self.squelch()
         intr.do_undo('')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.get_screen() == 'hello world\n')
         self.assertTrue(2 == len(intr.history_stack))
 
 
-
     def test_skip(self):
         intr = Interpreter()
         self.squelch()
         intr.do_skip('')
         self.unsquelch()
         self.assertTrue(intr.index == 1)
 
@@ -190,19 +186,20 @@
 
         self.squelch()
         intr.do_save('some name')
         self.unsquelch()
         self.assertTrue(intr.history_stack[1].name == 'some name')
         self.assertTrue(intr.history_stack[1].action == 'User Save')
 
-
     def test_inch(self):
         intr = Interpreter()
         self.squelch()
         intr.do_build("echo this")
+        for el in intr.env.action_stack:
+            print(el)
         intr.do_inch('')
         intr.do_inch('')
         self.assertTrue(intr.env.state.STDIO.OUT == 'this')
         intr.do_inch('')
         self.unsquelch()
         self.assertTrue(len(intr.env.action_stack) == 0)
 
@@ -216,151 +213,146 @@
         self.unsquelch()
         self.assertTrue(intr.index == 2)
         self.squelch()
         intr.do_inch('')
         intr.do_inch('-e')
         intr.do_inch('')
         intr.do_inch('-e')
+        intr.do_inch('')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'cat test.sh | grep grep\n')
-
+        self.assertTrue(intr.env.get_screen() == 'this\ncat test.sh | grep grep\n\n')
 
     def test_run(self):
         intr = Interpreter()
         self.squelch()
         intr.do_load('test.sh')
         self.unsquelch()
 
-        """ Build correct answers """
+        # Build correct answers #
         nodes = bashparser.parse('mv /usr/bin/something /usr/bin/else') + bashparser.parse('echo this') + bashparser.parse('cat test.sh | grep grep')
         nodes[1] = bashparser.align(nodes[1], nodes[0].pos[1] + 1)
         nodes[2] = bashparser.align(nodes[2], nodes[1].pos[1] + 1)
         
-        """  Verify the nodes properly loaded into Interpreter.prog_nodes """
+        #  Verify the nodes properly loaded into Interpreter.prog_nodes #
         self.assertTrue(len(intr.prog_nodes) == len(nodes))
         for i, node in enumerate(nodes):
             self.assertTrue(intr.prog_nodes[i] == nodes[i])
 
-
     def test_next(self):
         intr = Interpreter()
 
         intr.maintain_history = False
         initial_env_len = len(intr.history_stack)
 
-        """ Run the command flat out. No new history should be added """
-        intr.env.state.STDIO.OUT = ''
+        # Run the command flat out. No new history should be added #
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_run('echo hello world')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.state.get_screen() == 'hello world\n')
         self.assertTrue(initial_env_len == len(intr.history_stack))
 
-        """ Verify h flag will create a new history entry """
-        intr.env.state.STDIO.OUT = ''
+        # Verify h flag will create a new history entry #
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_run('-h echo hello world')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.state.get_screen() == 'hello world\n')
         self.assertTrue(initial_env_len + 1 == len(intr.history_stack))
         intr.history_stack = intr.history_stack[:-1]
 
-        """ Verify i flag will alias to build """
-        intr.env.state.STDIO.OUT = ''
+        # Verify i flag will alias to build #
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_run('-i echo hello world')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == '')
-        self.assertTrue(len(intr.env.action_stack) == 2)
+        self.assertTrue(intr.env.state.get_screen() == '')
+        self.assertTrue(len(intr.env.action_stack) == 3)
         intr.history_stack = intr.history_stack[:-1]
 
-        """ Verify the e flag will execute in the environment """
-        """ Actually move a file in the env """
+        # Verify the e flag will execute in the environment #
+        # Actually move a file in the env #
         intr.env.state.update_file_system('test.sh', 'some contents', location='.')
-        intr.env.state.STDIO.OUT = ''
+        intr.env.state.screen = ''
         self.squelch()
         intr.do_run('-e cp ./test.sh ./test2.sh')
         self.unsquelch()
 
-        """ Verify the move file exists in the env """
+        # Verify the move file exists in the env #
         files = [f for f in os.listdir('.') if os.path.isfile(f)]
         self.assertTrue('test2.sh' in files)
 
-        """ Delete the file in the env """
-        intr.env.state.STDIO.OUT = ''
+        # Delete the file in the env #
         self.squelch()
         intr.do_run('-e rm ./test2.sh')
         self.unsquelch()
         intr.history_stack = intr.history_stack[:-2]
 
-        """ Verify maintain_history = True will add an entry into the history """
+        # Verify maintain_history = True will add an entry into the history #
+        intr.env.state.screen = ''
         intr.maintain_history = True
-        intr.env.state.STDIO.OUT = ''
         self.squelch()
         intr.do_run('echo hello world')
         self.unsquelch()
-        self.assertTrue(intr.env.state.STDIO.OUT == 'hello world')
+        self.assertTrue(intr.env.state.get_screen() == 'hello world\n')
         self.assertTrue(initial_env_len == len(intr.history_stack))
 
-
     def test_build(self):
         intr = Interpreter()
         self.squelch()
         intr.do_build('echo this')
         self.unsquelch()
         
-        for i in range(0, len(intr.env.action_stack)-1, 2):
-            self.assertTrue(str(intr.env.action_stack[i]) == 'Initialize state for command')
-            self.assertTrue(str(intr.env.action_stack[i+1]) == 'Command node: echo')
+        self.assertTrue(str(intr.env.action_stack[0]) == 'Initialize state for command')
+        self.assertTrue(str(intr.env.action_stack[1]) == 'Command node: echo')
+        self.assertTrue(str(intr.env.action_stack[2]) == 'Exit Node Cleanup')
         self.assertTrue(len(intr.env.action_stack) == 3)
 
-        """ Verify that append works """
+        # Verify that append works #
         self.squelch()
         intr.do_build('-a echo this')
         self.unsquelch()
-        for i in range(0, len(intr.env.action_stack)-1, 2):
+        for i in range(0, len(intr.env.action_stack)-1, 3):
             self.assertTrue(str(intr.env.action_stack[i]) == 'Initialize state for command')
             self.assertTrue(str(intr.env.action_stack[i+1]) == 'Command node: echo')
-        self.assertTrue(len(intr.env.action_stack) == 4)
+            self.assertTrue(str(intr.env.action_stack[i+2]) == 'Exit Node Cleanup')
 
+        self.assertTrue(len(intr.env.action_stack) == 6)
 
     def test_syscall(self):
         self.squelch()
         Interpreter().do_shell('cp test.sh test2.sh')
         self.unsquelch()
         files = [f for f in os.listdir('.') if os.path.isfile(f)]
         self.assertTrue('test2.sh' in files)
         self.squelch()
         Interpreter().do_shell('rm test2.sh')
         self.unsquelch()
         files = [f for f in os.listdir('.') if os.path.isfile(f)]
         self.assertTrue('test2.sh' not in files)
 
-
     def test_dir(self):
         intr = Interpreter()
         self.squelch()
         intr.do_dir('one two')
         self.unsquelch()
         self.assertTrue(intr.env.state.working_dir == '~')
 
         self.squelch()
         intr.do_dir('~/one')
         self.unsquelch()
         self.assertTrue(intr.env.state.working_dir == '~/one')
 
-
     def test_stdin(self):
         intr = Interpreter()
         self.squelch()
         intr.do_stdin('some text')
         self.unsquelch()
         self.assertTrue(intr.env.state.STDIO.IN == 'some text')
 
-
     def test_stdout(self):
         intr = Interpreter()
         self.squelch()
         intr.do_stdout('some text')
         self.unsquelch()
         self.assertTrue(intr.env.state.STDIO.OUT == 'some text')
 
@@ -375,58 +367,56 @@
 
         self.squelch()
         intr.do_var('-p name1 : value1.5 name2:value2.5')
         self.unsquelch()
         self.assertTrue(intr.env.state.variables['name1'] == ['value1.5'])
         self.assertTrue(intr.env.state.variables['name2'] == ['value2.5'])
 
-
     def test_fs(self):
-        """ Verify that it works for 1 """
+        # Verify that it works for 1 #
         intr = Interpreter()
         self.squelch()
         intr.do_fs('name1:contents1:rwxrw-rw-')
         self.unsquelch()
         self.assertTrue('~/name1' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name1'] == File(name='~/name1', contents='contents1', permissions='rwxrw-rw-'))
 
-        """ Verify that it works for multiple """
+        # Verify that it works for multiple #
         intr = Interpreter()
         self.squelch()
         intr.do_fs('name1:contents1:rw-rw-rw- name2:contents2:rw-rw-rw- \
                 name3 : contents3 : rw-rw-rw-')
         self.unsquelch()
         self.assertTrue('~/name1' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name1'] == File('~/name1', 'contents1', 'rw-rw-rw-'))
         self.assertTrue('~/name2' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name2'] == File('~/name2', 'contents2', 'rw-rw-rw-'))
         self.assertTrue('~/name3' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name3'] == File('~/name3', 'contents3', 'rw-rw-rw-'))
 
-        """ Verify that it adds permisions for 1 """
+        # Verify that it adds permisions for 1 #
         intr = Interpreter()
         self.squelch()
         intr.do_fs('name1:contents1')
         self.unsquelch()
         self.assertTrue('~/name1' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name1'] == File('~/name1', 'contents1', 'rw-rw-rw-'))
 
-        """ Verify it adds permissions for multiple """
+        # Verify it adds permissions for multiple #
         intr = Interpreter()
         self.squelch()
         intr.do_fs('name1:contents1   name2 : contents2 name3: contents3')
         self.unsquelch()
         self.assertTrue('~/name1' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name1'] == File('~/name1', 'contents1', 'rw-rw-rw-'))
         self.assertTrue('~/name2' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name2'] == File('~/name2', 'contents2', 'rw-rw-rw-'))
         self.assertTrue('~/name3' in intr.env.state.fs)
         self.assertTrue(intr.env.state.fs['~/name3'] == File('~/name3', 'contents3', 'rw-rw-rw-'))
 
-
     def test_history(self):
         intr = Interpreter()
 
         self.squelch()
         intr.do_history('on')
         self.unsquelch()
         self.assertTrue(intr.maintain_history == True)
@@ -437,26 +427,24 @@
         self.assertTrue(intr.maintain_history == False)
 
         self.squelch()
         intr.do_history('toggle')
         self.unsquelch()
         self.assertTrue(intr.maintain_history == True)
 
-
     def test_alias(self):
         intr = Interpreter()
         self.squelch()
         intr.do_alias('t run echo this')
         self.unsquelch()
         expected_json = {
             't':'run echo this'
         }
         self.assertTrue(expected_json == intr.alias_table)
 
-
     def test_truth(self):
         intr = Interpreter()
         self.squelch()
         intr.do_truth('this:true that:false one:t two:f two')
         self.unsquelch()
         self.assertTrue(intr.env.state.truths == {})
```

### Comparing `jiujitsu-0.4/jiujitsu/test/test_jParser.py` & `jiujitsu-0.5/jiujitsu/test/test_jParser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from unittest import TestCase
-# from jParser import Parser, ParseError
-# from jNode import Flag, Arg
 from jiujitsu import Parser, ParseError, Flag, Arg
 
 
 class TestjParser(TestCase):
     
     def test_init(self):
         string = '-p run -p echo'
```

### Comparing `jiujitsu-0.4/jiujitsu.egg-info/SOURCES.txt` & `jiujitsu-0.5/jiujitsu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiujitsu-0.4/setup.cfg` & `jiujitsu-0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jiujitsu
-version = 0.4
+version = 0.5
 author = Spencer Stingley
 description = A custom bash interpreter for malware execution
 long_description = A custom bash interpreter for malware execution
 url = https://github.com/BlankCanvasStudio/jiujitsu
 keywords = bash, parsing, interpreter, analysis, malware
 python_requires = >=3.6
 classifiers =
```

### Comparing `jiujitsu-0.4/setup.py` & `jiujitsu-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jiujitsu",
-    version="0.4",
+    version="0.5",
     author="Spencer Stingley",
     author_email="sstingle@usc.edu",
     description="A custom bash interpreter for malware execution",
     long_description="A custom bash interpreter for malware execution",
     long_description_content_type="text/markdown",
     url="https://github.com/BlankCanvasStudio/jiujitsu",
     packages=setuptools.find_packages(),
```

