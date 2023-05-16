# Comparing `tmp/calcipy-1.2.3.tar.gz` & `tmp/calcipy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.2.3.tar", max compression
+gzip compressed data, was "calcipy-1.2.4.tar", max compression
```

## Comparing `calcipy-1.2.3.tar` & `calcipy-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-04-08 18:44:24.793480 calcipy-1.2.3/LICENSE
--rw-r--r--   0        0        0      167 2023-04-08 18:49:40.947990 calcipy-1.2.3/calcipy/__init__.py
--rw-r--r--   0        0        0     1259 2023-02-23 02:19:12.612069 calcipy-1.2.3/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.3/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8214 2023-03-02 02:41:41.090176 calcipy-1.2.3/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6261 2023-04-08 00:38:00.312188 calcipy-1.2.3/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.3/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0     9790 2023-02-26 00:17:08.509359 calcipy-1.2.3/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.3/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.3/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.3/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1915 2023-04-06 23:41:07.217109 calcipy-1.2.3/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.3/calcipy/file_search.py
--rw-r--r--   0        0        0     1814 2023-04-07 21:04:03.754244 calcipy-1.2.3/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.3/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7815 2023-02-23 02:19:12.614596 calcipy-1.2.3/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.3/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6546 2023-04-08 18:34:57.636140 calcipy-1.2.3/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1193 2023-03-02 02:45:23.652620 calcipy-1.2.3/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.3/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3104 2023-04-05 22:06:13.047283 calcipy-1.2.3/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     1876 2023-04-06 12:55:27.782578 calcipy-1.2.3/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1132 2023-02-23 02:54:45.453854 calcipy-1.2.3/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3589 2023-04-06 12:54:31.902116 calcipy-1.2.3/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     3869 2023-04-07 23:08:02.132045 calcipy-1.2.3/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      454 2023-02-23 02:19:12.617085 calcipy-1.2.3/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1275 2023-02-23 02:19:12.617365 calcipy-1.2.3/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      557 2023-02-23 02:19:12.617596 calcipy-1.2.3/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1498 2023-02-23 02:19:12.617900 calcipy-1.2.3/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3510 2023-04-06 23:41:29.742135 calcipy-1.2.3/calcipy/tasks/test.py
--rw-r--r--   0        0        0      634 2023-02-23 02:19:12.618406 calcipy-1.2.3/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-04-08 18:49:47.692190 calcipy-1.2.3/docs/README.md
--rw-r--r--   0        0        0     6455 2023-04-08 18:49:40.986914 calcipy-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     9950 1970-01-01 00:00:00.000000 calcipy-1.2.3/setup.py
--rw-r--r--   0        0        0    11358 1970-01-01 00:00:00.000000 calcipy-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-13 11:22:49.916008 calcipy-1.2.4/LICENSE
+-rw-r--r--   0        0        0      167 2023-05-16 23:29:56.121283 calcipy-1.2.4/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.2.4/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.4/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8262 2023-05-13 00:16:53.654649 calcipy-1.2.4/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6422 2023-05-13 10:55:55.582130 calcipy-1.2.4/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.4/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    10840 2023-05-13 11:22:33.621932 calcipy-1.2.4/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.4/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.4/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.4/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-13 11:16:09.447581 calcipy-1.2.4/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.4/calcipy/file_search.py
+-rw-r--r--   0        0        0     1814 2023-04-07 21:04:03.754244 calcipy-1.2.4/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.4/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7833 2023-04-22 15:51:43.990661 calcipy-1.2.4/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.4/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.2.4/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1193 2023-04-22 15:05:58.225355 calcipy-1.2.4/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.4/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3120 2023-04-08 22:31:05.741542 calcipy-1.2.4/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     1876 2023-04-06 12:55:27.782578 calcipy-1.2.4/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1132 2023-02-23 02:54:45.453854 calcipy-1.2.4/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3609 2023-04-22 14:59:14.141730 calcipy-1.2.4/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     3869 2023-04-07 23:08:02.132045 calcipy-1.2.4/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      454 2023-02-23 02:19:12.617085 calcipy-1.2.4/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1659 2023-05-16 23:12:39.188499 calcipy-1.2.4/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      557 2023-02-23 02:19:12.617596 calcipy-1.2.4/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1498 2023-02-23 02:19:12.617900 calcipy-1.2.4/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3659 2023-04-18 23:50:20.411698 calcipy-1.2.4/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      634 2023-02-23 02:19:12.618406 calcipy-1.2.4/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     6651 2023-05-16 23:30:13.497030 calcipy-1.2.4/docs/README.md
+-rw-r--r--   0        0        0     6547 2023-05-16 23:29:56.158760 calcipy-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9989 1970-01-01 00:00:00.000000 calcipy-1.2.4/setup.py
+-rw-r--r--   0        0        0    11420 1970-01-01 00:00:00.000000 calcipy-1.2.4/PKG-INFO
```

### Comparing `calcipy-1.2.3/LICENSE` & `calcipy-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/can_skip.py` & `calcipy-1.2.4/calcipy/can_skip.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
         if can_skip(prerequisites=[*Path('src').rglob('*.py')], targets=[Path('.coverage.xml')]):
             return  # Exit early
 
         ...  # Task code
     ```
 
     """
-    ts_prerequisites = [pth.stat().st_mtime for pth in prerequisites]
-    if not ts_prerequisites:
+    if not (ts_prerequisites := [pth.stat().st_mtime for pth in prerequisites]):
         raise ValueError('Required files do not exist', prerequisites)
 
     ts_targets = [pth.stat().st_mtime for pth in targets]
     if ts_targets and min(ts_targets) > max(ts_prerequisites):
         logger.warning('Skipping because targets are newer', targets=targets)
         return True
     return False
```

