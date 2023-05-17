# Comparing `tmp/cz_legacy-0.1.7.tar.gz` & `tmp/cz_legacy-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_legacy-0.1.7.tar", max compression
+gzip compressed data, was "cz_legacy-1.0.0rc0.tar", max compression
```

## Comparing `cz_legacy-0.1.7.tar` & `cz_legacy-1.0.0rc0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1066 2022-01-16 19:41:20.994377 cz_legacy-0.1.7/LICENSE
--rw-r--r--   0        0        0      221 2022-09-17 17:51:58.515191 cz_legacy-0.1.7/cz_legacy/__init__.py
--rw-r--r--   0        0        0     1720 2022-01-16 19:41:20.997299 cz_legacy-0.1.7/cz_legacy/cz_legacy.py
--rw-r--r--   0        0        0     3376 2022-09-17 17:52:31.804771 cz_legacy-0.1.7/docs/README.md
--rw-r--r--   0        0        0     1981 2022-09-17 17:51:58.548505 cz_legacy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 cz_legacy-0.1.7/setup.py
--rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 cz_legacy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 17:52:27.966560 cz_legacy-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0       70 2023-05-17 01:08:54.378400 cz_legacy-1.0.0rc0/cz_legacy/__init__.py
+-rw-r--r--   0        0        0     1865 2023-04-08 19:30:33.424759 cz_legacy-1.0.0rc0/cz_legacy/cz_legacy.py
+-rw-r--r--   0        0        0     3333 2023-05-17 01:09:00.397575 cz_legacy-1.0.0rc0/docs/README.md
+-rw-r--r--   0        0        0     1936 2023-05-17 01:08:54.395354 cz_legacy-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 cz_legacy-1.0.0rc0/PKG-INFO
```

### Comparing `cz_legacy-0.1.7/LICENSE` & `cz_legacy-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cz_legacy-0.1.7/cz_legacy/cz_legacy.py` & `cz_legacy-1.0.0rc0/cz_legacy/cz_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,38 @@
 Chg = "Change (old)"
 Fix = "Fix (old)"
 New = "New (old)"
 """
 """Example custom TOML file configuration. Note: should be kept consistent with the README."""
 
 
-class _LegacyCz(ConventionalCommitsCz):
+class _LegacyCz(ConventionalCommitsCz):  # type: ignore[misc]
 
-    def __init__(self, config: BaseConfig) -> None:
+    def __init__(self, config: BaseConfig) -> None:  # noqa: RBT002
         """Initialize the class and override the data members.
 
         Args:
             config: commitizen BaseConfig that stores the parsed settings. Passed to base class
 
         Raises:
             CustomError: commitizen-specific error and exit code to indicate that a configuration item is missing
 
         """
         super().__init__(config)
 
         # Read the user-specified legacy change types (ct)
         cz_legacy_map = self.config.settings.get('cz_legacy_map')
         if not cz_legacy_map:
-            raise CustomError(f'User must specify a `cz_legacy_map` dict in `[tool.commitizen]`. Example:\n{EXAMPLE}')
+            raise CustomError(
+                f'User must specify a `cz_legacy_map` dict in `[tool.commitizen]`. Example:\n{EXAMPLE}',  # noqa: EM102
+            )
         joined_types = '|'.join([*cz_legacy_map.keys()])
 
         self.commit_parser = defaults.commit_parser.replace('<change_type>', f'<change_type>{joined_types}|')
-        self.change_type_map = {**self.change_type_map, **cz_legacy_map}
+        self.change_type_map = {
+            **self.change_type_map,  # type: ignore[has-type]
+            **cz_legacy_map,
+        }
 
         extended_pattern = defaults.bump_pattern.replace('refactor', f'refactor|{joined_types}')
         self.bump_pattern = extended_pattern
         self.changelog_pattern = extended_pattern
```

### Comparing `cz_legacy-0.1.7/PKG-INFO` & `cz_legacy-1.0.0rc0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: cz-legacy
-Version: 0.1.7
+Version: 1.0.0rc0
 Summary: Extends Conventional Commits Change Types with User-Defined Legacy Types for Commitizen
 Home-page: https://github.com/kyleking/cz_legacy
 License: MIT
 Keywords: commitizen,conventional commits,git
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: commitizen (>=2.0.0)
 Project-URL: Bug Tracker, https://github.com/kyleking/cz_legacy/issues
 Project-URL: Changelog, https://github.com/kyleking/cz_legacy/blob/main/docs/docs/CHANGELOG.md
-Project-URL: Documentation, https://github.com/kyleking/cz_legacy/docs
+Project-URL: Documentation, https://cz_legacy.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/cz_legacy
 Description-Content-Type: text/markdown
 
 # cz_legacy
 
-Custom Commitizen parser for user-specified legacy change types. The parser utilizes the `cz_conventional_commits` pattern and extends with the tag mapping specified in the configuration file
+Custom Commitizen parser for user-specified legacy change types. The parser utilizes the `cz_conventional_commits` pattern and extends with the tag mapping specified in the configuration file.
 
-While old change types will appear in the Changelog, the user will be prevented from using them in new commits. This is the reverse of the [revert/chore logic](https://github.com/commitizen-tools/commitizen#why-are-revert-and-chore-valid-types-in-the-check-pattern-of-cz-conventional_commits-but-not-types-we-can-select) from commitizen that allows use of those commit types, but won't display them in the changelog
+While old change types will appear in the "Changelog", the user will be prevented from using them in new commits. This is the reverse of the [revert/chore logic](https://github.com/commitizen-tools/commitizen#why-are-revert-and-chore-valid-types-in-the-check-pattern-of-cz-conventional_commits-but-not-types-we-can-select) from commitizen that allows use of those commit types, but won't display them in the changelog.
 
 ## Alternatives
 
 This customization only works when old commits use the `<change_type>: <message>` format that can be parsed by commitizen. If that doesn't fit your use case, you may want to try out [incremental](https://commitizen-tools.github.io/commitizen/changelog/#incremental) which (I think) prepends to an existing `CHANGELOG`
 
 ## Usage
 
-### Install
+### Pre-Commit
 
-Install the package from PyPi: `pip install cz_legacy` or from git: `pip install git+https://github.com/KyleKing/cz_legacy.git@main`
+To use in pre-commit, add this to your `pre-commit-config.yml`. Run `pre-commit autoupdate` to get the latest version
+
+```yaml
+repos:
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: main
+    hooks:
+      - id: commitizen
+        additional_dependencies: [cz_legacy]
+        stages: [commit-msg]
+```
 
 ### Configuration
 
 At minimum, you must have the `name = "cz_legacy"` and `[tool.commitizen.cz_legacy_map]` in your configuration file. The below example is for TOML, you can also utilize a YAML or JSON file.
 
 Below is an example of the three change legacy types Chg, Fix, and New, but the user can choose any tag names and associated mapping for the Changelog
 
@@ -59,49 +70,45 @@
 
 [tool.commitizen.cz_legacy_map]
 Chg = "Change (old)"
 Fix = "Fix (old)"
 New = "New (old)"
 ```
 
-### Pre-Commit
+## Issues
 
-To use in pre-commit, add this to your `pre-commit-config.yml`
+If you have any feature requests, run into any bugs, or have questions, feel free to start a discussion or open an issue on Github at [https://github.com/kyleking/cz_legacy](https://github.com/kyleking/cz_legacy).
 
-```yaml
-repos:
-  - repo: https://github.com/commitizen-tools/commitizen
-    rev: v2.11.1
-    hooks:
-      - id: commitizen
-        additional_dependencies: [cz_legacy]
-        stages: [commit-msg]
-```
+## Project Status
 
-## Issues
+See the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].
 
-If you have any feature requests, run into any bugs, or have questions, feel free to start a discussion or open an issue on Github at [https://github.com/kyleking/cz_legacy](https://github.com/kyleking/cz_legacy).
+## Contributing
 
-## Background
+We welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:
 
-I couldn't find a good way of adding a few legacy change types from an old commit style to commitizen so I built a package to [extend the ConventionalCommitsCz](https://github.com/commitizen-tools/commitizen/blob/master/commitizen/cz/conventional_commits/conventional_commits.py) to [provide custom logic](https://commitizen-tools.github.io/commitizen/customization/#2-customize-through-customizing-a-class). For reference, these are the [default settings](https://github.com/commitizen-tools/commitizen/blob/master/commitizen/defaults.py)
+- [DEVELOPER_GUIDE]
+- [STYLE_GUIDE]
 
-## Roadmap
+## Code of Conduct
 
-See the `Open Issues` and `Milestones` for current status and [./docs/CODE_TAG_SUMMARY.md](./docs/CODE_TAG_SUMMARY.md) for annotations in the source code.
+We follow the [Contributor Covenant Code of Conduct][contributor-covenant].
 
-For release history, see the [./docs/CHANGELOG.md](./docs/CHANGELOG.md)
+### Open Source Status
 
-## Contributing
+We try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/cz_legacy)
 
-See the Developer Guide, Contribution Guidelines, etc
+## Responsible Disclosure
 
-- [./docs/DEVELOPER_GUIDE.md](./docs/DEVELOPER_GUIDE.md)
-- [./docs/STYLE_GUIDE.md](./docs/STYLE_GUIDE.md)
-- [./docs/CONTRIBUTING.md](./docs/CONTRIBUTING.md)
-- [./docs/CODE_OF_CONDUCT.md](./docs/CODE_OF_CONDUCT.md)
-- [./docs/SECURITY.md](./docs/SECURITY.md)
+If you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).
 
 ## License
 
-[LICENSE](https://github.com/KyleKing/calcipy/tree/main/LICENSE)
+[LICENSE]
+
+[changelog]: https://cz_legacy.kyleking.me/docs/CHANGELOG
+[code_tag_summary]: https://cz_legacy.kyleking.me/docs/CODE_TAG_SUMMARY
+[contributor-covenant]: https://www.contributor-covenant.org
+[developer_guide]: https://cz_legacy.kyleking.me/docs/DEVELOPER_GUIDE
+[license]: https://github.com/kyleking/cz_legacy/blob/main/LICENSE
+[style_guide]: https://cz_legacy.kyleking.me/docs/STYLE_GUIDE
```

