# Comparing `tmp/dorkbot-0.4.1.tar.gz` & `tmp/dorkbot-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorkbot-0.4.1.tar", last modified: Wed May 10 01:00:13 2023, max compression
+gzip compressed data, was "dorkbot-0.4.2.tar", last modified: Tue May 16 22:15:03 2023, max compression
```

## Comparing `dorkbot-0.4.1.tar` & `dorkbot-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.088159 dorkbot-0.4.1/
--rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.1/LICENSE
--rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.1/MANIFEST.in
--rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 01:00:13.088254 dorkbot-0.4.1/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)    10604 2023-05-10 00:18:30.000000 dorkbot-0.4.1/README.md
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.041996 dorkbot-0.4.1/dorkbot/
--rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.1/dorkbot/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)       22 2023-05-10 00:59:53.000000 dorkbot-0.4.1/dorkbot/_version.py
--rwxr-xr-x   0 jgor       (501) staff       (20)    32189 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/dorkbot.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.074958 dorkbot-0.4.1/dorkbot/indexers/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.1/dorkbot/indexers/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/bing_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     6022 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/commoncrawl.py
--rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.1/dorkbot/indexers/google.js
--rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/google.py
--rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/google_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     6285 2023-05-10 00:57:38.000000 dorkbot-0.4.1/dorkbot/indexers/pywb.py
--rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/stdin.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     4674 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/wayback.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.087746 dorkbot-0.4.1/dorkbot/scanners/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.1/dorkbot/scanners/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/scanners/arachni.py
--rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/scanners/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/scanners/wapiti.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.044706 dorkbot-0.4.1/dorkbot.egg-info/
--rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)      659 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/SOURCES.txt
--rw-r--r--   0 jgor       (501) staff       (20)        1 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/dependency_links.txt
--rw-r--r--   0 jgor       (501) staff       (20)       49 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/entry_points.txt
--rw-r--r--   0 jgor       (501) staff       (20)        8 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/top_level.txt
--rw-r--r--   0 jgor       (501) staff       (20)       74 2023-05-10 01:00:13.089142 dorkbot-0.4.1/setup.cfg
--rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.1/setup.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-16 22:15:03.906884 dorkbot-0.4.2/
+-rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.2/LICENSE
+-rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.2/MANIFEST.in
+-rw-r--r--   0 jgor       (501) staff       (20)    11141 2023-05-16 22:15:03.906978 dorkbot-0.4.2/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)    10739 2023-05-16 22:13:05.000000 dorkbot-0.4.2/README.md
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-16 22:15:03.871940 dorkbot-0.4.2/dorkbot/
+-rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.2/dorkbot/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)       22 2023-05-16 22:14:52.000000 dorkbot-0.4.2/dorkbot/_version.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)    32623 2023-05-16 22:12:20.000000 dorkbot-0.4.2/dorkbot/dorkbot.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-16 22:15:03.898622 dorkbot-0.4.2/dorkbot/indexers/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.2/dorkbot/indexers/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/bing_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6022 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/commoncrawl.py
+-rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.2/dorkbot/indexers/google.js
+-rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/google.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/google_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6285 2023-05-15 18:09:22.000000 dorkbot-0.4.2/dorkbot/indexers/pywb.py
+-rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/stdin.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     4674 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/indexers/wayback.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-16 22:15:03.906498 dorkbot-0.4.2/dorkbot/scanners/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.2/dorkbot/scanners/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/scanners/arachni.py
+-rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/scanners/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-10 00:18:30.000000 dorkbot-0.4.2/dorkbot/scanners/wapiti.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-16 22:15:03.874047 dorkbot-0.4.2/dorkbot.egg-info/
+-rw-r--r--   0 jgor       (501) staff       (20)    11141 2023-05-16 22:15:03.000000 dorkbot-0.4.2/dorkbot.egg-info/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)      659 2023-05-16 22:15:03.000000 dorkbot-0.4.2/dorkbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        1 2023-05-16 22:15:03.000000 dorkbot-0.4.2/dorkbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       49 2023-05-16 22:15:03.000000 dorkbot-0.4.2/dorkbot.egg-info/entry_points.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        8 2023-05-16 22:15:03.000000 dorkbot-0.4.2/dorkbot.egg-info/top_level.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       74 2023-05-16 22:15:03.907765 dorkbot-0.4.2/setup.cfg
+-rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.2/setup.py
```

### Comparing `dorkbot-0.4.1/LICENSE` & `dorkbot-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/PKG-INFO` & `dorkbot-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -47,17 +47,17 @@
 <pre>
 usage: dorkbot.py [-c CONFIG] [-r DIRECTORY] [--source [SOURCE]]
                   [--show-defaults] [--count COUNT] [--random] [-h]
                   [--log LOG] [-v] [-V] [-d DATABASE] [-u] [-l]
                   [--list-unscanned] [--add-target TARGET]
                   [--delete-target TARGET] [--flush-targets] [-i INDEXER]
                   [-o INDEXER_ARG] [-s SCANNER] [-p SCANNER_ARG] [-f]