### Comparing `calcipy-1.2.3/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.2.4/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         delta = pack.datetime.humanize()  # type: ignore[union-attr]
         latest = '' if pack.version == pack.latest_version else f' (*New version available: {pack.latest_version}*)'
         return f'- {delta}: {pack.name} {pack.version}{latest}'
 
     now = arrow.utcnow()
     stale_cutoff = now.shift(months=-1 * stale_months)
     stale_packages = [pack for pack in packages if not pack.datetime or pack.datetime < stale_cutoff]
+    # TODO: If no stale, write out five oldest?
     if stale_packages:
         pkgs = sorted(stale_packages, key=lambda x: x.datetime or stale_cutoff)
         stale_list = '\n'.join([format_package(_p) for _p in pkgs])
         logger.warning('Found stale packages that may be a dependency risk', stale_list=stale_list)
         return True
     oldest_date = np.amin([pack.datetime for pack in packages])  # pyright: ignore[reportGeneralTypeIssues]
     logger.text('No stale packages found', oldest=oldest_date.humanize(), stale_threshold=stale_months)
```

### Comparing `calcipy-1.2.3/calcipy/cli.py` & `calcipy-1.2.4/calcipy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,50 +33,51 @@
     keep_going: bool = False
     """Continue task execution regardless of failure."""
 
 
 class _CalcipyProgram(Program):  # type: ignore[misc]
     """Customized version of Invoke's `Program`."""
 
-    def print_help(self) -> None:
+    def print_help(self) -> None:  # pragma: no cover
         """Extend print_help with calcipy-specific global configuration.
 
         https://github.com/pyinvoke/invoke/blob/0bcee75e4a26ad33b13831719c00340ca12af2f0/invoke/program.py#L657-L667
 
         """
         super().print_help()
         print('Global Task Options:')  # noqa: T201
         print('')  # noqa: T201
         self.print_columns([
-            ('working_dir', 'Set the cwd for the program. Example: "../run --working-dir .. lint test"'),
             ('*file_args', 'List of Paths available globally to all tasks. Will resolve paths with working_dir'),
-            ('verbose', 'Globally configure logger verbosity (-vvv for most verbose)'),
+            ('--keep-going', 'Continue running tasks even on failure'),
+            ('--working_dir=STRING', 'Set the cwd for the program. Example: "../run --working-dir .. lint test"'),
+            ('-v,-vv,-vvv', 'Globally configure logger verbosity (-vvv for most verbose)'),
         ])
         print('')  # noqa: T201
 
 
 class CalcipyConfig(Config):  # type: ignore[misc]
     """Opinionated Config with better defaults."""
 
     @staticmethod
-    def global_defaults() -> Dict:  # type: ignore[type-arg]
+    def global_defaults() -> Dict:  # type: ignore[type-arg]  # pragma: no cover
         """Override the global defaults."""
         invoke_defaults = Config.global_defaults()
         calcipy_defaults = {
             'run': {
                 'echo': True,
                 'echo_format': '\033[2;3;37mRunning: {command}\033[0m',
                 'pty': use_pty(),
             },
         }
         return merge_dicts(invoke_defaults, calcipy_defaults)  # type: ignore[no-any-return]
 
 
 @beartype
