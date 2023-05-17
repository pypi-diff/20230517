# Comparing `tmp/geovisio_cli-0.0.5.tar.gz` & `tmp/geovisio_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.0.5.tar", last modified: Thu Apr 27 14:19:43 2023, max compression
+gzip compressed data, was "geovisio_cli-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.0.5.tar` & `geovisio_cli-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/.gitignore
--rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/.gitlab-ci.yml
--rw-r--r--   0        0        0     1714 2023-04-27 14:14:42.006482 geovisio_cli-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/Makefile
--rw-r--r--   0        0        0     7328 2023-04-27 14:14:42.006482 geovisio_cli-0.0.5/README.md
--rw-r--r--   0        0        0     2320 2023-04-14 07:21:46.587626 geovisio_cli-0.0.5/USAGE.md
--rw-r--r--   0        0        0       53 2023-04-27 14:14:42.006482 geovisio_cli-0.0.5/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     1972 2023-04-14 11:12:54.559203 geovisio_cli-0.0.5/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.0.5/geovisio_cli/exception.py
--rw-r--r--   0        0        0     3621 2023-04-14 07:21:46.587626 geovisio_cli-0.0.5/geovisio_cli/main.py
--rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/geovisio_cli/model.py
--rw-r--r--   0        0        0    14418 2023-04-24 11:28:19.596669 geovisio_cli-0.0.5/geovisio_cli/sequence.py
--rw-r--r--   0        0        0      896 2023-03-14 16:32:00.535627 geovisio_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/integration/__init__.py
--rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/integration/conftest.py
--rw-r--r--   0        0        0      671 2023-03-14 16:32:00.535627 geovisio_cli-0.0.5/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      319 2023-04-07 07:41:38.712978 geovisio_cli-0.0.5/tests/integration/test_status.py
--rw-r--r--   0        0        0     4914 2023-04-14 11:12:54.559203 geovisio_cli-0.0.5/tests/integration/test_upload.py
--rw-r--r--   0        0        0      528 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/tests/test_process.py
--rw-r--r--   0        0        0      813 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/tests/test_sequence.py
--rw-r--r--   0        0        0     8187 1970-01-01 00:00:00.000000 geovisio_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2558 2023-05-17 11:11:47.310135 geovisio_cli-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/LICENSE
+-rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/Makefile
+-rw-r--r--   0        0        0     7467 2023-05-15 17:41:10.367730 geovisio_cli-0.1.0/README.md
+-rw-r--r--   0        0        0     2502 2023-05-15 08:17:13.338400 geovisio_cli-0.1.0/USAGE.md
+-rw-r--r--   0        0        0       53 2023-05-17 11:11:47.310135 geovisio_cli-0.1.0/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     1937 2023-05-16 14:39:06.445129 geovisio_cli-0.1.0/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.1.0/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     4182 2023-05-15 08:17:13.342400 geovisio_cli-0.1.0/geovisio_cli/main.py
+-rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/geovisio_cli/model.py
+-rw-r--r--   0        0        0    19722 2023-05-17 11:07:32.865046 geovisio_cli-0.1.0/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0      948 2023-05-15 08:17:13.342400 geovisio_cli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0      651 2023-05-12 13:36:09.582468 geovisio_cli-0.1.0/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      369 2023-05-15 08:17:13.342400 geovisio_cli-0.1.0/tests/integration/test_status.py
+-rw-r--r--   0        0        0     8012 2023-05-15 17:46:58.046466 geovisio_cli-0.1.0/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.1.0/tests/test_process.py
+-rw-r--r--   0        0        0     2579 2023-05-15 17:51:20.171581 geovisio_cli-0.1.0/tests/test_sequence.py
+-rw-r--r--   0        0        0     8411 1970-01-01 00:00:00.000000 geovisio_cli-0.1.0/PKG-INFO
```

### Comparing `geovisio_cli-0.0.5/.gitlab-ci.yml` & `geovisio_cli-0.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/CHANGELOG.md` & `geovisio_cli-0.1.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [0.1.0] - 2023-05-17
+
+### Added
+- A new `--title` parameter to `geovisio upload` and `geovisio test_process` to provide a title to the uploaded collection. If no title is given, it will default to the directory name.
+- Broken uploads can now be recovered: if on a first upload try, some pictures fail, you can re-launch a second upload try by running the same `upload` command. The `_geovisio.toml` stores in a sequence folder which pictures were correctly sent, thus skip them on next try.
+
+### Changed
+- Command `test-process` generates a `_geovisio.toml` file in the sequence folder. This file can be edited before running command `upload` to change picture ordering.
+- Increase timeout to geovisio and add better error when a timeout happen or when a connection is lost
+
+
 ## [0.0.5] - 2023-04-27
 
 ### Fixed
 - Add a timeout to avoid `requests` module to hang forever if API is not responding
 
 
 ## [0.0.4] - 2023-04-14
