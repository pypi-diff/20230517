# Comparing `tmp/nldb-0.3.7.tar.gz` & `tmp/nldb-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nldb-0.3.7.tar", last modified: Thu Apr 27 10:43:10 2023, max compression
+gzip compressed data, was "nldb-0.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nldb-0.3.7.tar` & `nldb-0.3.8.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1824 2023-04-27 10:00:54.088720 nldb-0.3.7/.gitignore
--rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.7/LICENSE
--rw-r--r--   0        0        0     1955 2023-04-26 07:38:48.172206 nldb-0.3.7/README.md
--rw-r--r--   0        0        0       51 2023-04-27 10:42:46.187726 nldb-0.3.7/nldb/__init__.py
--rw-r--r--   0        0        0     1958 2023-04-26 14:39:27.585694 nldb-0.3.7/nldb/api.py
--rw-r--r--   0        0        0     2588 2023-04-26 12:11:29.217383 nldb-0.3.7/nldb/cli.py
--rw-r--r--   0        0        0     7292 2023-04-27 10:39:07.196449 nldb-0.3.7/nldb/core.py
--rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.7/nldb/templates/Dockerfile
--rw-r--r--   0        0        0     4703 2023-04-27 09:19:09.574559 nldb-0.3.7/nldb/templates/index.html
--rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.7/nldb/templates/prompt.txt
--rw-r--r--   0        0        0      557 2023-04-27 10:40:00.761170 nldb-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 nldb-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-05-17 12:50:48.893108 nldb-0.3.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1824 2023-05-17 12:50:48.893108 nldb-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1076 2023-05-17 12:50:48.893108 nldb-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1996 2023-05-17 12:50:48.893108 nldb-0.3.8/README.md
+-rw-r--r--   0        0        0       51 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/__init__.py
+-rw-r--r--   0        0        0     1885 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/api.py
+-rw-r--r--   0        0        0     2593 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/cli.py
+-rw-r--r--   0        0        0      267 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/config.py
+-rw-r--r--   0        0        0     7276 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/core.py
+-rw-r--r--   0        0        0      102 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/templates/Dockerfile
+-rw-r--r--   0        0        0     4703 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/templates/index.html
+-rw-r--r--   0        0        0     2068 2023-05-17 12:50:48.893108 nldb-0.3.8/nldb/templates/prompt.txt
+-rw-r--r--   0        0        0      577 2023-05-17 12:50:48.893108 nldb-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 nldb-0.3.8/PKG-INFO
```

### Comparing `nldb-0.3.7/.gitignore` & `nldb-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nldb-0.3.7/LICENSE` & `nldb-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nldb-0.3.7/README.md` & `nldb-0.3.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Installation
 
 ```bash
 pip install nldb
 ```
 
-An OpenAI API key should be available as the `OPENAI_API_KEY` environment variable, e.g. using `export OPENAI_API_KEY=sk-etc`.
+An OpenAI API key should be available as the `OPENAI_API_KEY` environment variable, e.g. using `export OPENAI_API_KEY=sk-etc` or adding it to your project `.env` file.
 
 ## Preparing your database
 NLDB can talk to SQLite and DuckDB databases. Call yours `nldb.db` or specify the name with a `DATABASE` environment variable.
 
 You may need to simplify and denormalise your database for NLDB to work well. Your columns should have names whose meaning is obvious. While NLDB can join across tables, combining your data into a single table will reduce your prompt size and improve the accuracy of NLDB's query generation.
 
 ## Initialise NLDB
```

### Comparing `nldb-0.3.7/nldb/api.py` & `nldb-0.3.8/nldb/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import os
 from typing import Union
 
 import uvicorn
 from fastapi import FastAPI
 from fastapi.responses import FileResponse
 from pydantic import BaseModel
 
 from nldb.core import NLDB
+from nldb.config import UVICORN_HOST, UVICORN_PORT
 
-UVICORN_HOST = os.environ.get("UVICORN_HOST", "0.0.0.0")
-UVICORN_PORT = int(os.environ.get("UVICORN_PORT", 8080))
 
 app = FastAPI()
 
 
 @app.on_event("startup")
 def load_prompt_template():
     """Load the prompt template on startup."""
