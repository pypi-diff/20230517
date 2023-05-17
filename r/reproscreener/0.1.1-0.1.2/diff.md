# Comparing `tmp/reproscreener-0.1.1.tar.gz` & `tmp/reproscreener-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reproscreener-0.1.1.tar", max compression
+gzip compressed data, was "reproscreener-0.1.2.tar", max compression
```

## Comparing `reproscreener-0.1.1.tar` & `reproscreener-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1091 2022-12-14 22:12:34.973208 reproscreener-0.1.1/LICENSE
--rw-r--r--   0        0        0     1028 2023-05-16 23:16:16.245839 reproscreener-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/__init__.py
--rw-r--r--   0        0        0      684 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/download_arxiv.py
--rw-r--r--   0        0        0     2482 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/keywords.py
--rw-r--r--   0        0        0     2749 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/main.py
--rw-r--r--   0        0        0     5563 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/repo_eval.py
--rw-r--r--   0        0        0     2851 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/tex_eval.py
--rw-r--r--   0        0        0      342 2023-05-16 22:58:59.439823 reproscreener-0.1.1/src/reproscreener/utils.py
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 reproscreener-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-12-14 22:12:34.973208 reproscreener-0.1.2/LICENSE
+-rw-r--r--   0        0        0      236 2023-05-17 18:34:03.761525 reproscreener-0.1.2/README.md
+-rw-r--r--   0        0        0     1241 2023-05-17 19:38:10.873373 reproscreener-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 22:58:59.439823 reproscreener-0.1.2/src/reproscreener/__init__.py
+-rw-r--r--   0        0        0      684 2023-05-17 19:47:31.643244 reproscreener-0.1.2/src/reproscreener/download_arxiv.py
+-rw-r--r--   0        0        0     2482 2023-05-16 22:58:59.439823 reproscreener-0.1.2/src/reproscreener/keywords.py
+-rw-r--r--   0        0        0     2818 2023-05-17 21:35:12.747017 reproscreener-0.1.2/src/reproscreener/main.py
+-rw-r--r--   0        0        0     7842 2023-05-17 21:35:31.668838 reproscreener-0.1.2/src/reproscreener/repo_eval.py
+-rw-r--r--   0        0        0     3863 2023-05-17 19:47:25.973218 reproscreener-0.1.2/src/reproscreener/tex_eval.py
+-rw-r--r--   0        0        0      342 2023-05-16 22:58:59.439823 reproscreener-0.1.2/src/reproscreener/utils.py
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 reproscreener-0.1.2/PKG-INFO
```

### Comparing `reproscreener-0.1.1/LICENSE` & `reproscreener-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reproscreener-0.1.1/pyproject.toml` & `reproscreener-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "reproscreener"
-version = "0.1.1"
-description = "Automated machine learning model verification"
+version = "0.1.2"
+description = "Automated verification of machine learning research"
 authors = ["Adhithya Bhaskar <adhi@adhi.dev>"]
 license = "MIT"
 packages = [{include = "reproscreener", from = "src"}]
+readme = "README.md"
+homepage = "https://reproscreener.com/"
+keywords = ["reproducibility", "machine-learning", "transparency", "verification"]
 
 [tool.poetry.scripts]
 reproscreener = "reproscreener.main:app"
 
 [tool.poetry.dependencies]
 python = "=3.9.13"
 requests = "^2.30.0"
@@ -35,11 +38,12 @@
 seaborn = "^0.12.2"
 types-requests = "^2.30.0.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pylint = "^2.17.4"
 vulture = "^2.7"
 pytest-mock = "^3.10.0"