-                  [-b BLOCKLIST] [--list-blocklist]
-                  [--add-blocklist-item ITEM] [--delete-blocklist-item ITEM]
-                  [--flush-blocklist]
+                  [--list-blocklist] [--add-blocklist-item ITEM]
+                  [--delete-blocklist-item ITEM] [--flush-blocklist]
+                  [-b EXTERNAL_BLOCKLIST]
 
 options:
   -c CONFIG, --config CONFIG
                         Configuration file
   -r DIRECTORY, --directory DIRECTORY
                         Dorkbot directory (default location of db, tools,
                         reports)
@@ -100,22 +100,23 @@
                         multiple times)
 
 fingerprints:
   -f, --flush-fingerprints
                         Delete all fingerprints of previously-scanned items
 
 blocklist:
-  -b BLOCKLIST, --blocklist BLOCKLIST
-                        Blocklist file/uri
-  --list-blocklist      List blocklist entries
+  --list-blocklist      List internal blocklist entries
   --add-blocklist-item ITEM
-                        Add an ip/host/regex pattern to the blocklist
+                        Add an ip/host/regex pattern to the internal blocklist
   --delete-blocklist-item ITEM
-                        Delete an item from the blocklist
-  --flush-blocklist     Delete all blocklist items
+                        Delete an item from the internal blocklist
+  --flush-blocklist     Delete all internal blocklist items
+  -b EXTERNAL_BLOCKLIST, --external-blocklist EXTERNAL_BLOCKLIST
+                        Supplemental external blocklist file/db (can be used
+                        multiple times)
 </pre>
 
 Tools / Dependencies
 =====
 * [psycopg2-binary](https://pypi.org/project/psycopg2-binary/) or [psycopg2](https://pypi.org/project/psycopg2/) (if using PostgreSQL)
 * [phoenixdb](https://pypi.org/project/phoenixdb/) (if using PhoenixDB)
 * [PhantomJS](http://phantomjs.org/) (if using non-api google indexer)
@@ -153,15 +154,15 @@
 [scanners.arachni]
 arachni_dir=/opt/arachni
 report_dir=/tmp/reports
 </pre>
 
 Blocklist
 =========
-The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blocklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blocklist. Note: --add-blocklist-item / --delete-blocklist-item are not implemented for file-based blocklists, and --flush-blocklist deletes the file.
+The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. The internal blocklist is maintained in the dorkbot database, but a separate file or databasecan be specified by passing the appropriate file path or connection uri to --external-blocklist. Targets are matched first against the internal blocklist and then optionally against any provided external blocklists.
 
 Supported external blocklists:
 * postgresql://[server info]
 * phoenixdb://[server info]
 * sqlite3:///path/to/blocklist.db
 * /path/to/blocklist.txt
```

### Comparing `dorkbot-0.4.1/README.md` & `dorkbot-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 <pre>
 usage: dorkbot.py [-c CONFIG] [-r DIRECTORY] [--source [SOURCE]]
                   [--show-defaults] [--count COUNT] [--random] [-h]
                   [--log LOG] [-v] [-V] [-d DATABASE] [-u] [-l]
                   [--list-unscanned] [--add-target TARGET]
                   [--delete-target TARGET] [--flush-targets] [-i INDEXER]
                   [-o INDEXER_ARG] [-s SCANNER] [-p SCANNER_ARG] [-f]
-                  [-b BLOCKLIST] [--list-blocklist]
-                  [--add-blocklist-item ITEM] [--delete-blocklist-item ITEM]
-                  [--flush-blocklist]
+                  [--list-blocklist] [--add-blocklist-item ITEM]
+                  [--delete-blocklist-item ITEM] [--flush-blocklist]
+                  [-b EXTERNAL_BLOCKLIST]
 
 options:
   -c CONFIG, --config CONFIG
                         Configuration file
   -r DIRECTORY, --directory DIRECTORY
                         Dorkbot directory (default location of db, tools,
                         reports)
@@ -87,22 +87,23 @@
                         multiple times)
 
 fingerprints:
   -f, --flush-fingerprints
                         Delete all fingerprints of previously-scanned items
 
 blocklist:
-  -b BLOCKLIST, --blocklist BLOCKLIST
-                        Blocklist file/uri
-  --list-blocklist      List blocklist entries
+  --list-blocklist      List internal blocklist entries
   --add-blocklist-item ITEM
-                        Add an ip/host/regex pattern to the blocklist
+                        Add an ip/host/regex pattern to the internal blocklist
   --delete-blocklist-item ITEM
-                        Delete an item from the blocklist
-  --flush-blocklist     Delete all blocklist items
+                        Delete an item from the internal blocklist
+  --flush-blocklist     Delete all internal blocklist items
+  -b EXTERNAL_BLOCKLIST, --external-blocklist EXTERNAL_BLOCKLIST
+                        Supplemental external blocklist file/db (can be used
+                        multiple times)
 </pre>
 
 Tools / Dependencies
 =====
 * [psycopg2-binary](https://pypi.org/project/psycopg2-binary/) or [psycopg2](https://pypi.org/project/psycopg2/) (if using PostgreSQL)
 * [phoenixdb](https://pypi.org/project/phoenixdb/) (if using PhoenixDB)
 * [PhantomJS](http://phantomjs.org/) (if using non-api google indexer)
@@ -140,15 +141,15 @@
 [scanners.arachni]
 arachni_dir=/opt/arachni
 report_dir=/tmp/reports
 </pre>
 
 Blocklist
 =========
-The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blocklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blocklist. Note: --add-blocklist-item / --delete-blocklist-item are not implemented for file-based blocklists, and --flush-blocklist deletes the file.
+The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. The internal blocklist is maintained in the dorkbot database, but a separate file or databasecan be specified by passing the appropriate file path or connection uri to --external-blocklist. Targets are matched first against the internal blocklist and then optionally against any provided external blocklists.
 
 Supported external blocklists:
 * postgresql://[server info]
 * phoenixdb://[server info]
 * sqlite3:///path/to/blocklist.db
 * /path/to/blocklist.txt
```

### Comparing `dorkbot-0.4.1/dorkbot/dorkbot.py` & `dorkbot-0.4.2/dorkbot/dorkbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,26 @@
             or args.list_targets or args.flush_targets \
             or args.add_target or args.delete_target \
             or args.list_blocklist or args.flush_blocklist \
             or args.add_blocklist_item or args.delete_blocklist_item \
             or args.flush_fingerprints or args.list_unscanned:
 
         db = TargetDatabase(args.database)
-        if args.blocklist:
-            blocklist = Blocklist(args.blocklist)
+
+        pattern = "^[^:]+://.*$"
+        regex = re.compile(pattern)
+        if (regex.match(args.database)):
+            blocklist = Blocklist(args.database)
         else:
-            pattern = "^[^:]+://.*$"
-            regex = re.compile(pattern)
-            if (regex.match(args.database)):
-                blocklist = Blocklist(args.database)
-            else:
-                blocklist = Blocklist("sqlite3://" + args.database)
+            blocklist = Blocklist("sqlite3://" + args.database)
+
+        blocklists = [blocklist]
+        if args.external_blocklist:
+            for external_blocklist in args.external_blocklist:
+                blocklists.append(Blocklist(external_blocklist))
 
         if args.flush_blocklist: blocklist.flush()
         if args.add_blocklist_item: blocklist.add(args.add_blocklist_item)
         if args.delete_blocklist_item: blocklist.delete(args.delete_blocklist_item)
         if args.list_blocklist:
             for item in blocklist.get_parsed_items(): print(item)
 
@@ -78,27 +81,27 @@
         db.close()
 
         if args.indexer:
             indexer_module = load_module("indexers", args.indexer)
             indexer_parser, other_args = get_module_parser(indexer_module)
             indexer_args = indexer_parser.parse_args(format_module_args(args.indexer_arg))
             try:
-                index(db, blocklist, indexer_module, args, indexer_args)
+                index(db, blocklists, indexer_module, args, indexer_args)
             except KeyboardInterrupt:
                 sys.exit(1)
 
         if args.prune:
-            prune(db, blocklist, args)
+            prune(db, blocklists, args)
 
         if args.scanner:
             scanner_module = load_module("scanners", args.scanner)
             scanner_parser, other_args = get_module_parser(scanner_module)
             scanner_args = scanner_parser.parse_args(format_module_args(args.scanner_arg))
             try:
-                scan(db, blocklist, scanner_module, args, scanner_args)
+                scan(db, blocklists, scanner_module, args, scanner_args)
             except KeyboardInterrupt:
                 sys.exit(1)
 
         db = TargetDatabase(args.database)
         if args.list_targets or args.list_unscanned:
             try:
                 urls = db.get_urls(unscanned_only=args.list_unscanned, source=args.source, randomize=args.random)
@@ -244,24 +247,24 @@
                           help="Pass an argument to the scanner module (can be used multiple times)")
 
     fingerprints = parser.add_argument_group('fingerprints')
     fingerprints.add_argument("-f", "--flush-fingerprints", action="store_true", \
                               help="Delete all fingerprints of previously-scanned items")
 
     blocklist = parser.add_argument_group('blocklist')
-    blocklist.add_argument("-b", "--blocklist", \
-                           help="Blocklist file/uri")
     blocklist.add_argument("--list-blocklist", action="store_true", \
-                           help="List blocklist entries")
+                           help="List internal blocklist entries")
     blocklist.add_argument("--add-blocklist-item", metavar="ITEM", \
-                           help="Add an ip/host/regex pattern to the blocklist")
+                           help="Add an ip/host/regex pattern to the internal blocklist")
     blocklist.add_argument("--delete-blocklist-item", metavar="ITEM", \
-                           help="Delete an item from the blocklist")
+                           help="Delete an item from the internal blocklist")
     blocklist.add_argument("--flush-blocklist", action="store_true", \
-                           help="Delete all blocklist items")
+                           help="Delete all internal blocklist items")
+    blocklist.add_argument("-b", "--external-blocklist", action="append", \
+                           help="Supplemental external blocklist file/db (can be used multiple times)")
 
     args = parser.parse_args(other_args, namespace=initial_args)
     return args, parser
 
 
 def get_module_parser(module, parent_parser=None):
     initial_args, other_args, initial_parser = get_initial_args_parser()
