# Comparing `tmp/eulertools-0.7.0.tar.gz` & `tmp/eulertools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-0.7.0.tar", max compression
+gzip compressed data, was "eulertools-0.8.0.tar", max compression
```

## Comparing `eulertools-0.7.0.tar` & `eulertools-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.7.0/README.rst
--rw-r--r--   0        0        0     2694 2023-05-16 20:28:40.942105 eulertools-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.7.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-05-16 20:28:40.939064 eulertools-0.7.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0     2881 2023-05-15 13:24:16.965570 eulertools-0.7.0/src/eulertools/compare.py
--rw-r--r--   0        0        0      849 2023-05-16 16:32:08.364284 eulertools-0.7.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     3362 2023-05-16 16:39:11.755484 eulertools-0.7.0/src/eulertools/main.py
--rw-r--r--   0        0        0     3175 2023-05-15 13:31:53.522885 eulertools-0.7.0/src/eulertools/run.py
--rw-r--r--   0        0        0      909 2023-05-16 16:40:55.360249 eulertools-0.7.0/src/eulertools/statement.py
--rw-r--r--   0        0        0     2586 2023-05-15 13:30:41.006142 eulertools-0.7.0/src/eulertools/time.py
--rw-r--r--   0        0        0     5829 2023-05-16 16:05:50.207080 eulertools-0.7.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     2679 2023-05-17 15:25:07.529316 eulertools-0.8.0/README.rst
+-rw-r--r--   0        0        0     2693 2023-05-17 15:25:59.778268 eulertools-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.8.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-17 15:25:59.781326 eulertools-0.8.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0     2881 2023-05-15 13:24:16.965570 eulertools-0.8.0/src/eulertools/compare.py
+-rw-r--r--   0        0        0      871 2023-05-16 21:00:03.640220 eulertools-0.8.0/src/eulertools/generate.py
+-rw-r--r--   0        0        0     3376 2023-05-17 13:06:15.125067 eulertools-0.8.0/src/eulertools/main.py
+-rw-r--r--   0        0        0     3175 2023-05-17 13:06:15.125983 eulertools-0.8.0/src/eulertools/run.py
+-rw-r--r--   0        0        0      969 2023-05-17 15:25:07.672109 eulertools-0.8.0/src/eulertools/statement.py
+-rw-r--r--   0        0        0     2586 2023-05-15 13:30:41.006142 eulertools-0.8.0/src/eulertools/time.py
+-rw-r--r--   0        0        0     6121 2023-05-17 15:25:08.070232 eulertools-0.8.0/src/eulertools/utils.py
+-rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 eulertools-0.8.0/PKG-INFO
```

### Comparing `eulertools-0.7.0/LICENSE.txt` & `eulertools-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eulertools-0.7.0/pyproject.toml` & `eulertools-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -98,30 +98,30 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "0.7.0"
+version = "0.8.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
 
 homepage = "https://eulertools.readthedocs.io/en/latest/"
 repository = "https://github.com/spapanik/eulertools"
 documentation = "https://eulertools.readthedocs.io/en/latest/"
 
 keywords = ["leetcode", "topcoder", "project_euler"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.scripts]
 euler = "eulertools.main:main"
 
 [tool.poetry.dependencies]
```

### Comparing `eulertools-0.7.0/src/eulertools/compare.py` & `eulertools-0.8.0/src/eulertools/compare.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.7.0/src/eulertools/generate.py` & `eulertools-0.8.0/src/eulertools/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,9 +17,11 @@
     def generate_solution(language: Language, problem: str) -> None:
         template_path = get_template(language)
         solution = get_solution(language, problem)
         context = get_context(language, problem)
         if solution.exists():
             return
 
-        template = jinja2.Template(template_path.read_text(), keep_trailing_newline=True)
+        template = jinja2.Template(
+            template_path.read_text(), keep_trailing_newline=True
+        )
         solution.write_text(template.render(context))
```

### Comparing `eulertools-0.7.0/src/eulertools/main.py` & `eulertools-0.8.0/src/eulertools/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
     compare_parser = subparsers.add_parser("compare", parents=[parent_parser])
     language_specific(compare_parser)
     problem_specific(compare_parser)
 
     statement_parser = subparsers.add_parser("statement", parents=[parent_parser])
     problem_specific(statement_parser)
-    statement_parser.add_argument("-H", "--hide-hints", dest="show_hints", action="store_false")
+    statement_parser.add_argument(
+        "-H", "--hide-hints", dest="show_hints", action="store_false"
+    )
 
     return parser.parse_args()
 
 
 def main() -> None:
     options = parse_args()
     if options.verbosity > 0:
