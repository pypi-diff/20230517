# Comparing `tmp/bardapi-0.1.3.tar.gz` & `tmp/bardapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.3.tar", last modified: Tue May 16 08:01:57 2023, max compression
+gzip compressed data, was "bardapi-0.1.4.tar", last modified: Wed May 17 16:57:03 2023, max compression
```

## Comparing `bardapi-0.1.3.tar` & `bardapi-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:57.844025 bardapi-0.1.3/
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6803 2023-05-16 08:01:57.842026 bardapi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5871 2023-05-16 08:01:33.000000 bardapi-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:57.823303 bardapi-0.1.3/bardapi/
--rw-rw-rw-   0        0        0      198 2023-05-16 08:00:37.000000 bardapi-0.1.3/bardapi/__init__.py
--rw-rw-rw-   0        0        0     3421 2023-05-16 08:01:33.000000 bardapi-0.1.3/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:57.840031 bardapi-0.1.3/bardapi.egg-info/
--rw-rw-rw-   0        0        0     6803 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 08:01:57.844530 bardapi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-05-16 08:00:32.000000 bardapi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:57:03.783180 bardapi-0.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7849 2023-05-17 16:57:03.783180 bardapi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6756 2023-05-17 16:42:09.000000 bardapi-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 16:57:03.772375 bardapi-0.1.4/bardapi/
+-rw-rw-rw-   0        0        0      198 2023-05-17 16:42:20.000000 bardapi-0.1.4/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     3714 2023-05-17 16:54:40.000000 bardapi-0.1.4/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:57:03.781145 bardapi-0.1.4/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     7849 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:57:03.784625 bardapi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-05-17 16:56:55.000000 bardapi-0.1.4/setup.py
```

### Comparing `bardapi-0.1.3/LICENSE` & `bardapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.3/PKG-INFO` & `bardapi-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
-Keywords: BARD,Python,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
-Classifier: Development Status :: 4 - Beta
+Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
+Classifier: Natural Language :: Korean
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Development Status :: 4 - Beta
+Development Status :: 5 - Production/Stable
 
 
 # Google <a href="https://bard.google.com/"><img src="https://camo.githubusercontent.com/adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667" height="20px"></a> Bard API 
 
 
 <p align="left">
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-BardAPI-black"></a>
-<a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 <!-- <a href="https://pepy.tech/project/bardapi"><img alt="Downloads" src="https://pepy.tech/badge/bardapi"></a> -->
 <!-- <a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/Bard-API?color=black"></a> -->
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=bardapi&edge_flat=false"/></a></a>
+<a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false"/></a>
+<a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 </p>
 
 > A package that returns Response of [Google Bard](https://bard.google.com/) through API
 
-![](./assets/bardapi.gif)
+![](./assets/bard_api.gif)
 
 
 I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
 
 <br>
 
 Never expose the `__Secure-1PSID` for your safety.
@@ -98,40 +101,63 @@
 # set your input text
 input_text = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 
 # Send an API request and get a response.
 response = bardapi.core.Bard().get_answer(input_text)
 ```
 
-Resolving errors due to delayed responses in Google Colab, containers, etc.
-- If a response error occurs even though the normal procedure has been followed, use the timeout variable.
+Addressing errors caused by delayed responses in environments like Google Colab and containers. If an error occurs despite following the proper procedure, utilize the timeout argument.
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
 bard = Bard(timeout=10) # Set timeout in seconds
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
+<br>
 
-## Behind a proxy
-
+## Futher
+### Behind a proxy
+If you are working behind a proxy, use the following.
 ```python
 from bardapi import Bard
 import os
 
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
-bard_inproxy = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
-bard_inproxy.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+```
+
+### Reusable session object
+```python
+from bardapi import Bard
+import os
+import requests
+
+os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
+session = requests.Session()
+session.headers = {
+            "Host": "bard.google.com",
+            "X-Same-Domain": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+            "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+            "Origin": "https://bard.google.com",
+            "Referer": "https://bard.google.com/",
+        }
+session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+
+bard = Bard(session=session)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
-Example
+Simple Example
 <br>
 
 <a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
 
 <br>
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.3 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.4 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
-parkminwoo1991@gmail.com Keywords: BARD,Python,Google Bard,Large Language
-Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
+parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
+Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
+Natural Language :: English Classifier: Natural Language :: Korean Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python ::
+3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 4 - Beta # Google [https://
+LICENSE Development Status :: 5 - Production/Stable # Google [https://
 camo.githubusercontent.com/
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
-[PyPI package] [PyPI]   [Code_style:_black] [https://hits.seeyoufarm.com/api/
-count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=bardapi&edge_flat=false]
+[PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
+incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
+[PyPI]
 > A package that returns Response of [Google Bard](https://bard.google.com/
-) through API ![](./assets/bardapi.gif) I referred to [this github repository
+) through API ![](./assets/bard_api.gif) I referred to [this github repository
 (github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference
 process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask
 questions and get answers from Google Bard. This package is designed for
 application to the Python package [ExceptNotifier](https://github.com/
 dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-
 Coder).
 Never expose the `__Secure-1PSID` for your safety. > Note that while I referred
@@ -44,26 +47,36 @@
 bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard
 ().get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ``` Or you can use this ```python import bardapi import
 os # set your __Secure-1PSID value to key os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # set your input text input_text = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤" # Send an API
 request and get a response. response = bardapi.core.Bard().get_answer
-(input_text) ``` Resolving errors due to delayed responses in Google Colab,
-containers, etc. - If a response error occurs even though the normal procedure
-has been followed, use the timeout variable. ```python from bardapi import Bard
-import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) # Set
-timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` ## Behind a proxy ```python
-from bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" #
-Change 'http://127.0.0.1:1080' to your http proxy # timeout in seconds
-bard_inproxy = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://
-127.0.0.1:1080'}, timeout=10) bard_inproxy.get_answer("ëì ë´
+(input_text) ``` Addressing errors caused by delayed responses in environments
+like Google Colab and containers. If an error occurs despite following the
+proper procedure, utilize the timeout argument. ```python from bardapi import
+Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) #
+Set timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+## Futher ### Behind a proxy If you are working behind a proxy, use the
+following. ```python from bardapi import Bard import os os.environ
+['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
+proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
+'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-Example
+### Reusable session object ```python from bardapi import Bard import os import
+requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' session = requests.Session
+() session.headers = { "Host": "bard.google.com", "X-Same-Domain": "1", "User-
+Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like
+Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type": "application/x-www-
+form-urlencoded;charset=UTF-8", "Origin": "https://bard.google.com", "Referer":
+"https://bard.google.com/", } session.cookies.set("__Secure-1PSID", os.environ
+["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
+ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
 -_[MIT](https://opensource.org/license/mit/)_-_I_hold_no_legal_responsibility;
 for_more_information,_please_refer_to_the_bottom_of_the_readme_file._I_just
 want_you_to_give_me_and_[them](https://github.com/acheong08/Bard)_a_star..._##
```

### Comparing `bardapi-0.1.3/README.md` & `bardapi-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Development Status :: 4 - Beta
+Development Status :: 5 - Production/Stable
 
 
 # Google <a href="https://bard.google.com/"><img src="https://camo.githubusercontent.com/adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667" height="20px"></a> Bard API 
 
 
 <p align="left">
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-BardAPI-black"></a>
-<a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 <!-- <a href="https://pepy.tech/project/bardapi"><img alt="Downloads" src="https://pepy.tech/badge/bardapi"></a> -->
 <!-- <a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/Bard-API?color=black"></a> -->
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=bardapi&edge_flat=false"/></a></a>
+<a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false"/></a>
+<a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 </p>
 
 > A package that returns Response of [Google Bard](https://bard.google.com/) through API
 
-![](./assets/bardapi.gif)
+![](./assets/bard_api.gif)
 
 
 I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
 
 <br>
 
 Never expose the `__Secure-1PSID` for your safety.
@@ -76,40 +76,63 @@
 # set your input text
 input_text = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 
 # Send an API request and get a response.
 response = bardapi.core.Bard().get_answer(input_text)
 ```
 
-Resolving errors due to delayed responses in Google Colab, containers, etc.
-- If a response error occurs even though the normal procedure has been followed, use the timeout variable.
+Addressing errors caused by delayed responses in environments like Google Colab and containers. If an error occurs despite following the proper procedure, utilize the timeout argument.
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
 bard = Bard(timeout=10) # Set timeout in seconds
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
+<br>
 
-## Behind a proxy
-
+## Futher
+### Behind a proxy
+If you are working behind a proxy, use the following.
 ```python
 from bardapi import Bard
 import os
 
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
-bard_inproxy = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
-bard_inproxy.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+```
+
+### Reusable session object
+```python
+from bardapi import Bard
+import os
+import requests
+
+os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
+session = requests.Session()
+session.headers = {
+            "Host": "bard.google.com",
+            "X-Same-Domain": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+            "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+            "Origin": "https://bard.google.com",
+            "Referer": "https://bard.google.com/",
+        }
+session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+
+bard = Bard(session=session)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
-Example
+Simple Example
 <br>
 
 <a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
 
 <br>
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-Development Status :: 4 - Beta # Google [https://camo.githubusercontent.com/
+Development Status :: 5 - Production/Stable # Google [https://
+camo.githubusercontent.com/
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
-[PyPI package] [PyPI]   [Code_style:_black] [https://hits.seeyoufarm.com/api/
-count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=bardapi&edge_flat=false]
+[PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
+incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
+[PyPI]
 > A package that returns Response of [Google Bard](https://bard.google.com/
-) through API ![](./assets/bardapi.gif) I referred to [this github repository
+) through API ![](./assets/bard_api.gif) I referred to [this github repository
 (github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference
 process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask
 questions and get answers from Google Bard. This package is designed for
 application to the Python package [ExceptNotifier](https://github.com/
 dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-
 Coder).
 Never expose the `__Secure-1PSID` for your safety. > Note that while I referred
@@ -31,26 +33,36 @@
 bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard
 ().get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ``` Or you can use this ```python import bardapi import
 os # set your __Secure-1PSID value to key os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # set your input text input_text = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤" # Send an API
 request and get a response. response = bardapi.core.Bard().get_answer
-(input_text) ``` Resolving errors due to delayed responses in Google Colab,
-containers, etc. - If a response error occurs even though the normal procedure
-has been followed, use the timeout variable. ```python from bardapi import Bard
-import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) # Set
-timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` ## Behind a proxy ```python
-from bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" #
-Change 'http://127.0.0.1:1080' to your http proxy # timeout in seconds
-bard_inproxy = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://
-127.0.0.1:1080'}, timeout=10) bard_inproxy.get_answer("ëì ë´
+(input_text) ``` Addressing errors caused by delayed responses in environments
+like Google Colab and containers. If an error occurs despite following the
+proper procedure, utilize the timeout argument. ```python from bardapi import
+Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) #
+Set timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+## Futher ### Behind a proxy If you are working behind a proxy, use the
+following. ```python from bardapi import Bard import os os.environ
+['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
+proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
+'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-Example
+### Reusable session object ```python from bardapi import Bard import os import
+requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' session = requests.Session
+() session.headers = { "Host": "bard.google.com", "X-Same-Domain": "1", "User-
+Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like
+Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type": "application/x-www-
+form-urlencoded;charset=UTF-8", "Origin": "https://bard.google.com", "Referer":
+"https://bard.google.com/", } session.cookies.set("__Secure-1PSID", os.environ
+["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
+ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
 -_[MIT](https://opensource.org/license/mit/)_-_I_hold_no_legal_responsibility;
 for_more_information,_please_refer_to_the_bottom_of_the_readme_file._I_just
 want_you_to_give_me_and_[them](https://github.com/acheong08/Bard)_a_star..._##
```

### Comparing `bardapi-0.1.3/bardapi/core.py` & `bardapi-0.1.4/bardapi/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,45 +3,55 @@
 import re
 import string
 import os
 import requests
 
 
 class Bard:
-    def __init__(self, timeout=6, proxies=None):
-        '''
+    def __init__(self, timeout=6, proxies=None, session=None):
+        """
         Initialize Bard
 
         :param timeout: (`int`, *optional*)
             Timeout in seconds when connecting bard server. The timeout is used on each request.
         :param proxies: (`Dict[str, str]`, *optional*)
             A dictionary of proxy servers to use by protocol or endpoint, e.g., `{'http': 'foo.bar:3128',
             'http://hostname': 'foo.bar:4012'}`. The proxies are used on each request.
-        '''
+        :param session: (`requests.Session`, *optional*)
+            An existing requests.Session object to be used for making HTTP requests.
+        """
         self.proxies = proxies
         self.timeout = timeout
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) "
+            "Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
         self._reqid = int("".join(random.choices(string.digits, k=4)))
         self.conversation_id = ""
         self.response_id = ""
         self.choice_id = ""
-        self.session = requests.Session()
-        self.session.headers = headers
-        self.session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+
+        if session is None:
+            self.session = requests.Session()
+            self.session.headers = headers
+            self.session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+        else:
+            self.session = session
+
         self.SNlM0e = self._get_snim0e()
 
     def _get_snim0e(self):
-        resp = self.session.get(url="https://bard.google.com/", timeout=self.timeout, proxies=self.proxies)
+        resp = self.session.get(
+            url="https://bard.google.com/", timeout=self.timeout, proxies=self.proxies
+        )
         if resp.status_code != 200:
             raise Exception(f"Response Status: {resp.status_code}")
         return re.search(r"SNlM0e\":\"(.*?)\"", resp.text).group(1)
 
     def get_answer(self, input_text: str) -> dict:
         params = {
             "bl": "boq_assistant-bard-web-server_20230419.00_p1",
@@ -58,17 +68,16 @@
             "at": self.SNlM0e,
         }
         resp = self.session.post(
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
             timeout=self.timeout,
-            proxies=self.proxies
+            proxies=self.proxies,
         )
-
         resp_dict = json.loads(resp.content.splitlines()[3])[0][2]
         if resp_dict is None:
             return {"content": f"Response Error: {resp.content}."}
         parsed_answer = json.loads(resp_dict)
         bard_answer = {
             "content": parsed_answer[0][0],
             "conversation_id": parsed_answer[1][0],
```

### Comparing `bardapi-0.1.3/bardapi.egg-info/PKG-INFO` & `bardapi-0.1.4/bardapi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
-Keywords: BARD,Python,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
-Classifier: Development Status :: 4 - Beta
+Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
+Classifier: Natural Language :: Korean
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Development Status :: 4 - Beta
+Development Status :: 5 - Production/Stable
 
 
 # Google <a href="https://bard.google.com/"><img src="https://camo.githubusercontent.com/adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667" height="20px"></a> Bard API 
 
 
 <p align="left">
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-BardAPI-black"></a>
-<a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 <!-- <a href="https://pepy.tech/project/bardapi"><img alt="Downloads" src="https://pepy.tech/badge/bardapi"></a> -->
 <!-- <a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/Bard-API?color=black"></a> -->
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=bardapi&edge_flat=false"/></a></a>
+<a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false"/></a>
+<a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 </p>
 
 > A package that returns Response of [Google Bard](https://bard.google.com/) through API
 
-![](./assets/bardapi.gif)
+![](./assets/bard_api.gif)
 
 
 I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
 
 <br>
 
 Never expose the `__Secure-1PSID` for your safety.
@@ -98,40 +101,63 @@
 # set your input text
 input_text = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 
 # Send an API request and get a response.
 response = bardapi.core.Bard().get_answer(input_text)
 ```
 
-Resolving errors due to delayed responses in Google Colab, containers, etc.
-- If a response error occurs even though the normal procedure has been followed, use the timeout variable.
+Addressing errors caused by delayed responses in environments like Google Colab and containers. If an error occurs despite following the proper procedure, utilize the timeout argument.
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
 bard = Bard(timeout=10) # Set timeout in seconds
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
+<br>
 
-## Behind a proxy
-
+## Futher
+### Behind a proxy
+If you are working behind a proxy, use the following.
 ```python
 from bardapi import Bard
 import os
 
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
-bard_inproxy = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
-bard_inproxy.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+```
+
+### Reusable session object
+```python
+from bardapi import Bard
+import os
+import requests
+
+os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
+session = requests.Session()
+session.headers = {
+            "Host": "bard.google.com",
+            "X-Same-Domain": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+            "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+            "Origin": "https://bard.google.com",
+            "Referer": "https://bard.google.com/",
+        }
+session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+
+bard = Bard(session=session)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
-Example
+Simple Example
 <br>
 
 <a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
 
 <br>
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.3 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.4 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
-parkminwoo1991@gmail.com Keywords: BARD,Python,Google Bard,Large Language
-Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
+parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
+Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
+Natural Language :: English Classifier: Natural Language :: Korean Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python ::
+3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 4 - Beta # Google [https://
+LICENSE Development Status :: 5 - Production/Stable # Google [https://
 camo.githubusercontent.com/
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
-[PyPI package] [PyPI]   [Code_style:_black] [https://hits.seeyoufarm.com/api/
-count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=bardapi&edge_flat=false]
+[PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
+incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
+[PyPI]
 > A package that returns Response of [Google Bard](https://bard.google.com/
-) through API ![](./assets/bardapi.gif) I referred to [this github repository
+) through API ![](./assets/bard_api.gif) I referred to [this github repository
 (github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference
 process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask
 questions and get answers from Google Bard. This package is designed for
 application to the Python package [ExceptNotifier](https://github.com/
 dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-
 Coder).
 Never expose the `__Secure-1PSID` for your safety. > Note that while I referred
@@ -44,26 +47,36 @@
 bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard
 ().get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
 ìë ¤ì¤")['content'] ``` Or you can use this ```python import bardapi import
 os # set your __Secure-1PSID value to key os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # set your input text input_text = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤" # Send an API
 request and get a response. response = bardapi.core.Bard().get_answer
-(input_text) ``` Resolving errors due to delayed responses in Google Colab,
-containers, etc. - If a response error occurs even though the normal procedure
-has been followed, use the timeout variable. ```python from bardapi import Bard
-import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) # Set
-timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` ## Behind a proxy ```python
-from bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" #
-Change 'http://127.0.0.1:1080' to your http proxy # timeout in seconds
-bard_inproxy = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://
-127.0.0.1:1080'}, timeout=10) bard_inproxy.get_answer("ëì ë´
+(input_text) ``` Addressing errors caused by delayed responses in environments
+like Google Colab and containers. If an error occurs despite following the
+proper procedure, utilize the timeout argument. ```python from bardapi import
+Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) #
+Set timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+## Futher ### Behind a proxy If you are working behind a proxy, use the
+following. ```python from bardapi import Bard import os os.environ
+['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
+proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
+'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-Example
+### Reusable session object ```python from bardapi import Bard import os import
+requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' session = requests.Session
+() session.headers = { "Host": "bard.google.com", "X-Same-Domain": "1", "User-
+Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like
+Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type": "application/x-www-
+form-urlencoded;charset=UTF-8", "Origin": "https://bard.google.com", "Referer":
+"https://bard.google.com/", } session.cookies.set("__Secure-1PSID", os.environ
+["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
+ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
 -_[MIT](https://opensource.org/license/mit/)_-_I_hold_no_legal_responsibility;
 for_more_information,_please_refer_to_the_bottom_of_the_readme_file._I_just
 want_you_to_give_me_and_[them](https://github.com/acheong08/Bard)_a_star..._##
```

### Comparing `bardapi-0.1.3/setup.py` & `bardapi-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,32 +21,34 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.3",
+    version="0.1.4",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
     install_requires=[],
-    keywords="BARD, Python, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
+    keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
+        "Natural Language :: Korean",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
-    entry_points={"console_scripts": ["bard_api=bard_api.cli:main"]},
 )
```