@@ -317,57 +320,60 @@
                 args.add(arg)
             else:
                 args.append("--" + arg)
 
     return args
 
 
-def index(db, blocklist, indexer, args, indexer_args):
+def index(db, blocklists, indexer, args, indexer_args):
     indexer_name = indexer.__name__.split(".")[-1]
     logging.info("Indexing: %s %s", indexer_name, vars(indexer_args))
     setattr(indexer_args, "directory", args.directory)
     urls, module_source = indexer.run(indexer_args)
     if args.source:
         source = args.source
     else:
         source = module_source
 
     targets = []
     for url in urls:
-        if not blocklist.match(Target(url)): targets.append(url)
+            if True in [blocklist.match(Target(url)) for blocklist in blocklists]:
+                logging.debug("Ignoring (matches blocklist pattern): %s", url)
+                continue
+            targets.append(url)
 
     db.connect()
     db.add_targets(targets, source)
     db.close()
 
 
-def prune(db, blocklist, args):
+def prune(db, blocklists, args):
     logging.info("Pruning database")
 
     db.connect()
-    db.prune(blocklist, args.random)
+    db.prune(blocklists, args.random)
     db.close()
 
 
-def scan(db, blocklist, scanner, args, scanner_args):
+def scan(db, blocklists, scanner, args, scanner_args):
     if not os.path.isdir(scanner_args.report_dir):
         try:
             os.makedirs(scanner_args.report_dir)
         except OSError as e:
             logging.error("Failed to create report directory - %s", str(e))
             sys.exit(1)
 
     scanned = 0
     while scanned < args.count or args.count == -1:
         db.connect()
         target = db.get_next_target(random=args.random)
         if not target:
             break
 
