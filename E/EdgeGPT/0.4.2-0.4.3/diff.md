# Comparing `tmp/EdgeGPT-0.4.2.tar.gz` & `tmp/EdgeGPT-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.4.2.tar", last modified: Tue May 16 05:43:49 2023, max compression
+gzip compressed data, was "EdgeGPT-0.4.3.tar", last modified: Wed May 17 11:46:00 2023, max compression
```

## Comparing `EdgeGPT-0.4.2.tar` & `EdgeGPT-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:43:49.276002 EdgeGPT-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 05:43:18.000000 EdgeGPT-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-16 05:43:49.276002 EdgeGPT-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 05:43:49.276002 EdgeGPT-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-16 05:43:18.000000 EdgeGPT-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:43:49.276002 EdgeGPT-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:43:49.276002 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 05:43:49.000000 EdgeGPT-0.4.2/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38314 2023-05-16 05:43:18.000000 EdgeGPT-0.4.2/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 05:43:18.000000 EdgeGPT-0.4.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.141100 EdgeGPT-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 11:45:29.000000 EdgeGPT-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-17 11:46:00.141100 EdgeGPT-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-17 11:45:59.000000 EdgeGPT-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 11:46:00.145099 EdgeGPT-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-17 11:45:29.000000 EdgeGPT-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.141100 EdgeGPT-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.141100 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-17 11:46:00.000000 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-17 11:46:00.000000 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:46:00.000000 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 11:46:00.000000 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 11:46:00.000000 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 11:46:00.000000 EdgeGPT-0.4.3/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38842 2023-05-17 11:45:29.000000 EdgeGPT-0.4.3/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 11:45:29.000000 EdgeGPT-0.4.3/src/ImageGen.py
```

### Comparing `EdgeGPT-0.4.2/LICENSE` & `EdgeGPT-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.4.2/PKG-INFO` & `EdgeGPT-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.4.2
+Version: 0.4.3
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -77,15 +77,15 @@
 
 >Instead of following steps 5-9 you can also use the following experimental helper function which has been tested on Windows 11 and requires `Selenium` and the latest version of Microsoft Edge:
 >
 >```
 >pip install selenium
 >```
 >```
->from EdgeGPT Cookie
+>from EdgeGPT import Cookie
 >Cookie.fetch_default()
 >```
 >This will automatically create a file called `bing_cookies__default.json` in your current working directory.
 >
 >The double underscore in the name ensures it always gets used first if you have other cookie files e.g. `bing_cookies_pete.json` (see below regarding multiple cookie files).
 >
 >The `bing_` prefix in the name should avoid confusion with any other cookie files you might be using and is also used as a default by the `Cookie` helper class (see later).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.3 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -29,66 +29,66 @@
 hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
 US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
 the extension 8. Click "Export" on the bottom right, then "Export as JSON"
 (This saves your cookies to clipboard) 9. Paste your cookies into a file
 `cookies.json` >Instead of following steps 5-9 you can also use the following
 experimental helper function which has been tested on Windows 11 and requires
 `Selenium` and the latest version of Microsoft Edge: > >``` >pip install
-selenium >``` >``` >from EdgeGPT Cookie >Cookie.fetch_default() >``` >This will
-automatically create a file called `bing_cookies__default.json` in your current
-working directory. > >The double underscore in the name ensures it always gets
-used first if you have other cookie files e.g. `bing_cookies_pete.json` (see
-below regarding multiple cookie files). > >The `bing_` prefix in the name
-should avoid confusion with any other cookie files you might be using and is
-also used as a default by the `Cookie` helper class (see later). > >    #
-Chatbot  ## Running from the Command Line ``` $ python3 -m EdgeGPT -h EdgeGPT -
-A demo of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/
-EdgeGPT By: Antonio Cheong !help for help Type !exit to exit Enter twice to
-send message or set --enter-once to send one line message usage: EdgeGPT.py [-
-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
-[--style {creative,balanced,precise}] [--cookie-file COOKIE_FILE] options: -h,
---help show this help message and exit --enter-once --no-stream --rich --proxy
-PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g.
-wss://sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --
-cookie-file COOKIE_FILE needed if environment variable COOKIE_FILE is not set
-``` ## Running in Python ### 1) The `Chatbot` class and `asyncio` for more
-granular control There are three main ways to pass in cookies: - Environment
-variable: `export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
-`cookies.json` in the argument `cookie_path` like this: ```python bot = await
-Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
-by the argument `cookies`, like this: ```python with open('./cookies.json',
-'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
-``` Use Async for the best experience, for example: ```python import asyncio
-from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
-Chatbot.create() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
-classes  Create a simple Bing Chat AI query (using the 'precise' conversation
-style by default) and see just the main text output rather than the whole API
-response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
-Give your answer as Python code") print(q) ``` Or change the conversation style
-or cookie file to be used: ```python q = Query( "What are you? Give your answer
-as Python code", style="creative", # or 'balanced' cookies="./
-bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
-snippets, list of sources/references, or suggested follow-on questions using
-the following attributes: ```python q.output q.code q.suggestions q.sources #
-for the full json output q.sources_dict # for a dictionary of titles and urls
-``` Get the orginal prompt and the conversation style you specified: ```python
-q.prompt q.style repr(q) ``` Access previous Queries made since importing
-`Query`: ```python Query.index # A list of Query objects; updated dynamically
-Query.request_count # A tally of requests made using each cookie file ``` And
-finally, the `Cookie` class supports multiple cookie files, so if you create
-additional cookie files with the naming convention `bing_cookies_*.json`, your
-queries will automatically try using the next file (alphabetically) if you've
-exceeded your daily quota of requests (currently set at 200). Here are the main
-attributes which you can access: ```python Cookie.current_file_index
-Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
-Cookie.files() # list as files that match .search_pattern
-Cookie.current_filepath Cookie.current_data Cookie.import_next()
-Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+selenium >``` >``` >from EdgeGPT import Cookie >Cookie.fetch_default() >```
+>This will automatically create a file called `bing_cookies__default.json` in
+your current working directory. > >The double underscore in the name ensures it
+always gets used first if you have other cookie files e.g.
+`bing_cookies_pete.json` (see below regarding multiple cookie files). > >The
+`bing_` prefix in the name should avoid confusion with any other cookie files
+you might be using and is also used as a default by the `Cookie` helper class
+(see later). > >    # Chatbot  ## Running from the Command Line ``` $ python3 -
+m EdgeGPT -h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
+github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
+exit Enter twice to send message or set --enter-once to send one line message
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
+-wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
+COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
+-no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
+link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
+{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
+variable COOKIE_FILE is not set ``` ## Running in Python ### 1) The `Chatbot`
+class and `asyncio` for more granular control There are three main ways to pass
+in cookies: - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
+- Specify the path to `cookies.json` in the argument `cookie_path` like this:
+```python bot = await Chatbot.create(cookie_path='./cookies.json') ``` - Pass
+in the cookies directly by the argument `cookies`, like this: ```python with
+open('./cookies.json', 'r') as f: cookies = json.load(f) bot = await
+Chatbot.create(cookies=cookies) ``` Use Async for the best experience, for
+example: ```python import asyncio from EdgeGPT import Chatbot,
+ConversationStyle async def main(): bot = await Chatbot.create() print(await
+bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
+await bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2)
+The `Query` and `Cookie` helper classes  Create a simple Bing Chat AI query
+(using the 'precise' conversation style by default) and see just the main text
+output rather than the whole API response: ```python from EdgeGPT import Query,
+Cookie q = Query("What are you? Give your answer as Python code") print(q) ```
+Or change the conversation style or cookie file to be used: ```python q = Query
+( "What are you? Give your answer as Python code", style="creative", # or
+'balanced' cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the
+text output, code snippets, list of sources/references, or suggested follow-on
+questions using the following attributes: ```python q.output q.code
+q.suggestions q.sources # for the full json output q.sources_dict # for a
+dictionary of titles and urls ``` Get the orginal prompt and the conversation
+style you specified: ```python q.prompt q.style repr(q) ``` Access previous
+Queries made since importing `Query`: ```python Query.index # A list of Query
+objects; updated dynamically Query.request_count # A tally of requests made
+using each cookie file ``` And finally, the `Cookie` class supports multiple
+cookie files, so if you create additional cookie files with the naming
+convention `bing_cookies_*.json`, your queries will automatically try using the
+next file (alphabetically) if you've exceeded your daily quota of requests
+(currently set at 200). Here are the main attributes which you can access:
+```python Cookie.current_file_index Cookie.dirpath Cookie.search_pattern #
+default is `bing_cookies_*.json` Cookie.files() # list as files that match
+.search_pattern Cookie.current_filepath Cookie.current_data Cookie.import_next
+() Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
 assumes you have a file cookies.json in your current working directory ``` bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
 following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
 -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style
 creative ```    # Image generator  ## Running from the Command Line ```bash $
 python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
```

### Comparing `EdgeGPT-0.4.2/README.md` & `EdgeGPT-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 >Instead of following steps 5-9 you can also use the following experimental helper function which has been tested on Windows 11 and requires `Selenium` and the latest version of Microsoft Edge:
 >
 >```
 >pip install selenium
 >```
 >```
->from EdgeGPT Cookie
+>from EdgeGPT import Cookie
 >Cookie.fetch_default()
 >```
 >This will automatically create a file called `bing_cookies__default.json` in your current working directory.
 >
 >The double underscore in the name ensures it always gets used first if you have other cookie files e.g. `bing_cookies_pete.json` (see below regarding multiple cookie files).
 >
 >The `bing_` prefix in the name should avoid confusion with any other cookie files you might be using and is also used as a default by the `Cookie` helper class (see later).
```

#### html2text {}

```diff
@@ -19,66 +19,66 @@
 hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
 US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
 the extension 8. Click "Export" on the bottom right, then "Export as JSON"
 (This saves your cookies to clipboard) 9. Paste your cookies into a file
 `cookies.json` >Instead of following steps 5-9 you can also use the following
 experimental helper function which has been tested on Windows 11 and requires
 `Selenium` and the latest version of Microsoft Edge: > >``` >pip install
-selenium >``` >``` >from EdgeGPT Cookie >Cookie.fetch_default() >``` >This will
-automatically create a file called `bing_cookies__default.json` in your current
-working directory. > >The double underscore in the name ensures it always gets
-used first if you have other cookie files e.g. `bing_cookies_pete.json` (see
-below regarding multiple cookie files). > >The `bing_` prefix in the name
-should avoid confusion with any other cookie files you might be using and is
-also used as a default by the `Cookie` helper class (see later). > >    #
-Chatbot  ## Running from the Command Line ``` $ python3 -m EdgeGPT -h EdgeGPT -
-A demo of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/
-EdgeGPT By: Antonio Cheong !help for help Type !exit to exit Enter twice to
-send message or set --enter-once to send one line message usage: EdgeGPT.py [-
-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
-[--style {creative,balanced,precise}] [--cookie-file COOKIE_FILE] options: -h,
---help show this help message and exit --enter-once --no-stream --rich --proxy
-PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g.
-wss://sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --
-cookie-file COOKIE_FILE needed if environment variable COOKIE_FILE is not set
-``` ## Running in Python ### 1) The `Chatbot` class and `asyncio` for more
-granular control There are three main ways to pass in cookies: - Environment
-variable: `export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
-`cookies.json` in the argument `cookie_path` like this: ```python bot = await
-Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
-by the argument `cookies`, like this: ```python with open('./cookies.json',
-'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
-``` Use Async for the best experience, for example: ```python import asyncio
-from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
-Chatbot.create() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
-classes  Create a simple Bing Chat AI query (using the 'precise' conversation
-style by default) and see just the main text output rather than the whole API
-response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
-Give your answer as Python code") print(q) ``` Or change the conversation style
-or cookie file to be used: ```python q = Query( "What are you? Give your answer
-as Python code", style="creative", # or 'balanced' cookies="./
-bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
-snippets, list of sources/references, or suggested follow-on questions using
-the following attributes: ```python q.output q.code q.suggestions q.sources #
-for the full json output q.sources_dict # for a dictionary of titles and urls
-``` Get the orginal prompt and the conversation style you specified: ```python
-q.prompt q.style repr(q) ``` Access previous Queries made since importing
-`Query`: ```python Query.index # A list of Query objects; updated dynamically
-Query.request_count # A tally of requests made using each cookie file ``` And
-finally, the `Cookie` class supports multiple cookie files, so if you create
-additional cookie files with the naming convention `bing_cookies_*.json`, your
-queries will automatically try using the next file (alphabetically) if you've
-exceeded your daily quota of requests (currently set at 200). Here are the main
-attributes which you can access: ```python Cookie.current_file_index
-Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
-Cookie.files() # list as files that match .search_pattern
-Cookie.current_filepath Cookie.current_data Cookie.import_next()
-Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+selenium >``` >``` >from EdgeGPT import Cookie >Cookie.fetch_default() >```
+>This will automatically create a file called `bing_cookies__default.json` in
+your current working directory. > >The double underscore in the name ensures it
+always gets used first if you have other cookie files e.g.
+`bing_cookies_pete.json` (see below regarding multiple cookie files). > >The
+`bing_` prefix in the name should avoid confusion with any other cookie files
+you might be using and is also used as a default by the `Cookie` helper class
+(see later). > >    # Chatbot  ## Running from the Command Line ``` $ python3 -
+m EdgeGPT -h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
+github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
+exit Enter twice to send message or set --enter-once to send one line message
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
+-wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
+COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
+-no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
+link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
+{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
+variable COOKIE_FILE is not set ``` ## Running in Python ### 1) The `Chatbot`
+class and `asyncio` for more granular control There are three main ways to pass
+in cookies: - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
+- Specify the path to `cookies.json` in the argument `cookie_path` like this:
+```python bot = await Chatbot.create(cookie_path='./cookies.json') ``` - Pass
+in the cookies directly by the argument `cookies`, like this: ```python with
+open('./cookies.json', 'r') as f: cookies = json.load(f) bot = await
+Chatbot.create(cookies=cookies) ``` Use Async for the best experience, for
+example: ```python import asyncio from EdgeGPT import Chatbot,
+ConversationStyle async def main(): bot = await Chatbot.create() print(await
+bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
+await bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2)
+The `Query` and `Cookie` helper classes  Create a simple Bing Chat AI query
+(using the 'precise' conversation style by default) and see just the main text
+output rather than the whole API response: ```python from EdgeGPT import Query,
+Cookie q = Query("What are you? Give your answer as Python code") print(q) ```
+Or change the conversation style or cookie file to be used: ```python q = Query
+( "What are you? Give your answer as Python code", style="creative", # or
+'balanced' cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the
+text output, code snippets, list of sources/references, or suggested follow-on
+questions using the following attributes: ```python q.output q.code
+q.suggestions q.sources # for the full json output q.sources_dict # for a
+dictionary of titles and urls ``` Get the orginal prompt and the conversation
+style you specified: ```python q.prompt q.style repr(q) ``` Access previous
+Queries made since importing `Query`: ```python Query.index # A list of Query
+objects; updated dynamically Query.request_count # A tally of requests made
+using each cookie file ``` And finally, the `Cookie` class supports multiple
+cookie files, so if you create additional cookie files with the naming
+convention `bing_cookies_*.json`, your queries will automatically try using the
+next file (alphabetically) if you've exceeded your daily quota of requests
+(currently set at 200). Here are the main attributes which you can access:
+```python Cookie.current_file_index Cookie.dirpath Cookie.search_pattern #
+default is `bing_cookies_*.json` Cookie.files() # list as files that match
+.search_pattern Cookie.current_filepath Cookie.current_data Cookie.import_next
+() Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
 assumes you have a file cookies.json in your current working directory ``` bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
 following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
 -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style
 creative ```    # Image generator  ## Running from the Command Line ```bash $
 python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
```

### Comparing `EdgeGPT-0.4.2/setup.py` & `EdgeGPT-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.4.2",
+    version="0.4.3",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.4.2/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.4.3/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.4.2
+Version: 0.4.3
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -77,15 +77,15 @@
 
 >Instead of following steps 5-9 you can also use the following experimental helper function which has been tested on Windows 11 and requires `Selenium` and the latest version of Microsoft Edge:
 >
 >```
 >pip install selenium
 >```
 >```
->from EdgeGPT Cookie
+>from EdgeGPT import Cookie
 >Cookie.fetch_default()
 >```
 >This will automatically create a file called `bing_cookies__default.json` in your current working directory.
 >
 >The double underscore in the name ensures it always gets used first if you have other cookie files e.g. `bing_cookies_pete.json` (see below regarding multiple cookie files).
 >
 >The `bing_` prefix in the name should avoid confusion with any other cookie files you might be using and is also used as a default by the `Cookie` helper class (see later).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.3 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -29,66 +29,66 @@
 hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
 US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
 the extension 8. Click "Export" on the bottom right, then "Export as JSON"
 (This saves your cookies to clipboard) 9. Paste your cookies into a file
 `cookies.json` >Instead of following steps 5-9 you can also use the following
 experimental helper function which has been tested on Windows 11 and requires
 `Selenium` and the latest version of Microsoft Edge: > >``` >pip install
-selenium >``` >``` >from EdgeGPT Cookie >Cookie.fetch_default() >``` >This will
-automatically create a file called `bing_cookies__default.json` in your current
-working directory. > >The double underscore in the name ensures it always gets
-used first if you have other cookie files e.g. `bing_cookies_pete.json` (see
-below regarding multiple cookie files). > >The `bing_` prefix in the name
-should avoid confusion with any other cookie files you might be using and is
-also used as a default by the `Cookie` helper class (see later). > >    #
-Chatbot  ## Running from the Command Line ``` $ python3 -m EdgeGPT -h EdgeGPT -
-A demo of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/
-EdgeGPT By: Antonio Cheong !help for help Type !exit to exit Enter twice to
-send message or set --enter-once to send one line message usage: EdgeGPT.py [-
-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
-[--style {creative,balanced,precise}] [--cookie-file COOKIE_FILE] options: -h,
---help show this help message and exit --enter-once --no-stream --rich --proxy
-PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g.
-wss://sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --
-cookie-file COOKIE_FILE needed if environment variable COOKIE_FILE is not set
-``` ## Running in Python ### 1) The `Chatbot` class and `asyncio` for more
-granular control There are three main ways to pass in cookies: - Environment
-variable: `export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
-`cookies.json` in the argument `cookie_path` like this: ```python bot = await
-Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
-by the argument `cookies`, like this: ```python with open('./cookies.json',
-'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
-``` Use Async for the best experience, for example: ```python import asyncio
-from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
-Chatbot.create() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
-classes  Create a simple Bing Chat AI query (using the 'precise' conversation
-style by default) and see just the main text output rather than the whole API
-response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
-Give your answer as Python code") print(q) ``` Or change the conversation style
-or cookie file to be used: ```python q = Query( "What are you? Give your answer
-as Python code", style="creative", # or 'balanced' cookies="./
-bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
-snippets, list of sources/references, or suggested follow-on questions using
-the following attributes: ```python q.output q.code q.suggestions q.sources #
-for the full json output q.sources_dict # for a dictionary of titles and urls
-``` Get the orginal prompt and the conversation style you specified: ```python
-q.prompt q.style repr(q) ``` Access previous Queries made since importing
-`Query`: ```python Query.index # A list of Query objects; updated dynamically
-Query.request_count # A tally of requests made using each cookie file ``` And
-finally, the `Cookie` class supports multiple cookie files, so if you create
-additional cookie files with the naming convention `bing_cookies_*.json`, your
-queries will automatically try using the next file (alphabetically) if you've
-exceeded your daily quota of requests (currently set at 200). Here are the main
-attributes which you can access: ```python Cookie.current_file_index
-Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
-Cookie.files() # list as files that match .search_pattern
-Cookie.current_filepath Cookie.current_data Cookie.import_next()
-Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+selenium >``` >``` >from EdgeGPT import Cookie >Cookie.fetch_default() >```
+>This will automatically create a file called `bing_cookies__default.json` in
+your current working directory. > >The double underscore in the name ensures it
+always gets used first if you have other cookie files e.g.
+`bing_cookies_pete.json` (see below regarding multiple cookie files). > >The
+`bing_` prefix in the name should avoid confusion with any other cookie files
+you might be using and is also used as a default by the `Cookie` helper class
+(see later). > >    # Chatbot  ## Running from the Command Line ``` $ python3 -
+m EdgeGPT -h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
+github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
+exit Enter twice to send message or set --enter-once to send one line message
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
+-wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
+COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
+-no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
+link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
+{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
+variable COOKIE_FILE is not set ``` ## Running in Python ### 1) The `Chatbot`
+class and `asyncio` for more granular control There are three main ways to pass
+in cookies: - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
+- Specify the path to `cookies.json` in the argument `cookie_path` like this:
+```python bot = await Chatbot.create(cookie_path='./cookies.json') ``` - Pass
+in the cookies directly by the argument `cookies`, like this: ```python with
+open('./cookies.json', 'r') as f: cookies = json.load(f) bot = await
+Chatbot.create(cookies=cookies) ``` Use Async for the best experience, for
+example: ```python import asyncio from EdgeGPT import Chatbot,
+ConversationStyle async def main(): bot = await Chatbot.create() print(await
+bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
+await bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2)
+The `Query` and `Cookie` helper classes  Create a simple Bing Chat AI query
+(using the 'precise' conversation style by default) and see just the main text
+output rather than the whole API response: ```python from EdgeGPT import Query,
+Cookie q = Query("What are you? Give your answer as Python code") print(q) ```
+Or change the conversation style or cookie file to be used: ```python q = Query
+( "What are you? Give your answer as Python code", style="creative", # or
+'balanced' cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the
+text output, code snippets, list of sources/references, or suggested follow-on
+questions using the following attributes: ```python q.output q.code
+q.suggestions q.sources # for the full json output q.sources_dict # for a
+dictionary of titles and urls ``` Get the orginal prompt and the conversation
+style you specified: ```python q.prompt q.style repr(q) ``` Access previous
+Queries made since importing `Query`: ```python Query.index # A list of Query
+objects; updated dynamically Query.request_count # A tally of requests made
+using each cookie file ``` And finally, the `Cookie` class supports multiple
+cookie files, so if you create additional cookie files with the naming
+convention `bing_cookies_*.json`, your queries will automatically try using the
+next file (alphabetically) if you've exceeded your daily quota of requests
+(currently set at 200). Here are the main attributes which you can access:
+```python Cookie.current_file_index Cookie.dirpath Cookie.search_pattern #
+default is `bing_cookies_*.json` Cookie.files() # list as files that match
+.search_pattern Cookie.current_filepath Cookie.current_data Cookie.import_next
+() Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
 assumes you have a file cookies.json in your current working directory ``` bash
 docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
 cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
 following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
 -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style
 creative ```    # Image generator  ## Running from the Command Line ```bash $
 python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
```

### Comparing `EdgeGPT-0.4.2/src/EdgeGPT.py` & `EdgeGPT-0.4.3/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from enum import Enum
 from pathlib import Path
 from typing import Generator
 from typing import Literal
 from typing import Optional
 from typing import Union
 
+import aiohttp
 import certifi
 import httpx
-import websockets.client as websockets
 from BingImageCreator import ImageGen, ImageGenAsync
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.live import Live
@@ -403,24 +403,26 @@
 
 
 class _ChatHub:
     """
     Chat API
     """
 
-    def __init__(self, conversation: _Conversation) -> None:
-        self.wss: websockets.WebSocketClientProtocol | None = None
+    def __init__(self, conversation: _Conversation, proxy: str = None) -> None:
+        self.session: aiohttp.ClientSession | None = None
+        self.wss: aiohttp.ClientWebSocketResponse | None = None
         self.request: _ChatHubRequest
         self.loop: bool
         self.task: asyncio.Task
         self.request = _ChatHubRequest(
             conversation_signature=conversation.struct["conversationSignature"],
             client_id=conversation.struct["clientId"],
             conversation_id=conversation.struct["conversationId"],
         )
+        self.proxy: str = proxy
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str,
         cookies: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
@@ -428,22 +430,25 @@
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
+        timeout = aiohttp.ClientTimeout(total=30)
+        self.session = aiohttp.ClientSession(timeout=timeout)
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
-        self.wss = await websockets.connect(
+        self.wss = await self.session.ws_connect(
             wss_link,
-            extra_headers=HEADERS,
-            max_size=None,
+            headers=HEADERS,
             ssl=ssl_context,
+            proxy=self.proxy,
+            ping_interval=None,
         )
         await self._initial_handshake()
         if self.request.invocation_id == 0:
             # Construct a ChatHub request
             self.request.update(
                 prompt=prompt,
                 conversation_style=conversation_style,
@@ -479,22 +484,23 @@
             # Construct a ChatHub request
             self.request.update(
                 prompt=prompt,
                 conversation_style=conversation_style,
                 options=options,
             )
         # Send request
-        await self.wss.send(_append_identifier(self.request.struct))
+        await self.wss.send_str(_append_identifier(self.request.struct))
         final = False
         draw = False
         resp_txt = ""
         result_text = ""
         resp_txt_no_link = ""
         while not final:
-            objects = str(await self.wss.recv()).split(DELIMITER)
+            msg = await self.wss.receive()
+            objects = msg.data.split(DELIMITER)
             for obj in objects:
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
@@ -542,14 +548,15 @@
                                     ][0]["body"][0]["inlines"][0].get("text")
                                     + "\n"
                                 )
                         yield False, resp_txt
 
                 elif response.get("type") == 2:
                     if response["item"]["result"].get("error"):
+                        await self.close()
                         raise Exception(
                             f"{response['item']['result']['value']}: {response['item']['result']['message']}",
                         )
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
@@ -565,26 +572,29 @@
                             "text"
                         ] = resp_txt
                         print(
                             "Preserved the message from being deleted",
                             file=sys.stderr,
                         )
                     final = True
+                    await self.close()
                     yield True, response
 
     async def _initial_handshake(self) -> None:
-        await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
-        await self.wss.recv()
+        await self.wss.send_str(_append_identifier({"protocol": "json", "version": 1}))
+        await self.wss.receive()
 
     async def close(self) -> None:
         """
         Close the connection
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
+        if self.session and not self.session.closed:
+            await self.session.close()
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
 
@@ -603,14 +613,15 @@
             except FileNotFoundError as exc:
                 raise FileNotFoundError("Cookie file not found") from exc
         else:
             self.cookies = cookies
         self.proxy: str | None = proxy
         self.chat_hub: _ChatHub = _ChatHub(
             _Conversation(self.cookies, self.proxy),
+            proxy=self.proxy,
         )
 
     @staticmethod
     async def create(
         cookies: dict = None,
         proxy: str | None = None,
         cookie_path: str = None,
@@ -625,14 +636,15 @@
             except FileNotFoundError as exc:
                 raise FileNotFoundError("Cookie file not found") from exc
         else:
             self.cookies = cookies
         self.proxy = proxy
         self.chat_hub = _ChatHub(
             await _Conversation.create(self.cookies, self.proxy),
+            proxy=self.proxy,
         )
         return self
 
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
@@ -692,14 +704,15 @@
     async def reset(self) -> None:
         """
         Reset the conversation
         """
         await self.close()
         self.chat_hub = _ChatHub(
             await _Conversation.create(self.cookies, self.proxy),
+            proxy=self.proxy,
         )
 
 
 async def _get_input_async(
     session: PromptSession = None,
     completer: WordCompleter = None,
 ) -> str:
```

