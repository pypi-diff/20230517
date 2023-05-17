# Comparing `tmp/uberduck-0.0.4.tar.gz` & `tmp/uberduck-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uberduck-0.0.4.tar", last modified: Thu Apr 20 09:27:30 2023, max compression
+gzip compressed data, was "uberduck-0.0.5.tar", last modified: Wed May 17 09:00:08 2023, max compression
```

## Comparing `uberduck-0.0.4.tar` & `uberduck-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 09:27:30.526666 uberduck-0.0.4/
--rw-rw-rw-   0        0        0     1056 2022-03-09 10:12:26.000000 uberduck-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5846 2023-04-20 09:27:30.525667 uberduck-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3455 2023-04-20 09:20:50.000000 uberduck-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 09:27:30.526666 uberduck-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2839 2022-12-25 04:32:37.000000 uberduck-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 09:27:30.462836 uberduck-0.0.4/uberduck/
--rw-rw-rw-   0        0        0     1781 2023-04-17 12:29:41.000000 uberduck-0.0.4/uberduck/__init__.py
--rw-rw-rw-   0        0        0     9038 2023-04-20 09:16:22.000000 uberduck-0.0.4/uberduck/classes.py
--rw-rw-rw-   0        0        0    13171 2022-03-10 05:52:01.000000 uberduck-0.0.4/uberduck/main.py
-drwxrwxrwx   0        0        0        0 2023-04-20 09:27:30.521710 uberduck-0.0.4/uberduck.egg-info/
--rw-rw-rw-   0        0        0     5846 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 09:27:29.000000 uberduck-0.0.4/uberduck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 09:00:08.478553 uberduck-0.0.5/
+-rw-rw-rw-   0        0        0     1056 2022-03-09 10:12:26.000000 uberduck-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5846 2023-05-17 09:00:08.476559 uberduck-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2023-04-20 09:20:50.000000 uberduck-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 09:00:08.478553 uberduck-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2988 2023-05-17 08:56:04.000000 uberduck-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:00:08.425696 uberduck-0.0.5/uberduck/
+-rw-rw-rw-   0        0        0     1781 2023-05-17 08:57:41.000000 uberduck-0.0.5/uberduck/__init__.py
+-rw-rw-rw-   0        0        0     9038 2023-04-20 09:16:22.000000 uberduck-0.0.5/uberduck/classes.py
+-rw-rw-rw-   0        0        0    13260 2023-05-17 08:57:19.000000 uberduck-0.0.5/uberduck/main.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:00:08.472568 uberduck-0.0.5/uberduck.egg-info/
+-rw-rw-rw-   0        0        0     5846 2023-05-17 09:00:07.000000 uberduck-0.0.5/uberduck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-17 09:00:07.000000 uberduck-0.0.5/uberduck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:00:07.000000 uberduck-0.0.5/uberduck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-17 09:00:07.000000 uberduck-0.0.5/uberduck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 09:00:07.000000 uberduck-0.0.5/uberduck.egg-info/top_level.txt
```

### Comparing `uberduck-0.0.4/LICENSE` & `uberduck-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uberduck-0.0.4/PKG-INFO` & `uberduck-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uberduck
-Version: 0.0.4
+Version: 0.0.5
 Summary: A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.
 Home-page: https://github.com/ImNimboss/uberduck
 Author: ImNimboss
 Author-email: nimit.grover24@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ImNimboss/uberduck/tree/main/Documentation
 Project-URL: Issue Tracker, https://github.com/ImNimboss/uberduck/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uberduck Version: 0.0.4 Summary: A synchronous and
+Metadata-Version: 2.1 Name: uberduck Version: 0.0.5 Summary: A synchronous and
 asynchronous API wrapper for the UberDuck text-to-speech service (https://
 uberduck.ai) with 100% coverage and top-notch utilities. Home-page: https://
 github.com/ImNimboss/uberduck Author: ImNimboss Author-email:
 nimit.grover24@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/ImNimboss/uberduck/tree/main/Documentation Project-URL: Issue
 Tracker, https://github.com/ImNimboss/uberduck/issues Project-URL: Source,
 https://github.com/ImNimboss/uberduck Project-URL: Funding, https://