-        if blocklist.match(target):
+        if True in [blocklist.match(target) for blocklist in blocklists]:
             logging.debug("Deleting (matches blocklist pattern): %s", target.url)
             db.delete_target(target.url)
             continue
 
         db.close()
 
         logging.info("Scanning: %s", target.url)
@@ -598,15 +604,15 @@
         try:
             with self.db, closing(self.db.cursor()) as c:
                 c.execute("DELETE FROM targets")
         except self.module.Error as e:
             logging.error("Failed to flush targets - %s", str(e))
             sys.exit(1)
 
-    def prune(self, blocklist, randomize=False):
+    def prune(self, blocklists, randomize=False):
         fingerprints = set()
 
         urls = self.get_urls()
 
         if randomize:
             random.shuffle(urls)
 
@@ -616,15 +622,15 @@
             fingerprint = generate_fingerprint(target)
             with self.db, closing(self.db.cursor()) as c:
                 if fingerprint in fingerprints or self.get_scanned(fingerprint, c):
                     logging.debug("Marking scanned (matches fingerprint of another target): %s", target.url)
                     self.mark_scanned(target.url, c)
                     continue
 
-            if blocklist.match(target):
+            if True in [blocklist.match(target) for blocklist in blocklists]:
                 logging.debug("Deleting (matches blocklist pattern): %s", target.url)
                 self.delete_target(target.url)
                 continue
 
             fingerprints.add(fingerprint)
