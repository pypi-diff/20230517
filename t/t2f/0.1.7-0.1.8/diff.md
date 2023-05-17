# Comparing `tmp/t2f-0.1.7.tar.gz` & `tmp/t2f-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.7.tar", max compression
+gzip compressed data, was "t2f-0.1.8.tar", max compression
```

## Comparing `t2f-0.1.7.tar` & `t2f-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.7/README.md
--rw-r--r--   0        0        0      347 2023-05-14 20:34:41.459112 t2f-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.7/t2f/__init__.py
--rw-r--r--   0        0        0    43498 2023-05-14 07:08:34.228998 t2f-0.1.7/t2f/patched_asm.py
--rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.7/t2f/stdlib.py
--rw-r--r--   0        0        0    11888 2023-05-14 20:34:19.176126 t2f-0.1.7/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.7/t2f/utils.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.8/README.md
+-rw-r--r--   0        0        0      347 2023-05-17 02:17:19.175153 t2f-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.8/t2f/__init__.py
+-rw-r--r--   0        0        0    43498 2023-05-17 01:59:52.410855 t2f-0.1.8/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.8/t2f/stdlib.py
+-rw-r--r--   0        0        0    14592 2023-05-17 02:17:10.551721 t2f-0.1.8/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.8/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.8/PKG-INFO
```

### Comparing `t2f-0.1.7/t2f/patched_asm.py` & `t2f-0.1.8/t2f/patched_asm.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
 x{CF3C} @Defop(8u+1) BCHKBITSQ#
 x{CF3D} @Defop BCHKBITSQ
 x{CF3E} @Defop BCHKREFSQ
 x{CF3F} @Defop BCHKBITREFSQ
 x{CF40} @Defop STZEROES
 x{CF41} @Defop STONES
 x{CF42} @Defop STSAME
