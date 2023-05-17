# Comparing `tmp/awsparams-1.4.1.tar.gz` & `tmp/awsparams-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsparams-1.4.1.tar", max compression
+gzip compressed data, was "awsparams-1.5.0.tar", max compression
```

## Comparing `awsparams-1.4.1.tar` & `awsparams-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-02-17 21:50:43.591867 awsparams-1.4.1/LICENSE
--rw-r--r--   0        0        0     4245 2023-02-17 21:50:43.591867 awsparams-1.4.1/README.md
--rw-r--r--   0        0        0    10098 2023-02-17 21:50:43.591867 awsparams-1.4.1/awsparams/__init__.py
--rwxr-xr-x   0        0        0     8655 2023-02-17 21:50:43.591867 awsparams-1.4.1/awsparams/cli.py
--rw-r--r--   0        0        0      680 2023-02-17 21:50:43.591867 awsparams-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 awsparams-1.4.1/setup.py
--rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 awsparams-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 16:32:04.534822 awsparams-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4646 2023-05-17 16:32:04.534822 awsparams-1.5.0/README.md
+-rw-r--r--   0        0        0    10098 2023-05-17 16:32:04.534822 awsparams-1.5.0/awsparams/__init__.py
+-rwxr-xr-x   0        0        0    10305 2023-05-17 16:32:04.534822 awsparams-1.5.0/awsparams/cli.py
+-rw-r--r--   0        0        0      680 2023-05-17 16:32:04.534822 awsparams-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5539 1970-01-01 00:00:00.000000 awsparams-1.5.0/PKG-INFO
```

### Comparing `awsparams-1.4.1/LICENSE` & `awsparams-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsparams-1.4.1/README.md` & `awsparams-1.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -91,16 +91,26 @@
 
 ls with values no decryption: `awsparams ls --values` or `awsparams ls -v`
 
 ls with values and decryption: `awsparams ls --with-decryption`
 
 ls by prefix: `awsparams ls appname.prd`
 
-ls with values, formatted as an environment variable string: `awsparams ls -v --env-format <prefix>` or `awsparams ls -v -f <prefix>`
-> *`--env-format`/`-f` is used for easy quickly pasting into run configurations in IDE's*
+ls with values, formatted for using in a Jetbrains run configuration: `awsparams ls -r <prefix>`
+or `awsparams ls --jetbrains-run-config <prefix>`
+
+ls with values, formatted for using in a `.env` file: `awsparams ls -e <prefix>`
+or `awsparams ls --dot-env <prefix>`
+
+ls with values, formatted for using in a `.tfvars` file: `awsparams ls -t <prefix>`
+or `awsparams ls --tfvars <prefix>`
+
+For the above two options, add the `-q` or `--esc-quotes` flag for adding `\` in front of any quotation marks in
+the values, such as in stringify-ed JSON objects. Most `.env` file parsers don't require this, but `.tfvars`
+probably does.
 
 ## new usage
 
 new interactively: `awsparams new`
 
 new semi-interactively: `awsparams new --name appname.prd.username`
```

### Comparing `awsparams-1.4.1/awsparams/__init__.py` & `awsparams-1.5.0/awsparams/__init__.py`

 * *Files identical despite different names*

### Comparing `awsparams-1.4.1/awsparams/cli.py` & `awsparams-1.5.0/awsparams/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,45 +30,78 @@
 
 
 @main.command("ls")
 @click.argument("prefix", default="")
 @click.option("--profile", type=click.STRING, help="profile to run with")
 @click.option("--region", type=click.STRING, help="optional region to use")
 @click.option("-v", "--values", is_flag=True, help="display values")
-@click.option("-f", "--env-format", is_flag=True, help="format as a list of env vars (used with -v)")
+@click.option("-e", "--dot-env", is_flag=True, help="format list for a .env file")
+@click.option("-t", "--tfvars", is_flag=True, help="format list for a .tfvars file")
+@click.option("-r", "--jetbrains-run-config", is_flag=True, help="format list for a Jetbrains run configuration")
+@click.option("-q", "--esc-quotes", is_flag=True, help="Escape quotes in values (for --env-vars or --tfvars)")
 @click.option(
     "--decryption/--no-decryption",
     help="by default display decrypted values",
     default=True,
 )