```

### Comparing `dorkbot-0.4.1/dorkbot/indexers/bing_api.py` & `dorkbot-0.4.2/dorkbot/indexers/bing_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/commoncrawl.py` & `dorkbot-0.4.2/dorkbot/indexers/commoncrawl.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/google.js` & `dorkbot-0.4.2/dorkbot/indexers/google.js`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/google.py` & `dorkbot-0.4.2/dorkbot/indexers/google.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/google_api.py` & `dorkbot-0.4.2/dorkbot/indexers/google_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/pywb.py` & `dorkbot-0.4.2/dorkbot/indexers/pywb.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/stdin.py` & `dorkbot-0.4.2/dorkbot/indexers/stdin.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/indexers/wayback.py` & `dorkbot-0.4.2/dorkbot/indexers/wayback.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/scanners/arachni.py` & `dorkbot-0.4.2/dorkbot/scanners/arachni.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/scanners/example.py` & `dorkbot-0.4.2/dorkbot/scanners/example.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot/scanners/wapiti.py` & `dorkbot-0.4.2/dorkbot/scanners/wapiti.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/dorkbot.egg-info/PKG-INFO` & `dorkbot-0.4.2/dorkbot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -47,17 +47,17 @@
 <pre>
 usage: dorkbot.py [-c CONFIG] [-r DIRECTORY] [--source [SOURCE]]
                   [--show-defaults] [--count COUNT] [--random] [-h]
                   [--log LOG] [-v] [-V] [-d DATABASE] [-u] [-l]
                   [--list-unscanned] [--add-target TARGET]
                   [--delete-target TARGET] [--flush-targets] [-i INDEXER]
                   [-o INDEXER_ARG] [-s SCANNER] [-p SCANNER_ARG] [-f]
-                  [-b BLOCKLIST] [--list-blocklist]
-                  [--add-blocklist-item ITEM] [--delete-blocklist-item ITEM]
-                  [--flush-blocklist]
+                  [--list-blocklist] [--add-blocklist-item ITEM]
+                  [--delete-blocklist-item ITEM] [--flush-blocklist]
+                  [-b EXTERNAL_BLOCKLIST]
 
 options:
   -c CONFIG, --config CONFIG
                         Configuration file
   -r DIRECTORY, --directory DIRECTORY
                         Dorkbot directory (default location of db, tools,
                         reports)
@@ -100,22 +100,23 @@
                         multiple times)
 
 fingerprints:
   -f, --flush-fingerprints
                         Delete all fingerprints of previously-scanned items
 
 blocklist:
-  -b BLOCKLIST, --blocklist BLOCKLIST
-                        Blocklist file/uri
-  --list-blocklist      List blocklist entries
+  --list-blocklist      List internal blocklist entries
   --add-blocklist-item ITEM
-                        Add an ip/host/regex pattern to the blocklist
+                        Add an ip/host/regex pattern to the internal blocklist
   --delete-blocklist-item ITEM
-                        Delete an item from the blocklist
-  --flush-blocklist     Delete all blocklist items
+                        Delete an item from the internal blocklist
+  --flush-blocklist     Delete all internal blocklist items
+  -b EXTERNAL_BLOCKLIST, --external-blocklist EXTERNAL_BLOCKLIST
+                        Supplemental external blocklist file/db (can be used
+                        multiple times)
 </pre>
 
 Tools / Dependencies
 =====
 * [psycopg2-binary](https://pypi.org/project/psycopg2-binary/) or [psycopg2](https://pypi.org/project/psycopg2/) (if using PostgreSQL)
 * [phoenixdb](https://pypi.org/project/phoenixdb/) (if using PhoenixDB)
 * [PhantomJS](http://phantomjs.org/) (if using non-api google indexer)
@@ -153,15 +154,15 @@
 [scanners.arachni]
 arachni_dir=/opt/arachni
 report_dir=/tmp/reports
 </pre>
 
 Blocklist
 =========
-The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blocklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blocklist. Note: --add-blocklist-item / --delete-blocklist-item are not implemented for file-based blocklists, and --flush-blocklist deletes the file.
+The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. The internal blocklist is maintained in the dorkbot database, but a separate file or databasecan be specified by passing the appropriate file path or connection uri to --external-blocklist. Targets are matched first against the internal blocklist and then optionally against any provided external blocklists.
 
 Supported external blocklists:
 * postgresql://[server info]
 * phoenixdb://[server info]
 * sqlite3:///path/to/blocklist.db
 * /path/to/blocklist.txt
```

### Comparing `dorkbot-0.4.1/dorkbot.egg-info/SOURCES.txt` & `dorkbot-0.4.2/dorkbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.1/setup.py` & `dorkbot-0.4.2/setup.py`

 * *Files identical despite different names*

