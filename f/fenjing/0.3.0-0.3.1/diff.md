# Comparing `tmp/fenjing-0.3.0.tar.gz` & `tmp/fenjing-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.0.tar", last modified: Wed May 17 10:25:43 2023, max compression
+gzip compressed data, was "fenjing-0.3.1.tar", last modified: Wed May 17 11:29:38 2023, max compression
```

## Comparing `fenjing-0.3.0.tar` & `fenjing-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-17 10:25:32.000000 fenjing-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 10:25:32.000000 fenjing-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 10:25:43.834142 fenjing-0.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5727 2023-05-17 10:25:32.000000 fenjing-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 10:25:32.000000 fenjing-0.3.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing/static/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:25:32.000000 fenjing-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:25:43.838142 fenjing-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 10:25:32.000000 fenjing-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-17 11:29:26.000000 fenjing-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 11:29:26.000000 fenjing-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 11:29:38.229593 fenjing-0.3.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5727 2023-05-17 11:29:26.000000 fenjing-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 11:29:26.000000 fenjing-0.3.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3992 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-17 11:29:26.000000 fenjing-0.3.1/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:29:38.229593 fenjing-0.3.1/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 11:29:38.000000 fenjing-0.3.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 11:29:26.000000 fenjing-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:29:38.229593 fenjing-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 11:29:26.000000 fenjing-0.3.1/setup.py
```

### Comparing `fenjing-0.3.0/LICENSE` & `fenjing-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/PKG-INFO` & `fenjing-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.0/README.md` & `fenjing-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/cli.py` & `fenjing-0.3.1/fenjing/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,19 +182,14 @@
             cracker = FormCracker(url=page_url, form=form, requester=requester)
             result = cracker.crack()
             if result is None:
                 continue
             full_payload_gen, field = result
             cmd_exec_func = partial(cmd_exec, cracker=cracker,
                                     field=field, full_payload_gen=full_payload_gen)
-            # def cmd_exec_func(cmd):
-            #     r = cracker.submit(
-            #         {field: payload_gen(cmd)})
-            #     assert r is not None
-            #     return r.text
             if exec_cmd == "":
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
```

### Comparing `fenjing-0.3.0/fenjing/colorize.py` & `fenjing-0.3.1/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/config_payload.py` & `fenjing-0.3.1/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/const.py` & `fenjing-0.3.1/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/form.py` & `fenjing-0.3.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/full_payload_gen.py` & `fenjing-0.3.1/fenjing/full_payload_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,21 +80,14 @@
         return True
 
     def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
 
         if not self.prepared and not self.do_prepare():
             return None, None
 
-        # inner_payload = payload_gen.generate(
-        #     gen_type,
-        #     *args,
-        #     waf_func=self.waf_func,
-        #     context=self.context
-        # )
-
         inner_payload = self.payload_gen.generate(gen_type, *args)
 
         if inner_payload is None:
             logger.warning("Bypassing WAF Failed.")
             return None, None
 
         assert isinstance(self.outer_pattern, str)
```

### Comparing `fenjing-0.3.0/fenjing/int_vars.py` & `fenjing-0.3.1/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/payload_gen.py` & `fenjing-0.3.1/fenjing/payload_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,14 @@
             self.count_success(gen_type, req_gen_func.__name__)
             self.cache_add(gen_type, *args, result=payload)
             self.callback(CALLBACK_GENERATE_PAYLOAD, {
                 "gen_type": gen_type,
                 "args": args,
                 "payload": payload
             })
-
             # 为了日志的简洁，仅打印一部分日志
             if gen_type in (INTEGER, STRING) and payload != str(args[0]):
                 logger.info("{great}, {gen_type}({args_repl}) can be {payload}".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
                                       for arg in args)),
@@ -141,61 +140,14 @@
         return generate_func(gen_type, *args)
 
 
 def generate(gen_type, *args, waf_func: Callable, context: Union[dict, None] = None) -> Union[str, None]:
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
-# def generate(gen_type, *args, waf_func: Union[Callable, None] = None, context: Union[dict, None] = None, cache: Union[dict, None] = None) -> Union[str, None]:
-
-#     if waf_func is None:
-#         raise Exception("waf_func cannot be None")
-#     if context is None:
-#         context = {}
-#     if cache is None:
-#         cache = {}
-
-#     if (gen_type, *args) in cache:
-#         return cache[(gen_type, *args)]
-
-#     if gen_type == LITERAL:
-#         value = args[0]
-#         if not waf_func(value):
-#             return None
-#         return value
-#     if gen_type == UNSATISFIED:
-#         return None
-
-#     if gen_type not in req_gens:
-#         raise Exception(f"gen_type {gen_type} not found")
-
-#     for gen_func in req_gens[gen_type].copy():
-#         generated_payload = ""
-#         son_req = gen_func(context, *args)
-#         assert isinstance(
-#             son_req, list), f"Wrong son_req {son_req} from {gen_func.__name__}"
-#         assert all(isinstance(req_type, str) for req_type, *
-#                    others in son_req), f"Wrong son_req {son_req} from {gen_func.__name__}"
-#         for son_type, *son_args in son_req:
-#             payload = generate(son_type, *son_args,
-#                                waf_func=waf_func, context=context, cache=cache)
-#             if payload is None:
-#                 generated_payload = None
-#                 break
-#             generated_payload += payload
-#         if generated_payload is not None and waf_func(generated_payload):
-#             used_count[gen_func.__name__] += 1
-#             req_gens[gen_type].sort(
-#                 key=lambda f: used_count[f.__name__], reverse=True)
-#             cache[(gen_type, *args)] = generated_payload
-#             return generated_payload
-#     cache[(gen_type, *args)] = None
-#     return None
-
-
 # ---
 
 @req_gen
 def gen_string_string_concat_plus(context: dict):
     return [
         (LITERAL, "+")
     ]