+mkdocs-macros-plugin = {extras = ["test"], version = "^0.7.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reproscreener-0.1.1/src/reproscreener/download_arxiv.py` & `reproscreener-0.1.2/src/reproscreener/download_arxiv.py`

 * *Files identical despite different names*

### Comparing `reproscreener-0.1.1/src/reproscreener/keywords.py` & `reproscreener-0.1.2/src/reproscreener/keywords.py`

 * *Files identical despite different names*

### Comparing `reproscreener-0.1.1/src/reproscreener/main.py` & `reproscreener-0.1.2/src/reproscreener/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         urls = tex_eval.extract_tex_urls(combined_tex)
         found_links = tex_eval.find_data_repository_links(urls)
         paper_table = tex_eval.initialize_repo_evaluation_table(paper_id, "title", found_vars, found_links)
         console.print(paper_table, overflow="fold")
         console.print("\n")
 
     if repo:
+        if path_paper is None:
+            path_base = path_download
         console.rule("Repository evaluation")
         repo_name = repo.split("/")[-1].split(".git")[0]
         cloned_path = repo_eval.clone_repo(
             repo, (path_base / "repo" / repo_name) if path_base else (path_download / "repos")
         )
 
     elif local_repo:
```

### Comparing `reproscreener-0.1.1/src/reproscreener/repo_eval.py` & `reproscreener-0.1.2/src/reproscreener/repo_eval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from pathlib import Path
+from typing import List, Tuple
 
 import git
 import pandas as pd
 from rich.table import Table
 
 from reproscreener.utils import console
 
@@ -25,55 +26,92 @@
     "readme_requirements": [],
     "readme_dependencies": [],
     "readme_setup": [],
     "readme_install": [],
 }
 
 
-def check_files(dir_path, files):
+def check_files(dir_path: Path, files: List[str]) -> Tuple[List[str], List[str]]:
+    """
+    Check if the given files exist in the directory.
+
+    Args:
+        dir_path (Path): Path to the directory to check.
+        files (List[str]): List of filenames to look for.
+
+    Returns:
+        Tuple[List[str], List[str]]: Two lists containing the found files and not found files.
+    """
     found_files = []
     not_found_files = list(files)
 
     for f in dir_path.glob("*"):
         if f.stem in files:
             if f.suffix in ext_mapping.get(f.stem, [""]):
                 found_files.append(f.name)
                 not_found_files.remove(f.stem)
 
     return found_files, not_found_files
 
 
-def check_dependencies(dir_path):
+def check_dependencies(dir_path: Path) -> Tuple[List[str], List[str]]:
+    """
+    Check if the necessary dependency files exist in the directory.
+
+    Args:
+        dir_path (Path): Path to the directory to check.
+
+    Returns:
+        Tuple[List[str], List[str]]: Two lists containing the found dependency files and not found dependency files.
+    """
     dependency_files = [
         "Dockerfile",
         "requirements",
         "setup.py",
         "environment",
         "Pipfile",
         "pyproject.toml",
         "pip_reqs",
         "conda_reqs",
     ]
     return check_files(dir_path, dependency_files)
 
 
-def check_wrapper_scripts(dir_path):
+def check_wrapper_scripts(dir_path: Path) -> Tuple[List[str], List[str]]:
+    """
+    Check if the necessary wrapper script files exist in the directory.
+
+    Args:
+        dir_path (Path): Path to the directory to check.
+
+    Returns:
+        Tuple[List[str], List[str]]: Two lists containing the found wrapper script files and not found wrapper script files.
+    """
     wrapper_files = [
         "run",
         "main",
         "run_all",
         "run_experiments",
         "MAKEFILE",
         "Makefile",
         "Dockerfile",
     ]
     return check_files(dir_path, wrapper_files)
 
 