```

### Comparing `uberduck-0.0.4/README.md` & `uberduck-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `uberduck-0.0.4/setup.py` & `uberduck-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from setuptools import setup
+from sys import version_info
 
 with open('README.md') as file:
     long_description = file.read()
 
 with open('uberduck/__init__.py') as file:
     lines = file.readlines()
 
 for line in lines:
     if line.startswith('__version__: str = '):
         version = line[20:-2]
         break
 
+dependencies = [
+    'requests', 'aiohttp', 'polling', 'pydub', 'simpleaudio'
+]
+if version_info < (3,8):
+    dependencies.append('typing_extensions')
+
 setup(
     name = 'uberduck',
     version = version,
     description = 'A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author = 'ImNimboss',
@@ -22,15 +29,15 @@
     url = 'https://github.com/ImNimboss/uberduck',
     license = 'MIT',
     packages = ['uberduck'],
     keywords = [
         'uberduck', 'wrapper', 'api', 'text-to-speech', 'async', 'famous',
         'tts', 'texttospeech', 'AI', 'api-wrapper', 'api-key', 'api-secret'
     ],
-    install_requires = ['requests', 'aiohttp', 'polling', 'pydub'],
+    install_requires = dependencies,
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

### Comparing `uberduck-0.0.4/uberduck/__init__.py` & `uberduck-0.0.5/uberduck/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 from uberduck.main import UberDuck, get_voices, get_voices_async
 from uberduck.classes import *
 import logging as _logging
 
 __author__: str = 'ImNimboss'
 __license__: str = 'MIT'
-__version__: str = '0.0.4'
+__version__: str = '0.0.5'
 GITHUB: str = 'https://github.com/ImNimboss/uberduck'
 ISSUE_TRACKER: str = 'https://github.com/ImNimboss/uberduck/issues'
 DOCUMENTATION: str = 'https://github.com/ImNimboss/uberduck/tree/main/Documentation'
 SPONSOR: str = 'https://patreon.com/ImNimboss'
 API_CREDITS: str = 'https://uberduck.ai'
 
 _logging.getLogger(__name__).addHandler(_logging.NullHandler())
```

### Comparing `uberduck-0.0.4/uberduck/classes.py` & `uberduck-0.0.5/uberduck/classes.py`

 * *Files identical despite different names*

### Comparing `uberduck-0.0.4/uberduck/main.py` & `uberduck-0.0.5/uberduck/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 from requests import post, get
 from aiohttp import request, BasicAuth
 from asyncio import get_event_loop, AbstractEventLoop
-from typing import Union, Literal, Optional, List
+from typing import Union, Optional, List
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 from uberduck.classes import *
 from polling import poll
 from pydub import AudioSegment
 from pydub.playback import play
 from io import BytesIO
 from logging import getLogger
```

### Comparing `uberduck-0.0.4/uberduck.egg-info/PKG-INFO` & `uberduck-0.0.5/uberduck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uberduck
-Version: 0.0.4
+Version: 0.0.5
 Summary: A synchronous and asynchronous API wrapper for the UberDuck text-to-speech service (https://uberduck.ai) with 100% coverage and top-notch utilities.
 Home-page: https://github.com/ImNimboss/uberduck
 Author: ImNimboss
 Author-email: nimit.grover24@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ImNimboss/uberduck/tree/main/Documentation
 Project-URL: Issue Tracker, https://github.com/ImNimboss/uberduck/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uberduck Version: 0.0.4 Summary: A synchronous and
+Metadata-Version: 2.1 Name: uberduck Version: 0.0.5 Summary: A synchronous and
 asynchronous API wrapper for the UberDuck text-to-speech service (https://
 uberduck.ai) with 100% coverage and top-notch utilities. Home-page: https://
 github.com/ImNimboss/uberduck Author: ImNimboss Author-email:
 nimit.grover24@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/ImNimboss/uberduck/tree/main/Documentation Project-URL: Issue
 Tracker, https://github.com/ImNimboss/uberduck/issues Project-URL: Source,
 https://github.com/ImNimboss/uberduck Project-URL: Funding, https://
```