```

### Comparing `nldb-0.3.7/nldb/cli.py` & `nldb-0.3.8/nldb/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import inspect
 import os
 import shutil
 from typing import Optional
 
 import typer
 from nldb.api import serve
-from nldb.core import DATABASE, NLDB
+from nldb.core import NLDB
+from nldb.config import DATABASE, OPENAI_API_KEY
 
 
 def preflight_checks():
     # check that the prompt.txt file exists
     failures = 0
     if not os.path.exists("prompt.txt"):
         typer.echo("prompt.txt file not found")
         typer.echo("Run `nldb init` to create a new prompt.txt file")
         failures += 1
     if not os.path.exists(DATABASE):
         typer.echo(f"Database file not found: {DATABASE}")
         failures += 1
-    if not os.environ.get("OPENAI_API_KEY"):
+    if not OPENAI_API_KEY:
         typer.echo("OPENAI_API_KEY environment variable not set")
         failures += 1
     if failures > 0:
         raise typer.Exit(code=1)
 
 
 def init():
@@ -40,15 +41,15 @@
     if not os.path.exists(charts_dir):
         os.mkdir(charts_dir)
         typer.echo(f"Created directory at {charts_dir}")
 
 
 def deploy_instructions():
     typer.echo("Printing deployment instructions")
-    openai_api_key = os.environ.get("OPENAI_API_KEY", "your OpenAI API key")
+    openai_api_key = OPENAI_API_KEY or "your OpenAI API key"
     instructions = inspect.cleandoc(
         f"""
         # For fly.io:
         fly launch # answer no to Postgres, Redis and deploying now 
         fly secrets set OPENAI_API_KEY={openai_api_key} 
         fly deploy
```

### Comparing `nldb-0.3.7/nldb/core.py` & `nldb-0.3.8/nldb/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from timeit import default_timer as timer
 from typing import Tuple
 
 import duckdb
 import openai
 from tabulate import tabulate
 
-DATABASE = os.environ.get("DATABASE", "nldb.db")
+from nldb.config import DATABASE
 
 
 class ttimer:
     """A tiny timer context manager"""
 
     def __enter__(self):
         self.start_time = timer()
```

### Comparing `nldb-0.3.7/nldb/templates/index.html` & `nldb-0.3.8/nldb/templates/index.html`

 * *Files identical despite different names*

### Comparing `nldb-0.3.7/nldb/templates/prompt.txt` & `nldb-0.3.8/nldb/templates/prompt.txt`

 * *Files identical despite different names*

### Comparing `nldb-0.3.7/pyproject.toml` & `nldb-0.3.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "openai",
     "fastapi",
     "uvicorn[standard]",
     "tabulate",
     "typer",
     "duckdb",
     "matplotlib",
+    "python-dotenv"
 ]
 
 [project.urls]
 Home = "https://github.com/tomdyson/nldb"
 
 [project.scripts]
 nldb = "nldb.cli:cli_wrapper"
```

### Comparing `nldb-0.3.7/PKG-INFO` & `nldb-0.3.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: nldb
-Version: 0.3.7
+Version: 0.3.8
 Summary: talk to your database
 Author-email: Tom Dyson <tom@torchbox.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: openai
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: tabulate
 Requires-Dist: typer
 Requires-Dist: duckdb
 Requires-Dist: matplotlib
+Requires-Dist: python-dotenv
 Project-URL: Home, https://github.com/tomdyson/nldb
 
 # nldb
 
 Natural Language Databasing. Talk to your data in English, via CLI, API or a simple web interface.
 
 ## Installation
 
 ```bash
 pip install nldb
 ```
 
-An OpenAI API key should be available as the `OPENAI_API_KEY` environment variable, e.g. using `export OPENAI_API_KEY=sk-etc`.
+An OpenAI API key should be available as the `OPENAI_API_KEY` environment variable, e.g. using `export OPENAI_API_KEY=sk-etc` or adding it to your project `.env` file.
 
 ## Preparing your database
 NLDB can talk to SQLite and DuckDB databases. Call yours `nldb.db` or specify the name with a `DATABASE` environment variable.
 
 You may need to simplify and denormalise your database for NLDB to work well. Your columns should have names whose meaning is obvious. While NLDB can join across tables, combining your data into a single table will reduce your prompt size and improve the accuracy of NLDB's query generation.
 
 ## Initialise NLDB
```

