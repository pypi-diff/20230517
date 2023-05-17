# Comparing `tmp/vagd-0.3.6.tar.gz` & `tmp/vagd-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-0.3.6.tar", last modified: Sat Apr 15 12:44:21 2023, max compression
+gzip compressed data, was "vagd-0.3.8.tar", last modified: Wed May 17 09:43:09 2023, max compression
```

## Comparing `vagd-0.3.6.tar` & `vagd-0.3.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.328289 vagd-0.3.6/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.3.6/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-04-15 12:44:21.328289 vagd-0.3.6/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2282 2023-03-21 08:25:45.000000 vagd-0.3.6/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-04-15 12:01:40.000000 vagd-0.3.6/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-04-15 12:44:21.328289 vagd-0.3.6/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.324956 vagd-0.3.6/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.324956 vagd-0.3.6/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.3.6/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.3.6/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      900 2023-04-15 11:40:48.000000 vagd-0.3.6/src/vagd/box.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.324956 vagd-0.3.6/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.3.6/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.3.6/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.3.6/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.3.6/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.3.6/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.3.6/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.3.6/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.3.6/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.3.6/src/vagd/helper.py
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      753 2023-03-20 15:06:29.000000 vagd-0.3.6/src/vagd/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      734 2023-03-20 14:52:11.000000 vagd-0.3.6/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.328289 vagd-0.3.6/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.3.6/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4202 2023-03-21 09:12:24.000000 vagd-0.3.6/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10093 2023-03-21 08:36:32.000000 vagd-0.3.6/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10084 2023-04-15 12:42:53.000000 vagd-0.3.6/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.3.6/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.3.6/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.3.6/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.324956 vagd-0.3.6/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-04-15 12:44:21.000000 vagd-0.3.6/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-04-15 12:44:21.000000 vagd-0.3.6/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-04-15 12:44:21.000000 vagd-0.3.6/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-04-15 12:44:21.000000 vagd-0.3.6/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-04-15 12:44:21.000000 vagd-0.3.6/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-04-15 12:44:21.328289 vagd-0.3.6/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.3.6/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.3.8/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-17 09:43:09.142420 vagd-0.3.8/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2282 2023-03-21 08:25:45.000000 vagd-0.3.8/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-05-17 09:40:53.000000 vagd-0.3.8/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-05-17 09:43:09.142420 vagd-0.3.8/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.135753 vagd-0.3.8/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.139087 vagd-0.3.8/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.3.8/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      900 2023-04-15 11:40:48.000000 vagd-0.3.8/src/vagd/box.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.3.8/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.3.8/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.3.8/src/vagd/helper.py
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      753 2023-03-20 15:06:29.000000 vagd-0.3.8/src/vagd/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      734 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4202 2023-03-21 09:12:24.000000 vagd-0.3.8/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10244 2023-05-17 09:35:51.000000 vagd-0.3.8/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10853 2023-04-15 14:11:22.000000 vagd-0.3.8/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.3.8/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.139087 vagd-0.3.8/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.3.8/test/test.py
```

### Comparing `vagd-0.3.6/LICENSE` & `vagd-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/PKG-INFO` & `vagd-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.3.6
+Version: 0.3.8
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vagd-0.3.6/README.md` & `vagd-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/pyproject.toml` & `vagd-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vagd"
-version = "0.3.6"
+version = "0.3.8"
 authors = [
   { name="0x6fe1be2", email="author@example.com" },
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['pwntools', 'python-vagrant', 'docker']
```

### Comparing `vagd-0.3.6/src/vagd/box.py` & `vagd-0.3.8/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/gdb/__init__.pyi` & `vagd-0.3.8/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/gdb/events.pyi` & `vagd-0.3.8/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/gdb/printing.pyi` & `vagd-0.3.8/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/gdb/types.pyi` & `vagd-0.3.8/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/gdb/xmethod.pyi` & `vagd-0.3.8/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/helper.py` & `vagd-0.3.8/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/template.txt` & `vagd-0.3.8/src/vagd/template.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/templates.py` & `vagd-0.3.8/src/vagd/templates.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/virts/dogd.py` & `vagd-0.3.8/src/vagd/virts/dogd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/virts/pwngd.py` & `vagd-0.3.8/src/vagd/virts/pwngd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 import pwn
+import pathlib
 from shutil import which
 from abc import ABC, abstractmethod
 from typing import Union, Dict, Iterable
 
 
 class Pwngd(ABC):
     LOCAL_DIR = './.vagd/'
     HOME_DIR = os.path.expanduser('~/.vagd/')
     SYSROOT = LOCAL_DIR + 'sysroot/'
     SYSROOT_LIB = SYSROOT + 'lib/'
+    SYSROOT_LIB_DEBUG = SYSROOT + 'lib/debug'
     KEYFILE = LOCAL_DIR + 'keyfile'
     DEFAULT_PORT = 2222
 
     _path: str
     _binary: str
     _ssh: pwn.ssh
     _experimental: bool
@@ -49,20 +51,22 @@
         """
         mount remote dir on local wiith sshfs
         :param remote_dir: directory on remote to mount
         :param local_dir: local mount point
         """
         if not which('sshfs'):
             pwn.log.error('sshfs isn\'t installed')
-        os.system(Pwngd._SSHFS_TEMPLATE.format(port=self._ssh.port,
-                                               keyfile=self._ssh.keyfile,
+        cmd = Pwngd._SSHFS_TEMPLATE.format(port=self._ssh.port,
+                                               keyfile="$PWD/" + self._ssh.keyfile,
                                                user=self._ssh.user,
                                                host=self._ssh.host,
                                                remote_dir=remote_dir,
-                                               local_dir=local_dir))
+                                               local_dir=local_dir)
+        pwn.log.info(cmd)
+        os.system(cmd)
 
     def _mount_lib(self, remote_lib: str = '/usr/lib') -> None:
         """
         mount the lib directory of remote
         """
         if not (os.path.exists(Pwngd.SYSROOT) and os.path.exists(Pwngd.SYSROOT_LIB)):
             os.makedirs(Pwngd.SYSROOT_LIB)
@@ -207,18 +211,18 @@
 
         # Find what port we need to connect to
         port = pwn.gdb._gdbserver_port(gdbserver, ssh)
 
         host = '127.0.0.1'
 
         if self._fast:
-            gdb_args += ["-ex", f"set sysroot = ./sysroot"]
-            gdbscript = "set debug-file-directory ./sysroot/lib/debug\n" + gdbscript
+            gdb_args += ["-ex", f"set sysroot {pathlib.Path().resolve()}/{Pwngd.SYSROOT}"]
+            gdbscript = f"set debug-file-directory {Pwngd.SYSROOT_LIB_DEBUG}\n" + gdbscript
         elif sysroot:
-            gdb_args += ["-ex", f"set sysroot = {sysroot}"]
+            gdb_args += ["-ex", f"set sysroot {sysroot}"]
             gdbscript = f"set debug-file-directory ./{sysroot}/lib/debug\n" + gdbscript
         else:
             gdbscript = "set debug-file-directory /lib/debug\n" + gdbscript
 
         gdb_args += ["-ex", f"file -readnow {self._path}"]
 
         tmp = pwn.gdb.attach((host, port), exe=exe, gdbscript=gdbscript,
```

### Comparing `vagd-0.3.6/src/vagd/virts/qegd.py` & `vagd-0.3.8/src/vagd/virts/qegd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
+import sys
+
 import pwn
 import time
 import requests
+
+from typing import Dict
 from urllib.parse import urlparse
 from shutil import which, copyfile
 
 from vagd import helper
 from vagd.box import Box
 from vagd.virts.pwngd import Pwngd
 
@@ -59,14 +63,15 @@
 
     _img: str
     _new: bool = False
     _local_img: str
     _user: str
     _host: str
     _port: int
+    _ports: Dict[int, int]
     _qemu: str
     _cpu: str
     _machine: str
     _keyfile: str
 
     @staticmethod
     def _is_local(url) -> bool:
@@ -132,22 +137,24 @@
                 helper.generate_keypair()
                 with open(Qegd.USER_DATA_FILE, 'w') as user_data_file:
                     with open(Pwngd.KEYFILE + '.pub', 'r') as pubkey_file:
                         pubkey = pubkey_file.readline()
                     user_data_file.write(Qegd._USER_DATA.format(pubkey=pubkey))
             os.system(Qegd._GENERATE_SEED_IMG)
 
+    _QEMU_PORT_FORWARDING = ',hostfwd=tcp::{host}-:{guest}'
     _QEMU_START = "{qemu} " \
                   + "{machine} " \
                   + "{cpu} " \
                   + "-m 2G " \
                   + "-nographic " \
                   + "{pflash} " \
                   + "-device virtio-net-pci,netdev=net0 " \
-                  + "-netdev user,id=net0,hostfwd=tcp::{port}-:22 " \
+                  + "-netdev user,id=net0,hostfwd=tcp::{port}-:22" \
+                  + "{ports} " \
                   + "-drive if=virtio,format=qcow2,file={img} " \
                   + "-drive if=virtio,format=raw,file={seed} " \
                   + "{custom} " \
                   + "> /dev/null; " \
                   + "rm {lock} {current}"
 
     _QEMU_ARM_START = ""
@@ -160,25 +167,32 @@
         pwn.log.info(f"starting qemu machine, ssh port {self._port}")
         with open(Qegd.LOCKFILE, 'w') as lockfile:
             lockfile.write(str(self._port))
         pid = os.fork()
         if pid == 0:
             copyfile(Qegd.ARM_FLASH, Qegd.DEFAULT_QEMU_ARM_PFLASH)
             qemu_cmd = Qegd._QEMU_START.format(qemu=self._qemu,
-                                              machine=" ".join((Qegd.DEFAULT_QEMU_MACHINE_PREFIX, self._machine)) if self._machine else '',
-                                              cpu=" ".join((Qegd.DEFAULT_QEMU_CPU_PREFIX, self._cpu)) if self._cpu else '',
-                                              pflash=" ".join((Qegd.DEFAULT_QEMU_PFLASH_PREFIX, self._pflash)) if self._pflash else '',
-                                              port=self._port,
-                                              img=Qegd.CURRENT_IMG,
-                                              custom='',
-                                              seed=Qegd.SEED_FILE,
-                                              lock=Qegd.LOCKFILE,
-                                              current=Qegd.CURRENT_IMG)
+                                               machine=" ".join((Qegd.DEFAULT_QEMU_MACHINE_PREFIX,
+                                                                 self._machine)) if self._machine else '',
+                                               cpu=" ".join(
+                                                   (Qegd.DEFAULT_QEMU_CPU_PREFIX, self._cpu)) if self._cpu else '',
+                                               pflash=" ".join((Qegd.DEFAULT_QEMU_PFLASH_PREFIX,
+                                                                self._pflash)) if self._pflash else '',
+                                               port=self._port,
+                                               ports="".join(
+                                                   [Qegd._QEMU_PORT_FORWARDING.format(host=host, guest=guest) for
+                                                    host, guest in self._ports.items()]),
+                                               img=Qegd.CURRENT_IMG,
+                                               custom='',
+                                               seed=Qegd.SEED_FILE,
+                                               lock=Qegd.LOCKFILE,
+                                               current=Qegd.CURRENT_IMG)
             pwn.log.info(qemu_cmd)
             os.system(qemu_cmd)
+            sys.exit(0)
 
     def _new_vm(self) -> None:
         """
         create new vm
         """
         self._new = True
 
@@ -229,25 +243,27 @@
                     pwn.log.info('Trying again')
                 time.sleep(15)
 
     def __init__(self,
                  binary: str,
                  img: str = DEFAULT_IMG,
                  user: str = DEFAULT_USER,
+                 ports: Dict[int, int] = None,
                  arm: bool = False,
                  qemu: str = DEFAULT_QEMU_CMD,
                  machine: str = DEFAULT_QEMU_MACHINE,
                  cpu: str = DEFAULT_QEMU_CPU,
                  pflash: str = None,
                  **kwargs):
         """
 
         :param binary: binary for VM debugging
         :param img: qemu image to use (requires ssh)
         :param user: user inside qemu image
+        :param ports: forwarded ports
         :param arm: if qemu is arm
         :param qemu: qemu cmd
         :param cpu: value for :code -cpu
         :param machine: value for :code -machine
         :param pflash: value for :code -pflash
         :param kwargs: parameters to pass through to super
         """
@@ -255,22 +271,23 @@
         if not which('qemu-system-x86_64'):
             pwn.log.error('qemu-system-x86_64 isn\'t installed')
 
         if not os.path.exists(Qegd.QEMU_DIR):
             pwn.log.info(f"Generating {Qegd.QEMU_DIR} dir")
             os.makedirs(Qegd.QEMU_DIR)
 
-        if arm :
+        if arm:
             qemu = Qegd.DEFAULT_QEMU_ARM_CMD if qemu == Qegd.DEFAULT_QEMU_CMD else qemu
             cpu = Qegd.DEFAULT_QEMU_ARM_CPU if cpu == Qegd.DEFAULT_QEMU_CPU else cpu
             machine = Qegd.DEFAULT_QEMU_ARM_MACHINE if machine == Qegd.DEFAULT_QEMU_MACHINE else machine
             pflash = Qegd.DEFAULT_QEMU_ARM_PFLASH_OPTIONS + Qegd.DEFAULT_QEMU_ARM_PFLASH if pflash is None else pflash
 
         self._img = img
         self._user = user
+        self._ports = ports if ports else dict()
         self._arm = arm
         self._qemu = qemu
         self._cpu = cpu
         self._machine = machine
         self._pflash = pflash
 
         self._vm_setup()
```

### Comparing `vagd-0.3.6/src/vagd/virts/shgd.py` & `vagd-0.3.8/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/virts/vagd.py` & `vagd-0.3.8/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd/wrapper.py` & `vagd-0.3.8/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/src/vagd.egg-info/PKG-INFO` & `vagd-0.3.8/src/vagd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.3.6
+Version: 0.3.8
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vagd-0.3.6/src/vagd.egg-info/SOURCES.txt` & `vagd-0.3.8/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.3.6/test/test.py` & `vagd-0.3.8/test/test.py`

 * *Files identical despite different names*