@@ -35,13 +46,14 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.1.0...main
+[0.1.0]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...0.1.0
 [0.0.5]: https://gitlab.com/geovisio/cli/-/compare/0.0.4...0.0.5
 [0.0.4]: https://gitlab.com/geovisio/cli/-/compare/0.0.3...0.0.4
 [0.0.3]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...0.0.3
 [0.0.2]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...0.0.2
 [0.0.1]: https://gitlab.com/PanierAvide/geovisio/-/commits/0.0.1
```

### Comparing `geovisio_cli-0.0.5/CODE_OF_CONDUCT.md` & `geovisio_cli-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/LICENSE` & `geovisio_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/Makefile` & `geovisio_cli-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/README.md` & `geovisio_cli-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 
 ```bash
 geovisio upload --api-url http://localhost:5000/ ./my_sequence
 ```
 
 You can also add a `--wait` flag to wait for geovisio to process all the pictures.
 
+Note that you can launch again the same command to recover a partial sequence import, for example if only some pictures failed to upload.
+
 #### Authentication
 
 If the GeoVisio API requires a login for the upload, the user/password can either be set:
 * with command-line arguments (`--user` / `--password`)
 * with environment variables (`GEOVISIO_USER` / `GEOVISIO_PASSWORD`)
 
 If no information is set but required by the GeoVisio instance, they will be asked interactively. This is the best way to enter the password so it will not be stored in the command-line history.
```

### Comparing `geovisio_cli-0.0.5/USAGE.md` & `geovisio_cli-0.1.0/USAGE.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `collection-status`: Print the status of a collection.
-* `test-process`: (For testing) Generates a JSON file with...
+* `test-process`: (For testing) Generates a TOML file with...
 * `upload`: Processes and sends a given sequence on...
 
 ## `geovisio collection-status`
 
 Print the status of a collection.
 
 Either a --location should be provided, with the full location url of the collection
@@ -39,28 +39,29 @@
 * `--api-url TEXT`: GeoVisio endpoint URL
 * `--location TEXT`: Full url of the collection
 * `--wait / --no-wait`: wait for all pictures to be ready  [default: no-wait]
 * `--help`: Show this message and exit.
 
 ## `geovisio test-process`
 
-(For testing) Generates a JSON file with metadata used for upload
+(For testing) Generates a TOML file with metadata used for upload
 
 **Usage**:
 
 ```console
 $ geovisio test-process [OPTIONS] PATH
 ```
 
 **Arguments**:
 
 * `PATH`: Local path to your sequence folder  [required]
 
 **Options**:
 
+* `--title TEXT`: Collection title. If not provided, the title will be the directory name.
 * `--help`: Show this message and exit.
 
 ## `geovisio upload`
 
 Processes and sends a given sequence on your GeoVisio API
 
 **Usage**:
@@ -79,8 +80,9 @@
 * `--user TEXT`: GeoVisio user name if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the username will be asked during run.  [env var: GEOVISIO_USER]
 * `--password TEXT`: GeoVisio password if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the password will be asked during run.
 Note: is is advised to wait for prompt without using this variable.  [env var: GEOVISIO_PASSWORD]
 * `--wait / --no-wait`: Wait for all pictures to be ready  [default: no-wait]
 * `--is-blurred / --is-not-blurred`: Define if sequence is already blurred or not  [default: is-not-blurred]
+* `--title TEXT`: Collection title. If not provided, the title will be the directory name.
 * `--help`: Show this message and exit.
```

### Comparing `geovisio_cli-0.0.5/geovisio_cli/auth.py` & `geovisio_cli-0.1.0/geovisio_cli/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,28 @@
     return url
 
 
 def login(s: Session, geovisio: Geovisio):
     """
     Login to geovisio and store auth cookie in session
     """