```

### Comparing `eulertools-0.7.0/src/eulertools/run.py` & `eulertools-0.8.0/src/eulertools/run.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.7.0/src/eulertools/statement.py` & `eulertools-0.8.0/src/eulertools/statement.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
     def run(self) -> None:
         for problem in self.problems:
             self.show_statement(problem)
 
     def show_statement(self, problem: str) -> None:
         statement = get_statement(problem)["common"]
-        print(ANSIEscape.OKGREEN, statement["title"], ANSIEscape.ENDC, sep="")
-        print(ANSIEscape.OKGREEN, "~" * len(statement["title"]), ANSIEscape.ENDC, sep="")
+        if title := statement.get("title", ""):
+            print(ANSIEscape.OKGREEN, title, ANSIEscape.ENDC, sep="")
+            print(
+                ANSIEscape.OKGREEN, "~" * len(title), ANSIEscape.ENDC, sep=""
+            )
         print(statement["description"].strip())
         if self.show_hints and (hint := statement.get("hint")):
             print("")
             print(ANSIEscape.OKBLUE, "Hint", ANSIEscape.ENDC, sep="")
             print(ANSIEscape.OKBLUE, "~" * len("Hint"), ANSIEscape.ENDC, sep="")
             print(hint.strip())
```

### Comparing `eulertools-0.7.0/src/eulertools/time.py` & `eulertools-0.8.0/src/eulertools/time.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.7.0/src/eulertools/utils.py` & `eulertools-0.8.0/src/eulertools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,25 +54,27 @@
     def __str__(self) -> str:
         return f"{self.time}{self.unit}"
 
 
 @dataclass(frozen=True, slots=True, order=True)
 class Language:
     name: str
-    extension: str
+    extension: str = field(repr=False, compare=False)
+    path: Path = field(repr=False, compare=False)
     runner: Path = field(repr=False, compare=False)
 
     @classmethod
     def from_settings(cls, name: str) -> Self:
         project_root = _get_project_root()
         settings = get_settings()
         language = settings["languages"][name]
         return cls(
-            name=language["name"],
+            name=name,
             extension=language["extension"],
+            path=project_root.joinpath(language.get("path", name)),
             runner=project_root.joinpath(language["runner"]),
         )
 
 
 def _get_project_root() -> Path:
     cwd = Path.cwd().resolve()
     while not cwd.joinpath("leet.toml").exists():
@@ -83,19 +85,25 @@
 
 
 def _get_settings() -> Path:
     return _get_project_root().joinpath("leet.toml")
 
 
 def _get_answers() -> Path:
-    return _get_project_root().joinpath("common", "answers.txt")
+    file = _get_project_root().joinpath("common", "answers.txt")
+    if not file.exists():
+        file.touch(mode=0o644)
+    return file
 
 
 def _get_timings(language: Language) -> Path:
-    return _get_project_root().joinpath(language.name, ".leet", "timings.txt")
+    file = language.path.joinpath(".leet", "timings.txt")
+    if not file.exists():
+        file.touch(mode=0o644)
+    return file
 
 
 def _get_statements_dir() -> Path:
     return _get_project_root().joinpath("common", "statements")
 
 
 def _get_statement(problem: str) -> Path:
@@ -103,20 +111,20 @@
     if not statement.exists():
         raise FileNotFoundError("No problem description found. Aborting...")
 
     return statement
 
 
 def get_template(language: Language) -> Path:
-    return _get_project_root().joinpath(language.name, ".leet", "solution.jinja")
+    return language.path.joinpath(".leet", "solution.jinja")
 
 
 def get_solution(language: Language, problem: str) -> Path:
-    return _get_project_root().joinpath(
-        language.name, "src", "solutions", f"{problem}.{language.extension}"
+    return language.path.joinpath(
+        "src", "solutions", f"{problem}.{language.extension}"
     )
 
 
 def get_statement(problem: str) -> dict[str, Any]:
     return SettingsParser(_get_statement(problem)).data
 
 
@@ -146,14 +154,15 @@
 def get_context(language: Language, problem: str) -> dict[str, str]:
     statement = get_statement(problem)
     return {
         "problem": problem,
         "title": statement["common"].get("title", ""),
         "method": statement["common"].get("method", ""),
         "args": statement.get(language.name, {}).get("args", ""),
+        "rtype": statement.get(language.name, {}).get("rtype", ""),
     }
 
 
 def update_timings(language: Language, timings: dict[str, dict[int, Timing]]) -> None:
     timings_path = _get_timings(language)
     with timings_path.open("w") as file:
         for problem in sorted(timings):
```