-def start_program(
+def start_program(  # pragma: no cover
     pkg_name: str,
     pkg_version: str,
     module: Optional[ModuleType] = None,
     collection: Optional[Collection] = None,
 ) -> None:
     """Run the customized Invoke Program.
 
@@ -160,14 +161,15 @@
 
     try:
         return _run_task(func, ctx, *args, show_task_info=show_task_info, **kwargs)
     except Exception:
         if not ctx.config.gto.keep_going:
             raise
         logger.exception('Task Failed', func=str(func), args=args, kwargs=kwargs)
+    return None
 
 
 @beartype
 def task(*task_args: Any, show_task_info: bool = True, **task_kwargs: Any) -> Callable[[Any], Task]:
     """Wrapper to accept arguments for an invoke task."""
     @beartype
     def wrapper(func: Any) -> Task:  # noqa: ANN001
```

### Comparing `calcipy-1.2.3/calcipy/code_tag_collector/_collector.py` & `calcipy-1.2.4/calcipy/code_tag_collector/_collector.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,70 +137,100 @@
     # > git@github.com:KyleKing/calcipy.git
     # > https://github.com/KyleKing/calcipy.git
     sub_url = re.findall(r'^.+github.com[:/]([^.]+)(?:\.git)?$', clone_uri)[0]
     repo_url = f'https://github.com/{sub_url}'
     return git_dir, repo_url
 
 
+class _CollectorRow(BaseModel):
+    """Each row of the Code Tag table."""
+
+    tag_name: str
+    comment: str
+    last_edit: str
+    source_file: str
+
+    @classmethod
+    @beartype
+    def from_code_tag(cls, code_tag: _CodeTag, last_edit: str, source_file: str) -> '_CollectorRow':
+        return cls(
+            tag_name=f'{code_tag.tag:>7}',
+            comment=code_tag.text,
+            last_edit=last_edit,
+            source_file=source_file,
+        )
+
+
+@beartype
+def _format_from_blame(
+    *, collector_row: _CollectorRow, blame: str, repo_url: str, cwd: Path, rel_path: Path,
+) -> _CollectorRow:
+    """Parse the git blame for useful timestamps and author when available."""
+    # Note: line number may be different in older blame (and relative path)
+    revision, old_line_number = blame.split('\n')[0].split(' ')[:2]
+    # If the change has not yet been committed, use the branch name as best guess
+    if all(_c == '0' for _c in revision):
+        revision = capture_shell('git branch --show-current', cwd=cwd)
+    # Format a nice timestamp of the last edit to the line
+    blame_dict = {
+        line.split(' ')[0]: ' '.join(line.split(' ')[1:])
+        for line in blame.split('\n')
+    }
+
+    # Handle uncommitted files that only have author-time and author-tz
+    user = 'committer' if 'committer-tz' in blame_dict else 'author'
+    dt = arrow.get(int(blame_dict[f'{user}-time']))
+    tz = blame_dict[f'{user}-tz'][:3] + ':' + blame_dict[f'{user}-tz'][-2:]
+    collector_row.last_edit = arrow.get(dt.isoformat()[:-6] + tz).format('YYYY-MM-DD')
+
+    # Filename may not be present if uncommitted. Use local path as fallback
+    remote_file_path = blame_dict.get('filename', rel_path.as_posix())
+    # Assumes Github format
+    git_url = f'{repo_url}/blame/{revision}/{remote_file_path}#L{old_line_number}'
+    collector_row.source_file = f'[{collector_row.source_file}]({git_url})'
+
+    return collector_row
+
+
 @beartype
-def _format_record(base_dir: Path, file_path: Path, comment: _CodeTag) -> Dict[str, str]:
+def _format_record(base_dir: Path, file_path: Path, comment: _CodeTag) -> _CollectorRow:
     """Format each table row for the code tag summary file. Include git permalink.
 
     Args:
         base_dir: base path of the project if git directory is not known
         file_path: path to the file of interest
         comment: _CodeTag information for the matched tag
 
     Returns:
         Dict[str, str]: formatted dictionary with file info
 
     """
     cwd = file_path.parent
     _git_dir, repo_url = _git_info(cwd=cwd)
-    blame = None
+
+    # Set fallback values if git logic doesn't work
+    rel_path = file_path.relative_to(base_dir)
+    collector_row = _CollectorRow.from_code_tag(
+        code_tag=comment,
+        last_edit='N/A',
+        source_file=f'{rel_path.as_posix()}:{comment.lineno}',
+    )
+
     try:
         blame = capture_shell(f'git blame {file_path} -L {comment.lineno},{comment.lineno} --porcelain', cwd=cwd)
+        collector_row = _format_from_blame(
+            collector_row=collector_row, blame=blame, repo_url=repo_url, cwd=cwd, rel_path=rel_path,
+        )
     except CalledProcessError as exc:
         handled_errors = (128,)
         if exc.returncode not in handled_errors:
             raise
         logger.text_debug('Skipping blame', file_path=file_path, exc=exc)
 
-    # Set fallback values if git logic doesn't work
-    rel_path = file_path.relative_to(base_dir)
-    source_file = f'{rel_path.as_posix()}:{comment.lineno}'
-    ts = 'N/A'
-    if blame:
-        # Note: line number may be different in older blame (and relative path)
-        revision, old_line_number = blame.split('\n')[0].split(' ')[:2]
-        # If the change has not yet been committed, use the branch name as best guess
-        if all(_c == '0' for _c in revision):
-            revision = capture_shell('git branch --show-current', cwd=cwd)
-        # Format a nice timestamp of the last edit to the line
-        blame_dict = {
-            line.split(' ')[0]: ' '.join(line.split(' ')[1:])
-            for line in blame.split('\n')
-        }
-        # Handle uncommitted files that only have author-time and author-tz
-        user = 'committer' if 'committer-tz' in blame_dict else 'author'
-        dt = arrow.get(int(blame_dict[f'{user}-time']))
-        tz = blame_dict[f'{user}-tz'][:3] + ':' + blame_dict[f'{user}-tz'][-2:]
-        ts = arrow.get(dt.isoformat()[:-6] + tz).format('YYYY-MM-DD')
-        # Filename may not be present if uncommitted. Use local path as fallback
-        remote_file_path = blame_dict.get('filename', rel_path.as_posix())
-        # Assumes Github
-        git_url = f'{repo_url}/blame/{revision}/{remote_file_path}#L{old_line_number}'
-        source_file = f'[{source_file}]({git_url})'
-
-    return {
-        'Type': f'{comment.tag:>7}',
-        'Comment': comment.text,
-        'Last Edit': ts,
-        'Source File': source_file,
-    }
+    return collector_row
 
 
 @beartype
 def _format_report(  # noqa: CAC001
     base_dir: Path, code_tags: List[_Tags], tag_order: List[str],
 ) -> str:
     """Pretty-format the code tags by file and line number.
@@ -216,15 +246,21 @@
     """
     output = ''
     records = []
     counter: Dict[str, int] = defaultdict(lambda: 0)
     for comments in sorted(code_tags, key=lambda tc: tc.path_source, reverse=False):
         for comment in comments.code_tags:
             if comment.tag in tag_order:
-                records.append(_format_record(base_dir, comments.path_source, comment))
+                collector_row = _format_record(base_dir, comments.path_source, comment)
+                records.append({
+                    'Type': collector_row.tag_name,
+                    'Comment': collector_row.comment,
+                    'Last Edit': collector_row.last_edit,
+                    'Source File': collector_row.source_file,
+                })
                 counter[comment.tag] += 1
     if records:
         df_tags = pd.DataFrame(records)
         # Prevent URLs from appearing on multiple lines
         content = df_tags.to_markdown(index=False, tablefmt='github', maxcolwidths=None) or ''
         for line in content.split('\n'):
             if not line.startswith('/'):
@@ -252,17 +288,17 @@
 ) -> None:
     """Create the code tag summary file.
 
     Args:
         path_tag_summary: Path to the output file
         paths_source: list of source files to parse
         base_dir: base directory relative to the searched files
-        regex_compiled: compiled regular expression. Expected to have matching groups `(tag, text)`.
+        regex: compiled regular expression. Expected to have matching groups `(tag, text)`.
             Default is CODE_TAG_RE with tags from tag_order
-        tag_order: subset of all tags to include in the report and specified order. Default is COMMON_CODE_TAGS
+        tags: subset of all tags to include in the report and specified order. Default is COMMON_CODE_TAGS
         header: header text
 
     """
     tag_order = [_t.strip() for _t in tags.split(',') if _t] or COMMON_CODE_TAGS
     regex_compiled = re.compile((regex or CODE_TAG_RE).format(tag='|'.join(tag_order)))
 
     matches = _search_files(paths_source, regex_compiled)
```

### Comparing `calcipy-1.2.3/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.2.4/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.2.4/calcipy/experiments/check_duplicate_test_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     """Print info about the function."""
     logger.info('> name', name=function.name)
     if function.args.args:
         logger.info('\t args', args=function.args.args)
 
 
 @beartype
-def run(test_path: Path) -> List[str]:  # noqa: C901,CAC001
+def run(test_path: Path) -> List[str]:  # noqa: C901,CAC001  # pylint: disable=too-complex
     """Check for duplicates in the test suite.
 
     Inspired by: https://stackoverflow.com/a/67840804/3219667
 
     """
     summary = set()
     duplicates = []
 
-    for path_test in test_path.rglob('test_*.py'):
+    for path_test in test_path.rglob('test_*.py'):  # pylint: disable=too-many-nested-blocks
         logger.info(path_test.as_posix())
         parsed_ast = ast.parse(path_test.read_text())
 
         for node in parsed_ast.body:
             if isinstance(node, ast.FunctionDef):
                 if node.name in summary and node.name.startswith('test_'):
                     duplicates.append(node.name)
```

### Comparing `calcipy-1.2.3/calcipy/file_search.py` & `calcipy-1.2.4/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/invoke_helpers.py` & `calcipy-1.2.4/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/md_writer/_writer.py` & `calcipy-1.2.4/calcipy/md_writer/_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,8 +227,8 @@
         'SOURCE_FILE=': _handle_source_file,
     }
 
     paths = paths_md or find_project_files_by_suffix(get_project_path()).get('md') or []
     for path_md in paths:
         logger.text_debug('Processing', path_md=path_md)
         if md_lines := _ReplacementMachine().parse(read_lines(path_md), _lookup, path_md):
-            path_md.write_text('\n'.join(md_lines) + '\n')
+            path_md.write_text('\n'.join(md_lines) + '\n', encoding='utf-8')
```

### Comparing `calcipy-1.2.3/calcipy/noxfile/_noxfile.py` & `calcipy-1.2.4/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/scripts.py` & `calcipy-1.2.4/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/tasks/all_tasks.py` & `calcipy-1.2.4/calcipy/tasks/all_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,30 +65,31 @@
         tasks.extend([call(progress, index=ix + offset, total=total), item])  # pyright: ignore[reportGeneralTypeIssues]
     return tasks  # pyright: ignore[reportGeneralTypeIssues]
 
 
 _MAIN_TASKS = [
     lint.fix,
     types.mypy,
+    types.pyright,
     call(nox.noxfile, session='tests'),  # pyright: ignore[reportGeneralTypeIssues]
     call(lint.pre_commit, no_update=True),  # pyright: ignore[reportGeneralTypeIssues]
     lint.security,
     tags.collect_code_tags,
     cl.write,
     pack.lock,
     test.coverage,
     doc.build,
     stale.check_for_stale_packages,
 ]
 _OTHER_TASKS = [
+    test.check,
     lint.flake8,
     lint.pylint,
     pack.check_licenses,
     test.step,
-    types.pyright,
 ]
 
 
 @task(post=with_progress(_MAIN_TASKS))
 def main(_ctx: Context) -> None:
     """Main task pipeline."""
```

### Comparing `calcipy-1.2.3/calcipy/tasks/cl.py` & `calcipy-1.2.4/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/tasks/defaults.py` & `calcipy-1.2.4/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/tasks/doc.py` & `calcipy-1.2.4/calcipy/tasks/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 @task()
 def watch(ctx: Context) -> None:
     """Serve local documentation for local editing."""
     if _is_mkdocs_local():  # pragma: no cover
         path_doc_index = get_out_dir() / 'index.html'
         open_in_browser(path_doc_index)
-    else:
+    else:  # pragma: no cover
         webbrowser.open('http://localhost:8000')
         run(ctx, 'poetry run mkdocs serve --dirtyreload')
 
 
 @task()
 def deploy(ctx: Context) -> None:
     """Deploy docs to the Github `gh-pages` branch."""
```

### Comparing `calcipy-1.2.3/calcipy/tasks/lint.py` & `calcipy-1.2.4/calcipy/tasks/lint.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/tasks/pack.py` & `calcipy-1.2.4/calcipy/tasks/pack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """Packaging CLI."""
 
+from corallium import file_helpers  # Required for mocking read_pyproject
 from corallium.file_helpers import LOCK, PROJECT_TOML
 from corallium.log import logger
 from invoke import Context
 
 from .. import can_skip  # Required for mocking can_skip.can_skip
 from ..cli import task
 from ..invoke_helpers import run
 from ..noxfile._noxfile import BASE_NOX_COMMAND
 
 
 @task()
+def install_extras(ctx: Context) -> None:
+    """Run poetry install with all extras."""
+    poetry_config = file_helpers.read_pyproject()['tool']['poetry']
+    extras = (poetry_config.get('extras') or {}).keys()
+    run(ctx, ' '.join(['poetry install --sync', *[f'--extras={ex}' for ex in extras]]))
+
+
+@task()
 def lock(ctx: Context) -> None:
     """Ensure poetry.lock is  up-to-date."""
     if can_skip.can_skip(prerequisites=[PROJECT_TOML], targets=[LOCK]):
         return  # Exit early
 
     run(ctx, 'poetry lock --no-update')
```

### Comparing `calcipy-1.2.3/calcipy/tasks/stale.py` & `calcipy-1.2.4/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/tasks/tags.py` & `calcipy-1.2.4/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/calcipy/tasks/test.py` & `calcipy-1.2.4/calcipy/tasks/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         'min_cover': 'Fail if coverage less than threshold',
         **KM_HELP,
     },
 )
 def pytest(ctx: Context, *, keyword: str = '', marker: str = '', min_cover: int = 0) -> None:
     """Run pytest with default arguments."""
     pkg_name = read_package_name()
-    _inner_task(ctx, cli_args=f' --cov={pkg_name} --cov-report=term-missing',
+    durations = '--durations=25 --durations-min="0.1"'
+    _inner_task(ctx,
+                cli_args=f' --cov={pkg_name} --cov-branch --cov-report=term-missing {durations}',
                 keyword=keyword, marker=marker, min_cover=min_cover)
 
 
 @task(help=KM_HELP)
 def step(ctx: Context, *, keyword: str = '', marker: str = '') -> None:
     """Run pytest optimized to stop on first error."""
     _inner_task(ctx, cli_args=_STEPWISE_ARGS, keyword=keyword, marker=marker)
@@ -85,18 +87,20 @@
 def coverage(ctx: Context, *, min_cover: int = 0, out_dir: Optional[str] = None, view: bool = False) -> None:
     """Generate useful coverage outputs after running pytest.
 
     Creates `coverage.json` used in `doc.build`
 
     """
     pkg_name = read_package_name()
-    _inner_task(ctx, cli_args='', min_cover=min_cover, command=f'coverage run --source={pkg_name} --module pytest')
+    _inner_task(ctx, cli_args='', min_cover=min_cover,
+                command=f'coverage run --branch --source={pkg_name} --module pytest')
 
     cov_dir = Path(out_dir or from_ctx(ctx, 'test', 'out_dir'))
     cov_dir.mkdir(exist_ok=True, parents=True)
+    print('')  # noqa: T201
     for cmd in (
         'poetry run python -m coverage report --show-missing',  # Write to STDOUT
         f'poetry run python -m coverage html --directory={cov_dir}',  # Write to HTML
         'poetry run python -m coverage json',  # Create coverage.json file for "_handle_coverage"
     ):
         run(ctx, cmd)
```

### Comparing `calcipy-1.2.3/calcipy/tasks/types.py` & `calcipy-1.2.4/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/docs/README.md` & `calcipy-1.2.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.3/pyproject.toml` & `calcipy-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.3"
+version = "1.2.4"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,25 +26,25 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.2.3"
+version = "1.2.4"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # flake8
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
 bidict = {optional = true, version = ">=0.22.1"} # stale
 commitizen = {optional = true, version = ">=2.42.0"} # doc
-corallium = ">=0.1.1"
+corallium = ">=0.2.1"
 dlint = {optional = true, version = ">=0.14.0"} # flake8
 flake8 = {optional = true, version = ">=6.0.0"} # flake8
 flake8-adjustable-complexity = {optional = true, version = ">=0.0.6"} # flake8
 flake8-annotations-complexity = {optional = true, version = ">=0.0.7"} # flake8
 flake8-executable = {optional = true, version = ">=2.1.3"} # flake8
 flake8-expression-complexity = {optional = true, version = ">=0.0.11"} # flake8
 flake8-functions = {optional = true, version = ">=0.0.7"} # flake8
@@ -56,30 +56,31 @@
 flake8-sql = {optional = true, version = ">=0.4.1"} # flake8
 flake8-string-format = {optional = true, version = ">=0.3.0"} # flake8
 flake8-super = {optional = true, version = ">=0.1.3"} # flake8
 flake8-tuple = {optional = true, version = ">=0.4.1"} # flake8
 flake8-typing-imports = {optional = true, version = ">=1.14.0"} # flake8
 flake8-use-pathlib = {optional = true, version = ">=0.3.0"} # flake8
 flake8-variables-names = {optional = true, version = ">=0.0.5"} # flake8
-invoke = ">=2.0.0"
+invoke = ">=2.1.0"
 mkdocs = {optional = true, version = ">=1.4.1"} # doc
 mkdocs-build-plantuml-plugin = {optional = true, version = ">=1.7.4"} # doc
 mkdocs-gen-files = {optional = true, version = ">=0.4.0"} # doc
 mkdocs-git-revision-date-localized-plugin = {optional = true, version = ">=1.0.1"} # doc
 mkdocs-include-markdown-plugin = {markers = "python_version < '3.12'", optional = true, version = ">=4.0.3"} # doc
 mkdocs-literate-nav = {optional = true, version = ">=0.5.0"} # doc
 mkdocs-material = {optional = true, version = ">=8.2.16"} # doc
 mkdocs-section-index = {optional = true, version = ">=0.3.4"} # doc
-mkdocstrings = {extras = ["python"], optional = true, version = ">=0.18.1"} # doc
+mkdocstrings = {extras = ["python"], optional = true, version = ">=0.21.1"} # doc
 mypy = {optional = true, version = ">=1.0.0"} # types
 nox-poetry = {optional = true, version = ">=1.0.2"} # test
 pandas = {optional = true, version = ">=1.5.3"} # docs,tags
 pip-check = {optional = true, version = ">=2.8.1"} # lint
 pydantic = ">=1.10.5"
 pylint = {optional = true, version = ">=2.16.2"} # doc,pylint
+pymdown-extensions = {optional = true, version = ">=10.0.1"} # docs
 pyrate_limiter = {optional = true, version = ">=2.4"} # stale
 pytest = {optional = true, version = ">=7.2.1"} # test
 pytest-cov = {optional = true, version = ">=4.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
 pytest-watcher = {optional = true, version = ">=0.2.6"} # test
 python-box = {optional = true, version = ">=6.0.2"} # ddict
 pyyaml = {optional = true, version = ">=5.2"} # doc,tags
@@ -100,14 +101,15 @@
   "mkdocs-include-markdown-plugin",
   "mkdocs-literate-nav",
   "mkdocs-material",
   "mkdocs-section-index",
   "mkdocstrings",
   "pandas",
   "pylint", # for 'pyreverse'
+  "pymdown-extensions",
   "pyyaml",
   "transitions",
 ]
 flake8 = [
   "dlint",
   "flake8",
   "flake8-adjustable-complexity",
```

### Comparing `calcipy-1.2.3/setup.py` & `calcipy-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,30 @@
  'calcipy.noxfile',
  'calcipy.tasks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beartype>=0.12.0', 'corallium>=0.1.1', 'invoke>=2.0.0', 'pydantic>=1.10.5']
+['beartype>=0.12.0', 'corallium>=0.2.1', 'invoke>=2.1.0', 'pydantic>=1.10.5']
 
 extras_require = \
 {'ddict': ['python-box>=6.0.2'],
  'doc': ['commitizen>=2.42.0',
          'mkdocs>=1.4.1',
          'mkdocs-build-plantuml-plugin>=1.7.4',
          'mkdocs-gen-files>=0.4.0',
          'mkdocs-git-revision-date-localized-plugin>=1.0.1',
          'mkdocs-literate-nav>=0.5.0',
          'mkdocs-material>=8.2.16',
          'mkdocs-section-index>=0.3.4',
-         'mkdocstrings[python]>=0.18.1',
+         'mkdocstrings[python]>=0.21.1',
          'pandas>=1.5.3',
          'pylint>=2.16.2',
+         'pymdown-extensions>=10.0.1',
          'pyyaml>=5.2',
          'transitions>=0.9.0'],
  'doc:python_version < "3.12"': ['mkdocs-include-markdown-plugin>=4.0.3'],
  'flake8': ['dlint>=0.14.0',
             'flake8>=6.0.0',
             'flake8-adjustable-complexity>=0.0.6',
             'flake8-annotations-complexity>=0.0.7',
@@ -74,15 +75,15 @@
 {'console_scripts': ['calcipy = calcipy.scripts:start',
                      'calcipy_lint = calcipy.scripts:start_lint',
                      'calcipy_tags = calcipy.scripts:start_tags',
                      'calcipy_types = calcipy.scripts:start_types']}
 
 setup_kwargs = {
     'name': 'calcipy',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'Python package to simplify development',
     'long_description': '# calcipy\n\n![./calcipy-banner-wide.svg](https://raw.githubusercontent.com/KyleKing/calcipy/main/docs/calcipy-banner-wide.svg)\n\n`calcipy` is a Python package that implements best practices such as code style (linting, auto-fixes), documentation, CI/CD, and logging. Like the calcium carbonate in hard coral, packages can be built on the `calcipy` foundation.\n\n`calcipy` has some configurability, but is tailored for my particular use cases. If you want the same sort of functionality, there are a number of alternatives to consider:\n\n- [pyscaffold](https://github.com/pyscaffold/pyscaffold) is a much more mature project that aims for the same goals, but with a slightly different approach and tech stack (tox vs. nox, cookiecutter vs. copier, etc.)\n- [tidypy](https://github.com/jayclassless/tidypy#features), [pylama](https://github.com/klen/pylama), and [codecheck](https://pypi.org/project/codecheck/) offer similar functionality of bundling and running static checkers, but makes far fewer assumptions\n- [pytoil](https://github.com/FollowTheProcess/pytoil) is a general CLI tool for developer automation\n- And many more such as [pyta](https://github.com/pyta-uoft/pyta), [prospector](https://github.com/PyCQA/prospector), [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) / [cjolowicz/cookiecutter-hypermodern-python](https://github.com/cjolowicz/cookiecutter-hypermodern-python), [formate](https://github.com/python-formate/formate), [johnthagen/python-blueprint](https://github.com/johnthagen/python-blueprint), [oxsecurity/megalinter](https://github.com/oxsecurity/megalinter), etc.\n\n## Installation\n\nCalcipy needs a few static files managed using copier and a template project: [kyleking/calcipy_template](https://github.com/KyleKing/calcipy_template/)\n\nYou can quickly use the template to create a new project or add calcipy to an existing one:\n\n```sh\n# Install copier. pipx is recommended\npipx install copier\n\n# To create a new project\ncopier copy gh:KyleKing/calcipy_template new_project\ncd new_project\n\n# Or convert/update an existing one\ncd my_project\ncopier copy gh:KyleKing/calcipy_template .\ncopier update\n```\n\nSee [./Advanced_Configuration.md](./Advanced_Configuration.md) for documentation on the configurable aspects of `calcipy`\n\n### Calcipy CLI\n\nAdditionally, `calcipy` can be run as a CLI application without adding the package as a dependency.\n\nQuick Start:\n\n```sh\npipx install calcipy\n\n# Use \'tags\' to create a CODE_TAG_SUMMARY of the specified directory\ncalcipy tags --help\ncalcipy tags --base-dir=~/path/to/my_project\n\n# See additional documentation from the CLI help\n> calcipy\n\nSubcommands:\n\nmain                                     Main task pipeline.\nother                                    Run tasks that are otherwise not exercised in main.\nrelease                                  Release pipeline.\ncl.bump                                  Bumps project version based on commits & settings in pyproject.toml.\ncl.write                                 Write a Changelog file with the raw Git history.\ndoc.build                                Build documentation with mkdocs.\ndoc.deploy                               Deploy docs to the Github `gh-pages` branch.\ndoc.watch                                Serve local documentation for local editing.\nlint.autopep8                            Run autopep8.\nlint.check (lint)                        Run ruff as check-only.\nlint.fix                                 Run ruff and apply fixes.\nlint.flake8                              Run ruff and apply fixes.\nlint.pre-commit                          Run pre-commit.\nlint.pylint                              Run ruff and apply fixes.\nlint.security                            Attempt to identify possible security vulnerabilities.\nlint.watch                               Run ruff as check-only.\nnox.noxfile (nox)                        Run nox from the local noxfile.\npack.check-licenses                      Check licenses for compatibility with `licensecheck`.\npack.lock                                Ensure poetry.lock is  up-to-date.\npack.publish                             Build the distributed format(s) and publish.\nstale.check-for-stale-packages (stale)   Identify stale dependencies.\ntags.collect-code-tags (tags)            Create a `CODE_TAG_SUMMARY.md` with a table for TODO- and FIXME-style code comments.\ntest.coverage                            Generate useful coverage outputs after running pytest.\ntest.pytest (test)                       Run pytest with default arguments.\ntest.step                                Run pytest optimized to stop on first error.\ntest.watch                               Run pytest with polling and optimized to stop on first error.\ntypes.mypy                               Run mypy.\ntypes.pyright                            Run pyright.\n\nGlobal Task Options:\n\nworking_dir   Set the cwd for the program. Example: "../run --working-dir .. lint test"\n*file_args    List of Paths available globally to all tasks. Will resolve paths with working_dir\nverbose       Globally configure logger verbosity (-vvv for most verbose)\n```\n\n### Calcipy Pre-Commit\n\n`calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:\n\n```yaml\nrepos:\n  - repo: https://github.com/KyleKing/calcipy\n    rev: main\n    hooks:\n      - id: tags\n      - id: lint-fix\n      - id: types\n```\n\n## Project Status\n\nSee the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].\n\n## Contributing\n\nWe welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:\n\n- [DEVELOPER_GUIDE]\n- [STYLE_GUIDE]\n\n## Code of Conduct\n\nWe follow the [Contributor Covenant Code of Conduct][contributor-covenant].\n\n### Open Source Status\n\nWe try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/calcipy)\n\n## Responsible Disclosure\n\nIf you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).\n\n## License\n\n[LICENSE]\n\n[changelog]: https://calcipy.kyleking.me/docs/CHANGELOG\n[code_tag_summary]: https://calcipy.kyleking.me/docs/CODE_TAG_SUMMARY\n[contributor-covenant]: https://www.contributor-covenant.org\n[developer_guide]: https://calcipy.kyleking.me/docs/DEVELOPER_GUIDE\n[license]: https://github.com/kyleking/calcipy/blob/main/LICENSE\n[style_guide]: https://calcipy.kyleking.me/docs/STYLE_GUIDE\n',
     'author': 'Kyle King',
     'author_email': 'dev.act.kyle@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyleking/calcipy',
```

### Comparing `calcipy-1.2.3/PKG-INFO` & `calcipy-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -35,15 +35,15 @@
 Provides-Extra: types
 Requires-Dist: arrow (>=1.2.3) ; extra == "stale" or extra == "tags"
 Requires-Dist: autopep8 (>=2.0.1) ; extra == "lint"
 Requires-Dist: bandit (>=1.7.4) ; extra == "lint"
 Requires-Dist: beartype (>=0.12.0)
 Requires-Dist: bidict (>=0.22.1) ; extra == "stale"
 Requires-Dist: commitizen (>=2.42.0) ; extra == "doc"
-Requires-Dist: corallium (>=0.1.1)
+Requires-Dist: corallium (>=0.2.1)
 Requires-Dist: dlint (>=0.14.0) ; extra == "flake8"
 Requires-Dist: flake8 (>=6.0.0) ; extra == "flake8"
 Requires-Dist: flake8-adjustable-complexity (>=0.0.6) ; extra == "flake8"
 Requires-Dist: flake8-annotations-complexity (>=0.0.7) ; extra == "flake8"
 Requires-Dist: flake8-executable (>=2.1.3) ; extra == "flake8"
 Requires-Dist: flake8-expression-complexity (>=0.0.11) ; extra == "flake8"
 Requires-Dist: flake8-functions (>=0.0.7) ; extra == "flake8"
@@ -55,30 +55,31 @@
 Requires-Dist: flake8-sql (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-string-format (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-super (>=0.1.3) ; extra == "flake8"
 Requires-Dist: flake8-tuple (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-typing-imports (>=1.14.0) ; extra == "flake8"
 Requires-Dist: flake8-use-pathlib (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-variables-names (>=0.0.5) ; extra == "flake8"
-Requires-Dist: invoke (>=2.0.0)
+Requires-Dist: invoke (>=2.1.0)
 Requires-Dist: mkdocs (>=1.4.1) ; extra == "doc"
 Requires-Dist: mkdocs-build-plantuml-plugin (>=1.7.4) ; extra == "doc"
 Requires-Dist: mkdocs-gen-files (>=0.4.0) ; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin (>=1.0.1) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3) ; (python_version < "3.12") and (extra == "doc")
 Requires-Dist: mkdocs-literate-nav (>=0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.2.16) ; extra == "doc"
 Requires-Dist: mkdocs-section-index (>=0.3.4) ; extra == "doc"
-Requires-Dist: mkdocstrings[python] (>=0.18.1) ; extra == "doc"
+Requires-Dist: mkdocstrings[python] (>=0.21.1) ; extra == "doc"
 Requires-Dist: mypy (>=1.0.0) ; extra == "types"
 Requires-Dist: nox-poetry (>=1.0.2) ; extra == "nox"
 Requires-Dist: pandas (>=1.5.3) ; extra == "doc" or extra == "tags"
 Requires-Dist: pip-check (>=2.8.1) ; extra == "lint"
 Requires-Dist: pydantic (>=1.10.5)
 Requires-Dist: pylint (>=2.16.2) ; extra == "doc" or extra == "pylint"
+Requires-Dist: pymdown-extensions (>=10.0.1) ; extra == "doc"
 Requires-Dist: pyrate_limiter (>=2.4) ; extra == "stale"
 Requires-Dist: pytest (>=7.2.1) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
 Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
 Requires-Dist: python-box (>=6.0.2) ; extra == "ddict"
 Requires-Dist: pyyaml (>=5.2) ; extra == "doc" or extra == "tags"
```

