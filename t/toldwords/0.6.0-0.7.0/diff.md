# Comparing `tmp/toldwords-0.6.0.tar.gz` & `tmp/toldwords-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toldwords-0.6.0.tar", max compression
+gzip compressed data, was "toldwords-0.7.0.tar", max compression
```

## Comparing `toldwords-0.6.0.tar` & `toldwords-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1132 2023-04-05 12:14:24.274774 toldwords-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0       72 2023-04-05 11:36:21.908246 toldwords-0.6.0/README.md
--rw-r--r--   0        0        0     1999 2023-05-05 09:58:10.852661 toldwords-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      521 2023-05-05 09:58:16.732875 toldwords-0.6.0/toldwords/__init__.py
--rw-r--r--   0        0        0     1788 2023-04-06 08:36:19.873813 toldwords-0.6.0/toldwords/openai.py
--rw-r--r--   0        0        0     5100 2023-05-05 09:57:30.479346 toldwords-0.6.0/toldwords/pretalx.py
--rw-r--r--   0        0        0        0 2023-04-19 02:44:37.772682 toldwords-0.6.0/toldwords/py.typed
--rw-r--r--   0        0        0      166 2023-05-04 06:45:27.125645 toldwords-0.6.0/toldwords/utils.py
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 toldwords-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-04-05 12:14:24.274774 toldwords-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0       72 2023-04-05 11:36:21.908246 toldwords-0.7.0/README.md
+-rw-r--r--   0        0        0     1990 2023-05-17 02:46:11.152718 toldwords-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      521 2023-05-17 02:43:19.968588 toldwords-0.7.0/toldwords/__init__.py
+-rw-r--r--   0        0        0     1788 2023-04-06 08:36:19.873813 toldwords-0.7.0/toldwords/openai.py
+-rw-r--r--   0        0        0     5357 2023-05-17 02:44:00.138741 toldwords-0.7.0/toldwords/pretalx.py
+-rw-r--r--   0        0        0        0 2023-04-19 02:44:37.772682 toldwords-0.7.0/toldwords/py.typed
+-rw-r--r--   0        0        0      166 2023-05-04 06:45:27.125645 toldwords-0.7.0/toldwords/utils.py
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 toldwords-0.7.0/PKG-INFO
```

### Comparing `toldwords-0.6.0/LICENSE.txt` & `toldwords-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toldwords-0.6.0/pyproject.toml` & `toldwords-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toldwords"
-version = "0.6.0"
+version = "0.7.0"
 description = "Using ChatGPT to make keywords for the papers from COSCUP."
 authors = ["Toomore Chiang <toomore0929@gmail.com>"]
 license = 'MIT'
 readme = "README.md"
 homepage = 'https://github.com/toomore/toldwords'
 repository = 'https://github.com/toomore/toldwords'
 packages = [
@@ -23,15 +23,15 @@
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
-certifi = "^2022.12.7"
+certifi = "*"
 pydantic = "^1.10.6"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 pylint = "^2.17.0"
 autopep8 = "^2.0.2"
 types-requests = "^2.28.11.15"
```

### Comparing `toldwords-0.6.0/toldwords/__init__.py` & `toldwords-0.7.0/toldwords/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ''' __init__ '''
-__version__ = '0.6.0'
+__version__ = '0.7.0'
 from .openai import (Choice, Message, OpenAIAPI, RespCompletions, Role,
                      TokenUsage)
 from .pretalx import Pretalx, PretalxResponse, Room, Speaker, Submission, Talk
 from .utils import DATA2022, DATA2023
 
 __all__ = [
     "__version__",
```

### Comparing `toldwords-0.6.0/toldwords/openai.py` & `toldwords-0.7.0/toldwords/openai.py`

 * *Files identical despite different names*

### Comparing `toldwords-0.6.0/toldwords/pretalx.py` & `toldwords-0.7.0/toldwords/pretalx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ''' Fetch data from pretalx '''
 from typing import List, Generator, Any
 from requests import Session
-from pydantic import BaseModel, Field, parse_obj_as
+from pydantic import BaseModel, Field, parse_obj_as, validator
 
 
 class Talk(BaseModel):
     ''' Talk '''
     code: str = Field(default_factory=str,
                       description='A unique, alphanumeric identifier, also used in URLs')
     title: str = Field(default_factory=str,
@@ -27,14 +27,15 @@
     submissions: list[str] | None = Field(default_factory=list)
     email: str | None = Field(default_factory=str)
     availabilities: list[dict[str, Any]] = Field(default_factory=list)
 
 
 class Submission(BaseModel):
     ''' Submission '''
+    # pylint: disable=no-self-argument
     code: str = Field(default_factory=str,
                       description='A unique, alphanumeric identifier, also used in URLs')
     speakers: list[Speaker] = Field(
         default_factory=list, description='A list of speaker objects')
     title: str = Field(default_factory=str,
                        description='The submission’s title')
     track: dict[str, str] = Field(
@@ -51,14 +52,22 @@
         default_factory=int, description='The talk’s duration in minutes, or null')
     content_locale: str = Field(
         default_factory=str, description='The language the submission is in, e.g. “en” or “de”')
     notes: str = Field(default_factory=str, description='note')
     internal_notes: str | None = Field(
         description='Notes the organisers left on the submission. Available if the requesting user has organiser permissions.')
 
+    @validator('track', pre=True)
+    def verify_track(cls, value: Any) -> dict[str, str]:
+        ''' verify track '''
+        if value is None:
+            return {'en': 'no track'}
+
+        return value
+
 
 class Room(BaseModel):
     ''' Room '''
     id: int = Field(default_factory=int,
                     description="The unique ID of the room object")
     name: str = Field(default_factory=str, description='The name of the room')
     description: str = Field(
```

### Comparing `toldwords-0.6.0/PKG-INFO` & `toldwords-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toldwords
-Version: 0.6.0
+Version: 0.7.0
 Summary: Using ChatGPT to make keywords for the papers from COSCUP.
 Home-page: https://github.com/toomore/toldwords
 License: MIT
 Keywords: API,ChatGPT,pretalx,COSCUP,openai
 Author: Toomore Chiang
 Author-email: toomore0929@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: certifi
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/toomore/toldwords
 Description-Content-Type: text/markdown
 
 # toldwords
```

