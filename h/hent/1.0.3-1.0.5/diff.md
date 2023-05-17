# Comparing `tmp/hent-1.0.3.tar.gz` & `tmp/hent-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hent-1.0.3.tar", last modified: Sun Mar  7 15:08:55 2021, max compression
+gzip compressed data, was "hent-1.0.5.tar", last modified: Wed May 17 09:00:03 2023, max compression
```

## Comparing `hent-1.0.3.tar` & `hent-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 sofi      (1000) sofi      (1000)        0 2021-03-07 15:08:55.578972 hent-1.0.3/
--rw-r--r--   0 sofi      (1000) sofi      (1000)     1921 2021-03-07 15:08:55.578972 hent-1.0.3/PKG-INFO
--rw-r--r--   0 sofi      (1000) sofi      (1000)     1025 2021-02-28 15:43:57.000000 hent-1.0.3/README.md
-drwxr-xr-x   0 sofi      (1000) sofi      (1000)        0 2021-03-07 15:08:55.578972 hent-1.0.3/hent/
--rw-r--r--   0 sofi      (1000) sofi      (1000)       53 2021-02-28 15:41:35.000000 hent-1.0.3/hent/__init__.py
--rw-r--r--   0 sofi      (1000) sofi      (1000)       40 2021-02-28 15:41:45.000000 hent-1.0.3/hent/__main__.py
--rwxr-xr-x   0 sofi      (1000) sofi      (1000)     5652 2021-03-07 15:08:35.000000 hent-1.0.3/hent/console_script.py
-drwxr-xr-x   0 sofi      (1000) sofi      (1000)        0 2021-03-07 15:08:55.578972 hent-1.0.3/hent.egg-info/
--rw-r--r--   0 sofi      (1000) sofi      (1000)     1921 2021-03-07 15:08:55.000000 hent-1.0.3/hent.egg-info/PKG-INFO
--rw-r--r--   0 sofi      (1000) sofi      (1000)      261 2021-03-07 15:08:55.000000 hent-1.0.3/hent.egg-info/SOURCES.txt
--rw-r--r--   0 sofi      (1000) sofi      (1000)        1 2021-03-07 15:08:55.000000 hent-1.0.3/hent.egg-info/dependency_links.txt
--rw-r--r--   0 sofi      (1000) sofi      (1000)       36 2021-03-07 15:08:55.000000 hent-1.0.3/hent.egg-info/entry_points.txt
--rw-r--r--   0 sofi      (1000) sofi      (1000)        7 2021-03-07 15:08:55.000000 hent-1.0.3/hent.egg-info/requires.txt
--rw-r--r--   0 sofi      (1000) sofi      (1000)        5 2021-03-07 15:08:55.000000 hent-1.0.3/hent.egg-info/top_level.txt
--rw-r--r--   0 sofi      (1000) sofi      (1000)      104 2021-02-28 15:34:06.000000 hent-1.0.3/pyproject.toml
--rw-r--r--   0 sofi      (1000) sofi      (1000)      664 2021-03-07 15:08:55.579972 hent-1.0.3/setup.cfg
+drwxr-xr-x   0 sofi      (1000) users      (100)        0 2023-05-17 09:00:03.647966 hent-1.0.5/
+-rw-r--r--   0 sofi      (1000) users      (100)     1080 2023-05-17 08:02:42.000000 hent-1.0.5/LICENSE
+-rw-r--r--   0 sofi      (1000) users      (100)     1636 2023-05-17 09:00:03.647966 hent-1.0.5/PKG-INFO
+-rw-r--r--   0 sofi      (1000) users      (100)     1122 2023-05-17 08:07:51.000000 hent-1.0.5/README.md
+drwxr-xr-x   0 sofi      (1000) users      (100)        0 2023-05-17 09:00:03.646966 hent-1.0.5/hent/
+-rw-r--r--   0 sofi      (1000) users      (100)       57 2023-05-17 08:17:36.000000 hent-1.0.5/hent/__init__.py
+-rw-r--r--   0 sofi      (1000) users      (100)       45 2023-05-17 08:17:23.000000 hent-1.0.5/hent/__main__.py
+-rwxr-xr-x   0 sofi      (1000) users      (100)     6273 2023-05-17 08:48:43.000000 hent-1.0.5/hent/console_script.py
+drwxr-xr-x   0 sofi      (1000) users      (100)        0 2023-05-17 09:00:03.647966 hent-1.0.5/hent.egg-info/
+-rw-r--r--   0 sofi      (1000) users      (100)     1636 2023-05-17 09:00:03.000000 hent-1.0.5/hent.egg-info/PKG-INFO
+-rw-r--r--   0 sofi      (1000) users      (100)      269 2023-05-17 09:00:03.000000 hent-1.0.5/hent.egg-info/SOURCES.txt
+-rw-r--r--   0 sofi      (1000) users      (100)        1 2023-05-17 09:00:03.000000 hent-1.0.5/hent.egg-info/dependency_links.txt
+-rw-r--r--   0 sofi      (1000) users      (100)       35 2023-05-17 09:00:03.000000 hent-1.0.5/hent.egg-info/entry_points.txt
+-rw-r--r--   0 sofi      (1000) users      (100)        7 2023-05-17 09:00:03.000000 hent-1.0.5/hent.egg-info/requires.txt
+-rw-r--r--   0 sofi      (1000) users      (100)        5 2023-05-17 09:00:03.000000 hent-1.0.5/hent.egg-info/top_level.txt
+-rw-r--r--   0 sofi      (1000) users      (100)      104 2023-05-17 08:02:42.000000 hent-1.0.5/pyproject.toml
+-rw-r--r--   0 sofi      (1000) users      (100)      643 2023-05-17 09:00:03.647966 hent-1.0.5/setup.cfg
```

### Comparing `hent-1.0.3/PKG-INFO` & `hent-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 Metadata-Version: 2.1
 Name: hent
