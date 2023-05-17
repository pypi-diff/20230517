# Comparing `tmp/xklb-1.28.4.tar.gz` & `tmp/xklb-1.28.5.tar.gz`

## Comparing `xklb-1.28.4.tar` & `xklb-1.28.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.4/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.4/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.4/Windows.md
--rw-r--r--   0        0        0   416122 2020-02-02 00:00:00.000000 xklb-1.28.4/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.4/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.4/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.4/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/__init__.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/books.py
--rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/consts.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/dl_extract.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/fs_extract.py
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/lb.py
--rw-r--r--   0        0        0    37757 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/playback.py
--rw-r--r--   0        0        0    30250 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/stats.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/tube_extract.py
--rw-r--r--   0        0        0    28913 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.28.4/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.4/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.4/LICENSE
--rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.4/README.md
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 xklb-1.28.4/pyproject.toml
--rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.4/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.5/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.5/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.5/Windows.md
+-rw-r--r--   0        0        0   416122 2020-02-02 00:00:00.000000 xklb-1.28.5/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.5/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.5/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/__init__.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/books.py
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/consts.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/lb.py
+-rw-r--r--   0        0        0    37757 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/playback.py
+-rw-r--r--   0        0        0    30250 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/stats.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28913 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.5/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.5/LICENSE
+-rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.5/README.md
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 xklb-1.28.5/pyproject.toml
+-rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.5/PKG-INFO
```

### Comparing `xklb-1.28.4/Windows.md` & `xklb-1.28.5/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/pdm.lock` & `xklb-1.28.5/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/readme.py` & `xklb-1.28.5/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.28.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.28.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/.github/workflows/push.yaml` & `xklb-1.28.5/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/sql/transfer.sql` & `xklb-1.28.5/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/av.py` & `xklb-1.28.5/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/books.py` & `xklb-1.28.5/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/consts.py` & `xklb-1.28.5/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/db.py` & `xklb-1.28.5/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/dl_config.py` & `xklb-1.28.5/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/dl_extract.py` & `xklb-1.28.5/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/fs_extract.py` & `xklb-1.28.5/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/gui.py` & `xklb-1.28.5/xklb/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
 from typing import NoReturn, Tuple
 
 from xklb.utils import log
 
+base_folder = Path(__file__).resolve().parent
+
 
 class UserQuit(BaseException):
     pass
 
 
 class MrSuperDialogue:
     def __init__(self, path, qty, geom_data=None, true_action="keep", false_action="delete") -> None:
@@ -21,15 +23,15 @@
         self.root = Tk()
         self.root.title("Library dialogue")
         self.root.wm_attributes("-alpha", 0)
 
         style = Style(self.root)
         style.theme_use("clam")
 
-        photo = PhotoImage(file=str(Path("assets/kotobago.png")))
+        photo = PhotoImage(file=str(base_folder / "assets" / "kotobago.png"))
         self.root.wm_iconphoto(True, photo)  # noqa: FBT003
         self.root.wm_attributes("-topmost", 1)
 
         for keyseq in ("<Escape>", "<Control-c>", "<Control-q>"):
             self.root.bind(keyseq, lambda _ev: self.user_quit())
 
         # menu left
```

### Comparing `xklb-1.28.4/xklb/hn_extract.py` & `xklb-1.28.5/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/lb.py` & `xklb-1.28.5/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/play_actions.py` & `xklb-1.28.5/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/playback.py` & `xklb-1.28.5/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/player.py` & `xklb-1.28.5/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/praw_extract.py` & `xklb-1.28.5/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/stats.py` & `xklb-1.28.5/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/subtitle.py` & `xklb-1.28.5/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/tabs_actions.py` & `xklb-1.28.5/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/tabs_extract.py` & `xklb-1.28.5/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/tube_backend.py` & `xklb-1.28.5/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/tube_extract.py` & `xklb-1.28.5/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/utils.py` & `xklb-1.28.5/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/__init__.py` & `xklb-1.28.5/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/bigdirs.py` & `xklb-1.28.5/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/christen.py` & `xklb-1.28.5/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/copy_play_counts.py` & `xklb-1.28.5/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/dedupe.py` & `xklb-1.28.5/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/merge_dbs.py` & `xklb-1.28.5/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/merge_online_local.py` & `xklb-1.28.5/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/move_list.py` & `xklb-1.28.5/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/optimize_db.py` & `xklb-1.28.5/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/redownload.py` & `xklb-1.28.5/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/relmv.py` & `xklb-1.28.5/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/scatter.py` & `xklb-1.28.5/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/streaming_tab_loader.py` & `xklb-1.28.5/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/mining/data.py` & `xklb-1.28.5/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/mining/extract_links.py` & `xklb-1.28.5/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/mining/nouns.py` & `xklb-1.28.5/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/mining/pushshift.py` & `xklb-1.28.5/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.28.5/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/xklb/assets/kotobago.png` & `xklb-1.28.5/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/.gitignore` & `xklb-1.28.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/LICENSE` & `xklb-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/README.md` & `xklb-1.28.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.004)
+    xk media library subcommands (v1.28.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.28.4/pyproject.toml` & `xklb-1.28.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.4/PKG-INFO` & `xklb-1.28.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.28.4
+Version: 1.28.5
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
-    xk media library subcommands (v1.28.004)
+    xk media library subcommands (v1.28.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

