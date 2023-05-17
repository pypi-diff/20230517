# Comparing `tmp/xklb-1.28.1.tar.gz` & `tmp/xklb-1.28.2.tar.gz`

## Comparing `xklb-1.28.1.tar` & `xklb-1.28.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.1/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.1/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.1/Windows.md
--rw-r--r--   0        0        0   416100 2020-02-02 00:00:00.000000 xklb-1.28.1/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.1/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.1/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.1/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/__init__.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/books.py
--rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/consts.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/dl_extract.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/lb.py
--rw-r--r--   0        0        0    35902 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/playback.py
--rw-r--r--   0        0        0    30256 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/stats.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/tube_extract.py
--rw-r--r--   0        0        0    28492 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.1/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.28.1/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.1/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.1/LICENSE
--rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.1/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.28.1/pyproject.toml
--rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.1/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.2/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.2/Windows.md
+-rw-r--r--   0        0        0   416100 2020-02-02 00:00:00.000000 xklb-1.28.2/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.2/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/__init__.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/books.py
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/consts.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/lb.py
+-rw-r--r--   0        0        0    37573 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/playback.py
+-rw-r--r--   0        0        0    30250 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/stats.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28913 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.28.2/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.2/LICENSE
+-rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.2/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.28.2/pyproject.toml
+-rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.2/PKG-INFO
```

### Comparing `xklb-1.28.1/Windows.md` & `xklb-1.28.2/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/pdm.lock` & `xklb-1.28.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/readme.py` & `xklb-1.28.2/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.28.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.28.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/.github/workflows/push.yaml` & `xklb-1.28.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/sql/transfer.sql` & `xklb-1.28.2/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/av.py` & `xklb-1.28.2/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/books.py` & `xklb-1.28.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/consts.py` & `xklb-1.28.2/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/db.py` & `xklb-1.28.2/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/dl_config.py` & `xklb-1.28.2/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/dl_extract.py` & `xklb-1.28.2/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/fs_extract.py` & `xklb-1.28.2/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/gui.py` & `xklb-1.28.2/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/hn_extract.py` & `xklb-1.28.2/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/lb.py` & `xklb-1.28.2/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/play_actions.py` & `xklb-1.28.2/xklb/play_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import argparse, shlex, shutil, sys, time
+from collections import deque
+from concurrent.futures import ThreadPoolExecutor
+from copy import deepcopy
 from pathlib import Path
 from random import random
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple
 
 from xklb import consts, db, player, subtitle, tube_backend, utils
 from xklb.consts import SC
 from xklb.playback import now_playing
 from xklb.player import get_ordinal_media, mark_media_deleted, override_sort
 from xklb.utils import cmd_interactive, log, random_filename, safe_unpack
 
@@ -303,16 +306,16 @@
         ),
         (args.sort, args.sort, args.sort),
         (args.action in (SC.listen, SC.watch) and args.include, "duration desc", "duration"),
         (args.action in (SC.listen, SC.watch) and args.include, "size desc", "size"),
         (args.action in (SC.listen, SC.watch) and "play_count" in m_columns, "play_count", "play_count desc"),
         (
             args.action in (SC.listen, SC.watch) and "size" in m_columns and "duration" in m_columns,
-            "ntile(1000) over (order by size) desc, duration",
-            "ntile(1000) over (order by size), duration desc",
+            "size desc, duration",
+            "size, duration desc",
         ),
         (args.action == SC.filesystem, "sparseness", "sparseness desc"),
         (args.action == SC.filesystem, "size", "size desc"),
         (True, "m.path", "m.path desc"),
         (True, "random", "random"),
     ]
 
@@ -700,36 +703,56 @@
         "2",
         "-b:a",
         "128k",
         "-filter:a",
         "loudnorm=i=-18:lra=17",
         temp_video,
     )
+
     Path(path).unlink()
     shutil.move(temp_video, transcode_dest)
+    with args.db.conn:
+        args.db.conn.execute("UPDATE media SET path = ? where path = ?", [transcode_dest, path])
     return transcode_dest
 
 