-Version: 1.0.3
+Version: 1.0.5
 Summary: A neofetch alternative written in python.
-Home-page: https://gitlab.com/imsofi/hent/
-Author: imSofi
-Author-email: 6748208-imsofi@users.noreply.gitlab.com
+Home-page: https://github.com/imsofi/hent
+Author: Sofi
+Author-email: sofi+hent@mailbox.org
 License: MIT
-Description: # Hent
-        
-        Neofetch alternative built in python
-        
-        ## Usage:
-        ```
-        $ ./hent.py
-                 ..             Distro: Arch Linux
-                 cc             Kernel: 5.10.16-zen1-1-zen
-                :ooc            Uptime: 3 hours, 45 minutes
-               ::lool         Packages: 1864 (pacman), 38 (flatpak)
-             .looooool.          Shell: bash
-            .loo;..;ooo.      Terminal: kitty
-           'oooo    looc.          CPU: Intel i7-4790K @ 4.00GHz
-          ;l;'..     .';l;         GPU: GeForce RTX 2060 Rev. A
-         ..              .'     Memory: 6325MB / 24562MB
-        ```
-        ```
-        $ ./hent.py --help
-        usage: hent.py [-h] [--distro distro] [--color true/false]
-        
-        Neofetch inspired fetch tool built in python.
-        
-        optional arguments:
-          -h, --help          show this help message and exit
-          --distro distro     which ascii art to use
-          --color true/false  enable/disable colored output
-        ```
-        
-        ## Installation:
-        
-        ### With pip:
-        ```
-        pip3 install hent
-        ```
-        
-        ### With git:
-        ```
-        git clone https://gitlab.com/imsofi/hent
-        cd hent
-        pip3 install --upgrade build
-        python3 -m build
-        pip3 install dist/*.whl
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hent
+
+Neofetch alternative built in python
+
+## Usage:
+```
+$ hent
+         ..             Distro: Arch Linux
+         cc             Kernel: 5.10.16-zen1-1-zen
+        :ooc            Uptime: 3 hours, 45 minutes
+       ::lool         Packages: 1864 (pacman), 38 (flatpak)
+     .looooool.          Shell: bash
+    .loo;..;ooo.      Terminal: kitty
+   'oooo    looc.          CPU: Intel i7-4790K @ 4.00GHz
+  ;l;'..     .';l;         GPU: GeForce RTX 2060 Rev. A
+ ..              .'     Memory: 6325MB / 24562MB
+```
+```
+$ hent --help
+usage: hent [-h] [--distro distro] [--color true/false]
+
+Neofetch inspired fetch tool built in python.
+
+optional arguments:
+  -h, --help          show this help message and exit
+  --distro distro     which ascii art to use
+  --color true/false  enable/disable colored output
+```
+
+## Installation:
+
+### With pip:
+```
+pip3 install hent
+```
+
+### With git:
+```
+git clone https://github.com/imsofi/hent.git
+cd hent
+pip3 install --upgrade build
+python3 -m build
+pip3 install dist/*.whl
+```
+
+## Development
+
+```
+python3 -m venv .venv
+source .venv/bin/activate
+pip3 install -r requirements.txt
+```
```

### Comparing `hent-1.0.3/README.md` & `hent-1.0.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Hent
 
 Neofetch alternative built in python
 
 ## Usage:
 ```
-$ ./hent.py
+$ hent
          ..             Distro: Arch Linux
          cc             Kernel: 5.10.16-zen1-1-zen
         :ooc            Uptime: 3 hours, 45 minutes
        ::lool         Packages: 1864 (pacman), 38 (flatpak)
      .looooool.          Shell: bash
     .loo;..;ooo.      Terminal: kitty
    'oooo    looc.          CPU: Intel i7-4790K @ 4.00GHz
   ;l;'..     .';l;         GPU: GeForce RTX 2060 Rev. A
  ..              .'     Memory: 6325MB / 24562MB
 ```
 ```
-$ ./hent.py --help
-usage: hent.py [-h] [--distro distro] [--color true/false]
+$ hent --help
+usage: hent [-h] [--distro distro] [--color true/false]
 
 Neofetch inspired fetch tool built in python.
 
 optional arguments:
   -h, --help          show this help message and exit
   --distro distro     which ascii art to use
   --color true/false  enable/disable colored output
@@ -32,13 +32,21 @@
 ### With pip:
 ```
 pip3 install hent
 ```
 
 ### With git:
 ```
-git clone https://gitlab.com/imsofi/hent
+git clone https://github.com/imsofi/hent.git
 cd hent
 pip3 install --upgrade build
 python3 -m build
 pip3 install dist/*.whl
 ```
+
+## Development
+
+```
+python3 -m venv .venv
+source .venv/bin/activate
+pip3 install -r requirements.txt
+```
```

### Comparing `hent-1.0.3/hent/console_script.py` & `hent-1.0.5/hent/console_script.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 
 import argparse
+import datetime
 from itertools import zip_longest
 import platform
 import subprocess
 import os
 import psutil
 
 DISTROS_ART = {
@@ -93,47 +94,58 @@
 
 PKGS = {
     'pacman': ['pacman', '-Qq'],
     'rpm': ['rpm', '-qa'],
     'dpkg': ['dpkg', '--list'],
     'flatpak': ['flatpak', 'list'],
     'snap': ['snap', 'list'],
+    'nix-system': ['nix-store', '-qR', '/run/current-system/sw'],
+    'nix-user': ['nix-store', '-qR', os.path.expanduser('~/.nix-profile')],
 }
 
 TERM_NAMES = {
     'hyper': 'Hyper Terminal',
     'gnome-terminal': 'GNOME Terminal',
     'urxvt': 'urxvt',
     'kitty': 'kitty',
     'nvim': 'Neovim Terminal',
     'NeoVimServer': 'VimR Terminal',
 }
 
+ENVIRONMENT = os.environ.copy()
+ENVIRONMENT["LANG"] = "C" # Standardize subprocess calls to English.
+
 def os_release() -> dict:
     with open('/etc/os-release') as f:
         return dict(line.replace('"', '').split('=', 1)
                     for line in f.read().splitlines())
 
 
 def distro():
     return f"{os_release()['PRETTY_NAME']}"
 
 
 def uptime():
-    cmd = subprocess.run(['uptime', '--pretty'], capture_output=True)
-    return cmd.stdout.decode('ascii')[3:-1]
+    try:
+        cmd = subprocess.run(['uptime', '--pretty'], capture_output=True, env=ENVIRONMENT, check=True)
+        return cmd.stdout.decode('ascii')[3:-1]
+    except (FileNotFoundError, subprocess.CalledProcessError):
+        with open('/proc/uptime') as f:
+            uptime = f.read()
+        seconds = int(uptime.split(".", 1)[0])
+        return str(datetime.timedelta(seconds=seconds))
 
 
 def count_pkgs():
     output = {}
     for manager, command in PKGS.items():
         try:
-            cmd = subprocess.run(command, capture_output=True)
+            cmd = subprocess.run(command, capture_output=True, env=ENVIRONMENT, check=True)
             output[manager] = cmd.stdout.decode('ascii').count('\n')
-        except FileNotFoundError:
+        except (FileNotFoundError, subprocess.CalledProcessError):
             pass
     return ', '.join(f"{count} ({manager})"
                      for manager, count in output.items())
 
 
 def shell():
     return os.environ['SHELL'].split('/')[-1]
@@ -166,15 +178,15 @@
         buffers = meminfo['Buffers']
         used = total_used - (cache + buffers)
 
         return f"{int(used/1000)}MB / {int(total/1000)}MB"
 
 
 def gpu():
-    cmd = subprocess.run(['lspci'], capture_output=True)
+    cmd = subprocess.run(['lspci'], capture_output=True, env=ENVIRONMENT)
     stdout = cmd.stdout.decode('ascii')
 
     for line in stdout.splitlines():
         if 'VGA' in line:
             if '[' in line:
                 return line[line.rfind('[') + 1:line.rfind(']')]
             else:
```

### Comparing `hent-1.0.3/hent.egg-info/PKG-INFO` & `hent-1.0.5/hent.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 Metadata-Version: 2.1
 Name: hent
-Version: 1.0.3
+Version: 1.0.5
 Summary: A neofetch alternative written in python.
-Home-page: https://gitlab.com/imsofi/hent/
-Author: imSofi
-Author-email: 6748208-imsofi@users.noreply.gitlab.com
+Home-page: https://github.com/imsofi/hent
+Author: Sofi
+Author-email: sofi+hent@mailbox.org
 License: MIT
-Description: # Hent
-        
-        Neofetch alternative built in python
-        
-        ## Usage:
-        ```
-        $ ./hent.py
-                 ..             Distro: Arch Linux
-                 cc             Kernel: 5.10.16-zen1-1-zen
-                :ooc            Uptime: 3 hours, 45 minutes
-               ::lool         Packages: 1864 (pacman), 38 (flatpak)
-             .looooool.          Shell: bash
-            .loo;..;ooo.      Terminal: kitty
-           'oooo    looc.          CPU: Intel i7-4790K @ 4.00GHz
-          ;l;'..     .';l;         GPU: GeForce RTX 2060 Rev. A
-         ..              .'     Memory: 6325MB / 24562MB
-        ```
-        ```
-        $ ./hent.py --help
-        usage: hent.py [-h] [--distro distro] [--color true/false]
-        
-        Neofetch inspired fetch tool built in python.
-        
-        optional arguments:
-          -h, --help          show this help message and exit
-          --distro distro     which ascii art to use
-          --color true/false  enable/disable colored output
-        ```
-        
-        ## Installation:
-        
-        ### With pip:
-        ```
-        pip3 install hent
-        ```
-        
-        ### With git:
-        ```
-        git clone https://gitlab.com/imsofi/hent
-        cd hent
-        pip3 install --upgrade build
-        python3 -m build
-        pip3 install dist/*.whl
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hent
+
+Neofetch alternative built in python
+
+## Usage:
+```
+$ hent
+         ..             Distro: Arch Linux
+         cc             Kernel: 5.10.16-zen1-1-zen
+        :ooc            Uptime: 3 hours, 45 minutes
+       ::lool         Packages: 1864 (pacman), 38 (flatpak)
+     .looooool.          Shell: bash
+    .loo;..;ooo.      Terminal: kitty
+   'oooo    looc.          CPU: Intel i7-4790K @ 4.00GHz
+  ;l;'..     .';l;         GPU: GeForce RTX 2060 Rev. A
+ ..              .'     Memory: 6325MB / 24562MB
+```
+```
+$ hent --help
+usage: hent [-h] [--distro distro] [--color true/false]
+
+Neofetch inspired fetch tool built in python.
+
+optional arguments:
+  -h, --help          show this help message and exit
+  --distro distro     which ascii art to use
+  --color true/false  enable/disable colored output
+```
+
+## Installation:
+
+### With pip:
+```
+pip3 install hent
+```
+
+### With git:
+```
+git clone https://github.com/imsofi/hent.git
+cd hent
+pip3 install --upgrade build
+python3 -m build
+pip3 install dist/*.whl
+```
+
+## Development
+
+```
+python3 -m venv .venv
+source .venv/bin/activate
+pip3 install -r requirements.txt
+```
```