-def check_parsed_readme(dir_path):
+def check_parsed_readme(dir_path: Path) -> Tuple[List[str], List[str]]:
+    """
+    Check if the necessary sections exist in the README file.
+
+    Args:
+        dir_path (Path): Path to the directory to check.
+
+    Returns:
+        Tuple[List[str], List[str]]: Two lists containing the found sections and not found sections.
+    """
     readme_path = dir_path / "README.md"
     possible_headers = ["requirements", "dependencies", "setup", "install"]
     if readme_path.is_file():
         with open(readme_path, "r", encoding="utf-8") as file:
             content = file.read()
             found_headers = re.findall(
                 r"^\s*#{1,6}\s*(" + "|".join(possible_headers) + ")",
@@ -84,16 +122,24 @@
             not_found_headers = list(set(possible_headers) - set(found_headers))
             return ["readme_" + header for header in found_headers], [
                 "readme_" + header for header in not_found_headers
             ]
     return [], possible_headers
 
 
-def evaluate_repo(path_corpus):
-    path_corpus = Path(path_corpus)
+def evaluate_repo(path_corpus: Path) -> pd.DataFrame:
+    """
+    Evaluate a repository by checking the existence of certain files and sections in README.
+
+    Args:
+        path_corpus (Path): Path to the repository.
+
+    Returns:
+        pd.DataFrame: A DataFrame with the evaluation results.
+    """
     if (path_corpus / "repo").is_dir():
         repo_path = path_corpus / "repo"
     else:
         repo_path = path_corpus
 
     dependencies_found, dependencies_not_found = check_dependencies(repo_path)
     parsed_readme_found, parsed_readme_not_found = check_parsed_readme(repo_path)
@@ -128,15 +174,22 @@
 
     return pd.DataFrame(
         data,
         columns=["Category", "Item", "Found", "Extensions", "Found_Extension"],
     )
 
 
-def display_dataframe(df_table, title=""):
+def display_dataframe(df_table: pd.DataFrame, title: str = ""):
+    """
+    Display a DataFrame as a rich table in console.
+
+    Args:
+        df_table (pd.DataFrame): DataFrame to display.
+        title (str, optional): Title of the table. Defaults to "".
+    """
     for category, group in df_table.groupby("Category"):
         table = Table(title=f"{category}")
         table.add_column("Item")
         table.add_column("Found")
         table.add_column("Extensions")
 
         for _, row in group.iterrows():
@@ -155,15 +208,26 @@
             found_str = "[green]Found[/green]" if found else "[red]Not Found[/red]"
             table.add_row(item, found_str, ext_color_str)
 
         console.print(table)
         console.print("\n")
 
 
-def clone_repo(repo_url: str, path_corpus: Path, overwrite=False):
+def clone_repo(repo_url: str, path_corpus: Path, overwrite: bool = False) -> Path:
+    """
+    Clone a repository from the given URL to the given path. If the repository already exists, it won't be overwritten unless specified.
+
+    Args:
+        repo_url (str): URL of the repository to clone.
+        path_corpus (Path): Path to clone the repository to.
+        overwrite (bool, optional): Whether to overwrite the existing repository. Defaults to False.
+
+    Returns:
+        Path: Path to the cloned repository. Returns False if cloning fails.
+    """
     path_exists = path_corpus.is_dir()
 
     if path_exists and not overwrite:
         console.print(f"Repo directory already exists: {path_corpus}, use the overwrite flag to download\n")
         return path_corpus
 
     path_corpus.mkdir(parents=True, exist_ok=True)
```

### Comparing `reproscreener-0.1.1/src/reproscreener/tex_eval.py` & `reproscreener-0.1.2/src/reproscreener/tex_eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,114 @@
 import glob
 import urllib.parse
 from pathlib import Path
-from typing import Set
+from typing import List, Set
 
-import pandas as pd
 from flashtext import KeywordProcessor
-from rich import print as rprint
 from rich.table import Table
 from urlextract import URLExtract
 
 from reproscreener import keywords
 from reproscreener.utils import log
 
 
 def combine_tex_in_folder(folder_path: Path) -> Path:
+    """
+    Combine all .tex files in a given directory into a single file.
+
+    Args:
+        folder_path (Path): Path to the directory containing .tex files.
+
+    Returns:
+        Path: Path to the combined .tex file.
+    """
     # Create a combined file of all .tex files in folder_path directory
     combined_path = folder_path / "combined.tex"
     with open(combined_path, "w", encoding="utf-8") as outfile:
         for name in glob.glob(f"{folder_path}/*.tex"):
             with open(name, encoding="utf-8") as infile:
                 outfile.write(infile.read())
     return combined_path
 
 
-def find_tex_variables(combined_path: Path) -> Set:
+def find_tex_variables(combined_path: Path) -> Set[str]:
     """
     Find variables in the combined tex file.
     Uses the `KeywordProcessor` from `flashtext` package to extract variables.
+
+    Args:
+        combined_path (Path): Path to the combined .tex file.
+
+    Returns:
+        Set[str]: Set of found variables.
     """
     keyword_dict = keywords.generate_gunderson_dict()
     keyword_processor = KeywordProcessor(case_sensitive=True)
     keyword_processor.add_keywords_from_dict(keyword_dict)
     with open(combined_path, "r", errors="replace", encoding="utf-8") as f:
         data = f.readlines()
         all_found = [keyword_processor.extract_keywords(line, span_info=True) for line in data]
         non_empty_found = [x for x in all_found if x != []]
         # Using set comprehension to avoid duplicates
         found_vars = {j[0] for i in non_empty_found for j in i}
     return found_vars
 
 
-def extract_tex_urls(combined_path: Path) -> Set:
+def extract_tex_urls(combined_path: Path) -> Set[str]:
     """
     Extract URLs from the combined tex file.
+
+    Args:
+        combined_path (Path): Path to the combined .tex file.
+
+    Returns:
+        Set[str]: Set of found URLs.
     """
     with open(combined_path, "r", errors="replace", encoding="utf-8") as f:
         data = f.read()
     extractor = URLExtract()
     urls = extractor.find_urls(data)
     log.debug("All urls:\n %s \n", urls)
     return set(urls)
 
 
-def find_data_repository_links(url_list: Set[str], allowed_domains: list = ["github", "gitlab", "zenodo"]) -> list:
+def find_data_repository_links(
+    url_list: Set[str], allowed_domains: List[str] = ["github", "gitlab", "zenodo"]
+) -> List[str]:
     """
     Find URLs belonging to allowed domains (default - github, gitlab, zenodo).
+
+    Args:
+        url_list (Set[str]): Set of URLs to process.
+        allowed_domains (List[str], optional): List of allowed domain names. Defaults to ["github", "gitlab", "zenodo"].
+
+    Returns:
+        List[str]: List of found URLs belonging to allowed domains.
     """
     found_list = [
         url for url in url_list if any(domain in urllib.parse.urlparse(url).netloc for domain in allowed_domains)
     ]
     for url in found_list:
         log.debug(f"Found {urllib.parse.urlparse(url).netloc} link: {url}")
     return found_list
 
 
-def initialize_repo_evaluation_table(paper_id: str, title: str, found_vars: Set, found_links: list) -> Table:
-    # Create a rich Table object with specified columns and add a row
+def initialize_repo_evaluation_table(paper_id: str, title: str, found_vars: Set[str], found_links: List[str]) -> Table:
+    """
+    Initialize a rich Table object with specified columns and add a row.
+
+    Args:
+        paper_id (str): ID of the paper.
+        title (str): Title of the paper.
+        found_vars (Set[str]): Set of found variables.
+        found_links (List[str]): List of found URLs.
+
+    Returns:
+        Table: Initialized Table object.
+    """
     table = Table()
     table.add_column("ID", justify="right", style="cyan")
     table.add_column("Title", style="magenta")
     table.add_column("Found Variables", justify="right", style="green")
     table.add_column("Found Links", style="yellow")
 
     table.add_row(paper_id, title, ", ".join(found_vars), ", ".join(found_links))
```