@@ -902,14 +854,18 @@
 
 
 @req_gen
 def gen_string_formatfunc2(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
+    if re.match("^[a-z]+$", value): # avoid infinite recursion
+        return [
+            (UNSATISFIED, )
+        ]
     if "{:c}" not in context.values():
         return [
             (UNSATISFIED, )
         ]
     k = [k for k, v in context.values() if v == "{:c}"][0]
     cs = "({c}*{l})".format(
         c=k,
@@ -927,14 +883,18 @@
 
 
 @req_gen
 def gen_string_formatfunc3(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
+    if re.match("^[a-z]+$", value): # avoid infinite recursion
+        return [
+            (UNSATISFIED, )
+        ]
     cs = "(({c})*{l})".format(
         c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)",
         l=len(value)
     )
     format_func = (ATTRIBUTE, (LITERAL, cs), "format")
     req = [
         (LITERAL, "("),
@@ -1235,15 +1195,14 @@
 if __name__ == "__main__":
     import time
     import functools
 
     @functools.lru_cache(100)
     def waf_func(payload: str):
         time.sleep(0.2)
-        # print(payload)
         return all(word not in payload for word in ['\'', '"', '.', '_', 'import', 'request', 'url', '\\x', 'os', 'system', '\\u', '22'])
 
     payload = generate(
         OS_POPEN_READ,
         "ls",
         waf_func=waf_func,
         context={"loo": 100, "lo": 10, "l": 1, "un": "_"}
```

### Comparing `fenjing-0.3.0/fenjing/requester.py` & `fenjing-0.3.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/scan_url.py` & `fenjing-0.3.1/fenjing/scan_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from typing import Union
-from .requester import Requester
 from .form import parse_forms
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("scan_url")
```

### Comparing `fenjing-0.3.0/fenjing/shell_payload.py` & `fenjing-0.3.1/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/static/style.css` & `fenjing-0.3.1/fenjing/static/style.css`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/fenjing/templates/index.html` & `fenjing-0.3.1/fenjing/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             <input type="text" id="inputs" name="inputs" placeholder="id,name" />
             <br /><br />
 
             <label for="action">提交 URL:</label>
             <input type="text" id="action" name="action" placeholder="可不填，默认和URL相同" />
             <br /><br />
 
-            <label for="action">请求间隔</label>
+            <label for="action">请求间隔:</label>
             <input type="text" id="interval" name="interval" value="0.1" />
             <br /><br />
 
             <input type="hidden" name="type" value="crack" />
             <input type="submit" value="开始分析">
         </form>
             <textarea name="taskFlashMessage" id="taskFlashMessage" cols="100" rows="3" readonly></textarea>
```

#### html2text {}

```diff
@@ -8,11 +8,11 @@
 
 è¯·æ±æ¹å¼: [One of: POST/GET]
 
 è¡¨åçææè¾å¥: [inputs              ]
 
 æäº¤ URL: [action              ]
 
-è¯·æ±é´é [0.1                 ]
+è¯·æ±é´é: [0.1                 ]
 
  [å¼å§åæ]
 [cmd                 ]   [æ§è¡Shellæä»¤]
```

### Comparing `fenjing-0.3.0/fenjing/waf_func_gen.py` & `fenjing-0.3.1/fenjing/waf_func_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from urllib.parse import urlparse
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
 from typing import List, Dict, Tuple, Callable, Any, Union
 
 from .const import *
-from .form import Form, random_fill, fill_form
+from .form import fill_form
 from .requester import Requester
 from .colorize import colored
 
 
 logger = logging.getLogger("waf_func_gen")
 Result = namedtuple("Result", "payload_generate_func input_field")
```

### Comparing `fenjing-0.3.0/fenjing/webui.py` & `fenjing-0.3.1/fenjing/webui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from flask import Flask, render_template, request, jsonify
 
 import logging
 import threading
 import uuid
 from urllib.parse import urlparse
-from traceback import print_exc
-from typing import Callable, List
-from functools import partial
 
 from .form import Form
 from .form_cracker import FormCracker
-from .full_payload_gen import FullPayloadGen
-from .scan_url import yield_form
 from .requester import Requester
 from .const import *
-from .colorize import colored
 
 logger = logging.getLogger("webui")
 app = Flask(__name__)
 tasks = {}
 
 class CallBackLogger:
     def __init__(self, flash_messages, messages):
```

### Comparing `fenjing-0.3.0/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.1/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.0/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.1/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.0/setup.py` & `fenjing-0.3.1/setup.py`

 * *Files identical despite different names*