+
     # we need to authenticate ourselves
     login = s.get(f"{geovisio.url}/api/auth/login")
 
     # For the moment we only manage login on keycloak via password, we'll need to change this for api token
     url = _get_keycloak_authenticate_form_url(login)
 
     if geovisio.user is None:
-        username = Prompt.ask("Enter username")
+        username = Prompt.ask("👤 Enter username")
     else:
         username = geovisio.user
 
     if geovisio.password is None:
-        password = Prompt.ask(
-            prompt="🗝 Enter password to log in geovisio", password=True
-        )
+        password = Prompt.ask(prompt="🗝 Enter password", password=True)
     else:
         password = geovisio.password
 
     r = s.post(
         url,
         data={"username": username, "password": password},
         headers={"Content-Type": "application/x-www-form-urlencoded"},
```

### Comparing `geovisio_cli-0.0.5/geovisio_cli/main.py` & `geovisio_cli-0.1.0/geovisio_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 from pathlib import Path
 from geovisio_cli import sequence, exception, model
 from rich import print
 from rich.panel import Panel
 from typing import Optional
+import os
 
 
 app = typer.Typer(help="GeoVisio command-line client")
 
 
 @app.command()
 def upload(
@@ -30,43 +31,56 @@
     ),
     wait: bool = typer.Option(default=False, help="Wait for all pictures to be ready"),
     isBlurred: bool = typer.Option(
         False,
         "--is-blurred/--is-not-blurred",
         help="Define if sequence is already blurred or not",
     ),
+    title: Optional[str] = typer.Option(
+        default=None,
+        help="Collection title. If not provided, the title will be the directory name.",
+    ),
 ):
     """Processes and sends a given sequence on your GeoVisio API"""
-
     geovisio = model.Geovisio(url=api_url, user=user, password=password)
     try:
-        sequence.upload(path, geovisio, wait, isBlurred)
+        sequence.upload(
+            path, geovisio, wait=wait, alreadyBlurred=isBlurred, title=title
+        )
     except exception.CliException as e:
         print(
             Panel(
                 f"{e}",
                 title="[red]Error while importing collection",
                 border_style="red",
             )
         )
         return 1
 
 
 @app.command()
 def test_process(
     path: Path = typer.Argument(..., help="Local path to your sequence folder"),
+    title: Optional[str] = typer.Option(
+        default=None,
+        help="Collection title. If not provided, the title will be the directory name.",
+    ),
 ):
-    """(For testing) Generates a JSON file with metadata used for upload"""
+    """(For testing) Generates a TOML file with metadata used for upload"""
 
     import json
     from dataclasses import asdict
 
     try:
