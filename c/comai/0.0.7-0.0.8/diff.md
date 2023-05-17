# Comparing `tmp/comai-0.0.7.tar.gz` & `tmp/comai-0.0.8.tar.gz`

## Comparing `comai-0.0.7.tar` & `comai-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.0.7/.github/workflows/release.yml
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 comai-0.0.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.0.7/src/comai/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 comai-0.0.7/src/comai/__main__.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 comai-0.0.7/src/comai/cli.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 comai-0.0.7/src/comai/config.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 comai-0.0.7/tests/test_comai.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 comai-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.0.7/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 comai-0.0.7/README.md
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 comai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    41380 2020-02-02 00:00:00.000000 comai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 comai-0.0.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/__main__.py
+-rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/cli.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 comai-0.0.8/src/comai/config.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 comai-0.0.8/tests/test_comai.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 comai-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 comai-0.0.8/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 comai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    43802 2020-02-02 00:00:00.000000 comai-0.0.8/PKG-INFO
```

### Comparing `comai-0.0.7/.github/workflows/release.yml` & `comai-0.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `comai-0.0.7/.github/workflows/tests.yml` & `comai-0.0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `comai-0.0.7/src/comai/cli.py` & `comai-0.0.8/src/comai/cli.py`

 * *Files identical despite different names*

### Comparing `comai-0.0.7/src/comai/config.py` & `comai-0.0.8/src/comai/config.py`

 * *Files identical despite different names*

### Comparing `comai-0.0.7/tests/test_comai.py` & `comai-0.0.8/tests/test_comai.py`

 * *Files identical despite different names*

### Comparing `comai-0.0.7/LICENSE` & `comai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `comai-0.0.7/pyproject.toml` & `comai-0.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,17 @@
   "appdirs==1.4.4",
   "cryptography==40.0.2",
   "termcolor==2.3.0",
   "getch==1.0",
 ]
 
 [project.urls]
+homepage = "https://github.com/ricopinazo/comai"
 repository = "https://github.com/ricopinazo/comai"
+issues = "https://github.com/ricopinazo/comai/issues"
 
 [project.scripts]
 comai = "comai.cli:main"
 
 [project.optional-dependencies]
 test = [
     "pytest",
```

### Comparing `comai-0.0.7/PKG-INFO` & `comai-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: comai
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI powered console assistant
+Project-URL: homepage, https://github.com/ricopinazo/comai
 Project-URL: repository, https://github.com/ricopinazo/comai
+Project-URL: issues, https://github.com/ricopinazo/comai/issues
 Author-email: Pedro Rico <ricopinazo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -692,8 +694,63 @@
 Requires-Dist: termcolor==2.3.0
 Provides-Extra: test
 Requires-Dist: hatchling; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: python-dotenv; extra == 'test'
 Description-Content-Type: text/markdown
 
-# comai
+# Comai - The AI powered terminal assistant
+
+`comai` is an open source terminal assistant powered by OpenAI API that enables you to interact with your command line interface using natural language instructions. It simplifies your workflow by converting natural language queries into executable commands. No more memorizing complex syntax. Just chat with `comai` using plain English!
+
+## Installation 🚀
+
+Getting `comai` up and running is a breeze. Simply use `pip` to install the latest tested version:
+
+```shell
+pip install comai
+```
+
+The first time you run it, it'll ask you for an OpenAI API key. You can create a developer account [here](https://platform.openai.com/overview). Once in your account, go to `API Keys` section and `Create new secret key`. We recommend setting a usage limit under `Billing`/`Usage limits`.
+
+## Usage Examples 🎉
+
+Using `comai` is straightforward. Simply invoke the `comai` command followed by your natural language instruction. `comai` will provide you with the corresponding executable command, which you can execute by pressing Enter or ignore by pressing any other key.
+
+Let's dive into some exciting examples of how you can harness the power of `comai`:
+
+1. Unleash your creativity with an ASCII art cow:
+```shell
+$ comai print a cow saying Moo!
+💡≫ echo "Moo!" | cowsay
+```
+
+2. Update the main branch and merge it into the current branch:
+```shell
+$ comai update the main branch and merge it into the current
+💡≫ git checkout main; git pull; git checkout -; git merge main
+```
+
+
+3. Check the weather forecast for your location:
+```shell
+$ comai show me the weather forecast
+💡≫ curl wttr.in
+```
+
+3. Find the annoying process using the port 8000:
+```shell
+$ comai show me the process using port 8000
+💡≫ lsof -i :8000
+```
+
+4. Discover your future with a fortune cookie quote:
+```shell
+$ comai give me a fortune cookie quote
+💡≫ fortune cookie
+```
+
+These are just a few examples of how `comai` can help you harness the power of the command line and provide you with useful and entertaining commands. Feel free to explore and experiment with the commands generated by `comai` to discover more exciting possibilities!
+
+## License 📜
+
+Comai is licensed under the GPLv3. You can find the full text of the license in the [LICENSE](./LICENSE) file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