-def play(args, m: Dict) -> None:
-    original_path = m["path"]
+def prep_media(args, m: Dict):
+    t = utils.Timer()
+    if is_play_in_order_lvl2(args, m["path"]):
+        m = player.get_ordinal_media(args, m)
+        log.debug("player.get_ordinal_media: %s", t.elapsed())
+
+    m["original_path"] = m["path"]
     if args.action in (SC.watch, SC.listen) and not m["path"].startswith("http"):
         media_path = Path(args.prefix + m["path"]).resolve() if args.prefix else Path(m["path"])
         m["path"] = str(media_path)
 
         if not media_path.exists():
+            log.debug("media_path exists: %s", t.elapsed())
             log.warning("[%s]: Does not exist. Skipping...", m["path"])
-            mark_media_deleted(args, original_path)
-            return
+            mark_media_deleted(args, m["original_path"])
+            log.debug("mark_media_deleted: %s", t.elapsed())
+            return None
 
         if args.transcode or args.transcode_audio:
             m["path"] = transcode(args, m["path"])
+            log.debug("transcode: %s", t.elapsed())
+
+    m["now_playing"] = now_playing(m["path"])
 
-    print(now_playing(m["path"]))
+    return m
+
+
+def play(args, m) -> None:
+    t = utils.Timer()
+    print(m["now_playing"])
+    log.debug("now_playing: %s", t.elapsed())
 
     args.player = player.parse(args, m)
+    log.debug("player.parse: %s", t.elapsed())
 
     start_time = time.time()
     if args.chromecast:
         try:
             chromecast_play(args, m)
         except Exception:
             if args.ignore_errors:
@@ -750,26 +773,31 @@
             else:
                 raise SystemExit(r.returncode)
 
     m_columns = args.db["media"].columns_dict
     if "playhead" in m_columns:
         playhead = utils.get_playhead(
             args,
-            original_path,
+            m["original_path"],
             start_time,
             existing_playhead=m.get("playhead"),
             media_duration=m.get("duration"),
         )
         if playhead:
-            player.set_playhead(args, original_path, playhead)
-    player.post_act(args, original_path)
+            player.set_playhead(args, m["original_path"], playhead)
+
+    t.reset()
+    player.post_act(args, m["original_path"])
+    log.debug("player.post_act: %s", t.elapsed())
 
 
 def process_playqueue(args) -> None:
+    t = utils.Timer()
     query, bindings = construct_query(args)
+    log.debug("construct_query: %s", t.elapsed())
 
     if args.print and not any(
         [
             args.partial,
             args.lower,
             args.upper,
             args.safe,
@@ -777,20 +805,23 @@
             args.related >= consts.RELATED,
         ]
     ):
         player.printer(args, query, bindings)
         return
 
     media = list(args.db.query(query, bindings))
+    log.debug("query: %s", t.elapsed())
 
     if args.partial and Path(args.watch_later_directory).exists():
         media = utils.mpv_enrich2(args, media)
+        log.debug("utils.mpv_enrich2: %s", t.elapsed())
 
     if args.lower is not None or args.upper is not None:
         media = utils.filter_episodic(args, media)
+        log.debug("utils.filter_episodic: %s", t.elapsed())
 
     if not media:
         utils.no_media_found()
 
     if all(
         [
             Path(args.watch_later_directory).exists(),
@@ -798,35 +829,48 @@
             args.related == 0,
             "sort" in args.defaults,
             not args.partial,
             not args.random,
         ],
     ):
         media = utils.mpv_enrich(args, media)
+        log.debug("utils.mpv_enrich: %s", t.elapsed())
 
     if args.safe:
         media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
+        log.debug("tube_backend.is_supported: %s", t.elapsed())
 
     if args.print:
         if args.related >= consts.RELATED:
             media = player.get_related_media(args, media[0])
         if args.play_in_order >= consts.SIMILAR:
             media = [player.get_ordinal_media(args, d) for d in media]
         player.media_printer(args, media)
     elif args.multiple_playback:
         args.gui = True
         player.multiple_player(args, media)
     else:
         if args.related >= consts.RELATED:
             media = player.get_related_media(args, media[0])
+            log.debug("player.get_related_media: %s", t.elapsed())
         try:
