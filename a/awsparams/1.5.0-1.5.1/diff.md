# Comparing `tmp/awsparams-1.5.0.tar.gz` & `tmp/awsparams-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsparams-1.5.0.tar", max compression
+gzip compressed data, was "awsparams-1.5.1.tar", max compression
```

## Comparing `awsparams-1.5.0.tar` & `awsparams-1.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-17 16:32:04.534822 awsparams-1.5.0/LICENSE
--rw-r--r--   0        0        0     4646 2023-05-17 16:32:04.534822 awsparams-1.5.0/README.md
--rw-r--r--   0        0        0    10098 2023-05-17 16:32:04.534822 awsparams-1.5.0/awsparams/__init__.py
--rwxr-xr-x   0        0        0    10305 2023-05-17 16:32:04.534822 awsparams-1.5.0/awsparams/cli.py
--rw-r--r--   0        0        0      680 2023-05-17 16:32:04.534822 awsparams-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5539 1970-01-01 00:00:00.000000 awsparams-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 18:24:30.060033 awsparams-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4646 2023-05-17 18:24:30.060033 awsparams-1.5.1/README.md
+-rw-r--r--   0        0        0    10098 2023-05-17 18:24:30.060033 awsparams-1.5.1/awsparams/__init__.py
+-rwxr-xr-x   0        0        0    10341 2023-05-17 18:24:30.060033 awsparams-1.5.1/awsparams/cli.py
+-rw-r--r--   0        0        0      680 2023-05-17 18:24:30.064033 awsparams-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5539 1970-01-01 00:00:00.000000 awsparams-1.5.1/PKG-INFO
```

### Comparing `awsparams-1.5.0/LICENSE` & `awsparams-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awsparams-1.5.0/README.md` & `awsparams-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `awsparams-1.5.0/awsparams/__init__.py` & `awsparams-1.5.1/awsparams/__init__.py`

 * *Files identical despite different names*

### Comparing `awsparams-1.5.0/awsparams/cli.py` & `awsparams-1.5.1/awsparams/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,28 +39,28 @@
 @click.option("-r", "--jetbrains-run-config", is_flag=True, help="format list for a Jetbrains run configuration")
 @click.option("-q", "--esc-quotes", is_flag=True, help="Escape quotes in values (for --env-vars or --tfvars)")
 @click.option(
     "--decryption/--no-decryption",
     help="by default display decrypted values",
     default=True,
 )
-def ls(prefix="", profile="", region="", values=False, run_config=False, env_vars=False, tfvars=False, esc_quotes=False, decryption=True):
+def ls(prefix="", profile="", region="", values=False, dot_env=False, tfvars=False, jetbrains_run_config=False, esc_quotes=False, decryption=True):
     """
     List Parameters, optionally matching a specific prefix
     """
     aws_params = AWSParams(profile, region)
-    if run_config or env_vars or tfvars:  # all of these options should also fetch the values
+    if jetbrains_run_config or dot_env or tfvars:  # all of these options should also fetch the values
         values = True
     if not values:
         decryption = False
     for parm in aws_params.get_all_parameters(
             prefix=prefix, values=values, decryption=decryption, trim_name=False
     ):
         if values:
-            if run_config or env_vars or tfvars:
+            if jetbrains_run_config or dot_env or tfvars:
                 param_parts = parm.Name.split('/')
                 prefix_parts = prefix.split('/')
                 # remove any duplicate, leading, or trailing delimiters from both lists
                 for arr in [param_parts, prefix_parts]:
                     for part in arr:
                         if part == '':
                             arr.remove(part)
@@ -72,19 +72,19 @@
                 # reconstruct the param name
                 name = '/'.join(name)
                 """
                 run_config - print out separated by '=' and ended with ';'
                 env_vars - print out separated by '=', values wrapped in quotes
                 tfvars - print out separated by ' = ', values wrapped in quotes
                 """
-                if env_vars:
+                if dot_env:
                     click.echo(f"{name}=\"{escape_quotes(parm.Value) if esc_quotes else parm.Value}\"")
                 elif tfvars:
                     click.echo(f"{name} = \"{escape_quotes(parm.Value) if esc_quotes else parm.Value}\"")
-                elif run_config:
+                elif jetbrains_run_config:
                     click.echo(f"{name}={parm.Value};")
             else:
                 click.echo(f"{parm.Name}: {parm.Value}")
         else:
             click.echo(parm.Name)
```

### Comparing `awsparams-1.5.0/pyproject.toml` & `awsparams-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsparams"
-version = "1.5.0"
+version = "1.5.1"
 description = "A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters"
 authors = ["Nate Peterson <ndpete@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/byu-oit/awsparams"
 repository = "https://github.com/byu-oit/awsparams"
```

### Comparing `awsparams-1.5.0/PKG-INFO` & `awsparams-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsparams
-Version: 1.5.0
+Version: 1.5.1
 Summary: A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters
 Home-page: https://github.com/byu-oit/awsparams
 License: Apache-2.0
 Author: Nate Peterson
 Author-email: ndpete@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