-{ tuck sbitrefs swap 23 + swap @havebitrefs not
+{ tuck sbitrefs swap 22 + swap @havebitrefs not
   { swap PUSHSLICE STSLICER }
   { over sbitrefs 2dup 57 3 2x<=
     { rot x{CFC_} s, swap 2 u, over 6 + 3 >> tuck 3 u, 3 roll s,
       -rot 3 << 2 + swap - @scomplete }
     { 2drop swap PUSHSLICE STSLICER } cond
   } cond
 } : STSLICECONST
```

### Comparing `t2f-0.1.7/t2f/stdlib.py` & `t2f-0.1.8/t2f/stdlib.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.7/t2f/t2f.py` & `t2f-0.1.8/t2f/t2f.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 
 
 class Procedure(object):
 
     def __init__(self, code):
         code_lines = code.split('\n')
         self.name = code_lines[0]
+        if self.name.endswith("_macro"):
+            self.name = self.name[0:-6]
         self.body = Procedure.process_code(code_lines[1:])
     
     def process_code(code_lines):
         global DEBUG
         result_list = [Continuation()]
         
         for line in code_lines:
@@ -97,14 +99,24 @@
                 #     cont_else.change_type("ELSE")
                 #     cont_1.opcodes.append(cont_0)
                 #     cont_1.opcodes.append(cont_else)
                 elif cont_0.type == "SECOND_":
                     cont_1.opcodes[-1].change_type("IF")
                     cont_0.change_type("ELSE")
                     cont_1.opcodes.append(cont_0)
+                elif cont_0.type == "COMPUTE":
+                    func_name = cont_0.opcodes[0].params[0]
+                    new_opcode = Opcode("", [f"<{{\n{func_name} INLINECALL\n}}>s 0 runvmx drop"])
+                    prev_opcode = cont_1.opcodes.pop()
+                    if prev_opcode.opcode in ["PUSHREF", "PUSHSLICE", "PUSHSLICE"] and prev_opcode.params is None:
+                        cont_1.opcodes.append(new_opcode)
+                        cont_1.opcodes.append(prev_opcode)
+                    else:
+                        cont_1.opcodes.append(prev_opcode)
+                        cont_1.opcodes.append(new_opcode)
                 else:
                     cont_1.add_opcode(cont_0)
                 result_list.append(cont_1)
             else:
                 ll = line.split(" ")
                 opcode_name = ll[-1]
                 params = None
@@ -114,23 +126,46 @@
                      result_list[-1].opcodes[-1].change_type("ELSE")
                      result_list[-1].opcodes[-2].change_type("IF")
                 elif opcode_name in ["IF", "IFNOT", "REPEAT", "IFJMP", "IFNOTJMP"]:
                      result_list[-1].opcodes[-1].change_type(opcode_name)
                 elif opcode_name == "WHILE":
                      result_list[-1].opcodes[-1].change_type("DO")
                      result_list[-1].opcodes[-2].change_type("WHILE")
+                elif opcode_name == "INLINECALL":
+                    func_name = params[0]
+                    if func_name.endswith("_macro"):
+                        func_name = func_name[0:-6]
+                    cont_0 = result_list.pop()
+                    cont_0.add_opcode(Opcode(opcode_name, [func_name]))
+                    result_list.append(cont_0)
                 else:
                     cont_0 = result_list.pop()
                     cont_0.add_opcode(Opcode(opcode_name, params))
                     result_list.append(cont_0)
         cont_0 = result_list[0]
         proc_code = cont_0.build_body()
         proc_code = re.sub(r'}>\s*ELSE:<{', r'}>ELSE<{', proc_code)
         proc_code = re.sub(r'}>\s*DO:<{', r'}>DO<{', proc_code)
         return proc_code
+    
+    def inline_all(self, procs):
+        new_lines = []
+        for line in self.body.split("\n"):
+            if "INLINECALL" in line:
+                proc_name = line.split(" ")[0]
+                proc = procs[proc_name]
+                new_lines.append(f"// begin {proc_name}")
+                for idx, l in enumerate(proc.body.split("\n")):
+                    if not len(re.findall(r'^\s*$', l)):
+                        new_lines.append(l)
+                
+                new_lines.append(f"// end {proc_name}")
+            else:
+                new_lines.append(line)
+        self.body = "\n".join(new_lines)
 
 
 class Program(object):   
 
     def __init__(self, procs, root=''):
         self.procs = procs
         self.root = root
@@ -148,26 +183,26 @@
         r += "\n"
         for proc in self.procs:
             r = Program.add_proc_body(r, self.procs[proc])
         internal = "recv_internal" in self.procs.keys()
         external = "recv_external" in self.procs.keys()
         ticktock = "run_ticktock" in self.procs.keys()
         if internal and not external and not ticktock:
-            r += "IFNOT: recv_internal INLINECALL\n\n"
+            r += "DUP IFNOT: recv_internal INLINECALL\n\n"
         else:
             if ticktock:
                 r += "DUP -2 EQINT IFJMP:<{\n" \
-                        "DROP run_ticktock INLINECALL\n" \
+                        "run_ticktock INLINECALL\n" \
                     "}>\n\n"
             if internal:
-                r += "DUP 0 EQINT IFJMP:<{\n" \
-                        "DROP recv_internal INLINECALL\n" \
+                r += "DUP IFNOTJMP:<{\n" \
+                        "recv_internal INLINECALL\n" \
                     "}>\n\n"
             if external:
-                r += "-1 EQINT IFJMP:<{\n" \
+                r += "DUP -1 EQINT IFJMP:<{\n" \
                         "recv_external INLINECALL\n" \
                     "}>\n\n"
                   
         return r + self.root + "}>"
 
     def return_cell(self):
         return self.build() + "c"
@@ -227,29 +262,30 @@
 
     code = re.sub(r'\.loc.+\n', r'', code)
     code = re.sub(r'\.loc.+$', r'', code)
 
     code = code.replace(".internal-alias :main_internal, 0\n.internal :main_internal", "recv_internal")
     code = code.replace(".internal-alias :main_external, -1\n.internal :main_external", "recv_external")
     code = code.replace(".internal-alias :onTickTock, -2\n.internal :onTickTock", "run_ticktock")
-    code = re.sub(r'.macro (\w+)', r'\1', code)
+    code = re.sub(r'\.macro (\w+)(?=_macro)?', r'\1', code)
 
     if len(re.findall(r'onCodeUpgrade', code)):
         print("ERROR: onCodeUpgrade currently is not supported")
         exit(1)
-        
+
     code = code.replace("\s$", "")
     code = code.replace("^\s", "")
     code = code.replace(" {", ":<{")
     code = code.replace(",", "")
     code = code.replace(".", "")
     code = code.replace("}", "}>")
     code = code.replace("PUSHCONT:<{", "CONT:<{")
-    
+
     code = code.replace("IFREF", "IF")
+    code = code.replace("IFNOTREF", "IFNOT")
     code = code.replace("ELSEREF", "ELSE")
     code = code.replace("IFJMPREF", "IFJMP")
     code = code.replace("IFNOTJMPREF", "IFNOTJMP")
     code = code.replace("PUSHREFSLICE", "PUSHSLICE")
 
     code = re.sub(r'S(\d+)', r's\1', code)
     code = re.sub(r'S(-\d+)', r's(\1)', code)
@@ -259,31 +295,47 @@
 
     code = re.sub(r'(STSLICECONST|PUSHSLICE|blob) x([\w_]*)', r'\1 x{\2}', code)
     code = re.sub(r'STSLICECONST 0', r'STZERO', code)
     code = re.sub(r'STSLICECONST 1', r'STONE', code)
 
     code = re.sub(r';.+', r'', code)
 
-    code = re.sub(r'( *)(\w+ )([\w \-{}()]+)*', r'\1\3 \2', code)
+    code = re.sub(r'( *)(\w+ )([\w \-{}()$]+)*', r'\1\3 \2', code)
+
+    code = re.sub(r'\$([\w\d_]+)\$ compute', r'COMPUTE:<{\n\1 INLINECALL\n}>', code)
 
     code = re.sub(r'(\d+ MODPOW2)', r'\1#', code)
     code = re.sub(r'(\d+ RSHIFT)', r'\1#', code)
     code = re.sub(r'(\d+ LSHIFT)', r'\1#', code)
 
     code = re.sub(r'\t+', r'', code)
     code = re.sub(r'[ ]+', r' ', code)
     code = re.sub(r'[ ]*(\n+)[ ]*', r'\1', code)
 
     code = code.replace("IFELSE\n{", "IFELSE_:<{")
     code = code.replace("\n{", "\nSECOND_:<{")
 
     # BUILD
-    procs = {proc.name:proc for proc in [Procedure(proc_code) for proc_code in code.split("\n\n")]}
+    procs = sort_procs({proc.name:proc for proc in [Procedure(proc_code) for proc_code in code.split("\n\n")]})
+
+    if args.inline:
+        for proc_name in procs:
+            procs[proc_name].inline_all(procs)
+            
+        funcs = []
+        if "recv_internal" in procs:
+            funcs.append("recv_internal")
+        if "recv_external" in procs:
+            funcs.append("recv_external")
+        if "run_ticktock" in procs:
+            funcs.append("run_ticktock")
+
+        procs = {proc_name:procs[proc_name] for proc_name in funcs}
 
-    prog = Program(sort_procs(procs))
+    prog = Program(procs)
     prog_code = prog.return_cell()
 
 
     lvl = 0
     proc_rows = prog_code.split("\n")
     for idx, row in enumerate(proc_rows):
         if "}>" in row:
@@ -300,15 +352,20 @@
     if args.asm:
         patched_asm_path = os.path.join(os.path.dirname(args.output), "PatchedAsm.fif")
         with open(patched_asm_path, 'w') as file:
             file.write(patched_asm)
         prog_code = '"PatchedAsm.fif" include\n\n' + prog_code
 
     if args.tvc:
-        prog_code += f'\n\n<b b{{00110}} s, swap ref, <b b> ref, b>\n' \
+        prog_code += f'\n\n' \
+                     f'<b\n' \
+                     f'    b{{00110}} s,\n' \
+                     f'    swap ref,\n' \
+                     f'    <b x{{0000000000000000000000000000000000000000000000000000000000000000}} 0 dictnew 64 udict! drop dict, b> ref,\n' \
+                     f'b>\n\n' \
                      f'2 boc+>B "{os.path.splitext(args.output)[0]}.tvc" B>file\n'
 
     with open(args.output, 'w') as file:
         file.write(prog_code)
 
 DEBUG = False
 
@@ -319,14 +376,15 @@
         description='TVM Assembly to Fift Assembly Translator',
     )
 
     parser.add_argument('filename')
     parser.add_argument('-o', '--output', dest='output', default=None, help='output file name')
     parser.add_argument('-t', '--tvc', dest='tvc', default=False, help='add tvc generation', action='store_true')
     parser.add_argument('-a', '--asm-include', dest='asm', default=False, help='add PatchedAsm.fif', action='store_true')
+    parser.add_argument('-i', '--inline-all', dest='inline', default=False, help='raw inline all functions', action='store_true')
     parser.add_argument('--debug', dest='debug', default=False, action='store_true')
 
     args = parser.parse_args()
 
     default_output = f'{os.path.splitext(args.filename)[0]}.fif'
     args.output = default_output if args.output is None else args.output
     DEBUG = args.debug
```

### Comparing `t2f-0.1.7/t2f/utils.py` & `t2f-0.1.8/t2f/utils.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.7/PKG-INFO` & `t2f-0.1.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2f
-Version: 0.1.7
+Version: 0.1.8
 Summary: TVM Assembly to Fift Assembly Translator
 Author: Andrew Gutarev
 Author-email: gutarev01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

