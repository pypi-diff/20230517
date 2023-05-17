# Comparing `tmp/github_dependents_info-1.0.1.tar.gz` & `tmp/github_dependents_info-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_dependents_info-1.0.1.tar", max compression
+gzip compressed data, was "github_dependents_info-1.1.0.tar", max compression
```

## Comparing `github_dependents_info-1.0.1.tar` & `github_dependents_info-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-01 08:56:37.257248 github_dependents_info-1.0.1/LICENSE
--rw-r--r--   0        0        0    15767 2023-05-01 08:56:37.257248 github_dependents_info-1.0.1/README.md
--rw-r--r--   0        0        0      474 2023-05-01 08:56:37.261247 github_dependents_info-1.0.1/github_dependents_info/__init__.py
--rw-r--r--   0        0        0     3926 2023-05-01 08:56:37.261247 github_dependents_info-1.0.1/github_dependents_info/__main__.py
--rw-r--r--   0        0        0    19809 2023-05-01 08:56:37.261247 github_dependents_info-1.0.1/github_dependents_info/gh_dependents_info.py
--rw-r--r--   0        0        0     4180 2023-05-01 08:56:37.261247 github_dependents_info-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    17086 1970-01-01 00:00:00.000000 github_dependents_info-1.0.1/setup.py
--rw-r--r--   0        0        0    17040 1970-01-01 00:00:00.000000 github_dependents_info-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-17 21:42:56.051413 github_dependents_info-1.1.0/LICENSE
+-rw-r--r--   0        0        0    15767 2023-05-17 21:42:56.051413 github_dependents_info-1.1.0/README.md
+-rw-r--r--   0        0        0      474 2023-05-17 21:42:56.055413 github_dependents_info-1.1.0/github_dependents_info/__init__.py
+-rw-r--r--   0        0        0     3926 2023-05-17 21:42:56.055413 github_dependents_info-1.1.0/github_dependents_info/__main__.py
+-rw-r--r--   0        0        0    19818 2023-05-17 21:42:56.055413 github_dependents_info-1.1.0/github_dependents_info/gh_dependents_info.py
+-rw-r--r--   0        0        0     4185 2023-05-17 21:42:56.059413 github_dependents_info-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    17083 1970-01-01 00:00:00.000000 github_dependents_info-1.1.0/setup.py
+-rw-r--r--   0        0        0    17037 1970-01-01 00:00:00.000000 github_dependents_info-1.1.0/PKG-INFO
```

### Comparing `github_dependents_info-1.0.1/LICENSE` & `github_dependents_info-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `github_dependents_info-1.0.1/README.md` & `github_dependents_info-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `github_dependents_info-1.0.1/github_dependents_info/__main__.py` & `github_dependents_info-1.1.0/github_dependents_info/__main__.py`

 * *Files identical despite different names*

### Comparing `github_dependents_info-1.0.1/github_dependents_info/gh_dependents_info.py` & `github_dependents_info-1.1.0/github_dependents_info/gh_dependents_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,17 +377,17 @@
         return (
             f"[![](https://img.shields.io/static/v1?label={label}&message={str(nb)}"
             + f"&color={self.badge_color}&logo=slickpic)]({url})"
         )
 
     def requests_retry_session(
         self,
-        retries=3,
-        backoff_factor=0.5,
-        status_forcelist=(500, 502, 504),
+        retries=10,
+        backoff_factor=2,
+        status_forcelist=(429, 500, 502, 503, 504),
         session=None,
     ):
         session = session or requests.Session()
         retry = Retry(
             total=retries,
             read=retries,
             connect=retries,
```

### Comparing `github_dependents_info-1.0.1/pyproject.toml` & `github_dependents_info-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "github-dependents-info"
-version = "1.0.1"
+version = "1.1.0"
 description = "Collect information about dependencies between a github repo and other repositories. Results available in JSON, markdown and badges."
 readme = "README.md"
 authors = ["nvuillam <nicolas.vuillamy@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/nvuillam/github-dependents-info"
 homepage = "https://github.com/nvuillam/github-dependents-info"
 
@@ -30,47 +30,47 @@
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "github-dependents-info" = "github_dependents_info.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-typer = {extras = ["all"], version = "^0.4.0"}
+typer = {extras = ["all"], version = ">=0.4,<0.10"}
 rich = ">=12.6,<14.0"
 beautifulsoup4 = "4.12.2"
 pandas = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.5"
 black = {version = "^22.12.0", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.12.0"}
-mypy = "^1.2"
+mypy = "^1.3"
 mypy-extensions = "^1.0.0"
 pre-commit = "^2.21.0"
 pydocstyle = "^6.3.0"
-pylint = "^2.17.3"
+pylint = "^2.17.4"
 pytest = "^7.3.1"
-pyupgrade = "^3.3.1"
+pyupgrade = "^3.4.0"
 safety = "^2.3.5"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.4"
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.12.0"}
-mypy = "^1.2"
+mypy = "^1.3"
 pre-commit = "^2.20.0"
 pydocstyle = "^6.3.0"
 pylint = "^2.15.5"
 pytest = "^7.3.1"
-pyupgrade = "^3.3.1"
+pyupgrade = "^3.4.0"
 safety = "^2.3.5"
 coverage = "^6.5.0"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.0.0"
 
 [tool.black]
```

### Comparing `github_dependents_info-1.0.1/setup.py` & `github_dependents_info-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4==4.12.2',
  'pandas>=2.0.0,<3.0.0',
  'rich>=12.6,<14.0',
- 'typer[all]>=0.4.0,<0.5.0']
+ 'typer[all]>=0.4,<0.10']
 
 entry_points = \
 {'console_scripts': ['github-dependents-info = '
                      'github_dependents_info.__main__:app']}
 
 setup_kwargs = {
     'name': 'github-dependents-info',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'Collect information about dependencies between a github repo and other repositories. Results available in JSON, markdown and badges.',
     'long_description': '# github-dependents-info\n\n<div align="center">\n\n[![PyPI](https://img.shields.io/pypi/v/github-dependents-info)](https://pypi.org/project/github-dependents-info/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/github-dependents-info)](https://pypi.org/project/github-dependents-info/)\n[![GitHub stars](https://img.shields.io/github/stars/nvuillam/github-dependents-info?cacheSeconds=3600)](https://github.com/nvuillam/github-dependents-info/stargazers/)\n[![Build status](https://github.com/nvuillam/github-dependents-info/workflows/build/badge.svg?branch=main&event=push)](https://github.com/nvuillam/github-dependents-info/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/github-dependents-info.svg)](https://pypi.org/project/github-dependents-info/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/nvuillam/github-dependents-info/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![MegaLinter](https://github.com/nvuillam/github-dependents-info/workflows/MegaLinter/badge.svg?branch=main)](https://oxsecurity.github.io/megalinter)\n[![License](https://img.shields.io/github/license/nvuillam/github-dependents-info)](https://github.com/nvuillam/github-dependents-info/blob/master/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)\n\nCollect information about dependencies between a github repo and other repositories.\n\n</div>\n\n_________________\n## 🚀 Features\n\nGitHub API does not allow to collect information about package usage (**Used by** on home, **Dependents** in insights section)\n\nThis package uses GitHub HTML to collect dependents information and can:\n\n- Output as text\n- Output as json (including shields.io markdown badges)\n- Generate summary markdown file\n- Update existing markdown by inserting **Used by** badge within tags\n  - `<!-- gh-dependents-info-used-by-start --><!-- gh-dependents-info-used-by-end -->`\n- Handle multiple repositories packages\n- Filter results using minimum stars\n\nBadges example\n\n[![](https://img.shields.io/static/v1?label=Used%20by&message=15&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n[![](https://img.shields.io/static/v1?label=Used%20by%20(public)&message=11&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n[![](https://img.shields.io/static/v1?label=Used%20by%20(private)&message=4&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n[![](https://img.shields.io/static/v1?label=Used%20by%20(stars)&message=56&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n\n<details>\n  <summary>JSON output</summary>\n\n```json\n{\n    "all_public_dependent_repos": [\n        {\n            "name": "CIT-SeniorDesign/CIT-SeniorDesign.github.io",\n            "stars": 0\n        },\n        {\n            "name": "Moaz-Adel/Jobsity-Challenge",\n            "stars": 0\n        },\n        {\n            "name": "Moaz-Adel/automation-exercise-cypress",\n            "stars": 0\n        },\n        {\n            "name": "RecuencoJones/vscode-groovy-lint-issue",\n            "stars": 0\n        },\n        {\n            "name": "aboe026/data-structures",\n            "stars": 0\n        },\n        {\n            "name": "aboe026/shields.io-badge-results",\n            "stars": 0\n        },\n        {\n            "name": "aboe026/software-update-checker",\n            "stars": 2\n        },\n        {\n            "name": "katalon-labs/katalon-recorder-extension",\n            "stars": 0\n        },\n        {\n            "name": "mashafrancis/sa-jenkins",\n            "stars": 0\n        },\n        {\n            "name": "nvuillam/vscode-groovy-lint",\n            "stars": 52\n        },\n        {\n            "name": "run2cmd/dotfiles",\n            "stars": 2\n        }\n    ],\n    "packages": [\n        {\n            "id": null,\n            "name": "nvuillam/npm-groovy-lint",\n            "url": "https://github.com/nvuillam/npm-groovy-lint/network/dependents",\n            "public_dependent_stars": 56,\n            "public_dependents": [\n                {\n                    "name": "CIT-SeniorDesign/CIT-SeniorDesign.github.io",\n                    "stars": 0\n                },\n                {\n                    "name": "Moaz-Adel/Jobsity-Challenge",\n                    "stars": 0\n                },\n                {\n                    "name": "Moaz-Adel/automation-exercise-cypress",\n                    "stars": 0\n                },\n                {\n                    "name": "RecuencoJones/vscode-groovy-lint-issue",\n                    "stars": 0\n                },\n                {\n                    "name": "aboe026/data-structures",\n                    "stars": 0\n                },\n                {\n                    "name": "aboe026/shields.io-badge-results",\n                    "stars": 0\n                },\n                {\n                    "name": "aboe026/software-update-checker",\n                    "stars": 2\n                },\n                {\n                    "name": "katalon-labs/katalon-recorder-extension",\n                    "stars": 0\n                },\n                {\n                    "name": "mashafrancis/sa-jenkins",\n                    "stars": 0\n                },\n                {\n                    "name": "nvuillam/vscode-groovy-lint",\n                    "stars": 52\n                },\n                {\n                    "name": "run2cmd/dotfiles",\n                    "stars": 2\n                }\n            ],\n            "public_dependents_number": 11,\n            "private_dependents_number": 4,\n            "total_dependents_number": 15,\n            "badges": {\n                "total": "[![](https://img.shields.io/static/v1?label=Used%20by&message=15&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)",\n                "public": "[![](https://img.shields.io/static/v1?label=Used%20by%20(public)&message=11&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)",\n                "private": "[![](https://img.shields.io/static/v1?label=Used%20by%20(private)&message=4&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)",\n                "stars": "[![](https://img.shields.io/static/v1?label=Used%20by%20(stars)&message=56&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)"\n            }\n        }\n    ],\n    "total_dependents_number": 15,\n    "public_dependents_number": 11,\n    "private_dependents_number": 4,\n    "public_dependents_stars": 56,\n    "badges": {\n        "total": "[![](https://img.shields.io/static/v1?label=Used%20by&message=15&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)",\n        "public": "[![](https://img.shields.io/static/v1?label=Used%20by%20(public)&message=11&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)",\n        "private": "[![](https://img.shields.io/static/v1?label=Used%20by%20(private)&message=4&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)",\n        "stars": "[![](https://img.shields.io/static/v1?label=Used%20by%20(stars)&message=56&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)"\n    }\n}\n\n```\n</details>\n\n<details>\n  <summary>Markdown output for single package</summary>\n\n```markdown\n# Dependents stats for nvuillam/npm-groovy-lint\n\n## Package nvuillam/npm-groovy-lint\n\n[![](https://img.shields.io/static/v1?label=Used%20by&message=15&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n[![](https://img.shields.io/static/v1?label=Used%20by%20(public)&message=11&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n[![](https://img.shields.io/static/v1?label=Used%20by%20(private)&message=4&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n[![](https://img.shields.io/static/v1?label=Used%20by%20(stars)&message=56&color=informational&logo=slickpic)](https://github.com/nvuillam/npm-groovy-lint/network/dependents)\n\n| Repository                                                                                                    | Stars |\n|:--------------------------------------------------------------------------------------------------------------|------:|\n| [CIT-SeniorDesign/CIT-SeniorDesign.github.io](https://github.com/CIT-SeniorDesign/CIT-SeniorDesign.github.io) |     0 |\n| [Moaz-Adel/Jobsity-Challenge](https://github.com/Moaz-Adel/Jobsity-Challenge)                                 |     0 |\n| [Moaz-Adel/automation-exercise-cypress](https://github.com/Moaz-Adel/automation-exercise-cypress)             |     0 |\n| [RecuencoJones/vscode-groovy-lint-issue](https://github.com/RecuencoJones/vscode-groovy-lint-issue)           |     0 |\n| [aboe026/data-structures](https://github.com/aboe026/data-structures)                                         |     0 |\n| [aboe026/shields.io-badge-results](https://github.com/aboe026/shields.io-badge-results)                       |     0 |\n| [aboe026/software-update-checker](https://github.com/aboe026/software-update-checker)                         |     2 |\n| [katalon-labs/katalon-recorder-extension](https://github.com/katalon-labs/katalon-recorder-extension)         |     0 |\n| [mashafrancis/sa-jenkins](https://github.com/mashafrancis/sa-jenkins)                                         |     0 |\n| [nvuillam/vscode-groovy-lint](https://github.com/nvuillam/vscode-groovy-lint)                                 |    52 |\n| [run2cmd/dotfiles](https://github.com/run2cmd/dotfiles)                                                       |     2 |\n\n_Generated by [github-dependents-info](https://github.com/nvuillam/github-dependents-info)_\n```\n</details>\n\nNote: If your repository packages have millions of dependents, running github-dependent-infos could take hours, as it works by browsing and scraping HTML pages returned by GitHub. For example, [angular/angular dependents](assets/angular-package-usage.md) did run during several hours !\n_________________\n## ⚙️ Installation\n\n```bash\npip install -U github-dependents-info\n```\n\nor install with `Poetry`\n\n```bash\npoetry add github-dependents-info\n```\n\n_________________\n## 🛠️ Usage\n\n```shell\n    github-dependents-info [OPTIONS]\n```\n\n| Parameter                   | Type    | Description                                                                                                                                                                              |\n|-----------------------------|---------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| --repo                      | String  | Repository. Example: `oxsecurity/megalinter`                                                                                                                                             |\n| -b<br/> --badgemarkdownfile | String  | _(optional)_ Path to markdown file where to insert/update **Used by** badge <br/> (must contain tags `<!-- gh-dependents-info-used-by-start --><!-- gh-dependents-info-used-by-end -->`) |\n| -s<br/> --sort              | String  | _(optional)_ Sort order: name (default) or stars                                                                                                                                         |\n| -x<br/> --minstars          | String  | _(optional)_ If set, filters repositories to keep only those with more than X stars                                                                                                      |\n| -m<br/> --markdownfile      | String  | _(optional)_ Output markdown file file                                                                                                                                                   |\n| -p<br/> --mergepackages     | String  | _(optional)_ In case of multiple packages, merge their stats in a single one in markdown and json output                                                                                 |\n| -j<br/> --json              | String  | _(optional)_ Output in json format                                                                                                                                                       |\n| -v<br/> --version           | Boolean | _(optional)_ Displays version of github-dependents-info                                                                                                                                  |\n| --verbose                   | Boolean | _(optional)_ Verbose output                                                                                                                                                              |\n\n_________________\n## 🧪 Examples\n\n- Text output\n\n      github-dependents-info --repo nvuillam/npm-groovy-lint\n\n- JSON output\n\n      github-dependents-info --repo nvuillam/npm-groovy-lint --json\n\n- Insert/Update **Used by** markdown badge within an existing markdown file containing tags `<!-- gh-dependents-info-used-by-start --><!-- gh-dependents-info-used-by-end -->`\n\n      github-dependents-info --repo nvuillam/npm-groovy-lint --badgemarkdownfile ./README.md\n\n- Build markdown file with dependent repos (single package), sorted by name\n\n      github-dependents-info --repo nvuillam/npm-groovy-lint --markdownfile ./docs/package-usage.md --verbose\n\n- Build markdown file with dependent repos (single package), with minimum 10 stars\n\n      github-dependents-info --repo nvuillam/npm-groovy-lint --markdownfile ./docs/package-usage.md --minstars 10 --verbose\n\n- Build markdown file with dependent repos (multiple package), sorted by stars\n\n      github-dependents-info --repo oxsecurity/megalinter --markdownfile ./docs/package-usage.md --sort stars --verbose\n\n- Build markdown file with dependent repos (multiple package), with merged list of packages in output markdown\n\n      github-dependents-info --repo oxsecurity/megalinter --markdownfile ./docs/package-usage.md --sort stars --mergepackages --verbose\n\n_________________\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/nvuillam/github-dependents-info)](https://github.com/nvuillam/github-dependents-info/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/nvuillam/github-dependents-info/blob/master/LICENSE) for more details.\n\n_________________\n## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)\n\nThis package has been inspired by stackexchange post [How to use GitHub API to get a repository\'s dependents information in GitHub?](https://stackoverflow.com/questions/58734176/how-to-use-github-api-to-get-a-repositorys-dependents-information-in-github)\n- [Bertrand Martel](https://github.com/bertrandmartel)\n- [muvaf](https://stackoverflow.com/users/5233252/muvaf)\n- [Mo Ganji](https://www.linkedin.com/in/mohganji/) <!-- markdown-link-check-disable-line -->\n\nThis project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)\n',
     'author': 'nvuillam',
     'author_email': 'nicolas.vuillamy@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nvuillam/github-dependents-info',
```

### Comparing `github_dependents_info-1.0.1/PKG-INFO` & `github_dependents_info-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-dependents-info
-Version: 1.0.1
+Version: 1.1.0
 Summary: Collect information about dependencies between a github repo and other repositories. Results available in JSON, markdown and badges.
 Home-page: https://github.com/nvuillam/github-dependents-info
 License: MIT
 Keywords: github,dependent,used-by,repository,stats,dependencies,using
 Author: nvuillam
 Author-email: nicolas.vuillamy@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (==4.12.2)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: rich (>=12.6,<14.0)
-Requires-Dist: typer[all] (>=0.4.0,<0.5.0)
+Requires-Dist: typer[all] (>=0.4,<0.10)
 Project-URL: Repository, https://github.com/nvuillam/github-dependents-info
 Description-Content-Type: text/markdown
 
 # github-dependents-info
 
 <div align="center">
```