-            for m in media:
-                if is_play_in_order_lvl2(args, m["path"]):
-                    m = player.get_ordinal_media(args, m)
-                play(args, m)
+            media.reverse()  # because media.pop()
+            futures = deque()
+            with ThreadPoolExecutor(max_workers=1) as executor:
+                while media or futures:
+                    while media and len(futures) < 3:
+                        m = media.pop()
+                        future = executor.submit(prep_media, args, m)
+                        futures.append(future)
+
+                    if futures:
+                        future = futures.popleft()
+                        m = future.result()
+                        if m is not None:
+                            play(args, m)
         finally:
             if args.interdimensional_cable:
                 args.sock.send(b"raw quit \n")
             Path(args.mpv_socket).unlink(missing_ok=True)
             if args.chromecast:
                 Path(consts.CAST_NOW_PLAYING).unlink(missing_ok=True)
```

### Comparing `xklb-1.28.1/xklb/playback.py` & `xklb-1.28.2/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/player.py` & `xklb-1.28.2/xklb/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
 
 def multiple_player(args, media) -> None:
     args.player = parse(args, media[0])
 
     template = get_multiple_player_template(args)
     players = []
 
-    media.reverse()  # because I use media.pop()
+    media.reverse()  # because media.pop()
     try:
         while media or players:
             for t_idx, t in enumerate(template):
                 SINGLE_PLAYBACK = ("--fs", '--screen-name="eDP"', '--fs-screen-name="eDP"')
                 if len(t) == len(SINGLE_PLAYBACK):
                     player_hole = t
                     geom_data = None
```

### Comparing `xklb-1.28.1/xklb/praw_extract.py` & `xklb-1.28.2/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/stats.py` & `xklb-1.28.2/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/subtitle.py` & `xklb-1.28.2/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/tabs_actions.py` & `xklb-1.28.2/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/tabs_extract.py` & `xklb-1.28.2/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/tube_backend.py` & `xklb-1.28.2/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/tube_extract.py` & `xklb-1.28.2/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/utils.py` & `xklb-1.28.2/xklb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ast import literal_eval
 from collections.abc import Iterable
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
+from timeit import default_timer
 from typing import Any, Dict, Generator, List, NoReturn, Optional, Union
 
 import humanize
 from IPython.core import ultratb
 from IPython.terminal.debugger import TerminalPdb
 from rich import prompt
 from rich.logging import RichHandler
@@ -954,7 +955,23 @@
     except Exception:
         mpv_playhead = None
 
     for playhead in sorted([mpv_playhead or 0, python_playhead], reverse=True):
         if playhead > 0 and (media_duration is None or media_duration >= playhead):
             return playhead
     return None
+
+
+class Timer:
+    def __init__(self):
+        self.reset()
+
+    def reset(self):
+        self.start_time = default_timer()
+
+    def elapsed(self):
+        if not hasattr(self, "start_time"):
+            raise RuntimeError("Timer has not been started.")
+        end_time = default_timer()
+        elapsed_time = end_time - self.start_time
+        self.reset()
+        return elapsed_time
```

### Comparing `xklb-1.28.1/xklb/scripts/__init__.py` & `xklb-1.28.2/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/bigdirs.py` & `xklb-1.28.2/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/christen.py` & `xklb-1.28.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/copy_play_counts.py` & `xklb-1.28.2/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/dedupe.py` & `xklb-1.28.2/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/merge_dbs.py` & `xklb-1.28.2/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/merge_online_local.py` & `xklb-1.28.2/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/move_list.py` & `xklb-1.28.2/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/optimize_db.py` & `xklb-1.28.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/redownload.py` & `xklb-1.28.2/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/relmv.py` & `xklb-1.28.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/scatter.py` & `xklb-1.28.2/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/streaming_tab_loader.py` & `xklb-1.28.2/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/mining/data.py` & `xklb-1.28.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/mining/extract_links.py` & `xklb-1.28.2/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/mining/nouns.py` & `xklb-1.28.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/mining/pushshift.py` & `xklb-1.28.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.28.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/assets/kotobago.png` & `xklb-1.28.2/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/.gitignore` & `xklb-1.28.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/LICENSE` & `xklb-1.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/README.md` & `xklb-1.28.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.001)
+    xk media library subcommands (v1.28.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.28.1/pyproject.toml` & `xklb-1.28.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.1/PKG-INFO` & `xklb-1.28.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.28.1
+Version: 1.28.2
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.001)
+    xk media library subcommands (v1.28.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