-def ls(prefix="", profile="", region="", values=False, env_format=False, decryption=True):
+def ls(prefix="", profile="", region="", values=False, run_config=False, env_vars=False, tfvars=False, esc_quotes=False, decryption=True):
     """
-    List Paramters, optional matching a specific prefix
+    List Parameters, optionally matching a specific prefix
     """
     aws_params = AWSParams(profile, region)
+    if run_config or env_vars or tfvars:  # all of these options should also fetch the values
+        values = True
     if not values:
         decryption = False
     for parm in aws_params.get_all_parameters(
-        prefix=prefix, values=values, decryption=decryption, trim_name=False
+            prefix=prefix, values=values, decryption=decryption, trim_name=False
     ):
         if values:
-            if env_format:
-                short_param = parm.Name.replace(prefix, "")
-                # Sometimes leftover delimiters remain at the beginning of the string after this step
-                # This loop removes those delimiters so that the variables are formatted in a useful manner.
-                delimiters = ['.', '\\', '/']
-                while delimiters.count(short_param[0]) != 0:
-                    short_param = short_param[1:]
-                click.echo(f"{short_param}={parm.Value};")
+            if run_config or env_vars or tfvars:
+                param_parts = parm.Name.split('/')
+                prefix_parts = prefix.split('/')
+                # remove any duplicate, leading, or trailing delimiters from both lists
+                for arr in [param_parts, prefix_parts]:
+                    for part in arr:
+                        if part == '':
+                            arr.remove(part)
+                name = []
+                # 'subtract' the prefix from the name by starting from the rightmost element
+                #  and appending elements leftwards until you reach the prefix
+                for i in range(len(param_parts) - 1, len(prefix_parts) - 1, -1):
+                    name.insert(0, param_parts[i])
+                # reconstruct the param name
+                name = '/'.join(name)
+                """
+                run_config - print out separated by '=' and ended with ';'
+                env_vars - print out separated by '=', values wrapped in quotes
+                tfvars - print out separated by ' = ', values wrapped in quotes
+                """
+                if env_vars:
+                    click.echo(f"{name}=\"{escape_quotes(parm.Value) if esc_quotes else parm.Value}\"")
+                elif tfvars:
+                    click.echo(f"{name} = \"{escape_quotes(parm.Value) if esc_quotes else parm.Value}\"")
+                elif run_config:
+                    click.echo(f"{name}={parm.Value};")
             else:
                 click.echo(f"{parm.Name}: {parm.Value}")
         else:
             click.echo(parm.Name)
 
 
+def escape_quotes(string):
+    newstr = ''
+    for c in string:
+        if c == '"':
+            newstr += '\\"'
+        else:
+            newstr += c
+    return newstr
+
+
 @main.command("cp")
 @click.argument("src")
 @click.argument("dst", default="")
 @click.option("--src_profile", type=click.STRING, default="", help="source profile")
 @click.option(
     "--src_region", type=click.STRING, default="", help="optional source region"
 )
@@ -80,23 +113,23 @@
 )
 @click.option("--prefix", is_flag=True, help="copy set of parameters based on a prefix")
 @click.option("--overwrite", is_flag=True, help="overwrite existing parameters")
 @click.option(
     "--key", type=click.STRING, default="", help="kms key to use for new copy"
 )
 def cp(
-    src,
-    dst,
-    src_profile,
-    src_region,
-    dst_profile,
-    dst_region,
-    prefix=False,
-    overwrite=False,
-    key="",
+        src,
+        dst,
+        src_profile,
+        src_region,
+        dst_profile,
+        dst_region,
+        prefix=False,
+        overwrite=False,
+        key="",
 ):
     """
     Copy a parameter, optionally across accounts
     """
     aws_params = AWSParams(src_profile, src_region)
     # cross account copy without needing dst
     if dst_profile and src_profile != dst_profile and not dst:
@@ -143,15 +176,15 @@
 @click.pass_context
 def mv(ctx, src, dst, prefix=False, profile="", region=""):
     """
     Move or rename a parameter
     """
     if prefix:
         if ctx.invoke(
-            cp, src=src, dst=dst, src_profile=profile, prefix=prefix, src_region=region
+                cp, src=src, dst=dst, src_profile=profile, prefix=prefix, src_region=region
         ):
             ctx.invoke(
                 rm, src=src, force=True, prefix=True, profile=profile, region=region
             )
     else:
         if ctx.invoke(cp, src=src, dst=dst, src_profile=profile, src_region=region):
             ctx.invoke(rm, src=src, force=True, profile=profile, region=region)
@@ -204,22 +237,22 @@
 @click.option(
     "--description", type=click.STRING, default="", help="parameter description text"
 )
 @click.option("--profile", type=click.STRING, help="alternative profile to be used")
 @click.option("--region", type=click.STRING, help="alternative region to be used")
 @click.option("--overwrite", is_flag=True, help="overwrite exisiting parameters")
 def new(
-    name=None,
-    value=None,
-    param_type="String",
-    key="",
-    description="",
-    profile="",
-    region="",
-    overwrite=False,
+        name=None,
+        value=None,
+        param_type="String",
+        key="",
+        description="",
+        profile="",
+        region="",
+        overwrite=False,
 ):
     """
     Create a new parameter
     """
     AWSParams(profile, region).new_param(
         name,
         value,
```

### Comparing `awsparams-1.4.1/pyproject.toml` & `awsparams-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsparams"
-version = "1.4.1"
+version = "1.5.0"
 description = "A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters"
 authors = ["Nate Peterson <ndpete@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/byu-oit/awsparams"
 repository = "https://github.com/byu-oit/awsparams"
```

### Comparing `awsparams-1.4.1/setup.py` & `awsparams-1.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,153 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: awsparams
+Version: 1.5.0
+Summary: A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters
+Home-page: https://github.com/byu-oit/awsparams
+License: Apache-2.0
+Author: Nate Peterson
+Author-email: ndpete@gmail.com
+Requires-Python: >=3.6,<4
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.17.56,<2.0.0)
+Requires-Dist: click (>=7.1.2,<8.0.0)
+Project-URL: Repository, https://github.com/byu-oit/awsparams
+Description-Content-Type: text/markdown
+
+# Note
+Version 1 of this library is drastically different than previous versions.
+The CLI Application hasn't changed but the library it uses has.
+Please pay extra attention to the examples below or look at the underlying class for more information.
+
+# Why this script?
+
+The current (Jul 2017) AWS Console for the Systems Manager Parameter
+Store is good for adding and editing the values of parameters, but
+misses key productivity functions like copying (especially en mass),
+renaming, etc. The current `aws ssm` CLI is very similar in
+functionality to the AWS Console.
+
+This script is to automate a lot of the manual work currently needed
+with the existing AWS-provided UIs.
+
+# Docs
+Full documentation can be found here: https://awsparams.readthedocs.io/en/latest/
+
+# Installation
+
+  - AWSParams requires Python 3.6+
+  - Depending on your Python3.6 install either `pip install awsparams` or `pip3 install awsparams`
+    - If you're on windows, make sure that `C:\Users\{your user}\AppData\Roaming\Python\{your python version}\Scripts` has been added to your user path.
+
+# Usage
+## Library:
+
+```python
+from awsparams import AWSParams
+ 
+# Using default Profile
+aws_params = AWSParams()
+
+# Using a Custome Profile
+aws_params = AWSParams('MyProfile')
+
+#get a single parameter
+param = get_parameter('test1')
+# ParamResult(Name='test1', Value='test123', Type='SecureString')
+
+#ParamResult is a named tuple with properties Name, Value, Type
+param.Name # 'test1'
+param.Value # 'test123'
+param.Type # 'SecureString'
+
+# get multiple parameters with a prefix
+params = get_all_parameters(prefix="testing.testing.")
+# [ParamResult(Name='testing', Value='1234', Type='String'),
+#  ParamResult(Name='testing2', Value='1234', Type='String')]
+
+# get multiple parameters by path
+params = get_all_parameters(prefix="/testing/testing/", by_path=True)
+# [ParamResult(Name='testing', Value='1234', Type='String'),
+#  ParamResult(Name='testing2', Value='1234', Type='String')]
+
+# get multiple parameters by path
+params = get_all_parameters(prefix="/testing/testing/", by_path=True, trim_name=False)
+# [ParamResult(Name='/testing/testing/testing', Value='1234', Type='String'),
+#  ParamResult(Name='/testing/testing/testing2', Value='1234', Type='String')]
+
+# get just a parameter value
+value = get_parameter_value('test1')
+# test123
+```
+For more detailed examples of usage as a library see the cli implementation [here](https://github.com/byu-oit/awsparams/blob/master/awsparams/cli.py).
+
+## CLI application:
+Usage can be referenced by running `awsparams --help` or `awsparams
+subcommand --help` commands:
+
+    Usage: awsparams [OPTIONS] COMMAND [ARGS]...
+    
+    Options:
+    --version  Show the version and exit.
+    --help     Show this message and exit.
+    
+    Commands:
+    cp   Copy a parameter, optionally across accounts
+    ls   List Paramters, optional matching a specific...
+    mv   Move or rename a parameter
+    new  Create a new parameter
+    rm   Remove/Delete a parameter
+    set  Edit an existing parameter
+
+# Command Examples
+
+## ls usage
+
+ls names only: `awsparams ls`
+
+ls with values no decryption: `awsparams ls --values` or `awsparams ls -v`
+
+ls with values and decryption: `awsparams ls --with-decryption`
+
+ls by prefix: `awsparams ls appname.prd`
+
+ls with values, formatted for using in a Jetbrains run configuration: `awsparams ls -r <prefix>`
+or `awsparams ls --jetbrains-run-config <prefix>`
+
+ls with values, formatted for using in a `.env` file: `awsparams ls -e <prefix>`
+or `awsparams ls --dot-env <prefix>`
+
+ls with values, formatted for using in a `.tfvars` file: `awsparams ls -t <prefix>`
+or `awsparams ls --tfvars <prefix>`
+
+For the above two options, add the `-q` or `--esc-quotes` flag for adding `\` in front of any quotation marks in
+the values, such as in stringify-ed JSON objects. Most `.env` file parsers don't require this, but `.tfvars`
+probably does.
+
+## new usage
+
+new interactively: `awsparams new`
+
+new semi-interactively: `awsparams new --name appname.prd.username`
+
+new non-interactive: `awsparams new --name appname.prd.usrname --value parameter_value
+--description parameter_descripton`
+
+## cp usage
+
+copy a parameter: `awsparams cp appname.prd.username newappname.prd.username`
+
+copy set of parameters with prefix appname.dev. to appname.prd.: `awsparams cp appname.dev. appname.prd. --prefix`
+
+copy set of parameters starting with prefix repometa-generator.prd
+overwrite existing parameters accross different accounts: `awsparams cp repometa-generator.prd --src_profile=dev --dst_profile=trn
+--prefix=True`
 
-packages = \
-['awsparams']
+copy single parameters accross different accounts: `awsparams cp appname.dev.username appname.trb.us`
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['boto3>=1.17.56,<2.0.0', 'click>=7.1.2,<8.0.0']
-
-entry_points = \
-{'console_scripts': ['awsparams = awsparams.cli:main']}
-
-setup_kwargs = {
-    'name': 'awsparams',
-    'version': '1.4.1',
-    'description': 'A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters',
-    'long_description': '# Note\nVersion 1 of this library is drastically different than previous versions.\nThe CLI Application hasn\'t changed but the library it uses has.\nPlease pay extra attention to the examples below or look at the underlying class for more information.\n\n# Why this script?\n\nThe current (Jul 2017) AWS Console for the Systems Manager Parameter\nStore is good for adding and editing the values of parameters, but\nmisses key productivity functions like copying (especially en mass),\nrenaming, etc. The current `aws ssm` CLI is very similar in\nfunctionality to the AWS Console.\n\nThis script is to automate a lot of the manual work currently needed\nwith the existing AWS-provided UIs.\n\n# Docs\nFull documentation can be found here: https://awsparams.readthedocs.io/en/latest/\n\n# Installation\n\n  - AWSParams requires Python 3.6+\n  - Depending on your Python3.6 install either `pip install awsparams` or `pip3 install awsparams`\n    - If you\'re on windows, make sure that `C:\\Users\\{your user}\\AppData\\Roaming\\Python\\{your python version}\\Scripts` has been added to your user path.\n\n# Usage\n## Library:\n\n```python\nfrom awsparams import AWSParams\n \n# Using default Profile\naws_params = AWSParams()\n\n# Using a Custome Profile\naws_params = AWSParams(\'MyProfile\')\n\n#get a single parameter\nparam = get_parameter(\'test1\')\n# ParamResult(Name=\'test1\', Value=\'test123\', Type=\'SecureString\')\n\n#ParamResult is a named tuple with properties Name, Value, Type\nparam.Name # \'test1\'\nparam.Value # \'test123\'\nparam.Type # \'SecureString\'\n\n# get multiple parameters with a prefix\nparams = get_all_parameters(prefix="testing.testing.")\n# [ParamResult(Name=\'testing\', Value=\'1234\', Type=\'String\'),\n#  ParamResult(Name=\'testing2\', Value=\'1234\', Type=\'String\')]\n\n# get multiple parameters by path\nparams = get_all_parameters(prefix="/testing/testing/", by_path=True)\n# [ParamResult(Name=\'testing\', Value=\'1234\', Type=\'String\'),\n#  ParamResult(Name=\'testing2\', Value=\'1234\', Type=\'String\')]\n\n# get multiple parameters by path\nparams = get_all_parameters(prefix="/testing/testing/", by_path=True, trim_name=False)\n# [ParamResult(Name=\'/testing/testing/testing\', Value=\'1234\', Type=\'String\'),\n#  ParamResult(Name=\'/testing/testing/testing2\', Value=\'1234\', Type=\'String\')]\n\n# get just a parameter value\nvalue = get_parameter_value(\'test1\')\n# test123\n```\nFor more detailed examples of usage as a library see the cli implementation [here](https://github.com/byu-oit/awsparams/blob/master/awsparams/cli.py).\n\n## CLI application:\nUsage can be referenced by running `awsparams --help` or `awsparams\nsubcommand --help` commands:\n\n    Usage: awsparams [OPTIONS] COMMAND [ARGS]...\n    \n    Options:\n    --version  Show the version and exit.\n    --help     Show this message and exit.\n    \n    Commands:\n    cp   Copy a parameter, optionally across accounts\n    ls   List Paramters, optional matching a specific...\n    mv   Move or rename a parameter\n    new  Create a new parameter\n    rm   Remove/Delete a parameter\n    set  Edit an existing parameter\n\n# Command Examples\n\n## ls usage\n\nls names only: `awsparams ls`\n\nls with values no decryption: `awsparams ls --values` or `awsparams ls -v`\n\nls with values and decryption: `awsparams ls --with-decryption`\n\nls by prefix: `awsparams ls appname.prd`\n\nls with values, formatted as an environment variable string: `awsparams ls -v --env-format <prefix>` or `awsparams ls -v -f <prefix>`\n> *`--env-format`/`-f` is used for easy quickly pasting into run configurations in IDE\'s*\n\n## new usage\n\nnew interactively: `awsparams new`\n\nnew semi-interactively: `awsparams new --name appname.prd.username`\n\nnew non-interactive: `awsparams new --name appname.prd.usrname --value parameter_value\n--description parameter_descripton`\n\n## cp usage\n\ncopy a parameter: `awsparams cp appname.prd.username newappname.prd.username`\n\ncopy set of parameters with prefix appname.dev. to appname.prd.: `awsparams cp appname.dev. appname.prd. --prefix`\n\ncopy set of parameters starting with prefix repometa-generator.prd\noverwrite existing parameters accross different accounts: `awsparams cp repometa-generator.prd --src_profile=dev --dst_profile=trn\n--prefix=True`\n\ncopy single parameters accross different accounts: `awsparams cp appname.dev.username appname.trb.us`\n',
-    'author': 'Nate Peterson',
-    'author_email': 'ndpete@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/byu-oit/awsparams',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4',
-}
-
-
-setup(**setup_kwargs)
```