-        collection = sequence.process(path)
-        print(json.dumps(asdict(collection), indent=2))
+        collection = sequence.process(path, title)
+        outputFile = os.path.join(path, sequence.SEQUENCE_TOML_FILE)
+        print(
+            "✅ [green]Metadata file saved to: [bold]" + outputFile + "[/bold][/green]"
+        )
+
     except exception.CliException as e:
         print(
             Panel(
                 f"{e}",
                 title="[red]Error while importing collection",
                 border_style="red",
             )
@@ -86,24 +100,27 @@
     """
     Print the status of a collection.\n
     Either a --location should be provided, with the full location url of the collection
     or only the --id combined with the --api-url
     """
 
     try:
-        location = location
         if location is None:
             if api_url is None or id is None:
                 raise exception.CliException(
                     "The way to identify the collection should be either with --location or with --id combined with --api-url"
                 )
             location = f"{api_url}/api/collections/{id}"
-        sequence.display_sequence_status(location)
+
+        mySequence = sequence.Sequence(id=id, location=location)
+        sequence.display_sequence_status(mySequence)
+
         if wait:
-            sequence.wait_for_sequence(location)
+            sequence.wait_for_sequence(mySequence)
+
     except exception.CliException as e:
         print(
             Panel(
                 f"{e}",
                 title="[red]Error while getting collection status",
                 border_style="red",
             )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geovisio_cli-0.0.5/pyproject.toml` & `geovisio_cli-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
     "requests ~= 2.28.0",
     "typer ~= 0.7.0",
     "rich[all] ~= 13.3.0",
+    "toml ~= 0.10.2",
 ]
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/cli"
 
 [project.scripts]
 geovisio="geovisio_cli.main:app"
@@ -28,14 +29,15 @@
     "black ~= 22.8.0",
     "mypy ~= 1.0.0",
     "types-requests ~= 2.28.0",
     "pytest ~= 7.2.0",
     "testcontainers-compose ~= 0.0.1rc1",
     "pytest-datafiles ~= 2.0.1",
     "typer-cli ~= 0.0.13",
+    "types-toml ~= 0.10.8.6",
 ]
 build = ["flit ~= 3.8.0"]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `geovisio_cli-0.0.5/tests/fixtures/e1.jpg` & `geovisio_cli-0.1.0/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/tests/fixtures/e2.jpg` & `geovisio_cli-0.1.0/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/tests/fixtures/e3.jpg` & `geovisio_cli-0.1.0/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/tests/integration/conftest.py` & `geovisio_cli-0.1.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.5/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.1.0/tests/integration/docker-compose-geovisio.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 version: "3"
 # Docker-compose to run a geovisio in the integration tests
 services:
   geovisio-api:
-    image: panieravide/geovisio:develop
+    image: geovisio/api:develop
     command: api
     restart: always
     ports:
       - 5000
     depends_on:
       db:
         condition: service_healthy
     environment:
       - DB_URL=postgres://gvs:gvspwd@db/geovisio
-      - SERVER_NAME=localhost:5001
-      - BLUR_STRATEGY=DISABLE
+      - PICTURE_PROCESS_DERIVATES_STRATEGY=ON_DEMAND
 
   db:
     image: postgis/postgis:13-3.2
     environment:
       - POSTGRES_USER=gvs
       - POSTGRES_PASSWORD=gvspwd
       - POSTGRES_DB=geovisio
```

### Comparing `geovisio_cli-0.0.5/tests/test_process.py` & `geovisio_cli-0.1.0/tests/test_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
     os.path.join(FIXTURE_DIR, "not_a_pic.md"),
 )
 def test_upload_with_invalid_file(datafiles):
-    s = sequence.process(path=Path(datafiles))
+    s = sequence.process(path=Path(datafiles), title=None)
 
     assert len(s.pictures) == 3
     assert [PurePath(p.path).stem for p in s.pictures] == ["e1", "e2", "e3"]
+    assert s.title == Path(datafiles).name
```

### Comparing `geovisio_cli-0.0.5/PKG-INFO` & `geovisio_cli-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.0.5
+Version: 0.1.0
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.7.0
 Requires-Dist: rich[all] ~= 13.3.0
+Requires-Dist: toml ~= 0.10.2
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: black ~= 22.8.0 ; extra == "dev"
 Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
 Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
 Requires-Dist: testcontainers-compose ~= 0.0.1rc1 ; extra == "dev"
 Requires-Dist: pytest-datafiles ~= 2.0.1 ; extra == "dev"
 Requires-Dist: typer-cli ~= 0.0.13 ; extra == "dev"
+Requires-Dist: types-toml ~= 0.10.8.6 ; extra == "dev"
 Project-URL: Home, https://gitlab.com/geovisio/cli
 Provides-Extra: build
 Provides-Extra: dev
 
 # ![GeoVisio](https://gitlab.com/geovisio/api/-/raw/develop/images/logo_full.png)
 
 __GeoVisio__ is a complete solution for storing and __serving your own 📍📷 geolocated pictures__ (like [StreetView](https://www.google.com/streetview/) / [Mapillary](https://mapillary.com/)).
@@ -136,14 +138,16 @@
 
 ```bash
 geovisio upload --api-url http://localhost:5000/ ./my_sequence
 ```
 
 You can also add a `--wait` flag to wait for geovisio to process all the pictures.
 
+Note that you can launch again the same command to recover a partial sequence import, for example if only some pictures failed to upload.
+
 #### Authentication
 
 If the GeoVisio API requires a login for the upload, the user/password can either be set:
 * with command-line arguments (`--user` / `--password`)
 * with environment variables (`GEOVISIO_USER` / `GEOVISIO_PASSWORD`)
 
 If no information is set but required by the GeoVisio instance, they will be asked interactively. This is the best way to enter the password so it will not be stored in the command-line history.
```

